---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/09/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: df665565130322504c4794462098980b1064a6c7
ms.sourcegitcommit: c6dff58438d256647d4aa29a53eef4bf93a0cd24
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/11/2019
ms.locfileid: "59480000"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="1d3b4-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="1d3b4-103">Azure CLI release notes</span></span>
## <a name="april-9-2019"></a><span data-ttu-id="1d3b4-104">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-104">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-105">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-105">Core</span></span>
* <span data-ttu-id="1d3b4-106">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-106">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-107">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-107">ACR</span></span>
* <span data-ttu-id="1d3b4-108">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-108">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="1d3b4-109">AMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-109">AMS</span></span>
* [<span data-ttu-id="1d3b4-110">사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-110">DEPRECATED</span></span>]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [<span data-ttu-id="1d3b4-111">호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-111">BREAKING CHANGE</span></span>]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="1d3b4-112">??에 새 암호화 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-112">Added new encryption parameters support in</span></span> `ams streaming-policy create`
* <span data-ttu-id="1d3b4-113">??에 새 매개 변수 `--filters` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-113">Added new paramter `--filters` to</span></span> `ams streaming-locator create`

### <a name="appservice"></a><span data-ttu-id="1d3b4-114">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-114">AppService</span></span>
* <span data-ttu-id="1d3b4-115">??에 `--logs` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-115">Added `--logs` support to</span></span> `webapp up`
* <span data-ttu-id="1d3b4-116">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-116">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="1d3b4-117">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-117">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="1d3b4-118">[호환성이 손상되는 변경] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="1d3b4-118">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="1d3b4-119">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-119">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="1d3b4-120">??을(를) 사용하여 함수 앱 아래에 있는 플랜을 전환하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-120">Added ability to switch a plan underneath a function app using</span></span> `functionapp update --plan`
* <span data-ttu-id="1d3b4-121">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-121">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="1d3b4-122">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-122">CDN</span></span>
* <span data-ttu-id="1d3b4-123">`Microsoft_Standard` 및 ??에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-123">Added support for `Microsoft_Standard` and</span></span> `Standard_ChinaCdn`

### <a name="feedback"></a><span data-ttu-id="1d3b4-124">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="1d3b4-124">Feedback</span></span>
* <span data-ttu-id="1d3b4-125">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-125">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="1d3b4-126">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-126">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="1d3b4-127">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-127">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-128">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-128">Monitor</span></span>
* <span data-ttu-id="1d3b4-129">"count"가 ??에 허용되는 값이 아닌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-129">Fixed issue where "count" was not a permitted value with</span></span> `metrics alert [create|update]` 

### <a name="network"></a><span data-ttu-id="1d3b4-130">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-130">Network</span></span>
* <span data-ttu-id="1d3b4-131">??에서 테이블 형식이 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-131">Fixed table format not displaying with</span></span> `vnet-gateway list-bgp-peer-status`
* <span data-ttu-id="1d3b4-132">??에 `list-request-headers` 및 `list-response-headers` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-132">Added `list-request-headers` and `list-response-headers` commands to</span></span> `application-gateway rewrite-rule`
* <span data-ttu-id="1d3b4-133">??에 `list-server-variables` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-133">Added `list-server-variables` command to</span></span> `application-gateway rewrite-rule condition`
* <span data-ttu-id="1d3b4-134">Express 경로에 대한 링크 상태를 업데이트하면 알 수 없는 특성 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-134">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception</span></span> `express-route port update`

### <a name="privatedns"></a><span data-ttu-id="1d3b4-135">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-135">PrivateDNS</span></span>
* <span data-ttu-id="1d3b4-136">사설 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-136">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-137">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-137">Resource</span></span>
* <span data-ttu-id="1d3b4-138">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-138">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-139">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-139">Role</span></span>
* <span data-ttu-id="1d3b4-140">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-140">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="1d3b4-141">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-141">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-142">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-142">SQL</span></span>
* <span data-ttu-id="1d3b4-143">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-143">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-144">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-144">Storage</span></span>
* <span data-ttu-id="1d3b4-145">[호환성이 손상되는 변경] ??의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-145">[BREAKING CHANGE] Removed result of</span></span> `storage blob delete`
* <span data-ttu-id="1d3b4-146">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-146">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="1d3b4-147">스냅숏에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-147">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="1d3b4-148">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-148">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="1d3b4-149">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-149">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="1d3b4-150">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-150">Core</span></span>
* <span data-ttu-id="1d3b4-151">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-151">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="1d3b4-152">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-152">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="1d3b4-153">클라우드</span><span class="sxs-lookup"><span data-stu-id="1d3b4-153">Cloud</span></span>
* <span data-ttu-id="1d3b4-154">??의 '구독을 찾을 수 없음' 오류 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-154">Fixed a 'subscription not found' error in</span></span> `cloud set`

### <a name="acr"></a><span data-ttu-id="1d3b4-155">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-155">ACR</span></span>
* <span data-ttu-id="1d3b4-156">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-156">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="1d3b4-157">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-157">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="1d3b4-158">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-158">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="1d3b4-159">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-159">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-160">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-160">AppService</span></span>
* <span data-ttu-id="1d3b4-161">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-161">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="1d3b4-162">슬롯이 ??에서 작동하지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-162">Fixed bug where slots didn't work for</span></span> `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a><span data-ttu-id="1d3b4-163">BOT Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-163">BOT Service</span></span>
* <span data-ttu-id="1d3b4-164">??을(를) 통한 봇 배포를 준비하는 `bot prepare-deploy` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-164">Added `bot prepare-deploy` to prepare for deploying bots via</span></span> `webapp`
* <span data-ttu-id="1d3b4-165">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-165">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="1d3b4-166">[호환성이 손상되는 변경] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-166">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="1d3b4-167">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-167">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="1d3b4-168">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-168">CDN</span></span>
* <span data-ttu-id="1d3b4-169">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-169">Added support for `--no-wait` to</span></span> `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="1d3b4-171">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-171">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1d3b4-172">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-172">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-173">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="1d3b4-173">Cosmosdb</span></span>
* <span data-ttu-id="1d3b4-174">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-174">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="1d3b4-175">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-175">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-176">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-176">Interactive</span></span>
* <span data-ttu-id="1d3b4-177">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-177">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-178">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-178">Monitor</span></span>
* <span data-ttu-id="1d3b4-179">??에 `*` 차원 값을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-179">Changed to allow dimension value `*` for</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="1d3b4-180">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-180">Network</span></span>
* <span data-ttu-id="1d3b4-181">`rewrite-rule` 명령 그룹을 ??에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-181">Added `rewrite-rule` command group to</span></span> `application-gateway`

### <a name="profile"></a><span data-ttu-id="1d3b4-182">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-182">Profile</span></span>
* <span data-ttu-id="1d3b4-183">관리 서비스 ID에 대한 테넌트 수준 계정 지원을 ??에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-183">Added tenant level account support for managed service identity to</span></span> `login`

### <a name="postgres"></a><span data-ttu-id="1d3b4-184">Postgres</span><span class="sxs-lookup"><span data-stu-id="1d3b4-184">Postgres</span></span> 
* <span data-ttu-id="1d3b4-185">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-185">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="1d3b4-186">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-186">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-187">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-187">Resource</span></span>
* <span data-ttu-id="1d3b4-188">??의 테이블 출력 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-188">Improved table output for</span></span> `deployment [create|list|show]`
* <span data-ttu-id="1d3b4-189">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-189">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="1d3b4-190">그래프</span><span class="sxs-lookup"><span data-stu-id="1d3b4-190">Graph</span></span>
* <span data-ttu-id="1d3b4-191">??에 `--end-date` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-191">Added support for `--end-date` to</span></span> `ad [app|sp] credential reset`
* <span data-ttu-id="1d3b4-192">??을(를) 사용하여 권한을 추가하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-192">Added support to add permissions with</span></span> `ad app permission add`
* <span data-ttu-id="1d3b4-193">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-193">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="1d3b4-194">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-194">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="1d3b4-195">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-195">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-196">저장소</span><span class="sxs-lookup"><span data-stu-id="1d3b4-196">storage</span></span>
* <span data-ttu-id="1d3b4-197">공유 스냅숏에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-197">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="1d3b4-198">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-198">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="1d3b4-199">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-199">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="1d3b4-200">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-200">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-201">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-201">VM</span></span>
* <span data-ttu-id="1d3b4-202">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-202">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="1d3b4-203">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-203">March 12, 2019</span></span>

<span data-ttu-id="1d3b4-204">2.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="1d3b4-204">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-205">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-205">Core</span></span>

* <span data-ttu-id="1d3b4-206">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-206">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-207">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-207">ACR</span></span>

* <span data-ttu-id="1d3b4-208">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-208">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-209">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-209">ACS</span></span>

* <span data-ttu-id="1d3b4-210">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-210">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="1d3b4-211">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-211">AppService</span></span>

* <span data-ttu-id="1d3b4-212">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-212">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="1d3b4-213">??에 대한 잘못된 인쇄 문 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-213">Removed erroneous print statement for</span></span> `webapp auth update`
* <span data-ttu-id="1d3b4-214">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-214">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="1d3b4-215">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-215">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="1d3b4-216">Botservice</span><span class="sxs-lookup"><span data-stu-id="1d3b4-216">Botservice</span></span>

* <span data-ttu-id="1d3b4-217">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-217">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1d3b4-218">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-218">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="1d3b4-219">??이(가) 종료할 때 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-219">Removed single quotes from `bot publish` command output at end of</span></span> `bot create`
* <span data-ttu-id="1d3b4-220">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-220">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-221">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-221">Container</span></span>

* <span data-ttu-id="1d3b4-222">??에 `--no-wait` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-222">Added `--no-wait` argument to</span></span> `container [start|restart]`

### <a name="eventhub"></a><span data-ttu-id="1d3b4-223">EventHub</span><span class="sxs-lookup"><span data-stu-id="1d3b4-223">EventHub</span></span>

* <span data-ttu-id="1d3b4-224">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-224">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="1d3b4-225">찾기</span><span class="sxs-lookup"><span data-stu-id="1d3b4-225">Find</span></span>

* <span data-ttu-id="1d3b4-226">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-226">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1d3b4-227">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1d3b4-227">HDInsight</span></span>

* <span data-ttu-id="1d3b4-228">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-228">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-229">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-229">Network</span></span>

* <span data-ttu-id="1d3b4-230">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-230">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1d3b4-231">Rdbms</span></span>

* <span data-ttu-id="1d3b4-232">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-232">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-233">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-233">Role</span></span>

* <span data-ttu-id="1d3b4-234">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-234">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="1d3b4-235">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-235">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1d3b4-236">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1d3b4-236">Service Fabric</span></span>

* <span data-ttu-id="1d3b4-237">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-237">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="1d3b4-238">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-238">February 26, 2019</span></span>

<span data-ttu-id="1d3b4-239">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="1d3b4-239">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-240">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-240">Core</span></span>

* <span data-ttu-id="1d3b4-241">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-241">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-242">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-242">ACR</span></span>

* <span data-ttu-id="1d3b4-243">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-243">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="1d3b4-244">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-244">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-245">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-245">ACS</span></span>

* <span data-ttu-id="1d3b4-246">??에 `--listen-address` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-246">Added `--listen-address` option to</span></span> `aks port-forward`

### <a name="appservice"></a><span data-ttu-id="1d3b4-247">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-247">AppService</span></span>

* <span data-ttu-id="1d3b4-248">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-248">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-249">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-249">Batch</span></span>
* <span data-ttu-id="1d3b4-250">[호환성이 손상되는 변경] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-250">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="1d3b4-251">[호환성이 손상되는 변경] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-251">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="1d3b4-252">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-252">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="1d3b4-253">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-253">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="1d3b4-254">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-254">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="1d3b4-255">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-255">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-256">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-256">CosmosDB</span></span>

* <span data-ttu-id="1d3b4-257">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-257">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="1d3b4-258">Kusto</span><span class="sxs-lookup"><span data-stu-id="1d3b4-258">Kusto</span></span>

* <span data-ttu-id="1d3b4-259">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-259">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-260">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-260">Network</span></span>

* <span data-ttu-id="1d3b4-261">??에 `--express-route-gateway-bypass` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-261">Added `--express-route-gateway-bypass` argument to</span></span> `vpn-connection [create|update]`
* <span data-ttu-id="1d3b4-262">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-262">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="1d3b4-263">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-263">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="1d3b4-264">??에 `--legacy-mode` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-264">Added argument `--legacy-mode` to</span></span> `express-route peering [create|update]` 
* <span data-ttu-id="1d3b4-265">??에 `--allow-classic-operations` 및 `--express-route-port` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-265">Added arguments `--allow-classic-operations` and `--express-route-port` to</span></span> `express-route [create|update]`
* <span data-ttu-id="1d3b4-266">??에 `--gateway-default-site` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-266">Added `--gateway-default-site` argument to</span></span> `vnet-gateway [create|update]`
* <span data-ttu-id="1d3b4-267">??에 `ipsec-policy` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-267">Added `ipsec-policy` commands to</span></span> `vnet-gateway`

### <a name="resource"></a><span data-ttu-id="1d3b4-268">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-268">Resource</span></span>

* <span data-ttu-id="1d3b4-269">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-269">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="1d3b4-270">??에 URI 기반 매개 변수 파일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-270">Added support for URI-based parameters file to</span></span> `policy assignment create`
* <span data-ttu-id="1d3b4-271">??에 URI 기반 매개 변수 및 정의에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-271">Added support for URI-based parameters and definitions to</span></span> `policy set-definition update`
* <span data-ttu-id="1d3b4-272">??에 대한 매개 변수 및 규칙 처리 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-272">Fixed handling of parameters and rules for</span></span> `policy definition update`
* <span data-ttu-id="1d3b4-273">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-273">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-274">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-274">Role</span></span>

* <span data-ttu-id="1d3b4-275">??에 앱 역할에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-275">Added support for app roles to</span></span> `ad app [create|update]`

### <a name="vm"></a><span data-ttu-id="1d3b4-276">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-276">VM</span></span>

* <span data-ttu-id="1d3b4-277">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-277">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="1d3b4-278">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-278">February 12, 2019</span></span>

<span data-ttu-id="1d3b4-279">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="1d3b4-279">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-280">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-280">Core</span></span>

* `az --version` <span data-ttu-id="1d3b4-281">이제 업데이트할 수 있는 패키지를 포함하는 경우 알림을 표시</span><span class="sxs-lookup"><span data-stu-id="1d3b4-281">now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="1d3b4-282">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-282">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-283">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-283">ACR</span></span>
* <span data-ttu-id="1d3b4-284">[호환성이 손상되는 변경] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-284">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="1d3b4-285">[호환성이 손상되는 변경] ??에서 `--tag` 및 `--manifest` 옵션 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-285">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from</span></span> `acr repository delete`

### <a name="acs"></a><span data-ttu-id="1d3b4-286">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-286">ACS</span></span>
* <span data-ttu-id="1d3b4-287">??에 대/소문자를 구분하지 않는 이름에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-287">Added support for case-insensitive names to</span></span> `aks [enable-addons|disable-addons]`
* <span data-ttu-id="1d3b4-288">??을(를) 사용하여 Azure Active Directory 업데이트 작업에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-288">Added support for Azure Active Directory updating operation using</span></span> `aks update-credentials --reset-aad`
* <span data-ttu-id="1d3b4-289">??에 대한 `--output`은 무시된다는 설명 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-289">Added clarification that `--output` is ignored for</span></span> `aks get-credentials`

### <a name="ams"></a><span data-ttu-id="1d3b4-290">AMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-290">AMS</span></span>
* <span data-ttu-id="1d3b4-291">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-291">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="1d3b4-292">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-292">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-293">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-293">Appservice</span></span>
* <span data-ttu-id="1d3b4-294">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-294">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="1d3b4-295">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-295">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="1d3b4-296">??에 대한 도움말 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-296">Improved help for</span></span> `appservice-plan-update`
* <span data-ttu-id="1d3b4-297">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-297">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="1d3b4-298">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-298">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="1d3b4-299">Botservice</span><span class="sxs-lookup"><span data-stu-id="1d3b4-299">Botservice</span></span>
* <span data-ttu-id="1d3b4-300">??에 대한 UX 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-300">Improved UX for</span></span> `bot publish`
* <span data-ttu-id="1d3b4-301">?? 중에 `npm install`을 실행할 때 시간 제한에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-301">Added warning for timeouts when running `npm install` during</span></span> `az bot publish`
* <span data-ttu-id="1d3b4-302">??의 `--name`에서 잘못된 문자 `.` 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-302">Removed invalid char `.` from `--name`  in</span></span> `az bot create`
* <span data-ttu-id="1d3b4-303">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-303">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="1d3b4-304">[사용되지 않음] ??을(를) 위해 `--proj-name`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-304">[DEPRECATED] Deprecated `--proj-name` argument in favor of</span></span> `--proj-file-path`
* <span data-ttu-id="1d3b4-305">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-305">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="1d3b4-306">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-306">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="1d3b4-307">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-307">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="1d3b4-308">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-308">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="1d3b4-309">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-309">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="1d3b4-310">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-310">Key Vault</span></span>
* <span data-ttu-id="1d3b4-311">??을(를) 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 수신하는 `keyvault secret backup` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-311">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using</span></span> `--id`

### <a name="monitor"></a><span data-ttu-id="1d3b4-312">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-312">Monitor</span></span>
* <span data-ttu-id="1d3b4-313">차원 값을 허용하도록 `monitor metrics alert [create|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-313">Changed `monitor metrics alert [create|update]` to allow dimension value</span></span> `*`

### <a name="network"></a><span data-ttu-id="1d3b4-314">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-314">Network</span></span>
* <span data-ttu-id="1d3b4-315">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-315">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="1d3b4-316">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-316">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="1d3b4-317">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-317">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="1d3b4-318">??에 `--idle-timeout` 및 `--floating-ip` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-318">Added `--idle-timeout` and `--floating-ip` to</span></span> `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a><span data-ttu-id="1d3b4-319">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1d3b4-319">Policy Insights</span></span>
* <span data-ttu-id="1d3b4-320">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-320">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-321">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-321">RDBMS</span></span>
* <span data-ttu-id="1d3b4-322">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-322">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="1d3b4-323">Redis</span><span class="sxs-lookup"><span data-stu-id="1d3b4-323">Redis</span></span>
* <span data-ttu-id="1d3b4-324">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-324">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="1d3b4-325">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-325">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="1d3b4-326">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-326">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="1d3b4-327">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-327">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="1d3b4-328">[호환성이 손상되는 변경] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-328">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="1d3b4-329">[호환성이 손상되는 변경] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-329">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="1d3b4-330">[사용되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-330">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-331">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-331">Role</span></span>
* <span data-ttu-id="1d3b4-332">[호환성이 손상되는 변경] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-332">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="1d3b4-333">SQL VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-333">SQL VM</span></span>
* <span data-ttu-id="1d3b4-334">[사용되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-334">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-335">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-335">VM</span></span>
* <span data-ttu-id="1d3b4-336">?? 대신 `--all`을 사용할 수 있도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-336">Changed `vm list-skus` to allow use of `--all` in place of</span></span> `--all true`
* <span data-ttu-id="1d3b4-337">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-337">Added</span></span> `vmss run-command [invoke | list | show]`
* <span data-ttu-id="1d3b4-338">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-338">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="1d3b4-339">[호환성이 손상되는 변경] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-339">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="1d3b4-340">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-340">January 31, 2019</span></span>

<span data-ttu-id="1d3b4-341">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="1d3b4-341">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-342">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-342">Core</span></span>

* <span data-ttu-id="1d3b4-343">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-343">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="1d3b4-344">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-344">January 28, 2019</span></span>

<span data-ttu-id="1d3b4-345">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="1d3b4-345">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-346">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-346">ACR</span></span>
* <span data-ttu-id="1d3b4-347">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-347">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-348">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-348">ACS</span></span>
* <span data-ttu-id="1d3b4-349">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-349">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1d3b4-350">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-350">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="1d3b4-351">??을(를) 사용하여 서비스 주체 업데이트 작업에 대한 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-351">Added support for service principal updates operation with</span></span> `aks update-credentials -reset-service-principal`

### <a name="ams"></a><span data-ttu-id="1d3b4-352">AMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-352">AMS</span></span>
* <span data-ttu-id="1d3b4-353">[호환성이 손상되는 변경] `ams asset get-streaming-locators`의 이름을 다음으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-353">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to</span></span> `ams asset list-streaming-locators`
* <span data-ttu-id="1d3b4-354">[호환성이 손상되는 변경] `ams streaming-locator get-content-keys`의 이름을 다음으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-354">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to</span></span> `ams streaming-locator list-content-keys`

### <a name="appservice"></a><span data-ttu-id="1d3b4-355">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-355">Appservice</span></span>
* <span data-ttu-id="1d3b4-356">??에 App Insights에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-356">Added support for app insights on</span></span> `functionapp create`
* <span data-ttu-id="1d3b4-357">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 Function Apps에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-357">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="1d3b4-358">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-358">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-359">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-359">Container</span></span>
* <span data-ttu-id="1d3b4-360">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-360">Added `container start` command</span></span>
* <span data-ttu-id="1d3b4-361">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-361">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1d3b4-362">EventGrid</span><span class="sxs-lookup"><span data-stu-id="1d3b4-362">EventGrid</span></span>
* <span data-ttu-id="1d3b4-363">??에 `--deadletter-endpoint` 매개 변수가 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-363">Added `--deadletter-endpoint` parameter to</span></span> `event-subscription [create|update]`
* <span data-ttu-id="1d3b4-364">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-364">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="1d3b4-365">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-365">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="1d3b4-366">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-366">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="1d3b4-367">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-367">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1d3b4-368">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1d3b4-368">HDInsight</span></span>
* <span data-ttu-id="1d3b4-369">[호환성이 손상되는 변경] ??에서 `--virtual-network` 및 `--subnet-name` 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-369">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from</span></span> `hdinsight [application] create`
* <span data-ttu-id="1d3b4-370">[호환성이 손상되는 변경] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-370">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="1d3b4-371">??에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-371">Added `--vnet-name` and `--subnet-name` parameters to</span></span> `hdinsight create`
* <span data-ttu-id="1d3b4-372">??에 Enterprise Security Package 및 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-372">Added support for Enterprise Security Package and disk encryption to</span></span> `hdinsight create` 
* <span data-ttu-id="1d3b4-373">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-373">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="1d3b4-374">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-374">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-375">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-375">IoT</span></span>
* <span data-ttu-id="1d3b4-376">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-376">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="1d3b4-377">Kusto</span><span class="sxs-lookup"><span data-stu-id="1d3b4-377">Kusto</span></span>
* <span data-ttu-id="1d3b4-378">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-378">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-379">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-379">Monitor</span></span>
* <span data-ttu-id="1d3b4-380">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-380">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="1d3b4-381">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-381">Profile</span></span>
* <span data-ttu-id="1d3b4-382">??에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-382">Enable tenant level account for managed service identity for</span></span> `login`

### <a name="network"></a><span data-ttu-id="1d3b4-383">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-383">Network</span></span>
* <span data-ttu-id="1d3b4-384">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-384">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="1d3b4-385">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-385">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-386">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-386">Resource</span></span>
* <span data-ttu-id="1d3b4-387">??에 URI 매개 변수 파일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-387">Added support for URI parameters file to</span></span> `group deployment create`
* <span data-ttu-id="1d3b4-388">??에 관리 ID에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-388">Added support for managed identity to</span></span> `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a><span data-ttu-id="1d3b4-389">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="1d3b4-389">SQL Virtual Machine</span></span>
* <span data-ttu-id="1d3b4-390">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-390">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-391">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-391">Storage</span></span>
* <span data-ttu-id="1d3b4-392">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-392">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="1d3b4-393">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-393">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-394">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-394">VM</span></span>
* <span data-ttu-id="1d3b4-395">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-395">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="1d3b4-396">??에 `--force` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-396">Added `--force` flag to</span></span> `vm encryption enable`

## <a name="january-15-2019"></a><span data-ttu-id="1d3b4-397">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-397">January 15, 2019</span></span>

<span data-ttu-id="1d3b4-398">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="1d3b4-398">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-399">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-399">ACR</span></span>
* <span data-ttu-id="1d3b4-400">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-400">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="1d3b4-401">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-401">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="1d3b4-402">[사용되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-402">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="1d3b4-403">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-403">ACS</span></span>
* <span data-ttu-id="1d3b4-404">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-404">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-405">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-405">Appservice</span></span>
* <span data-ttu-id="1d3b4-406">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-406">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="1d3b4-407">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-407">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="1d3b4-408">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-408">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="1d3b4-409">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-409">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="1d3b4-410">Botservice</span><span class="sxs-lookup"><span data-stu-id="1d3b4-410">Botservice</span></span>
* <span data-ttu-id="1d3b4-411">??에 배포 상태 업데이트 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-411">Added deployment status updates to</span></span> `bot create`

### <a name="configure"></a><span data-ttu-id="1d3b4-412">구성</span><span class="sxs-lookup"><span data-stu-id="1d3b4-412">Configure</span></span>
* <span data-ttu-id="1d3b4-413">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-413">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-414">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-414">CosmosDB</span></span>
* <span data-ttu-id="1d3b4-415">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-415">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1d3b4-416">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1d3b4-416">HDInsight</span></span>
* <span data-ttu-id="1d3b4-417">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-417">Added commands for managing applications</span></span>
* <span data-ttu-id="1d3b4-418">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-418">Added commands for managing script actions</span></span>
* <span data-ttu-id="1d3b4-419">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-419">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="1d3b4-420">??에 지역별 사용량을 나열하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-420">Added support to list regional usage to</span></span> `hdinsight list-usage`
* <span data-ttu-id="1d3b4-421">[호환성이 손상되는 변경] ??에서 기본 클러스터 유형 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-421">[BREAKING CHANGE] Removed default cluster type from</span></span> `hdinsight create`

### <a name="network"></a><span data-ttu-id="1d3b4-422">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-422">Network</span></span>
* <span data-ttu-id="1d3b4-423">??에 `--custom-headers` 및 `--status-code-ranges` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-423">Added `--custom-headers` and `--status-code-ranges` arguments to</span></span> `traffic-manager profile [create|update]`
* <span data-ttu-id="1d3b4-424">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-424">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="1d3b4-425">??에 `--custom-headers` 및 `--subnets` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-425">Added `--custom-headers` and `--subnets` arguments to</span></span> `traffic-manager endpoint [create|update]`  
* <span data-ttu-id="1d3b4-426">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-426">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-427">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-427">Role</span></span>
* <span data-ttu-id="1d3b4-428">[사용되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-428">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="1d3b4-429">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-429">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="1d3b4-430">보안</span><span class="sxs-lookup"><span data-stu-id="1d3b4-430">Security</span></span>
* <span data-ttu-id="1d3b4-431">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-431">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-432">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-432">Storage</span></span>
* <span data-ttu-id="1d3b4-433">[호환성이 손상되는 변경] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-433">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="1d3b4-434">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-434">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="1d3b4-435">??에 `--marker` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-435">Added `--marker` parameter to</span></span> `storage [blob|file|container|share] list`
* <span data-ttu-id="1d3b4-436">??의 STDERR에 다음 페이지에 대한 로그 표식 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-436">Added log marker for next page to STDERR for</span></span> `storage [blob|file|container|share] list` 
* <span data-ttu-id="1d3b4-437">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-437">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-438">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-438">VM</span></span>
* <span data-ttu-id="1d3b4-439">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-439">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="1d3b4-440">??을(를) 참조하는 테넌트 간 이미지에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-440">Added support for cross tenant image referencing to</span></span> `[vm|vmss] create`
* <span data-ttu-id="1d3b4-441">??의 기본 구성에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-441">Fixed bug with default configuration in</span></span> `vm diagnostics get-default-config --windows-os`
* <span data-ttu-id="1d3b4-442">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-442">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="1d3b4-443">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-443">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="1d3b4-444">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-444">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="1d3b4-445">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-445">December 20, 2018</span></span>

<span data-ttu-id="1d3b4-446">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="1d3b4-446">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="1d3b4-447">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-447">Appservice</span></span>
* <span data-ttu-id="1d3b4-448">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-448">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="1d3b4-449">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-449">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="1d3b4-450">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-450">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1d3b4-451">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="1d3b4-451">IoTCentral</span></span>
* <span data-ttu-id="1d3b4-452">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-452">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-453">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-453">Role</span></span>
* <span data-ttu-id="1d3b4-454">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-454">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-455">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-455">SQL</span></span>
* <span data-ttu-id="1d3b4-456">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-456">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-457">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-457">VM</span></span>
* <span data-ttu-id="1d3b4-458">??에 `---os-type` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-458">Added `---os-type` parameter to</span></span> `disk create`

## <a name="december-18-2018"></a><span data-ttu-id="1d3b4-459">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-459">December 18, 2018</span></span>

<span data-ttu-id="1d3b4-460">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="1d3b4-460">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="1d3b4-461">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-461">ACR</span></span>
* <span data-ttu-id="1d3b4-462">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-462">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="1d3b4-463">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-463">Condensed the table layout for task list</span></span>
* <span data-ttu-id="1d3b4-464">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-464">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-465">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-465">ACS</span></span>
* <span data-ttu-id="1d3b4-466">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-466">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="1d3b4-467">??에 대한 AAD 인수에서 "(미리 보기)" 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-467">Removed "(PREVIEW)" from AAD arguments to</span></span> `aks create`
* <span data-ttu-id="1d3b4-468">[사용되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-468">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="1d3b4-469">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-469">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="1d3b4-470">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-470">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="1d3b4-471">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-471">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-472">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-472">Appservice</span></span>
* <span data-ttu-id="1d3b4-473">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-473">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="1d3b4-474">Botservice</span><span class="sxs-lookup"><span data-stu-id="1d3b4-474">Botservice</span></span>
* <span data-ttu-id="1d3b4-475">??을(를) 호출할 때 `.bot` 파일 구문 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-475">Added support for `.bot` file parsing when calling</span></span> `bot show`
* <span data-ttu-id="1d3b4-476">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-476">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="1d3b4-477">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-477">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="1d3b4-478">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-478">Reduced Kudu network calls</span></span>
* <span data-ttu-id="1d3b4-479">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-479">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="1d3b4-480">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-480">Consumption</span></span>
* <span data-ttu-id="1d3b4-481">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-481">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-482">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-482">CosmosDB</span></span>
* <span data-ttu-id="1d3b4-483">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-483">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="1d3b4-484">지도</span><span class="sxs-lookup"><span data-stu-id="1d3b4-484">Maps</span></span>
* <span data-ttu-id="1d3b4-485">??에 S1 SKU에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-485">Added support for the S1 SKU to</span></span> `maps account [create|update]`

### <a name="network"></a><span data-ttu-id="1d3b4-486">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-486">Network</span></span>
* <span data-ttu-id="1d3b4-487">??에 `--format` 및 `--log-version`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-487">Added support for `--format` and `--log-version` to</span></span> `watcher flow-log configure`
* <span data-ttu-id="1d3b4-488">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-488">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-489">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-489">Resource</span></span>
* <span data-ttu-id="1d3b4-490">??에서 관리 그룹에 대한 범위 매개 변수 처리 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-490">Fixed handling of scope parameter for management groups in</span></span> `policy assignment [create|list|delete|show|update]` 
* <span data-ttu-id="1d3b4-491">새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-491">Added new command</span></span> `resource wait`

### <a name="storage"></a><span data-ttu-id="1d3b4-492">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-492">Storage</span></span>
*  <span data-ttu-id="1d3b4-493">??에 스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-493">Added ability to update log schema version for storage services in</span></span> `storage logging update`

### <a name="vm"></a><span data-ttu-id="1d3b4-494">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-494">VM</span></span>
* <span data-ttu-id="1d3b4-495">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-495">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="1d3b4-496">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-496">December 4, 2018</span></span>

<span data-ttu-id="1d3b4-497">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="1d3b4-497">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="1d3b4-498">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-498">Core</span></span>
* <span data-ttu-id="1d3b4-499">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-499">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="1d3b4-500">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-500">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-501">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-501">Appservice</span></span>
* <span data-ttu-id="1d3b4-502">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-502">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="1d3b4-503">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-503">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-504">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-504">Network</span></span>
* <span data-ttu-id="1d3b4-505">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-505">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-506">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-506">Role</span></span>
* <span data-ttu-id="1d3b4-507">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-507">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="1d3b4-508">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-508">VM</span></span>
* <span data-ttu-id="1d3b4-509">[사용되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-509">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="1d3b4-510">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-510">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="1d3b4-511">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-511">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="1d3b4-512">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-512">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="1d3b4-513">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-513">November 20, 2018</span></span>

<span data-ttu-id="1d3b4-514">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="1d3b4-514">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="1d3b4-515">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-515">Core</span></span>
* <span data-ttu-id="1d3b4-516">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-516">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-517">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-517">ACR</span></span>
* <span data-ttu-id="1d3b4-518">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-518">Added context token to task step</span></span>
* <span data-ttu-id="1d3b4-519">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-519">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="1d3b4-520">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-520">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-521">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-521">Appservice</span></span>
* <span data-ttu-id="1d3b4-522">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-522">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="1d3b4-523">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-523">Updated the default `node_version`.</span></span> <span data-ttu-id="1d3b4-524">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-524">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="1d3b4-525">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-525">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="1d3b4-526">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-526">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="1d3b4-527">IotCentral</span><span class="sxs-lookup"><span data-stu-id="1d3b4-527">IotCentral</span></span>
* <span data-ttu-id="1d3b4-528">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-528">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-529">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-529">KeyVault</span></span>
* <span data-ttu-id="1d3b4-530">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-530">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-531">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-531">Network</span></span>
* <span data-ttu-id="1d3b4-532">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-532">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="1d3b4-533">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-533">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="1d3b4-534">??에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-534">Added `--zones` for availability zone support to</span></span> `application-gateway create` 
* <span data-ttu-id="1d3b4-535">??에 `--file-upload-limit`, `--max-request-body-size` 및 `--request-body-check` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-535">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to</span></span> `application-gateway waf-config set`

### <a name="rdbms"></a><span data-ttu-id="1d3b4-536">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1d3b4-536">Rdbms</span></span>
* <span data-ttu-id="1d3b4-537">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-537">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="1d3b4-538">Rbac</span><span class="sxs-lookup"><span data-stu-id="1d3b4-538">Rbac</span></span>
* <span data-ttu-id="1d3b4-539">??에서 변경이 불가능한 자격 증명의 업데이트를 시도하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-539">Fixed an issue with attempting to update immutable credentials in</span></span> `ad app update`
* <span data-ttu-id="1d3b4-540">??에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-540">Added output warnings to communicate breaking changes in the near future for</span></span> `ad [app|sp] list` 

### <a name="storage"></a><span data-ttu-id="1d3b4-541">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-541">Storage</span></span>
* <span data-ttu-id="1d3b4-542">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-542">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="1d3b4-543">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-543">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="1d3b4-544">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-544">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="1d3b4-545">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-545">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-546">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-546">VM</span></span>
* <span data-ttu-id="1d3b4-547">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-547">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="1d3b4-548">`sig image-version`에 대한 버전 이름 매개 변수를 ??이(가) 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-548">Changed version name parameters to `sig image-version` to be</span></span> `--image-version -e`
* <span data-ttu-id="1d3b4-549">`sig image-version` 인수 `--image-version-name` 사용되지 않음, 다음으로 바꿈</span><span class="sxs-lookup"><span data-stu-id="1d3b4-549">Deprecated `sig image-version` argument `--image-version-name`, replaced by</span></span> `--image-version`
* <span data-ttu-id="1d3b4-550">??에 로컬 OS 디스크를 사용하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-550">Added support to use local OS disk to</span></span> `[vm|vmss] create --ephemeral-os-disk`
* <span data-ttu-id="1d3b4-551">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-551">Added support for `--no-wait` to</span></span> `snapshot create/update`
* <span data-ttu-id="1d3b4-552">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-552">Added `snapshot wait` command</span></span>
* <span data-ttu-id="1d3b4-553">??에 인스턴스 이름을 사용하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-553">Added support for using instance name with</span></span> `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a><span data-ttu-id="1d3b4-554">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-554">November 6, 2018</span></span>

<span data-ttu-id="1d3b4-555">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="1d3b4-555">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-556">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-556">Core</span></span>
* <span data-ttu-id="1d3b4-557">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-557">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-558">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-558">ACR</span></span>
* <span data-ttu-id="1d3b4-559">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-559">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="1d3b4-560">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-560">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-561">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-561">ACS</span></span>
* <span data-ttu-id="1d3b4-562">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-562">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="1d3b4-563">Advisor</span><span class="sxs-lookup"><span data-stu-id="1d3b4-563">Advisor</span></span>
* <span data-ttu-id="1d3b4-564">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-564">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="1d3b4-565">AMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-565">AMS</span></span>
* <span data-ttu-id="1d3b4-566">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-566">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="1d3b4-567">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-567">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="1d3b4-568">??에 암호화 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-568">Added encryption parameters support to</span></span> `ams streaming-policy create`
* <span data-ttu-id="1d3b4-569">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-569">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="1d3b4-570">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-570">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="1d3b4-571">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-571">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="1d3b4-572">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-572">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="1d3b4-573">[호환성이 손상되는 변경] `ams streaming locator` 명령을 ??(으)로 대체</span><span class="sxs-lookup"><span data-stu-id="1d3b4-573">[BREAKING CHANGE] Replaced `ams streaming locator` command with</span></span> `ams streaming-locator`
* <span data-ttu-id="1d3b4-574">[호환성이 손상되는 변경] ??의 `--content-keys` 인수 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-574">[BREAKING CHANGE] Updated `--content-keys` argument of</span></span> `ams streaming locator`
* <span data-ttu-id="1d3b4-575">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-575">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="1d3b4-576">[호환성이 손상되는 변경] `ams streaming policy` 명령을 ??(으)로 대체</span><span class="sxs-lookup"><span data-stu-id="1d3b4-576">[BREAKING CHANGE] Replaced `ams streaming policy` command with</span></span> `ams streaming-policy`
* <span data-ttu-id="1d3b4-577">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-577">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="1d3b4-578">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-578">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="1d3b4-579">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="1d3b4-579">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="1d3b4-580">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-580">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="1d3b4-581">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-581">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="1d3b4-582">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-582">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-583">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-583">AppService</span></span>
* <span data-ttu-id="1d3b4-584">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-584">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="1d3b4-585">구성</span><span class="sxs-lookup"><span data-stu-id="1d3b4-585">Configure</span></span>
* <span data-ttu-id="1d3b4-586">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-586">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-587">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-587">Container</span></span>
* <span data-ttu-id="1d3b4-588">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-588">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="1d3b4-589">EventHub</span><span class="sxs-lookup"><span data-stu-id="1d3b4-589">EventHub</span></span>
* <span data-ttu-id="1d3b4-590">??에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-590">Added `--enable-kafka` flag to support Kafka in</span></span> `eventhub namespace [create|update]`

### <a name="interactive"></a><span data-ttu-id="1d3b4-591">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-591">Interactive</span></span>
* <span data-ttu-id="1d3b4-592">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-592">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-593">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-593">Monitor</span></span>
* <span data-ttu-id="1d3b4-594">??의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-594">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="1d3b4-595">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-595">Network</span></span>
* <span data-ttu-id="1d3b4-596">??을(를) 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-596">Deprecated `network interface-endpoint` command names in favor of</span></span> `network private-endpoint`
* <span data-ttu-id="1d3b4-597">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-597">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="1d3b4-598">`--ip-tags`가 ??에서 제대로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-598">Fixed issue where `--ip-tags` did not work correctly with</span></span> `public-ip create` 

### <a name="profile"></a><span data-ttu-id="1d3b4-599">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-599">Profile</span></span>
* <span data-ttu-id="1d3b4-600">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-600">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-601">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-601">RDBMS</span></span>
* <span data-ttu-id="1d3b4-602">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-602">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-603">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-603">Resource</span></span>
* <span data-ttu-id="1d3b4-604">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-604">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-605">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-605">Role</span></span>
* <span data-ttu-id="1d3b4-606">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-606">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="1d3b4-607">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-607">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="1d3b4-608">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-608">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-609">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-609">Storage</span></span>
* <span data-ttu-id="1d3b4-610">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-610">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-611">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-611">VM</span></span>
* <span data-ttu-id="1d3b4-612">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-612">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="1d3b4-613">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-613">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="1d3b4-614">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-614">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="1d3b4-615">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-615">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="1d3b4-616">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="1d3b4-616">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="1d3b4-617">??에 대한 인수 유효성 검사 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-617">Improved argument validation for</span></span> `vm create --image`

## <a name="october-23-2018"></a><span data-ttu-id="1d3b4-618">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-618">October 23, 2018</span></span>

<span data-ttu-id="1d3b4-619">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="1d3b4-619">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-620">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-620">Core</span></span>
* <span data-ttu-id="1d3b4-621">`--subscription`이 ??의 구독보다 우선적으로 적용되는 `--ids` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-621">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in</span></span> `--ids`
* <span data-ttu-id="1d3b4-622">??을(를) 사용하여 매개 변수가 무시되는 경우 명시적 경고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-622">Added explicit warnings when parameters would be ignored by use of</span></span> `--ids`

### <a name="acr"></a><span data-ttu-id="1d3b4-623">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-623">ACR</span></span>
* <span data-ttu-id="1d3b4-624">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-624">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="1d3b4-625">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-625">CDN</span></span>
* <span data-ttu-id="1d3b4-626">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-626">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="1d3b4-627">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-627">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-628">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-628">Container</span></span>
* <span data-ttu-id="1d3b4-629">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-629">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="1d3b4-630">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-630">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="1d3b4-631">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-631">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="1d3b4-632">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-632">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="1d3b4-633">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-633">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="1d3b4-634">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-634">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="1d3b4-635">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-635">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-636">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-636">CosmosDB</span></span>
* <span data-ttu-id="1d3b4-637">??에 `--enable-multiple-write-locations` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-637">Added `--enable-multiple-write-locations` support to</span></span> `cosmosdb create`

### <a name="interactive"></a><span data-ttu-id="1d3b4-638">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-638">Interactive</span></span>
* <span data-ttu-id="1d3b4-639">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-639">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="1d3b4-640">IoT Central</span><span class="sxs-lookup"><span data-stu-id="1d3b4-640">IoT Central</span></span>
* <span data-ttu-id="1d3b4-641">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-641">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="1d3b4-642">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-642">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-643">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-643">Monitor</span></span>
* <span data-ttu-id="1d3b4-644">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-644">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="1d3b4-645">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-645">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="1d3b4-646">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-646">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1d3b4-647">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-647">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="1d3b4-648">`--namespace`를 사용되지 않는 옵션 ??에 대한 별칭으로 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-648">Added `--namespace` as alias for deprecated option</span></span> `--resource-provider`
  * <span data-ttu-id="1d3b4-649">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-649">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="1d3b4-650">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-650">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="1d3b4-651">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-651">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="1d3b4-652">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-652">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="1d3b4-653">??에 대한 `--event-hub` 및 `--event-hub-rule` 인수 유효성 검사 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-653">Improved validation for `--event-hub` and `--event-hub-rule` arguments to</span></span> `monitor diagnostic-settings create`

### <a name="network"></a><span data-ttu-id="1d3b4-654">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-654">Network</span></span>
* <span data-ttu-id="1d3b4-655">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-655">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="1d3b4-656">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-656">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="1d3b4-657">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1d3b4-657">ServiceBus</span></span>
* <span data-ttu-id="1d3b4-658">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-658">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-659">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-659">SQL</span></span>
* <span data-ttu-id="1d3b4-660">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-660">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-661">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-661">Storage</span></span>
* <span data-ttu-id="1d3b4-662">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-662">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="1d3b4-663">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-663">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-664">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-664">VM</span></span>
* <span data-ttu-id="1d3b4-665">??에서 Lv/Lv2 시리즈 머신에 대해 디스크 캐싱 모드가 `None`이 되도록 적용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-665">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in</span></span> `[vm|vmss] create`
* <span data-ttu-id="1d3b4-666">??에 대해 지원되는 크기 목록 지원 네트워킹 가속기 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-666">Updated supported size list supporting networking accelerator for</span></span> `vm create`
* <span data-ttu-id="1d3b4-667">??에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-667">Added strong typed arguments for ultrassd iops and mbps configs for</span></span> `disk create`

## <a name="october-16-2018"></a><span data-ttu-id="1d3b4-668">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-668">October 16, 2018</span></span>

<span data-ttu-id="1d3b4-669">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="1d3b4-669">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-670">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-670">VM</span></span>
* <span data-ttu-id="1d3b4-671">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-671">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="1d3b4-672">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-672">October 9, 2018</span></span>

<span data-ttu-id="1d3b4-673">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="1d3b4-673">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-674">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-674">Core</span></span>
* <span data-ttu-id="1d3b4-675">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-675">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-676">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-676">ACR</span></span>
* <span data-ttu-id="1d3b4-677">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-677">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-678">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-678">ACS</span></span>
* <span data-ttu-id="1d3b4-679">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="1d3b4-679">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="1d3b4-680">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-680">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="1d3b4-681">`aks create`가 더 이상 ??을(를) 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-681">Changed `aks create` to no longer require</span></span> `--aad-tenant-id`
* <span data-ttu-id="1d3b4-682">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-682">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-683">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-683">Container</span></span>
* <span data-ttu-id="1d3b4-684">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-684">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="1d3b4-685">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-685">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="1d3b4-686">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="1d3b4-686">Event Hub</span></span>
* <span data-ttu-id="1d3b4-687">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-687">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="1d3b4-688">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-688">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="1d3b4-689">확장</span><span class="sxs-lookup"><span data-stu-id="1d3b4-689">Extensions</span></span>
* <span data-ttu-id="1d3b4-690">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-690">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="1d3b4-691">HDInsight</span><span class="sxs-lookup"><span data-stu-id="1d3b4-691">HDInsight</span></span>
* <span data-ttu-id="1d3b4-692">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-692">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-693">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-693">IoT</span></span>
* <span data-ttu-id="1d3b4-694">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-694">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-695">KeyVault</span></span>
* <span data-ttu-id="1d3b4-696">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-696">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-697">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-697">Network</span></span>
* <span data-ttu-id="1d3b4-698">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-698">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="1d3b4-699">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="1d3b4-699">See #6052</span></span>
* <span data-ttu-id="1d3b4-700">??에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-700">Deprecated `--remote-vnet-id` for</span></span> `network vnet peering create`
* <span data-ttu-id="1d3b4-701">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-701">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="1d3b4-702">??에서 `network vnet create`에 대한 여러 서브넷 접두사 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-702">Added support for multiple subnet prefixes to `network vnet create` with</span></span> `--subnet-prefixes`
* <span data-ttu-id="1d3b4-703">??에서 `network vnet subnet [create|update]`에 대한 여러 서브넷 접두사 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-703">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with</span></span> `--address-prefixes`
* <span data-ttu-id="1d3b4-704">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-704">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="1d3b4-705">??에 `--service-endpoint-policy` 편의 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-705">Added `--service-endpoint-policy` convenience argument to</span></span> `network vnet subnet update`

### <a name="role"></a><span data-ttu-id="1d3b4-706">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-706">Role</span></span>
* <span data-ttu-id="1d3b4-707">??에 Azure AD 앱 소유자를 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-707">Added support for listing Azure AD app owners to</span></span> `ad app owner`
* <span data-ttu-id="1d3b4-708">??에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-708">Added support for listing Azure AD service principal owners to</span></span> `ad sp owner`
* <span data-ttu-id="1d3b4-709">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-709">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="1d3b4-710">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-710">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="1d3b4-711">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1d3b4-711">Service Bus</span></span>
* <span data-ttu-id="1d3b4-712">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-712">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-713">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-713">VM</span></span>
* <span data-ttu-id="1d3b4-714">?? 내의 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-714">Fixed empty `accessSas` field in</span></span> `disk grant-access`
* <span data-ttu-id="1d3b4-715">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-715">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="1d3b4-716">??에 대한 업데이트 명령 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-716">Fixed update commands for</span></span> `sig`
* <span data-ttu-id="1d3b4-717">??에 이미지 버전 관리를 위한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-717">Added `--no-wait` support for managing image versions in</span></span> `sig`
* <span data-ttu-id="1d3b4-718">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-718">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="1d3b4-719">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-719">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="1d3b4-720">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-720">September 21, 2018</span></span>

<span data-ttu-id="1d3b4-721">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="1d3b4-721">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-722">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-722">ACR</span></span>
* <span data-ttu-id="1d3b4-723">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-723">Added ACR Task commands</span></span>
* <span data-ttu-id="1d3b4-724">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-724">Added quick run command</span></span>
* <span data-ttu-id="1d3b4-725">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-725">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="1d3b4-726">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-726">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="1d3b4-727">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-727">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="1d3b4-728">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-728">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-729">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-729">ACS</span></span>
* <span data-ttu-id="1d3b4-730">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-730">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="1d3b4-731">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-731">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-732">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-732">AppService</span></span>

* <span data-ttu-id="1d3b4-733">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-733">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="1d3b4-734">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-734">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="1d3b4-735">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-735">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="1d3b4-736">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-736">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-737">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-737">Batch</span></span>
* <span data-ttu-id="1d3b4-738">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-738">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="1d3b4-739">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-739">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="1d3b4-740">??에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-740">Added `--max-tasks-per-node-option` to</span></span> `batch pool create`
* <span data-ttu-id="1d3b4-741">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-741">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1d3b4-742">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-742">Batch AI</span></span> 
* <span data-ttu-id="1d3b4-743">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-743">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1d3b4-744">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1d3b4-744">Cognitive Services</span></span>
* <span data-ttu-id="1d3b4-745">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-745">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="1d3b4-746">명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-746">Added command</span></span> `cognitiveservices account list-usage`
* <span data-ttu-id="1d3b4-747">명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-747">Added command</span></span> `cognitiveservices account list-kinds`
* <span data-ttu-id="1d3b4-748">명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-748">Added command</span></span> `cognitiveservices account list`
* <span data-ttu-id="1d3b4-749">사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-749">Deprecated</span></span> `cognitiveservices list`
* <span data-ttu-id="1d3b4-750">??에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-750">Changed `--name` to be optional for</span></span> `cognitiveservices account list-skus`

### <a name="container"></a><span data-ttu-id="1d3b4-751">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-751">Container</span></span>
* <span data-ttu-id="1d3b4-752">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-752">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="1d3b4-753">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-753">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="1d3b4-754">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-754">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="1d3b4-755">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-755">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="1d3b4-756">Datalake</span><span class="sxs-lookup"><span data-stu-id="1d3b4-756">Datalake</span></span>
* <span data-ttu-id="1d3b4-757">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-757">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="1d3b4-758">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="1d3b4-758">Interactive Shell</span></span>
* <span data-ttu-id="1d3b4-759">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-759">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="1d3b4-760">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-760">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-761">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-761">IoT</span></span>
* <span data-ttu-id="1d3b4-762">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-762">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="1d3b4-763">Key Vault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-763">Key Vault</span></span>
* <span data-ttu-id="1d3b4-764">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-764">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-765">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-765">Network</span></span>
* <span data-ttu-id="1d3b4-766">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-766">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="1d3b4-767">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-767">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="1d3b4-768">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-768">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="1d3b4-769">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-769">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="1d3b4-770">??에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-770">Add `--enable-tcp-reset` to</span></span> `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* <span data-ttu-id="1d3b4-771">??에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-771">Add `--disable-outbound-snat` to</span></span> `network lb rule create/update`
* <span data-ttu-id="1d3b4-772">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-772">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="1d3b4-773">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-773">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="1d3b4-774">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-774">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* `network express-route create/update`<span data-ttu-id="1d3b4-775">: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-775">: Add `--allow-global-reach` flag</span></span>
* `network vnet subnet create/update`<span data-ttu-id="1d3b4-776">: ??에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-776">: Add support for</span></span> `--delegation`
* <span data-ttu-id="1d3b4-777">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-777">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="1d3b4-778">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-778">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="1d3b4-779">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하는 논리가 수정됨. 사설 IP 주소가 제공되는 경우 정적 할당이 설정됨. 사설 IP 주소가 제공되지 않는 경우나 사설 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-779">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* `dns record-set * create/update`<span data-ttu-id="1d3b4-780">: ??에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-780">: Add support for</span></span> `--target-resource`
* <span data-ttu-id="1d3b4-781">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-781">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="1d3b4-782">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-782">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="1d3b4-783">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-783">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-784">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-784">RDBMS</span></span>
* <span data-ttu-id="1d3b4-785">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-785">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="1d3b4-786">예약</span><span class="sxs-lookup"><span data-stu-id="1d3b4-786">Reservation</span></span>
* <span data-ttu-id="1d3b4-787">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-787">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="1d3b4-788">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-788">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="1d3b4-789">앱 관리</span><span class="sxs-lookup"><span data-stu-id="1d3b4-789">Manage App</span></span>
* <span data-ttu-id="1d3b4-790">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-790">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="1d3b4-791">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-791">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-792">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-792">Role</span></span>
* <span data-ttu-id="1d3b4-793">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-793">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="1d3b4-794">SignalR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-794">SignalR</span></span>
* <span data-ttu-id="1d3b4-795">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-795">First release</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-796">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-796">Storage</span></span>
* <span data-ttu-id="1d3b4-797">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-797">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="1d3b4-798">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-798">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-799">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-799">VM</span></span>
* <span data-ttu-id="1d3b4-800">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-800">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="1d3b4-801">??을(를) 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-801">Added support for shared image gallery through</span></span> `az sig`

## <a name="august-28-2018"></a><span data-ttu-id="1d3b4-802">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-802">August 28, 2018</span></span>

<span data-ttu-id="1d3b4-803">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="1d3b4-803">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-804">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-804">Core</span></span>

* <span data-ttu-id="1d3b4-805">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-805">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="1d3b4-806">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-806">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-807">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-807">ACR</span></span>

* <span data-ttu-id="1d3b4-808">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-808">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="1d3b4-809">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-809">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-810">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-810">ACS</span></span>

* <span data-ttu-id="1d3b4-811">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-811">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="1d3b4-812">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-812">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-813">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-813">AppService</span></span>

* <span data-ttu-id="1d3b4-814">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-814">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="1d3b4-815">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-815">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="1d3b4-816">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-816">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="1d3b4-817">Backup</span><span class="sxs-lookup"><span data-stu-id="1d3b4-817">Backup</span></span>

* <span data-ttu-id="1d3b4-818">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-818">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="1d3b4-819">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-819">Bot Service</span></span>

* <span data-ttu-id="1d3b4-820">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-820">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1d3b4-821">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1d3b4-821">Cognitive Services</span></span>

* <span data-ttu-id="1d3b4-822">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-822">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-823">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-823">IoT</span></span>

* <span data-ttu-id="1d3b4-824">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-824">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-825">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-825">Monitor</span></span>

* <span data-ttu-id="1d3b4-826">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-826">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="1d3b4-827">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="1d3b4-827">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-828">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-828">Network</span></span>

* <span data-ttu-id="1d3b4-829">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-829">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-830">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-830">Resource</span></span>

* <span data-ttu-id="1d3b4-831">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-831">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-832">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-832">Storage</span></span>

* <span data-ttu-id="1d3b4-833">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-833">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-834">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-834">VM</span></span>

* <span data-ttu-id="1d3b4-835">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-835">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="1d3b4-836">??에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-836">Deprecated `--storage-caching` for</span></span> `vm create`

## <a name="auguest-14-2018"></a><span data-ttu-id="1d3b4-837">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-837">Auguest 14, 2018</span></span>

<span data-ttu-id="1d3b4-838">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="1d3b4-838">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-839">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-839">Core</span></span>

* <span data-ttu-id="1d3b4-840">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-840">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="1d3b4-841">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="1d3b4-841">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="1d3b4-842">원격 분석</span><span class="sxs-lookup"><span data-stu-id="1d3b4-842">Telemetry</span></span>

* <span data-ttu-id="1d3b4-843">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="1d3b4-843">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-844">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-844">ACR</span></span>

* <span data-ttu-id="1d3b4-845">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-845">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="1d3b4-846">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-846">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-847">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-847">ACS</span></span>

* <span data-ttu-id="1d3b4-848">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-848">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="1d3b4-849">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-849">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="1d3b4-850">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-850">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="1d3b4-851">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-851">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="1d3b4-852">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-852">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="1d3b4-853">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-853">AppService</span></span>

* <span data-ttu-id="1d3b4-854">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-854">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="1d3b4-855">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-855">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="1d3b4-856">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-856">BatchAI</span></span>

* <span data-ttu-id="1d3b4-857">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-857">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="1d3b4-858">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-858">Container</span></span>

* <span data-ttu-id="1d3b4-859">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-859">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="1d3b4-860">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-860">IoT</span></span>

* <span data-ttu-id="1d3b4-861">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="1d3b4-861">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="1d3b4-862">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-862">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="1d3b4-863">Iot Central</span><span class="sxs-lookup"><span data-stu-id="1d3b4-863">Iot Central</span></span>

* <span data-ttu-id="1d3b4-864">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-864">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-865">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-865">KeyVault</span></span>


* <span data-ttu-id="1d3b4-866">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-866">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="1d3b4-867">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-867">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="1d3b4-868">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-868">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="1d3b4-869">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-869">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="1d3b4-870">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-870">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="1d3b4-871">릴레이</span><span class="sxs-lookup"><span data-stu-id="1d3b4-871">Relay</span></span>

* <span data-ttu-id="1d3b4-872">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-872">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-873">Sql</span><span class="sxs-lookup"><span data-stu-id="1d3b4-873">Sql</span></span>

* <span data-ttu-id="1d3b4-874">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-874">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-875">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-875">Storage</span></span>

* <span data-ttu-id="1d3b4-876">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-876">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="1d3b4-877">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-877">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="1d3b4-878">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-878">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="1d3b4-879">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-879">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="1d3b4-880">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-880">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-881">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-881">VM</span></span>

* <span data-ttu-id="1d3b4-882">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-882">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="1d3b4-883">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-883">July 31, 2018</span></span>

<span data-ttu-id="1d3b4-884">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="1d3b4-884">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-885">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-885">ACR</span></span>

* <span data-ttu-id="1d3b4-886">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-886">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="1d3b4-887">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-887">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-888">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-888">ACS</span></span>

* <span data-ttu-id="1d3b4-889">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-889">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-890">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-890">Batch</span></span>

* <span data-ttu-id="1d3b4-891">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-891">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-892">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-892">Container</span></span>

* <span data-ttu-id="1d3b4-893">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-893">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-894">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-894">Network</span></span>

* <span data-ttu-id="1d3b4-895">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-895">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="1d3b4-896">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-896">Resource</span></span>

* <span data-ttu-id="1d3b4-897">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-897">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="1d3b4-898">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-898">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-899">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-899">Role</span></span>

* <span data-ttu-id="1d3b4-900">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-900">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="1d3b4-901">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-901">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="1d3b4-902">검색</span><span class="sxs-lookup"><span data-stu-id="1d3b4-902">Search</span></span>

* <span data-ttu-id="1d3b4-903">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-903">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="1d3b4-904">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1d3b4-904">Service Bus</span></span>

* <span data-ttu-id="1d3b4-905">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-905">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="1d3b4-906">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-906">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  `--enable-batched-operations` <span data-ttu-id="1d3b4-907">및 ?? 내의 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="1d3b4-907">and `--enable-dead-lettering-on-message-expiration` in</span></span> `queue`
  *  `--dead-letter-on-filter-exceptions` <span data-ttu-id="1d3b4-908">in</span><span class="sxs-lookup"><span data-stu-id="1d3b4-908">in</span></span> `subscriptions`

### <a name="storage"></a><span data-ttu-id="1d3b4-909">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-909">Storage</span></span>

* <span data-ttu-id="1d3b4-910">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-910">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="1d3b4-911">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="1d3b4-911">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-912">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-912">VM</span></span>

* <span data-ttu-id="1d3b4-913">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-913">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="1d3b4-914">??에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-914">Added support for</span></span> `StandardSSD_LRS`
* <span data-ttu-id="1d3b4-915">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-915">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="1d3b4-916">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-916">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="1d3b4-917">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-917">July 18, 2018</span></span>

<span data-ttu-id="1d3b4-918">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="1d3b4-918">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-919">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-919">Core</span></span>

* <span data-ttu-id="1d3b4-920">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-920">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="1d3b4-921">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-921">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="1d3b4-922">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-922">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-923">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-923">ACR</span></span>

* <span data-ttu-id="1d3b4-924">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-924">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="1d3b4-925">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-925">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="1d3b4-926">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-926">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="1d3b4-927">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-927">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-928">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-928">ACS</span></span>

* <span data-ttu-id="1d3b4-929">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-929">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-930">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-930">AppService</span></span>

* <span data-ttu-id="1d3b4-931">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-931">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-932">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-932">Batch</span></span>

* <span data-ttu-id="1d3b4-933">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-933">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="1d3b4-934">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-934">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1d3b4-935">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-935">Batch AI</span></span>

* <span data-ttu-id="1d3b4-936">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-936">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-937">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-937">Container</span></span>

* <span data-ttu-id="1d3b4-938">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-938">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="1d3b4-939">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-939">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-940">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-940">Network</span></span>

* <span data-ttu-id="1d3b4-941">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-941">Added `--no-wait` support to</span></span> `network nic [create|update|delete]` 
* <span data-ttu-id="1d3b4-942">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-942">Added</span></span> `network nic wait`
* <span data-ttu-id="1d3b4-943">??에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-943">Deprecated `--ids` argument for</span></span> `network vnet [subnet|peering] list`
* <span data-ttu-id="1d3b4-944">?? 출력에 기본 보안 규칙을 포함하도록 `--include-default` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-944">Added `--include-default` flag to include default security rules in the output of</span></span> `network nsg rule list`  

### <a name="resource"></a><span data-ttu-id="1d3b4-945">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-945">Resource</span></span>

* <span data-ttu-id="1d3b4-946">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-946">Added `--no-wait` support to</span></span> `group deployment delete`
* <span data-ttu-id="1d3b4-947">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-947">Added `--no-wait` support to</span></span> `deployment delete`
* <span data-ttu-id="1d3b4-948">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-948">Added `deployment wait` command</span></span>
* <span data-ttu-id="1d3b4-949">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-949">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-950">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-950">SQL</span></span>

* <span data-ttu-id="1d3b4-951">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-951">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="1d3b4-952">??을(를) 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-952">Allow configuring default sql server by executing</span></span> `az configure --defaults sql-server=<name>`
* <span data-ttu-id="1d3b4-953">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-953">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-954">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-954">Storage</span></span>

* <span data-ttu-id="1d3b4-955">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-955">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-956">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-956">VM</span></span>

* <span data-ttu-id="1d3b4-957">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-957">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="1d3b4-958">`vm extension [set|delete]` 및 ??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-958">Added `--no-wait` support to `vm extension [set|delete]` and</span></span> `vmss extension [set|delete]`
* <span data-ttu-id="1d3b4-959">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-959">Added</span></span> `vm extension wait`

## <a name="july-3-2018"></a><span data-ttu-id="1d3b4-960">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-960">July 3, 2018</span></span>

<span data-ttu-id="1d3b4-961">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="1d3b4-961">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="1d3b4-962">AKS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-962">AKS</span></span>

* <span data-ttu-id="1d3b4-963">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-963">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="1d3b4-964">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-964">July 3, 2018</span></span>

<span data-ttu-id="1d3b4-965">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="1d3b4-965">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-966">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-966">Core</span></span>

* <span data-ttu-id="1d3b4-967">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-967">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-968">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-968">ACR</span></span>

* <span data-ttu-id="1d3b4-969">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-969">Added polling build status</span></span>
* <span data-ttu-id="1d3b4-970">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-970">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="1d3b4-971">??에 대한 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-971">Added `--top` and `--orderby` parameters for</span></span> `show-manifests`

### <a name="acs"></a><span data-ttu-id="1d3b4-972">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-972">ACS</span></span>

* <span data-ttu-id="1d3b4-973">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-973">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="1d3b4-974">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-974">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="1d3b4-975">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-975">Updated options for `aks browse` command.</span></span> <span data-ttu-id="1d3b4-976">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-976">Added `--listen-port` support</span></span>
* <span data-ttu-id="1d3b4-977">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-977">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="1d3b4-978">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-978">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="1d3b4-979">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-979">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-980">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-980">AppService</span></span>

* <span data-ttu-id="1d3b4-981">??을(를) 통해 ID를 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-981">Added support for disabling identity via</span></span> `webapp identity remove`
* <span data-ttu-id="1d3b4-982">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-982">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="1d3b4-983">Backup</span><span class="sxs-lookup"><span data-stu-id="1d3b4-983">Backup</span></span>

* <span data-ttu-id="1d3b4-984">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-984">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="1d3b4-985">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-985">BatchAI</span></span>

* <span data-ttu-id="1d3b4-986">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-986">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="1d3b4-987">클라우드</span><span class="sxs-lookup"><span data-stu-id="1d3b4-987">Cloud</span></span>

* <span data-ttu-id="1d3b4-988">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-988">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-989">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-989">Container</span></span>

* <span data-ttu-id="1d3b4-990">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-990">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="1d3b4-991">Log Analytics 매개 변수 `--log-analytics-workspace` 추가 및</span><span class="sxs-lookup"><span data-stu-id="1d3b4-991">Added Log Analytics parameters `--log-analytics-workspace` and</span></span> `--log-analytics-workspace-key`
* <span data-ttu-id="1d3b4-992">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-992">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-993">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-993">Extension</span></span>

* <span data-ttu-id="1d3b4-994">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-994">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-995">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-995">Network</span></span>

* <span data-ttu-id="1d3b4-996">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-996">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-997">Rdbms</span><span class="sxs-lookup"><span data-stu-id="1d3b4-997">Rdbms</span></span>

* <span data-ttu-id="1d3b4-998">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-998">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-999">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-999">Resource</span></span>

* <span data-ttu-id="1d3b4-1000">새 작업 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1000">Added new operation group</span></span> `deployment`

### <a name="vm"></a><span data-ttu-id="1d3b4-1001">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1001">VM</span></span>

* <span data-ttu-id="1d3b4-1002">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1002">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="1d3b4-1003">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1003">June 25, 2018</span></span>

<span data-ttu-id="1d3b4-1004">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1004">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="1d3b4-1005">CLI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1005">CLI</span></span>

* <span data-ttu-id="1d3b4-1006">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1006">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="1d3b4-1007">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1007">June 19, 2018</span></span>

<span data-ttu-id="1d3b4-1008">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1008">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1009">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1009">Core</span></span>

* <span data-ttu-id="1d3b4-1010">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1010">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1011">ACR</span></span>

* <span data-ttu-id="1d3b4-1012">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1012">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="1d3b4-1013">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1013">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1014">ACS</span></span>

* <span data-ttu-id="1d3b4-1015">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1015">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="1d3b4-1016">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1016">Added `--update` support</span></span>
* <span data-ttu-id="1d3b4-1017">?? 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1017">Changed `aks get-credentials --admin` to not eplace the user context in</span></span> `$HOME/.kube/config`
* <span data-ttu-id="1d3b4-1018">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1018">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="1d3b4-1019">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1019">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="1d3b4-1020">`--connector-name`을 `aks install-connector`, `aks upgrade-connector` 및 ??에 대한 선택 사항으로 만듦</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1020">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and</span></span> `aks remove-connector`
* <span data-ttu-id="1d3b4-1021">??에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1021">Added new Azure Container Instance regions for</span></span> `aks install-connector`
* <span data-ttu-id="1d3b4-1022">helm 릴리스 이름 및 노드 이름으로 정규화된 위치를 ??에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1022">Added the normalized location into the helm release name and node name to</span></span> `aks install-connector`

### <a name="appservice"></a><span data-ttu-id="1d3b4-1023">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1023">AppService</span></span>

* <span data-ttu-id="1d3b4-1024">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1024">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="1d3b4-1025">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1025">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-1026">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1026">Batch</span></span>

* <span data-ttu-id="1d3b4-1027">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1027">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1d3b4-1028">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1028">Batch AI</span></span>

* <span data-ttu-id="1d3b4-1029">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1029">Added support for workspaces.</span></span> <span data-ttu-id="1d3b4-1030">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1030">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="1d3b4-1031">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1031">Added support for experiments.</span></span> <span data-ttu-id="1d3b4-1032">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1032">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="1d3b4-1033">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1033">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="1d3b4-1034">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1034">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="1d3b4-1035">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1035">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="1d3b4-1036">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1036">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="1d3b4-1037">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1037">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="1d3b4-1038">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1038">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="1d3b4-1039">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1039">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="1d3b4-1040">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1040">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="1d3b4-1041">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1041">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="1d3b4-1042">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1042">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="1d3b4-1043">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1043">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="1d3b4-1044">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1044">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="1d3b4-1045">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1045">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="1d3b4-1046">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1046">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="1d3b4-1047">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1047">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="1d3b4-1048">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1048">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1d3b4-1049">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1049">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="1d3b4-1050">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1050">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="1d3b4-1051">지도</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1051">Maps</span></span>

* <span data-ttu-id="1d3b4-1052">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1052">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1053">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1053">Network</span></span>

* <span data-ttu-id="1d3b4-1054">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1054">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="1d3b4-1055">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1055">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="1d3b4-1056">#6502</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1056">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="1d3b4-1057">예약</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1057">Reservations</span></span>

* <span data-ttu-id="1d3b4-1058">[호환성이 손상되는 변경] ??에 필수 매개 변수 `ReservedResourceType` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1058">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to</span></span> `reservations catalog show`
* <span data-ttu-id="1d3b4-1059">??에 매개 변수 `Location` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1059">Added parameter `Location`to</span></span> `reservations catalog show`
* <span data-ttu-id="1d3b4-1060">[호환성이 손상되는 변경] ??에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1060">[BREAKING CHANGE] Removed `kind` from</span></span> `ReservationProperties`
* <span data-ttu-id="1d3b4-1061">[호환성이 손상되는 변경] ?? 내에서 `capabilities`의 이름을 `sku_properties`로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1061">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in</span></span> `Catalog`
* <span data-ttu-id="1d3b4-1062">[호환성이 손상되는 변경] ??에서 `size` 및 `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1062">[BREAKING CHANGE] Removed `size` and `tier` properties from</span></span> `Catalog`
* <span data-ttu-id="1d3b4-1063">??에 `InstanceFlexibility` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1063">Added parameter `InstanceFlexibility` to</span></span> `reservations reservation update`

### <a name="role"></a><span data-ttu-id="1d3b4-1064">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1064">Role</span></span>

* <span data-ttu-id="1d3b4-1065">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1065">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1066">SQL</span></span>

* <span data-ttu-id="1d3b4-1067">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1067">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1068">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1068">Storage</span></span>

* <span data-ttu-id="1d3b4-1069">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1069">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1070">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1070">VM</span></span>

* <span data-ttu-id="1d3b4-1071">??의 가속화된 네트워킹 지원을 위한 VM 크기 확인 구체화 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1071">Improved refine vm size check for accelerated networking support in</span></span> `vm create`
* <span data-ttu-id="1d3b4-1072">기본 VM 크기가 `Standard_D1_v2`에서 ??(으)로 전환된다는 `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1072">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to</span></span> `Standard_DS1_v2`
* <span data-ttu-id="1d3b4-1073">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1073">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1d3b4-1074">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1074">June 13, 2018</span></span>

<span data-ttu-id="1d3b4-1075">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1075">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1076">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1076">Core</span></span>

* <span data-ttu-id="1d3b4-1077">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1077">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1d3b4-1078">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1078">June 13, 2018</span></span>

<span data-ttu-id="1d3b4-1079">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1079">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="1d3b4-1080">AKS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1080">AKS</span></span>

* <span data-ttu-id="1d3b4-1081">??에 고급 네트워킹 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1081">Added advanced networking options to</span></span> `aks create`
* <span data-ttu-id="1d3b4-1082">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1082">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="1d3b4-1083">??에 `--no-ssh-key` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1083">Added `--no-ssh-key` argument to</span></span> `aks create`
* <span data-ttu-id="1d3b4-1084">??에 `--enable-rbac` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1084">Added `--enable-rbac` argument to</span></span> `aks create`
* <span data-ttu-id="1d3b4-1085">[미리 보기] ??에 Azure Active Directory 인증 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1085">[PREVIEW] Added support for Azure Active Directory authentication to</span></span> `aks create`

### <a name="appservice"></a><span data-ttu-id="1d3b4-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1086">AppService</span></span>

* <span data-ttu-id="1d3b4-1087">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1087">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1d3b4-1088">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1088">June 5, 2018</span></span>

<span data-ttu-id="1d3b4-1089">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1089">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1090">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1090">Interactive</span></span>

* <span data-ttu-id="1d3b4-1091">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1091">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1d3b4-1092">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1092">June 5, 2018</span></span>

<span data-ttu-id="1d3b4-1093">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1093">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1094">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1094">Core</span></span>

* <span data-ttu-id="1d3b4-1095">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1095">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="1d3b4-1096">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1096">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1097">ACR</span></span>

* <span data-ttu-id="1d3b4-1098">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1098">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="1d3b4-1099">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1099">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="1d3b4-1100">AKS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1100">AKS</span></span>

* <span data-ttu-id="1d3b4-1101">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1101">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-1102">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1102">Batch</span></span>

* <span data-ttu-id="1d3b4-1103">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1103">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-1104">IOT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1104">IOT</span></span>

* <span data-ttu-id="1d3b4-1105">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1105">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1106">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1106">Network</span></span>

* <span data-ttu-id="1d3b4-1107">?? 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1107">Improved</span></span> `network vnet peering`

### <a name="policy-insights"></a><span data-ttu-id="1d3b4-1108">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1108">Policy Insights</span></span>

* <span data-ttu-id="1d3b4-1109">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1109">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="1d3b4-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1110">ARM</span></span>

* <span data-ttu-id="1d3b4-1111">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1111">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1112">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1112">SQL</span></span>

* <span data-ttu-id="1d3b4-1113">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1113">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="1d3b4-1114">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1114">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="1d3b4-1115">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1115">Storage</span></span>

* <span data-ttu-id="1d3b4-1116">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1116">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1117">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1117">VM</span></span>

* <span data-ttu-id="1d3b4-1118">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1118">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="1d3b4-1119">??에 `--accelerated-networking` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1119">Added `--accelerated-networking` option to</span></span> `vm create`
* <span data-ttu-id="1d3b4-1120">??에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1120">Added `--tags` to</span></span> `identity create`

## <a name="may-22-2018"></a><span data-ttu-id="1d3b4-1121">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1121">May 22, 2018</span></span>

<span data-ttu-id="1d3b4-1122">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1122">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1123">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1123">Core</span></span>

* <span data-ttu-id="1d3b4-1124">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1124">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1125">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1125">ACS</span></span>

* <span data-ttu-id="1d3b4-1126">새 Dev-Space 명령 `aks use-dev-spaces` 및 ?? 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1126">Added new Dev-Spaces commands `aks use-dev-spaces` and</span></span> `aks remove-dev-spaces`
* <span data-ttu-id="1d3b4-1127">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1127">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1128">AppService</span></span>

* <span data-ttu-id="1d3b4-1129">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1129">Improved generic update commands</span></span>
* <span data-ttu-id="1d3b4-1130">??에 대한 비동기 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1130">Added async support for</span></span> `webapp deployment source config-zip`

### <a name="container"></a><span data-ttu-id="1d3b4-1131">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1131">Container</span></span>

* <span data-ttu-id="1d3b4-1132">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1132">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="1d3b4-1133">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1133">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1134">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1134">Extension</span></span>

* <span data-ttu-id="1d3b4-1135">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1135">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1136">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1136">Interactive</span></span>

* <span data-ttu-id="1d3b4-1137">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1137">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="1d3b4-1138">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1138">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-1139">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1139">KeyVault</span></span>

* <span data-ttu-id="1d3b4-1140">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1140">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1141">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1141">Network</span></span>

* <span data-ttu-id="1d3b4-1142">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1142">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="1d3b4-1143">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1143">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1144">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1144">SQL</span></span>

* <span data-ttu-id="1d3b4-1145">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1145">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="1d3b4-1146">`serviceLevelObjective` 속성의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1146">Renamed `serviceLevelObjective` property to</span></span> `currentServiceObjectiveName`
    * <span data-ttu-id="1d3b4-1147">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1147">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="1d3b4-1148">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1148">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="1d3b4-1149">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1149">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * `requestedServiceObjectiveName`<span data-ttu-id="1d3b4-1150">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1150">.</span></span>  <span data-ttu-id="1d3b4-1151">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1151">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * `edition`<span data-ttu-id="1d3b4-1152">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1152">.</span></span> <span data-ttu-id="1d3b4-1153">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1153">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * `elasticPoolName`<span data-ttu-id="1d3b4-1154">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1154">.</span></span> <span data-ttu-id="1d3b4-1155">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1155">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="1d3b4-1156">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1156">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * `edition`<span data-ttu-id="1d3b4-1157">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1157">.</span></span> <span data-ttu-id="1d3b4-1158">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1158">To update, use the `--edition` parameter</span></span>
    * `dtu`<span data-ttu-id="1d3b4-1159">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1159">.</span></span> <span data-ttu-id="1d3b4-1160">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1160">To update, use the `--capacity` parameter</span></span>
    *  `databaseDtuMin`<span data-ttu-id="1d3b4-1161">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1161">.</span></span> <span data-ttu-id="1d3b4-1162">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1162">To update, use the `--db-min-capacity` parameter</span></span>
    *  `databaseDtuMax`<span data-ttu-id="1d3b4-1163">.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1163">.</span></span> <span data-ttu-id="1d3b4-1164">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1164">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="1d3b4-1165">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1165">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="1d3b4-1166">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1166">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1167">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1167">Storage</span></span>

* <span data-ttu-id="1d3b4-1168">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1168">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="1d3b4-1169">??의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1169">Fixed problem with</span></span> `storage entity query`

### <a name="vm"></a><span data-ttu-id="1d3b4-1170">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1170">VM</span></span>

* <span data-ttu-id="1d3b4-1171">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1171">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="1d3b4-1172">동일한 지원을 `vm update` 또는 ??을(를) 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1172">The same support can be accessed through `vm update` or</span></span> `vm disk attach`
* <span data-ttu-id="1d3b4-1173">??에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1173">Fixed extension image matching in</span></span> `[vm|vmss] extension`
* <span data-ttu-id="1d3b4-1174">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="1d3b4-1174">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="1d3b4-1175">??에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1175">Added `--license-type` to</span></span> `[vm|vmss] update`

## <a name="may-7-2018"></a><span data-ttu-id="1d3b4-1176">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1176">May 7, 2018</span></span>

<span data-ttu-id="1d3b4-1177">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1177">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1178">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1178">Core</span></span>

* <span data-ttu-id="1d3b4-1179">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1179">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="1d3b4-1180">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1180">Added limited support for positional arguments</span></span>
* <span data-ttu-id="1d3b4-1181">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1181">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="1d3b4-1182">#5591</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1182">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="1d3b4-1183">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1183">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="1d3b4-1184">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1184">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="1d3b4-1185">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1185">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="1d3b4-1186">사용자가 ??을(를) 입력하는 경우 오류 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1186">Improved error when users type</span></span> `az ''`
* <span data-ttu-id="1d3b4-1187">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1187">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1188">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1188">ACR</span></span>

* <span data-ttu-id="1d3b4-1189">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1189">Added ACR Build commands</span></span>
* <span data-ttu-id="1d3b4-1190">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1190">Improved resource not found error messages</span></span>
* <span data-ttu-id="1d3b4-1191">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1191">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="1d3b4-1192">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1192">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="1d3b4-1193">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1193">Improved repository commands error messages</span></span>
* <span data-ttu-id="1d3b4-1194">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1194">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1195">ACS</span></span>

* <span data-ttu-id="1d3b4-1196">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1196">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="1d3b4-1197">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1197">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="1d3b4-1198">AMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1198">AMS</span></span>

* <span data-ttu-id="1d3b4-1199">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1199">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1200">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1200">Appservice</span></span>

* <span data-ttu-id="1d3b4-1201">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1201">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="1d3b4-1202">??에서 `--runtime-version` 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1202">Removed `--runtime-version` from</span></span> `webapp auth update`
* <span data-ttu-id="1d3b4-1203">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1203">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="1d3b4-1204">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1204">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1d3b4-1205">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1205">Batch AI</span></span>

* <span data-ttu-id="1d3b4-1206">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1206">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1d3b4-1207">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1207">Cognitive Services</span></span>

* <span data-ttu-id="1d3b4-1208">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1208">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="1d3b4-1209">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1209">Consumption</span></span>

* <span data-ttu-id="1d3b4-1210">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1210">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1211">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1211">Container</span></span>

* <span data-ttu-id="1d3b4-1212">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1212">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1d3b4-1213">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1213">Cosmos DB</span></span>

* <span data-ttu-id="1d3b4-1214">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1214">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="1d3b4-1215">DMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1215">DMS</span></span>

* <span data-ttu-id="1d3b4-1216">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1216">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1217">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1217">Extension</span></span>

* <span data-ttu-id="1d3b4-1218">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1218">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1219">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1219">Interactive</span></span>

* <span data-ttu-id="1d3b4-1220">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1220">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="1d3b4-1221">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1221">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="1d3b4-1222">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1222">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="1d3b4-1223">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1223">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="1d3b4-1224">랩</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1224">Lab</span></span>

* <span data-ttu-id="1d3b4-1225">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1225">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1226">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1226">Network</span></span>

* <span data-ttu-id="1d3b4-1227">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1227">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="1d3b4-1228">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1228">Profile</span></span>

* <span data-ttu-id="1d3b4-1229">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1229">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="1d3b4-1230">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1230">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="1d3b4-1231">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1231">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="1d3b4-1232">Redis</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1232">Redis</span></span>

* <span data-ttu-id="1d3b4-1233">??을(를) 위해 `redis patch-schedule patch-schedule show`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1233">Deprecated `redis patch-schedule patch-schedule show` in favor of</span></span> `redis patch-schedule show`
* <span data-ttu-id="1d3b4-1234">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1234">Deprecated `redis list-all`.</span></span> <span data-ttu-id="1d3b4-1235">이 기능은 ??에 포함됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1235">This functionality has been folded into</span></span> `redis list`
* <span data-ttu-id="1d3b4-1236">??을(를) 위해 `redis import-method`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1236">Deprecated `redis import-method` in favor of</span></span> `redis import`
* <span data-ttu-id="1d3b4-1237">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1237">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-1238">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1238">Role</span></span>

* <span data-ttu-id="1d3b4-1239">[호환성이 손상되는 변경] 사용되지 않는 ?? 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1239">[BREAKING CHANGE] Removed deprecated</span></span> `ad sp reset-credentials`

### <a name="storage"></a><span data-ttu-id="1d3b4-1240">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1240">Storage</span></span>

* <span data-ttu-id="1d3b4-1241">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1241">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="1d3b4-1242">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1242">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="1d3b4-1243">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1243">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="1d3b4-1244">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1244">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="1d3b4-1245">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1245">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1246">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1246">VM</span></span>

* <span data-ttu-id="1d3b4-1247">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1247">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="1d3b4-1248">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1248">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="1d3b4-1249">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1249">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="1d3b4-1250">??에 대한 제거 정책 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1250">Added support for eviction policy to</span></span> `vmss`
* <span data-ttu-id="1d3b4-1251">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1251">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="1d3b4-1252">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1252">Added write accelerator support</span></span>
* <span data-ttu-id="1d3b4-1253">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1253">Added</span></span> `vmss perform-maintenance`
* <span data-ttu-id="1d3b4-1254">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1254">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="1d3b4-1255">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1255">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="1d3b4-1256">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1256">April 10, 2018</span></span>

<span data-ttu-id="1d3b4-1257">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1257">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1258">ACR</span></span>

* <span data-ttu-id="1d3b4-1259">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1259">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1260">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1260">ACS</span></span>

* <span data-ttu-id="1d3b4-1261">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1261">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1262">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1262">Appservice</span></span>

* [<span data-ttu-id="1d3b4-1263">호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1263">BREAKING CHANGE</span></span>]: Removed `assign-identity`
* <span data-ttu-id="1d3b4-1264">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1264">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="1d3b4-1265">BatchAI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1265">BatchAI</span></span>

* <span data-ttu-id="1d3b4-1266">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1266">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="1d3b4-1267">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1267">Job level mounting</span></span>
  - <span data-ttu-id="1d3b4-1268">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1268">Environment variables with secret values</span></span>
  - <span data-ttu-id="1d3b4-1269">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1269">Performance counters settings</span></span>
  - <span data-ttu-id="1d3b4-1270">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1270">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="1d3b4-1271">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1271">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="1d3b4-1272">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1272">Usage and limits reporting</span></span>
  - <span data-ttu-id="1d3b4-1273">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1273">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="1d3b4-1274">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1274">Support for custom images</span></span>
  - <span data-ttu-id="1d3b4-1275">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1275">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="1d3b4-1276">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1276">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="1d3b4-1277">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1277">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="1d3b4-1278">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1278">National clouds are supported</span></span>
* <span data-ttu-id="1d3b4-1279">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1279">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="1d3b4-1280">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1280">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="1d3b4-1281">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1281">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="1d3b4-1282">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1282">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="1d3b4-1283">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1283">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="1d3b4-1284">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1284">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="1d3b4-1285">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1285">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="1d3b4-1286">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1286">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="1d3b4-1287">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1287">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="1d3b4-1288">`cluster create` 및 ??에 `--generate-ssh-keys` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1288">Added `--generate-ssh-keys` option to `cluster create` and</span></span> `file-server create`
* <span data-ttu-id="1d3b4-1289">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1289">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="1d3b4-1290">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1290">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="1d3b4-1291">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1291">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="1d3b4-1292">결제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1292">Billing</span></span>

* <span data-ttu-id="1d3b4-1293">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1293">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="1d3b4-1294">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1294">Consumption</span></span>

* <span data-ttu-id="1d3b4-1295">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1295">Added `marketplace` commands</span></span>
* <span data-ttu-id="1d3b4-1296">[호환성이 손상되는 변경] `reservations summaries`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1296">[BREAKING CHANGE] Renamed `reservations summaries` to</span></span> `reservation summary`
* <span data-ttu-id="1d3b4-1297">[호환성이 손상되는 변경] `reservations details`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1297">[BREAKING CHANGE] Renamed `reservations details` to</span></span> `reservation detail`
* <span data-ttu-id="1d3b4-1298">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1298">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="1d3b4-1299">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1299">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="1d3b4-1300">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1300">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1301">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1301">Container</span></span>

* <span data-ttu-id="1d3b4-1302">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 ?? 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1302">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and</span></span> `--gitrepo-mount-path`
* <span data-ttu-id="1d3b4-1303">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1303">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1304">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1304">Extension</span></span>

* <span data-ttu-id="1d3b4-1305">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1305">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1306">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1306">Interactive</span></span>

* <span data-ttu-id="1d3b4-1307">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1307">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="1d3b4-1308">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1308">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="1d3b4-1309">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1309">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1310">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1310">Network</span></span>

* <span data-ttu-id="1d3b4-1311">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1311">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="1d3b4-1312">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1312">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="1d3b4-1313">#4910</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1313">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="1d3b4-1314">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1314">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="1d3b4-1315">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1315">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="1d3b4-1316">??에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1316">Fixed issue with `--disable-bgp-route-propagation` flag in</span></span> `network route-table [create|update]`
* <span data-ttu-id="1d3b4-1317">??에 대한 더미 인수 `--public-ip-address-type` 및 `--subnet-type` 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1317">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for</span></span> `network lb [create|update]`
* <span data-ttu-id="1d3b4-1318">`network dns zone [import|export]` 및 ??에 대한 RFC 1035 이스케이프 시퀀스를 포함하는 TXT 레코드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1318">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and</span></span> `network dns record-set txt add-record`

### <a name="profile"></a><span data-ttu-id="1d3b4-1319">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1319">Profile</span></span>

* <span data-ttu-id="1d3b4-1320">??에 있는 Azure Classic 계정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1320">Added support for Azure Classic accounts in</span></span> `account list`
* <span data-ttu-id="1d3b4-1321">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1321">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-1322">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1322">RDBMS</span></span>

* <span data-ttu-id="1d3b4-1323">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1323">Added `georestore` command</span></span>
* <span data-ttu-id="1d3b4-1324">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1324">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1325">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1325">Resource</span></span>

* <span data-ttu-id="1d3b4-1326">??에 `--metadata` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1326">Added support for `--metadata` to</span></span> `policy definition create`
* <span data-ttu-id="1d3b4-1327">??에 `--metadata`, `--set`, `--add`, `--remove` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1327">Added support for `--metadata`, `--set`, `--add`, `--remove` to</span></span> `policy definition update`

### <a name="sql"></a><span data-ttu-id="1d3b4-1328">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1328">SQL</span></span>

* <span data-ttu-id="1d3b4-1329">`sql elastic-pool op list` 및 ?? 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1329">Added `sql elastic-pool op list` and</span></span> `sql elastic-pool op cancel`

### <a name="storage"></a><span data-ttu-id="1d3b4-1330">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1330">Storage</span></span>

* <span data-ttu-id="1d3b4-1331">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1331">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1332">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1332">VM</span></span>

* <span data-ttu-id="1d3b4-1333">플랫폼 장애 도메인 수를 ??(으)로 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1333">Added support to configure platform fault domain count to</span></span> `vmss create`
* <span data-ttu-id="1d3b4-1334">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1334">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [<span data-ttu-id="1d3b4-1335">호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1335">BREAKING CHANGE</span></span>]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="1d3b4-1336">??에 공용-IP SKU 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1336">Added support for Public-IP SKU to</span></span> `vm create`
* <span data-ttu-id="1d3b4-1337">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1337">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="1d3b4-1338">#5718</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1338">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="1d3b4-1339">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1339">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="1d3b4-1340">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1340">March 27, 2018</span></span>

<span data-ttu-id="1d3b4-1341">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1341">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1342">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1342">Core</span></span>

* <span data-ttu-id="1d3b4-1343">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1343">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1344">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1344">ACS</span></span>

* <span data-ttu-id="1d3b4-1345">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1345">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1346">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1346">Appservice</span></span>

* <span data-ttu-id="1d3b4-1347">??에 HTTPS만 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1347">Added HTTPS-only support to</span></span> `webapp update`
* <span data-ttu-id="1d3b4-1348">`az webapp identity [assign|show]` 및 ??에 대한 슬롯 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1348">Added support for slots to `az webapp identity [assign|show]` and</span></span> `az functionapp identity [assign|show]`

### <a name="backup"></a><span data-ttu-id="1d3b4-1349">Backup</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1349">Backup</span></span>

* <span data-ttu-id="1d3b4-1350">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1350">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="1d3b4-1351">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1351">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="1d3b4-1352">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1352">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="1d3b4-1353">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1353">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1354">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1354">Container</span></span>

* <span data-ttu-id="1d3b4-1355">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1355">Added `container exec` command.</span></span> <span data-ttu-id="1d3b4-1356">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1356">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="1d3b4-1357">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1357">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1358">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1358">Extension</span></span>

* <span data-ttu-id="1d3b4-1359">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1359">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="1d3b4-1360">??을(를) 사용하여 전체 확장 데이터를 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1360">Changed `extension list-available` to show full extension data with</span></span> `--show-details`
* <span data-ttu-id="1d3b4-1361">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1361">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1362">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1362">Interactive</span></span>

* <span data-ttu-id="1d3b4-1363">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1363">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="1d3b4-1364">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1364">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="1d3b4-1365">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1365">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="1d3b4-1366">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1366">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="1d3b4-1367">랩</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1367">Lab</span></span>

* <span data-ttu-id="1d3b4-1368">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1368">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1369">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1369">Monitor</span></span>

* <span data-ttu-id="1d3b4-1370">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1370">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="1d3b4-1371">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1371">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="1d3b4-1372">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1372">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1373">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1373">Network</span></span>

* <span data-ttu-id="1d3b4-1374">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1374">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="1d3b4-1375">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1375">Profile</span></span>

* <span data-ttu-id="1d3b4-1376">??에 `--identity-port` 및 `--msi-port`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1376">Added warning for `--identity-port` and `--msi-port` to</span></span> `login`

### <a name="rdbms"></a><span data-ttu-id="1d3b4-1377">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1377">RDBMS</span></span>

* <span data-ttu-id="1d3b4-1378">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1378">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1379">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1379">Resource</span></span>

* [<span data-ttu-id="1d3b4-1380">호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1380">BREAKING CHANGE</span></span>]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="1d3b4-1381">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1381">Role</span></span>

* <span data-ttu-id="1d3b4-1382">??에 필수 액세스 구성 및 네이티브 클라이언트에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1382">Added support for required access configurations and native clients to</span></span> `az ad app create`
* <span data-ttu-id="1d3b4-1383">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1383">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="1d3b4-1384">자격 증명 관리 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1384">Added credential management commands</span></span> `ad sp credential [reset|list|delete]`
* <span data-ttu-id="1d3b4-1385">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1385">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="1d3b4-1386">??에 `dataActions` 및 `notDataActions` 권한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1386">Added support for `dataActions` and `notDataActions` permissions to</span></span> `role definition`

### <a name="storage"></a><span data-ttu-id="1d3b4-1387">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1387">Storage</span></span>

* <span data-ttu-id="1d3b4-1388">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1388">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="1d3b4-1389">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1389">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1390">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1390">VM</span></span>

* <span data-ttu-id="1d3b4-1391">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1391">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="1d3b4-1392">??에 영역 복원력 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1392">Added zone resilient support to</span></span> `vm [snapshot|image]`
* <span data-ttu-id="1d3b4-1393">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1393">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="1d3b4-1394">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1394">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="1d3b4-1395">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1395">March 13, 2018</span></span>

<span data-ttu-id="1d3b4-1396">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1396">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1397">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1397">ACR</span></span>

* <span data-ttu-id="1d3b4-1398">??에 `--image` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1398">Added support for `--image` parameter to</span></span> `repository delete`
* <span data-ttu-id="1d3b4-1399">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1399">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="1d3b4-1400">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1400">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1401">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1401">ACS</span></span>

* <span data-ttu-id="1d3b4-1402">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1402">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="1d3b4-1403">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1403">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="1d3b4-1404">Advisor</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1404">Advisor</span></span>

* <span data-ttu-id="1d3b4-1405">[호환성이 손상되는 변경] `advisor configuration get`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1405">[BREAKING CHANGE] Renamed `advisor configuration get` to</span></span> `advisor configuration list`
* <span data-ttu-id="1d3b4-1406">[호환성이 손상되는 변경] `advisor configuration set`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1406">[BREAKING CHANGE] Renamed `advisor configuration set` to</span></span> `advisor configuration update`
* <span data-ttu-id="1d3b4-1407">[호환성이 손상되는 변경] ?? 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1407">[BREAKING CHANGE] Removed</span></span> `advisor recommendation generate`
* <span data-ttu-id="1d3b4-1408">??에 `--refresh` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1408">Added `--refresh` parameter to</span></span> `advisor recommendation list`
* <span data-ttu-id="1d3b4-1409">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1409">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1410">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1410">Appservice</span></span>

* <span data-ttu-id="1d3b4-1411">사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1411">Deprecated</span></span> `[webapp|functionapp] assign-identity`
* <span data-ttu-id="1d3b4-1412">관리 ID 명령 `webapp identity [assign|show]` 및 ?? 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1412">Added managed identity commands `webapp identity [assign|show]` and</span></span> `functionapp identity [assign|show]`

### <a name="eventhubs"></a><span data-ttu-id="1d3b4-1413">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1413">Eventhubs</span></span>

* <span data-ttu-id="1d3b4-1414">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1414">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1415">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1415">Extension</span></span>

* <span data-ttu-id="1d3b4-1416">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1416">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1417">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1417">Interactive</span></span>

* <span data-ttu-id="1d3b4-1418">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1418">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="1d3b4-1419">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1419">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="1d3b4-1420">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1420">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="1d3b4-1421">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1421">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1422">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1422">Monitor</span></span>

* <span data-ttu-id="1d3b4-1423">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1423">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="1d3b4-1424">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1424">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="1d3b4-1425">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1425">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="1d3b4-1426">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1426">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1427">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1427">Network</span></span>

* <span data-ttu-id="1d3b4-1428">[호환성이 손상되는 변경] ??에서 `--tags` 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1428">[BREAKING CHANGE] Removed `--tags` parameter from</span></span>  `route-filter rule create`
* <span data-ttu-id="1d3b4-1429">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1429">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="1d3b4-1430">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1430">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="1d3b4-1431">??에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1431">Added `--vnet` and `--subnet` parameters to</span></span> `network watcher show-topology`

### <a name="profile"></a><span data-ttu-id="1d3b4-1432">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1432">Profile</span></span>

* <span data-ttu-id="1d3b4-1433">??의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1433">Deprecated `--msi` parameter for</span></span> `az login`
* <span data-ttu-id="1d3b4-1434">??을(를) 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1434">Added `--identity` parameter for `az login` to replace</span></span> `--msi`

### <a name="rdbms"></a><span data-ttu-id="1d3b4-1435">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1435">RDBMS</span></span>

* <span data-ttu-id="1d3b4-1436">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1436">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="1d3b4-1437">Service Bus</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1437">Service Bus</span></span>

* <span data-ttu-id="1d3b4-1438">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1438">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1439">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1439">Storage</span></span>

* <span data-ttu-id="1d3b4-1440">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1440">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="1d3b4-1441">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1441">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1442">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1442">VM</span></span>

* <span data-ttu-id="1d3b4-1443">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1443">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="1d3b4-1444">`[vm|vmss] assign-identity` 및 ?? 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1444">Deprecated `[vm|vmss] assign-identity` and</span></span> `[vm|vmss] remove-identity`
* <span data-ttu-id="1d3b4-1445">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1445">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="1d3b4-1446">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1446">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="1d3b4-1447">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1447">February 27, 2018</span></span>

<span data-ttu-id="1d3b4-1448">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1448">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1449">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1449">Core</span></span>

* <span data-ttu-id="1d3b4-1450">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1450">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="1d3b4-1451">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1451">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="1d3b4-1452">??에 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1452">Added HTTP logging to</span></span> `--debug`

### <a name="acs"></a><span data-ttu-id="1d3b4-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1453">ACS</span></span>

* <span data-ttu-id="1d3b4-1454">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1454">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="1d3b4-1455">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1455">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="1d3b4-1456">??에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1456">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to</span></span> `aks install-connector`
* <span data-ttu-id="1d3b4-1457">??에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1457">Removed deprecation notice from</span></span> `aks get-versions`

### <a name="appservice"></a><span data-ttu-id="1d3b4-1458">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1458">Appservice</span></span>

* <span data-ttu-id="1d3b4-1459">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1459">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="1d3b4-1460">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1460">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1d3b4-1461">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1461">Cognitive Services</span></span>

* <span data-ttu-id="1d3b4-1462">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1462">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="1d3b4-1463">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1463">Consumption</span></span>

* <span data-ttu-id="1d3b4-1464">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1464">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="1d3b4-1465">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1465">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1466">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1466">Container</span></span>

* <span data-ttu-id="1d3b4-1467">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1467">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1468">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1468">Network</span></span>

* <span data-ttu-id="1d3b4-1469">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: ??에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1469">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in</span></span> `network vnet-gateway vpn-client generate`

### <a name="resource"></a><span data-ttu-id="1d3b4-1470">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1470">Resource</span></span>

* <span data-ttu-id="1d3b4-1471">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1471">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-1472">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1472">Role</span></span>

* <span data-ttu-id="1d3b4-1473">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1473">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1474">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1474">SQL</span></span>

* <span data-ttu-id="1d3b4-1475">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1475">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1476">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1476">Storage</span></span>

* <span data-ttu-id="1d3b4-1477">??에 대상-경로/접두사 지정을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1477">Enabled specifying destination-path/prefix for</span></span> `storage blob [upload-batch|download-batch]`

### <a name="vm"></a><span data-ttu-id="1d3b4-1478">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1478">VM</span></span>

* <span data-ttu-id="1d3b4-1479">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1479">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="1d3b4-1480">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1480">February 13, 2018</span></span>

<span data-ttu-id="1d3b4-1481">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1481">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1482">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1482">Core</span></span>

* <span data-ttu-id="1d3b4-1483">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1483">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1484">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1484">ACS</span></span>

* <span data-ttu-id="1d3b4-1485">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1485">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="1d3b4-1486">??에 사용 가능한 Kubernetes 버전을 표시하도록 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1486">Changed `aks get-versions` to show Kubernetes versions available for</span></span> `aks create`
* <span data-ttu-id="1d3b4-1487">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1487">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="1d3b4-1488">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1488">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="1d3b4-1489">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1489">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="1d3b4-1490">??의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1490">Improved reliability when locating the dashboard pod for</span></span> `az aks browse`
* <span data-ttu-id="1d3b4-1491">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1491">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="1d3b4-1492">??에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 대한 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1492">Added a message to `az aks install-cli` to help get `kubectl` in</span></span> `$PATH`

### <a name="appservice"></a><span data-ttu-id="1d3b4-1493">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1493">Appservice</span></span>

* <span data-ttu-id="1d3b4-1494">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1494">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="1d3b4-1495">??을(를) 통한 기본 App Service 플랜에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1495">Added support for default app service plans through</span></span> `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a><span data-ttu-id="1d3b4-1496">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1496">CDN</span></span>

* <span data-ttu-id="1d3b4-1497">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1497">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1498">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1498">Container</span></span>

* <span data-ttu-id="1d3b4-1499">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1499">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="1d3b4-1500">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1500">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-1501">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1501">CosmosDB</span></span>

* <span data-ttu-id="1d3b4-1502">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1502">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1503">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1503">Extension</span></span>

* <span data-ttu-id="1d3b4-1504">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1504">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="1d3b4-1505">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1505">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="1d3b4-1506">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1506">Feedback</span></span>

* <span data-ttu-id="1d3b4-1507">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1507">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1508">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1508">Interactive</span></span>

* <span data-ttu-id="1d3b4-1509">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1509">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="1d3b4-1510">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1510">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-1511">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1511">IoT</span></span>

* <span data-ttu-id="1d3b4-1512">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1512">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1d3b4-1513">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1513">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1d3b4-1514">`iot dps access policy [create|update]` 및 ??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1514">Added `--no-wait` support to `iot dps access policy [create|update]` and</span></span> `iot dps linked-hub [create|update]`
* <span data-ttu-id="1d3b4-1515">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1515">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1516">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1516">Monitor</span></span>

* <span data-ttu-id="1d3b4-1517">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1517">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1518">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1518">Network</span></span>

* <span data-ttu-id="1d3b4-1519">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1519">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="1d3b4-1520">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1520">Profile</span></span>

* <span data-ttu-id="1d3b4-1521">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1521">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1522">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1522">Resource</span></span>

* <span data-ttu-id="1d3b4-1523">?? 다시 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1523">Added back</span></span> `feature show`

### <a name="role"></a><span data-ttu-id="1d3b4-1524">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1524">Role</span></span>

* <span data-ttu-id="1d3b4-1525">??에 `--available-to-other-tenants` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1525">Added `--available-to-other-tenants` argument to</span></span> `ad app update`

### <a name="sql"></a><span data-ttu-id="1d3b4-1526">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1526">SQL</span></span>

* <span data-ttu-id="1d3b4-1527">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1527">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="1d3b4-1528">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1528">Added</span></span> `sql db rename`
* <span data-ttu-id="1d3b4-1529">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1529">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1530">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1530">Storage</span></span>

* <span data-ttu-id="1d3b4-1531">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1531">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1532">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1532">VM</span></span>

* <span data-ttu-id="1d3b4-1533">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1533">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="1d3b4-1534">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1534">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="1d3b4-1535">수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1535">Fixed</span></span> `vm boot-diagnostics get-boot-log`


## <a name="january-31-2018"></a><span data-ttu-id="1d3b4-1536">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1536">January 31, 2018</span></span>

<span data-ttu-id="1d3b4-1537">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1537">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1538">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1538">Core</span></span>

* <span data-ttu-id="1d3b4-1539">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1539">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="1d3b4-1540">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1540">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="1d3b4-1541">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1541">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="1d3b4-1542">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1542">Use `--verbose` to see</span></span>
* <span data-ttu-id="1d3b4-1543">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1543">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1544">ACS</span></span>

* <span data-ttu-id="1d3b4-1545">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1545">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="1d3b4-1546">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1546">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1547">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1547">Appservice</span></span>

* <span data-ttu-id="1d3b4-1548">수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1548">Fixed</span></span> `webapp log [tail|download]`
* <span data-ttu-id="1d3b4-1549">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1549">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="1d3b4-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1550">CDN</span></span>

* <span data-ttu-id="1d3b4-1551">??의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1551">Fixed missing client issue with</span></span> `cdn custom-domain create`

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-1552">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1552">CosmosDB</span></span>

* <span data-ttu-id="1d3b4-1553">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1553">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1554">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1554">Interactive</span></span>

* <span data-ttu-id="1d3b4-1555">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1555">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1556">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1556">Network</span></span>

* <span data-ttu-id="1d3b4-1557">??에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1557">Added protection for `--cert-password` to</span></span> `application-gateway create`
* <span data-ttu-id="1d3b4-1558">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1558">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="1d3b4-1559">??에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1559">Added protection for `--shared-key` and `--authorization-key` to</span></span> `vpn-connection create`
* <span data-ttu-id="1d3b4-1560">??의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1560">Fixed missing client issue with</span></span> `asg create`
* <span data-ttu-id="1d3b4-1561">??에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1561">Added `--file-name / -f` parameter for exported names to</span></span> `dns zone export`
* <span data-ttu-id="1d3b4-1562">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1562">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="1d3b4-1563">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1563">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="1d3b4-1564">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1564">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="1d3b4-1565">??에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1565">Fixed issue where certain records were imported twice with</span></span> `dns zone import`
* <span data-ttu-id="1d3b4-1566">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1566">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="1d3b4-1567">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1567">Profile</span></span>

* <span data-ttu-id="1d3b4-1568">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1568">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1569">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1569">Resource</span></span>

* <span data-ttu-id="1d3b4-1570">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1570">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1571">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1571">Storage</span></span>

* <span data-ttu-id="1d3b4-1572">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1572">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="1d3b4-1573">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1573">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="1d3b4-1574">??에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1574">Fixed bug preventing "-n" arg option with</span></span> `storage account check-name`
* <span data-ttu-id="1d3b4-1575">??에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1575">Added 'snapshot' column to table output for</span></span> `blob [list|show]`
* <span data-ttu-id="1d3b4-1576">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1576">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1577">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1577">VM</span></span>

* <span data-ttu-id="1d3b4-1578">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1578">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="1d3b4-1579">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1579">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="1d3b4-1580">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1580">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="1d3b4-1581">??에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1581">Added protection for `--admin-password` to</span></span> `[vm|vmss] create`


## <a name="january-17-2018"></a><span data-ttu-id="1d3b4-1582">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1582">January 17, 2018</span></span>

<span data-ttu-id="1d3b4-1583">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1583">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1584">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1584">ACR</span></span>

* <span data-ttu-id="1d3b4-1585">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1585">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="1d3b4-1586">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1586">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1587">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1587">ACS</span></span>

* <span data-ttu-id="1d3b4-1588">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1588">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="1d3b4-1589">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1589">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1590">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1590">Appservice</span></span>

* <span data-ttu-id="1d3b4-1591">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1591">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="1d3b4-1592">??에 사용자 지정 URL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1592">Added support for custom URLs to</span></span> `browse`
* <span data-ttu-id="1d3b4-1593">??에 대한 슬롯 지원 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1593">Fixed slot support for</span></span> `log tail`

### <a name="backup"></a><span data-ttu-id="1d3b4-1594">Backup</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1594">Backup</span></span>

* <span data-ttu-id="1d3b4-1595">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1595">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="1d3b4-1596">??에 저장소 계정 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1596">Added storage account options to</span></span> `backup restore restore-disks`
* <span data-ttu-id="1d3b4-1597">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1597">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="1d3b4-1598">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1598">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="1d3b4-1599">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1599">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-1600">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1600">Batch</span></span>

* <span data-ttu-id="1d3b4-1601">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1601">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="1d3b4-1602">클라우드</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1602">Cloud</span></span>

* <span data-ttu-id="1d3b4-1603">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1603">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="1d3b4-1604">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1604">Consumption</span></span>

* <span data-ttu-id="1d3b4-1605">새 예약 명령 추가: `consumption reservations summaries` 및</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1605">Added new commands for reservations: `consumption reservations summaries` and</span></span> `consumption reservations details`

### <a name="event-grid"></a><span data-ttu-id="1d3b4-1606">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1606">Event Grid</span></span>

* <span data-ttu-id="1d3b4-1607">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 ??(으)로 이동됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1607">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="1d3b4-1608">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 ??(으)로 이동됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1608">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="1d3b4-1609">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1609">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="1d3b4-1610">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="1d3b4-1611">명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1611">Added command</span></span> `eventgrid topic update`
* <span data-ttu-id="1d3b4-1612">명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1612">Added command</span></span> `eventgrid event-subscription update`
* <span data-ttu-id="1d3b4-1613">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1613">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="1d3b4-1614">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1614">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-1615">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1615">Interactive</span></span>

* <span data-ttu-id="1d3b4-1616">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1616">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="1d3b4-1617">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1617">Fixed errors on startup</span></span>
* <span data-ttu-id="1d3b4-1618">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1618">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-1619">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1619">IoT</span></span>

* <span data-ttu-id="1d3b4-1620">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1620">Added support for device provisioning service</span></span>
* <span data-ttu-id="1d3b4-1621">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1621">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="1d3b4-1622">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1622">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1623">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1623">Monitor</span></span>

* <span data-ttu-id="1d3b4-1624">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1624">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="1d3b4-1625">`--name` 매개 변수가 이제 ??에 대해 필수임</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1625">The `--name` parameter is now required for</span></span> `az monitor diagnostic-settings create`
* <span data-ttu-id="1d3b4-1626">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1626">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1627">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1627">Network</span></span>

* <span data-ttu-id="1d3b4-1628">??을(를) 사용하여 활성-대기 모드로/에서 변경을 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1628">Fixed issue when trying to change to/from active-standby mode with</span></span> `vnet-gateway update`
* <span data-ttu-id="1d3b4-1629">??에 HTTP2 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1629">Added support for HTTP2 to</span></span> `application-gateway [create|update]`

### <a name="profile"></a><span data-ttu-id="1d3b4-1630">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1630">Profile</span></span>

* <span data-ttu-id="1d3b4-1631">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1631">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-1632">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1632">Role</span></span>

* <span data-ttu-id="1d3b4-1633">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1633">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1d3b4-1634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1634">Service Fabric</span></span>

* <span data-ttu-id="1d3b4-1635">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1635">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="1d3b4-1636">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1636">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1637">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1637">VM</span></span>

* <span data-ttu-id="1d3b4-1638">[미리 보기] ??에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1638">[PREVIEW] Cross-zone support for</span></span> `vmss`
* <span data-ttu-id="1d3b4-1639">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1639">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="1d3b4-1640">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1640">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="1d3b4-1641">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1641">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="1d3b4-1642">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1642">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="1d3b4-1643">??에 `--plan-name`, `--plan-product`, `--plan-promotion-code` 및 `--plan-publisher` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1643">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to</span></span> `[vm|vmss] create`
* <span data-ttu-id="1d3b4-1644">??에서 오류 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1644">Fixed error issues with</span></span> `[vm|vmss] create`
* <span data-ttu-id="1d3b4-1645">??에 의해 발생하는 과도한 리소스 사용량 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1645">Fixed excessive resource usage caused by</span></span> `vm image list --all`

## <a name="december-19-2017"></a><span data-ttu-id="1d3b4-1646">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1646">December 19, 2017</span></span>

<span data-ttu-id="1d3b4-1647">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1647">Version 2.0.23</span></span>

* <span data-ttu-id="1d3b4-1648">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1648">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1649">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1649">Container</span></span>

* <span data-ttu-id="1d3b4-1650">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1650">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1651">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1651">Network</span></span>

* <span data-ttu-id="1d3b4-1652">??에 `--disable-bgp-route-propagation` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1652">Added `--disable-bgp-route-propagation` argument to</span></span> `route-table [create|update]`
* <span data-ttu-id="1d3b4-1653">??에 `--ip-tags` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1653">Added `--ip-tags` argument to</span></span> `public-ip [create|update]`

### <a name="storage"></a><span data-ttu-id="1d3b4-1654">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1654">Storage</span></span>

* <span data-ttu-id="1d3b4-1655">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1655">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1656">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1656">VM</span></span>

* <span data-ttu-id="1d3b4-1657">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1657">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="1d3b4-1658">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1658">December 5, 2017</span></span>

<span data-ttu-id="1d3b4-1659">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1659">Version 2.0.22</span></span>

* <span data-ttu-id="1d3b4-1660">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1660">Removed `az component` commands.</span></span> <span data-ttu-id="1d3b4-1661">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1661">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1662">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1662">Core</span></span>
* <span data-ttu-id="1d3b4-1663">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1663">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="1d3b4-1664">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1664">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1665">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1665">ACS</span></span>

* <span data-ttu-id="1d3b4-1666">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1666">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="1d3b4-1667">??에 대한 오류 보고 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1667">Improved error reporting for</span></span> `acs create`
* <span data-ttu-id="1d3b4-1668">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1668">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="1d3b4-1669">Advisor</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1669">Advisor</span></span>

* <span data-ttu-id="1d3b4-1670">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1670">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1671">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1671">Appservice</span></span>

* <span data-ttu-id="1d3b4-1672">??을(를) 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1672">Fixed cert name generation with</span></span> `webapp config ssl upload`
* <span data-ttu-id="1d3b4-1673">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1673">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="1d3b4-1674">??에 대한 기본값 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1674">Added default value for</span></span> `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a><span data-ttu-id="1d3b4-1675">Consumption</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1675">Consumption</span></span>

* <span data-ttu-id="1d3b4-1676">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1676">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1677">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1677">Container</span></span>

* <span data-ttu-id="1d3b4-1678">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1678">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1679">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1679">Monitor</span></span>

* <span data-ttu-id="1d3b4-1680">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1680">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1681">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1681">Resource</span></span>

* <span data-ttu-id="1d3b4-1682">??에 `--include-response-body` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1682">Added `--include-response-body` argument to</span></span> `resource show`

### <a name="role"></a><span data-ttu-id="1d3b4-1683">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1683">Role</span></span>

* <span data-ttu-id="1d3b4-1684">??에 "클래식" 관리자에 대한 기본 할당 표시 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1684">Added display of default assignments for "classic" administraors to</span></span> `role assignment list`
* <span data-ttu-id="1d3b4-1685">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1685">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="1d3b4-1686">??에 대한 오류 보고 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1686">Improved error reporting for</span></span> `ad sp create-for-rbac`

### <a name="sql"></a><span data-ttu-id="1d3b4-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1687">SQL</span></span>

* <span data-ttu-id="1d3b4-1688">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1688">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="1d3b4-1689">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1689">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1690">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1690">VM</span></span>

* <span data-ttu-id="1d3b4-1691">??에 영역 정보 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1691">Added zone information to</span></span> `az vm list-skus`


## <a name="november-14-2017"></a><span data-ttu-id="1d3b4-1692">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1692">November 14, 2017</span></span>

<span data-ttu-id="1d3b4-1693">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1693">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-1694">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1694">ACR</span></span>

* <span data-ttu-id="1d3b4-1695">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1695">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1d3b4-1696">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1696">ACS</span></span>

* <span data-ttu-id="1d3b4-1697">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1697">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1d3b4-1698">??에 대한 `--orchestrator-release` 옵션이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1698">Deprecated `--orchestrator-release` option for</span></span> `acs create`
* <span data-ttu-id="1d3b4-1699">AKS의 기본 VM 크기를 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1699">Changed default VM size for AKS to</span></span> `Standard_D1_v2`
* <span data-ttu-id="1d3b4-1700">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1700">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1d3b4-1701">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1701">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1702">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1702">Appservice</span></span>

* <span data-ttu-id="1d3b4-1703">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1703">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1d3b4-1704">??에 `--docker-container-logging` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1704">Added `--docker-container-logging` option to</span></span> `az webapp log config`
* <span data-ttu-id="1d3b4-1705">??의 매개 변수 `--web-server-logging`에서 `storage` 옵션 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1705">Removed the `storage` option from the parameter `--web-server-logging` of</span></span> `az webapp log config`
* <span data-ttu-id="1d3b4-1706">??에 대한 오류 메시지 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1706">Improved error messages for</span></span> `deployment user set`
* <span data-ttu-id="1d3b4-1707">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1707">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1d3b4-1708">수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1708">Fixed</span></span> `list-locations`

### <a name="batch"></a><span data-ttu-id="1d3b4-1709">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1709">Batch</span></span>

* <span data-ttu-id="1d3b4-1710">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1710">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1d3b4-1711">Batchai</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1711">Batchai</span></span>

* <span data-ttu-id="1d3b4-1712">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1712">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1d3b4-1713">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1713">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1d3b4-1714">`job list-files` 및 ?? 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1714">Fixed documentation for `job list-files` and</span></span> `job stream-file`
* <span data-ttu-id="1d3b4-1715">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1715">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1d3b4-1716">클라우드</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1716">Cloud</span></span>

* <span data-ttu-id="1d3b4-1717">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1717">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1718">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1718">Container</span></span>

* <span data-ttu-id="1d3b4-1719">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1719">Added support to open multiple ports</span></span>
* <span data-ttu-id="1d3b4-1720">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1720">Added container group restart policy</span></span>
* <span data-ttu-id="1d3b4-1721">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1721">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1d3b4-1722">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1722">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1d3b4-1723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1723">Data Lake Analytics</span></span>

* <span data-ttu-id="1d3b4-1724">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1724">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1d3b4-1725">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1725">Data Lake Store</span></span>

* <span data-ttu-id="1d3b4-1726">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1726">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1d3b4-1727">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1727">Extension</span></span>

* <span data-ttu-id="1d3b4-1728">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1728">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1d3b4-1729">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1729">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-1730">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1730">IoT</span></span>

* <span data-ttu-id="1d3b4-1731">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1731">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1732">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1732">Monitor</span></span>

* <span data-ttu-id="1d3b4-1733">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1733">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1734">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1734">Network</span></span>

* <span data-ttu-id="1d3b4-1735">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1735">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1d3b4-1736">??(으)로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1736">Fixed issue where endpoints could not be updated with</span></span> `traffic-manager profile update`
* <span data-ttu-id="1d3b4-1737">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1737">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1d3b4-1738">??이(가) 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1738">Fixed issue where relative DNS names were incorrectly imported by</span></span> `dns zone import`

### <a name="reservations"></a><span data-ttu-id="1d3b4-1739">예약</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1739">Reservations</span></span>

* <span data-ttu-id="1d3b4-1740">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1740">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1741">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1741">Resource</span></span>

* <span data-ttu-id="1d3b4-1742">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1742">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1743">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1743">SQL</span></span>

* <span data-ttu-id="1d3b4-1744">??에 `--ignore-missing-vnet-service-endpoint` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1744">Added `--ignore-missing-vnet-service-endpoint` parameter to</span></span> `sql server vnet-rule [create|update]`

### <a name="storage"></a><span data-ttu-id="1d3b4-1745">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1745">Storage</span></span>

* <span data-ttu-id="1d3b4-1746">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1746">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1d3b4-1747">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1747">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1d3b4-1748">`--source-uri`를 ??와(과) 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1748">Fixed bug that prevented using `--source-uri` with</span></span> `storage [blob|file] copy start-batch`
* <span data-ttu-id="1d3b4-1749">GLOB에 명령 추가 및 ??을(를) 포함하는 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1749">Added commands to glob and delete multiple objects with</span></span> `storage [blob|file] delete-batch`
* <span data-ttu-id="1d3b4-1750">??(으)로 메트릭을 사용하도록 설정할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1750">Fixed issue when enabling metrics with</span></span> `storage metrics update`
* <span data-ttu-id="1d3b4-1751">??을(를) 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1751">Fixed issue with files over 200GB when using</span></span> `storage blob upload-batch`
* <span data-ttu-id="1d3b4-1752">??에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1752">Fixed issue where `--bypass` and `--default-action` were ignored by</span></span> `storage account [create|update]`

### <a name="vm"></a><span data-ttu-id="1d3b4-1753">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1753">VM</span></span>

* <span data-ttu-id="1d3b4-1754">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1754">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1d3b4-1755">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1755">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1d3b4-1756">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1756">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1d3b4-1757">`vm format-secret`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1757">Renamed `vm format-secret` to</span></span> `vm secret format`
* <span data-ttu-id="1d3b4-1758">??에 `--encrypt format` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1758">Added `--encrypt format` argument to</span></span> `vm encryption enable`

## <a name="october-24-2017"></a><span data-ttu-id="1d3b4-1759">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1759">October 24, 2017</span></span>

<span data-ttu-id="1d3b4-1760">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1760">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1761">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1761">Core</span></span>

* <span data-ttu-id="1d3b4-1762">`MGMT_STORAGE` API 버전 ??을(를) 사용하도록 `2017-03-09-profile` 업데이트</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1762">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version</span></span> `2016-01-01`

### <a name="acr"></a><span data-ttu-id="1d3b4-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1763">ACR</span></span>

* <span data-ttu-id="1d3b4-1764">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1764">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1d3b4-1765">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1765">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1d3b4-1766">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1766">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1767">ACS</span></span>

* <span data-ttu-id="1d3b4-1768">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1768">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1d3b4-1769">Kubernetes ?? 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1769">Fixed kubernetes</span></span> `get-credentials`

### <a name="appservice"></a><span data-ttu-id="1d3b4-1770">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1770">Appservice</span></span>

* <span data-ttu-id="1d3b4-1771">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1771">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1d3b4-1772">구성 요소</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1772">Component</span></span>

* <span data-ttu-id="1d3b4-1773">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1773">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-1774">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1774">Monitor</span></span>

* <span data-ttu-id="1d3b4-1775">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1775">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1776">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1776">Resource</span></span>

* <span data-ttu-id="1d3b4-1777">??의 최신 버전 msrest 종속성과의 비호환성 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1777">Fixed incompatibility with most recent version of msrest dependency in</span></span> `group export`
* <span data-ttu-id="1d3b4-1778">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1778">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1779">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1779">VM</span></span>

* <span data-ttu-id="1d3b4-1780">??에 `--accelerated-networking` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1780">Added `--accelerated-networking` argument to</span></span> `vmss create`


## <a name="october-9-2017"></a><span data-ttu-id="1d3b4-1781">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1781">October 9, 2017</span></span>

<span data-ttu-id="1d3b4-1782">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1782">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1783">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1783">Core</span></span>

* <span data-ttu-id="1d3b4-1784">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1784">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1785">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1785">Appservice</span></span>

* <span data-ttu-id="1d3b4-1786">새 명령 ??(으)로 일반 업데이트 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1786">Added generic update with new command</span></span> `webapp update`

### <a name="batch"></a><span data-ttu-id="1d3b4-1787">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1787">Batch</span></span>

* <span data-ttu-id="1d3b4-1788">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1788">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1d3b4-1789">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1789">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1d3b4-1790">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1790">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1d3b4-1791">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1791">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1d3b4-1792">Batchai</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1792">Batchai</span></span>

* <span data-ttu-id="1d3b4-1793">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1793">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-1794">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1794">Keyvault</span></span>

* <span data-ttu-id="1d3b4-1795">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1795">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1d3b4-1796">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1796">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1d3b4-1797">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1797">Network</span></span>

* <span data-ttu-id="1d3b4-1798">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1798">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1d3b4-1799">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1799">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1800">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1800">Resource</span></span>

* <span data-ttu-id="1d3b4-1801">??에 리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1801">Added support for `--resource-group/-g` options for resource group name to</span></span> `group`
* <span data-ttu-id="1d3b4-1802">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1802">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1d3b4-1803">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1803">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1d3b4-1804">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1804">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1805">Sql</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1805">Sql</span></span>

* <span data-ttu-id="1d3b4-1806">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1806">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1d3b4-1807">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1807">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1d3b4-1808">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1808">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1809">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1809">Storage</span></span>

* <span data-ttu-id="1d3b4-1810">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1810">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1811">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1811">Vm</span></span>

* <span data-ttu-id="1d3b4-1812">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1812">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1d3b4-1813">[미리 보기] ??에 롤링 업그레이드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1813">[PREVIEW] Added support for rolling upgrade to</span></span> `vmss create`
* <span data-ttu-id="1d3b4-1814">??을(를) 사용하여 암호화 설정 업데이트 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1814">Added support for updating encryption settings with</span></span> `vm encryption enable`
* <span data-ttu-id="1d3b4-1815">??에 `--os-disk-size-gb` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1815">Added `--os-disk-size-gb` parameter to</span></span> `vm create`
* <span data-ttu-id="1d3b4-1816">??에 Windows용 `--license-type` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1816">Added `--license-type` parameter for Windows to</span></span> `vmss create`


## <a name="september-22-2017"></a><span data-ttu-id="1d3b4-1817">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1817">September 22, 2017</span></span>

<span data-ttu-id="1d3b4-1818">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1818">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-1819">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1819">Resource</span></span>

* <span data-ttu-id="1d3b4-1820">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1820">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1d3b4-1821">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1821">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1d3b4-1822">??에 UI 정의 및 템플릿 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1822">Added support for UI definitions and templates to</span></span> `managedapp definition create`
* <span data-ttu-id="1d3b4-1823">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 ??(으)로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1823">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to</span></span> `applicationDefinitions`

### <a name="network"></a><span data-ttu-id="1d3b4-1824">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1824">Network</span></span>

* <span data-ttu-id="1d3b4-1825">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1825">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1d3b4-1826">??에 IPv6 Microsoft 피어링 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1826">Added support for IPv6 Microsoft Peering to</span></span> `express-route`
* <span data-ttu-id="1d3b4-1827">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1827">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1d3b4-1828">??에 `--application-security-groups` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1828">Added `--application-security-groups` argument to</span></span> `nic [create|ip-config create|ip-config update]`
* <span data-ttu-id="1d3b4-1829">??에 `--source-asgs` 및 `--destination-asgs` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1829">Added `--source-asgs` and `--destination-asgs` arguments to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="1d3b4-1830">??에 `--ddos-protection` 및 `--vm-protection` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1830">Added `--ddos-protection` and `--vm-protection` arguments to</span></span> `vnet [create|update]`
* <span data-ttu-id="1d3b4-1831">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1831">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1832">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1832">Storage</span></span>

* <span data-ttu-id="1d3b4-1833">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1833">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1d3b4-1834">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1834">Eventgrid</span></span>

* <span data-ttu-id="1d3b4-1835">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1835">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1836">SQL</span></span>

* <span data-ttu-id="1d3b4-1837">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1837">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1d3b4-1838">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1838">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1d3b4-1839">`db [create|copy|restore|update|replica create|create|update]` 및 ??에 `--no-wait` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1839">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and</span></span> `dw [create|update]`

### <a name="keyvault"></a><span data-ttu-id="1d3b4-1840">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1840">Keyvault</span></span>

* <span data-ttu-id="1d3b4-1841">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1841">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1842">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1842">VM</span></span>

* <span data-ttu-id="1d3b4-1843">??에 가용성 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1843">Added for support to availability zone to</span></span> `[vm|vmss|disk] create`
* <span data-ttu-id="1d3b4-1844">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1844">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1d3b4-1845">??에 `--asgs` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1845">Added `--asgs` argument to</span></span> `vm create`
* <span data-ttu-id="1d3b4-1846">??을(를) 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1846">Added support for running commands on VMs with</span></span> `vm run-command`
* <span data-ttu-id="1d3b4-1847">[미리 보기] ??을(를) 사용하여 VMSS 디스크 암호화 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1847">[PREVIEW] Added support for VMSS disk encryption with</span></span> `vmss encryption`
* <span data-ttu-id="1d3b4-1848">??을(를) 사용하여 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1848">Added support for performing maintenance on VMs with</span></span> `vm perform-maintenance`

### <a name="acs"></a><span data-ttu-id="1d3b4-1849">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1849">ACS</span></span>

* <span data-ttu-id="1d3b4-1850">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1850">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1851">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1851">Appservice</span></span>

* <span data-ttu-id="1d3b4-1852">??을(를) 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1852">Added ability to update and show authentication settings with</span></span> `webapp auth [update|show]`

### <a name="backup"></a><span data-ttu-id="1d3b4-1853">Backup</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1853">Backup</span></span>

* <span data-ttu-id="1d3b4-1854">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1854">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1d3b4-1855">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1855">September 11, 2017</span></span>

<span data-ttu-id="1d3b4-1856">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1856">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1d3b4-1857">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1857">Core</span></span>

* <span data-ttu-id="1d3b4-1858">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1858">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1d3b4-1859">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1859">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1860">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1860">Acs</span></span>

* <span data-ttu-id="1d3b4-1861">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1861">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1d3b4-1862">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1862">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1863">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1863">Appservice</span></span>

* <span data-ttu-id="1d3b4-1864">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1864">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1d3b4-1865">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1865">CDN</span></span>

* <span data-ttu-id="1d3b4-1866">??에 대한 'CustomDomain is not interable' 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1866">Fixed 'CustomDomain is not interable' bug for</span></span> `cdn custom-domain create`

### <a name="extension"></a><span data-ttu-id="1d3b4-1867">내선 번호</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1867">Extension</span></span>

* <span data-ttu-id="1d3b4-1868">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1868">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-1869">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1869">Keyvault</span></span>

* <span data-ttu-id="1d3b4-1870">??에 대한 사용 권한이 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1870">Fixed issue where permissions were case sensitive for</span></span> `keyvault set-policy`

### <a name="network"></a><span data-ttu-id="1d3b4-1871">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1871">Network</span></span>

* <span data-ttu-id="1d3b4-1872">`vnet list-private-access-services`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1872">Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="1d3b4-1873">??의 `--private-access-services` 인수 이름을 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1873">Renamed `--private-access-services` argument to `--service-endpoints` for</span></span> `vnet subnet create/update`
* <span data-ttu-id="1d3b4-1874">??에 여러 IP 범위 및 포트 범위에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1874">Added support for multiple IP ranges and port ranges to</span></span> `nsg rule create/update`
* <span data-ttu-id="1d3b4-1875">??에 SKU 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1875">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="1d3b4-1876">??에 SKU 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1876">Added support for SKU to</span></span> `public-ip create`

### <a name="resource"></a><span data-ttu-id="1d3b4-1877">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1877">Resource</span></span>

* <span data-ttu-id="1d3b4-1878">`policy definition create` 및 ??에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1878">Allow passing in resource policy parameter definitions in `policy definition create`, and</span></span> `policy definition update`
* <span data-ttu-id="1d3b4-1879">??의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1879">Allow passing in parameter values for</span></span> `policy assignment create`
* <span data-ttu-id="1d3b4-1880">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1880">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1d3b4-1881">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1881">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-1882">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1882">SQL</span></span>

* <span data-ttu-id="1d3b4-1883">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1883">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1884">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1884">VM</span></span>

* <span data-ttu-id="1d3b4-1885">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1885">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1d3b4-1886">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1886">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1d3b4-1887">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1887">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1d3b4-1888">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1888">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1d3b4-1889">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1889">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1d3b4-1890">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1890">August 31, 2017</span></span>

<span data-ttu-id="1d3b4-1891">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1891">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-1892">Keyvault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1892">Keyvault</span></span>

* <span data-ttu-id="1d3b4-1893">??(으)로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1893">Fixed bug when trying to automatically resolve secret encoding with</span></span> `secret download`

### <a name="sf"></a><span data-ttu-id="1d3b4-1894">Sf</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1894">Sf</span></span>

* <span data-ttu-id="1d3b4-1895">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1895">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1896">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1896">Storage</span></span>

* <span data-ttu-id="1d3b4-1897">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1897">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1d3b4-1898">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1898">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1d3b4-1899">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1899">August 28, 2017</span></span>

<span data-ttu-id="1d3b4-1900">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1900">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1d3b4-1901">CLI</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1901">CLI</span></span>

* <span data-ttu-id="1d3b4-1902">??에 법적 고지 사항 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1902">Added legal note to</span></span> `--version`

### <a name="acs"></a><span data-ttu-id="1d3b4-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1903">ACS</span></span>

* <span data-ttu-id="1d3b4-1904">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1904">Corrected preview regions</span></span>
* <span data-ttu-id="1d3b4-1905">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1905">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="1d3b4-1906">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1906">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1907">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1907">Appservice</span></span>

* <span data-ttu-id="1d3b4-1908">[호환성이 손상되는 변경] ?? 출력의 불일치 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1908">[BREAKING CHANGE] Fixed inconsistencies in the output of</span></span> `az webapp config appsettings [delete|set]`
* <span data-ttu-id="1d3b4-1909">??에 대한 `-i`의 새 별칭 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1909">Added a new alias of `-i` for</span></span> `az webapp config container set --docker-custom-image-name`
* <span data-ttu-id="1d3b4-1910">?? 공개</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1910">Exposed</span></span> `az webapp log show`
* <span data-ttu-id="1d3b4-1911">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1911">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1d3b4-1912">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1912">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-1913">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1913">IoT</span></span>

* <span data-ttu-id="1d3b4-1914">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1914">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1915">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1915">Network</span></span>

* <span data-ttu-id="1d3b4-1916">[호환성이 손상되는 변경] `vnet list-private-access-services`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1916">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="1d3b4-1917">[호환성이 손상되는 변경] ??에 대한 옵션 `--private-access-services`의 이름을 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1917">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for</span></span> `vnet subnet [create|update]`
* <span data-ttu-id="1d3b4-1918">??에 여러 IP 및 포트 범위에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1918">Added support for multiple IP and port ranges to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="1d3b4-1919">??에 SKU 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1919">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="1d3b4-1920">??에 SKU 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1920">Added support for SKU to</span></span> `public-ip create`

### <a name="profile"></a><span data-ttu-id="1d3b4-1921">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1921">Profile</span></span>

* <span data-ttu-id="1d3b4-1922">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1922">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1d3b4-1923">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1923">Service Fabric</span></span>

* <span data-ttu-id="1d3b4-1924">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1924">Preview release</span></span>
* <span data-ttu-id="1d3b4-1925">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1925">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1d3b4-1926">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1926">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1d3b4-1927">빈 ??에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1927">Added support for empty</span></span> `registry_cred`

### <a name="storage"></a><span data-ttu-id="1d3b4-1928">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1928">Storage</span></span>

* <span data-ttu-id="1d3b4-1929">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1929">Enabled setting blob tier</span></span>
* <span data-ttu-id="1d3b4-1930">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1930">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1d3b4-1931">??에 VNET 규칙 및 IP 기반 규칙을 추가하는 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1931">Added commands to add VNET rules and IP based rules to</span></span> `storage account network-rule`
* <span data-ttu-id="1d3b4-1932">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1932">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1d3b4-1933">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1933">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1d3b4-1934">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1934">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1935">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1935">VM</span></span>

* <span data-ttu-id="1d3b4-1936">??을(를) 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1936">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using</span></span> `--instance-id *`
* <span data-ttu-id="1d3b4-1937">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1937">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="1d3b4-1938">??에 대한 관리자 이름 블랙리스트에서 사람의 이름 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1938">Removed human names from the admin name blacklist for</span></span> `[vm|vmss] create`
* <span data-ttu-id="1d3b4-1939">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1939">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1d3b4-1940">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1940">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1d3b4-1941">`--no-wait` 인수가 ??에서 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1941">Fixed issue where `--no-wait` argument did not work wth</span></span> `vm availability-set create`


## <a name="august-15-2017"></a><span data-ttu-id="1d3b4-1942">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1942">August 15, 2017</span></span>

<span data-ttu-id="1d3b4-1943">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1943">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1944">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1944">ACS</span></span>

* <span data-ttu-id="1d3b4-1945">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1945">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-1946">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1946">Appservice</span></span>

* <span data-ttu-id="1d3b4-1947">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1947">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1d3b4-1948">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1948">Event Grid</span></span>

* <span data-ttu-id="1d3b4-1949">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1949">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1d3b4-1950">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1950">August 11, 2017</span></span>

<span data-ttu-id="1d3b4-1951">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1951">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-1952">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1952">ACS</span></span>

* <span data-ttu-id="1d3b4-1953">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1953">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1d3b4-1954">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1954">Batch</span></span>

* <span data-ttu-id="1d3b4-1955">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1955">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1d3b4-1956">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1956">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1d3b4-1957">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1957">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1d3b4-1958">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1958">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1d3b4-1959">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1959">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1d3b4-1960">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1960">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1d3b4-1961">구성 요소</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1961">Component</span></span>

* <span data-ttu-id="1d3b4-1962">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1962">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1d3b4-1963">컨테이너</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1963">Container</span></span>

* `create`<span data-ttu-id="1d3b4-1964">: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1964">: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1d3b4-1965">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1965">Data Lake Store</span></span>

* <span data-ttu-id="1d3b4-1966">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1966">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1d3b4-1967">Event Grid</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1967">Event Grid</span></span>

* <span data-ttu-id="1d3b4-1968">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1968">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-1969">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1969">Network</span></span>

* `lb`<span data-ttu-id="1d3b4-1970">: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1970">: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* `application-gateway {subresource} delete`<span data-ttu-id="1d3b4-1971">: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1971">: Fixed issue where `--no-wait` was not honored</span></span>
* `application-gateway http-settings update`<span data-ttu-id="1d3b4-1972">: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1972">: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1d3b4-1973">??에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1973">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with</span></span> `az network vpn-connection ipsec-policy add`

### <a name="profile"></a><span data-ttu-id="1d3b4-1974">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1974">Profile</span></span>

* `account list`<span data-ttu-id="1d3b4-1975">: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1975">: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-1976">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1976">Storage</span></span>

* <span data-ttu-id="1d3b4-1977">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1977">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-1978">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1978">VM</span></span>

* `availability-set`<span data-ttu-id="1d3b4-1979">: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1979">: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1d3b4-1980">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1980">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1d3b4-1981">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1981">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1d3b4-1982">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1982">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1d3b4-1983">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1983">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1d3b4-1984">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1984">July 28, 2017</span></span>

<span data-ttu-id="1d3b4-1985">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1985">Version 2.0.12</span></span>

* <span data-ttu-id="1d3b4-1986">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1986">Added container commands</span></span>
* <span data-ttu-id="1d3b4-1987">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1987">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1d3b4-1988">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1988">Core</span></span>

* <span data-ttu-id="1d3b4-1989">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1989">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1d3b4-1990">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1990">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1d3b4-1991">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1991">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1d3b4-1992">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1992">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1d3b4-1993">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1993">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1d3b4-1994">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1994">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1d3b4-1995">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1995">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1d3b4-1996">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1996">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1d3b4-1997">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1997">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1d3b4-1998">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1998">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1d3b4-1999">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="1d3b4-1999">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1d3b4-2000">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2000">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1d3b4-2001">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2001">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1d3b4-2002">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2002">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1d3b4-2003">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2003">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1d3b4-2004">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2004">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1d3b4-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2005">ACR</span></span>

* <span data-ttu-id="1d3b4-2006">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2006">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1d3b4-2007">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2007">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1d3b4-2008">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2008">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1d3b4-2009">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2009">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1d3b4-2010">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2010">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1d3b4-2011">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2011">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-2012">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2012">ACS</span></span>

* <span data-ttu-id="1d3b4-2013">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2013">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-2014">App Service</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2014">Appservice</span></span>

* <span data-ttu-id="1d3b4-2015">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2015">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1d3b4-2016">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2016">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1d3b4-2017">?? 아래의 모든 명령 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2017">Remove all commands under</span></span> `appservice web`
* <span data-ttu-id="1d3b4-2018">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2018">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1d3b4-2019">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2019">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1d3b4-2020">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2020">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1d3b4-2021">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2021">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1d3b4-2022">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2022">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1d3b4-2023">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2023">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1d3b4-2024">대신 사용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2024">Instead use</span></span> `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a><span data-ttu-id="1d3b4-2025">Batch</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2025">Batch</span></span>

* <span data-ttu-id="1d3b4-2026">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2026">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1d3b4-2027">??에 대한 `pool create` 옵션의 이름을 `--target-dedicated`로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2027">Renamed `pool create` option `--target-dedicated` to</span></span> `--target-dedicated-nodes`
* <span data-ttu-id="1d3b4-2028">`pool create` 옵션 `--target-low-priority-nodes` 추가 및</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2028">Added `pool create` options `--target-low-priority-nodes` and</span></span> `--application-licenses`

### <a name="cdn"></a><span data-ttu-id="1d3b4-2029">CDN</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2029">CDN</span></span>

* <span data-ttu-id="1d3b4-2030">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2030">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="1d3b4-2031">클라우드</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2031">Cloud</span></span>

* <span data-ttu-id="1d3b4-2032">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2032">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1d3b4-2033">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2033">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1d3b4-2034">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2034">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1d3b4-2035">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2035">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1d3b4-2036">?? 공개</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2036">Exposed</span></span> `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-2037">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2037">CosmosDB</span></span>

* <span data-ttu-id="1d3b4-2038">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2038">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1d3b4-2039">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2039">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1d3b4-2040">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2040">Data Lake Analytics</span></span>

* <span data-ttu-id="1d3b4-2041">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2041">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1d3b4-2042">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2042">Added</span></span> `dla job pipeline show`
* <span data-ttu-id="1d3b4-2043">추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2043">Added</span></span> `dla job recurrence list`

### <a name="data-lake-store"></a><span data-ttu-id="1d3b4-2044">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2044">Data Lake Store</span></span>

* <span data-ttu-id="1d3b4-2045">??에서 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2045">Added support for user managed key vault key rotation in</span></span> `dls account update`
* <span data-ttu-id="1d3b4-2046">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2046">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1d3b4-2047">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2047">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1d3b4-2048">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2048">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1d3b4-2049">대화형</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2049">Interactive</span></span>

* <span data-ttu-id="1d3b4-2050">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2050">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1d3b4-2051">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2051">Increased test coverage</span></span>
* <span data-ttu-id="1d3b4-2052">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2052">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1d3b4-2053">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2053">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1d3b4-2054">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2054">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1d3b4-2055">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2055">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1d3b4-2056">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2056">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1d3b4-2057">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2057">Added `--progress` flag</span></span>
* <span data-ttu-id="1d3b4-2058">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2058">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1d3b4-2059">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2059">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1d3b4-2060">IoT</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2060">IoT</span></span>

* <span data-ttu-id="1d3b4-2061">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2061">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1d3b4-2062">(#3934)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2062">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1d3b4-2063">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2063">Key vault</span></span>

* <span data-ttu-id="1d3b4-2064">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2064">Added commands for key vault recovery features:</span></span>
  * `keyvault` <span data-ttu-id="1d3b4-2065">하위 명령 `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2065">subcommands `purge`, `recover`,</span></span> `keyvault list-deleted`
  * `keyvault secret` <span data-ttu-id="1d3b4-2066">하위 명령 `backup`, `restore`, `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2066">subcommands `backup`, `restore`, `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault certificate` <span data-ttu-id="1d3b4-2067">하위 명령 `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2067">subcommands `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault key` <span data-ttu-id="1d3b4-2068">하위 명령 `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2068">subcommands `purge`, `recover`,</span></span> `list-deleted`
* <span data-ttu-id="1d3b4-2069">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2069">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1d3b4-2070">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2070">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1d3b4-2071">(#3307)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2071">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1d3b4-2072">랩</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2072">Lab</span></span>

* <span data-ttu-id="1d3b4-2073">??을(를) 통한 랩의 모든 VM 요청 작업에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2073">Added support for claiming any vm in the lab through</span></span> `az lab vm claim`
* <span data-ttu-id="1d3b4-2074">`az lab vm list` 및 ??에 대한 테이블 출력 포맷터 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2074">Added table output formatter for `az lab vm list` and</span></span> `az lab vm show`

### <a name="monitor"></a><span data-ttu-id="1d3b4-2075">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2075">Monitor</span></span>

* <span data-ttu-id="1d3b4-2076">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2076">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1d3b4-2077">`monitor alert-rule-incidents list`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2077">Renamed `monitor alert-rule-incidents list` to</span></span> `monitor alert list-incidents`
* <span data-ttu-id="1d3b4-2078">`monitor alert-rule-incidents show`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2078">Renamed `monitor alert-rule-incidents show` to</span></span> `monitor alert show-incident`
* <span data-ttu-id="1d3b4-2079">`monitor metric-defintions list`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2079">Renamed `monitor metric-defintions list` to</span></span> `monitor metrics list-definitions`
* <span data-ttu-id="1d3b4-2080">`monitor alert-rules`의 이름을 ??(으)로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2080">Renamed `monitor alert-rules` to</span></span> `monitor alert`
* <span data-ttu-id="1d3b4-2081">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2081">Changed `monitor alert create`:</span></span>
  * `condition` <span data-ttu-id="1d3b4-2082">및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2082">and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1d3b4-2083">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2083">Add numerous parameters to simplify the rule creation process</span></span>
  * `location` <span data-ttu-id="1d3b4-2084">??은(는) 더 이상 필수가 아님</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2084">no longer required</span></span>
  * <span data-ttu-id="1d3b4-2085">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2085">Add name and ID support for target</span></span>
  * <span data-ttu-id="1d3b4-2086">제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2086">Remove</span></span> `--alert-rule-resource-name`
  * <span data-ttu-id="1d3b4-2087">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2087">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * `description` <span data-ttu-id="1d3b4-2088">??은(는)이제 제공된 조건에 따라 기본적으로 설정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2088">defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1d3b4-2089">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2089">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1d3b4-2090">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2090">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1d3b4-2091">??에 편의 인수 및 예제 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2091">Added convenience arguments and examples to</span></span> `monitor alert rule update`

### <a name="network"></a><span data-ttu-id="1d3b4-2092">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2092">Network</span></span>

* <span data-ttu-id="1d3b4-2093">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2093">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1d3b4-2094">`vnet subnet create` 및 ??에 `--private-access-services` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2094">Added `--private-access-services` argument to `vnet subnet create` and</span></span> `vnet subnet update`
* <span data-ttu-id="1d3b4-2095">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2095">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1d3b4-2096">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2096">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1d3b4-2097">`application-gateway address-pool create` 및 ??에 `--servers` 인수를 사용하는 경우 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2097">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and</span></span> `application-gateway address-pool update`
* <span data-ttu-id="1d3b4-2098">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2098">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1d3b4-2099">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2099">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`,</span></span> `predefined show`
* <span data-ttu-id="1d3b4-2100">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2100">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span></span> `--min-protocol-version`
* <span data-ttu-id="1d3b4-2101">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2101">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1d3b4-2102">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2102">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`,</span></span> `--redirect-config`
* <span data-ttu-id="1d3b4-2103">??에 `--redirect-config` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2103">Added argument `--redirect-config` to</span></span> `application-gateway url-path-map rule create`
* <span data-ttu-id="1d3b4-2104">??에 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2104">Added support for `--no-wait` to</span></span> `application-gateway url-path-map rule delete`
* <span data-ttu-id="1d3b4-2105">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2105">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span></span> `--match-status-codes`
* <span data-ttu-id="1d3b4-2106">`application-gateway rule create` 및 ??에 `--redirect-config` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2106">Added argument `--redirect-config` to `application-gateway rule create` and</span></span> `application-gateway rule update`
* <span data-ttu-id="1d3b4-2107">`nic create` 및 ??에 `--accelerated-networking` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2107">Added support for `--accelerated-networking` to `nic create` and</span></span> `nic update`
* <span data-ttu-id="1d3b4-2108">??에서 `--internal-dns-name-suffix` 인수 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2108">Removed `--internal-dns-name-suffix` argument from</span></span> `nic create`
* <span data-ttu-id="1d3b4-2109">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2109">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1d3b4-2110">`local-gateway create`에서 ??을(를) 무시하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2110">Fixed bug where `local-gateway create` ignored</span></span> `--local-address-prefixes`
* <span data-ttu-id="1d3b4-2111">??에 `--dns-servers` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2111">Added support for `--dns-servers` to</span></span> `vnet update`
* <span data-ttu-id="1d3b4-2112">??을(를) 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2112">Fixed bug when creating a peering without route filtering with</span></span> `express-route peering create`
* <span data-ttu-id="1d3b4-2113">`--provider` 및 `--bandwidth` 인수가 ??에서 작동하지 않았던 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2113">Fixed bug where `--provider` and `--bandwidth` arguments did not work with</span></span> `express-route update`
* <span data-ttu-id="1d3b4-2114">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2114">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1d3b4-2115">??에 대한 출력 서식 지정 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2115">Improved output formatting for</span></span> `network list-usages`
* <span data-ttu-id="1d3b4-2116">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2116">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1d3b4-2117">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2117">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1d3b4-2118">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2118">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1d3b4-2119">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2119">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1d3b4-2120">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2120">Profile</span></span>

* <span data-ttu-id="1d3b4-2121">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2121">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1d3b4-2122">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2122">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1d3b4-2123">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2123">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1d3b4-2124">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2124">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1d3b4-2125">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2125">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1d3b4-2126">RDBMS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2126">RDBMS</span></span>

* <span data-ttu-id="1d3b4-2127">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2127">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1d3b4-2128">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2128">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1d3b4-2129">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2129">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1d3b4-2130">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2130">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-2131">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2131">Resource</span></span>

* <span data-ttu-id="1d3b4-2132">??의 누락된 매개 변수에 대한 프롬프트 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2132">Improved prompts for missing parameters for</span></span> `group deployment create`
* <span data-ttu-id="1d3b4-2133">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2133">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1d3b4-2134">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2134">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1d3b4-2135">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2135">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1d3b4-2136">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2136">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1d3b4-2137">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>` 및 ??을(를) 허용하도록 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2137">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and</span></span> `<resource-type>`
* <span data-ttu-id="1d3b4-2138">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2138">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1d3b4-2139">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2139">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-2140">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2140">Role</span></span>

* <span data-ttu-id="1d3b4-2141">??에 대한 SDK 인증 파일 형식의 출력 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2141">Support output in SDK auth file format for</span></span> `create-for-rbac`
* <span data-ttu-id="1d3b4-2142">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2142">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1d3b4-2143">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2143">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1d3b4-2144">??을(를) 사용할 때 사용 중단 경고 표시</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2144">Show deprecation warnings when using</span></span> `--expanded-view`
* <span data-ttu-id="1d3b4-2145">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2145">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1d3b4-2146">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2146">Service Fabric</span></span>
* <span data-ttu-id="1d3b4-2147">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2147">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1d3b4-2148">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2148">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1d3b4-2149">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2149">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-2150">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2150">SQL</span></span>

* <span data-ttu-id="1d3b4-2151">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2151">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1d3b4-2152">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2152">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1d3b4-2153">`sql db list-editions` 및 ?? 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2153">Added commands `sql db list-editions` and</span></span> `sql elastic-pool list-editions`

### <a name="storage"></a><span data-ttu-id="1d3b4-2154">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2154">Storage</span></span>

* <span data-ttu-id="1d3b4-2155">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2155">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1d3b4-2156">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2156">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1d3b4-2157">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2157">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1d3b4-2158">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2158">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="1d3b4-2159">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2159">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="1d3b4-2160">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2160">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-2161">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2161">VM</span></span>

* <span data-ttu-id="1d3b4-2162">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2162">Support configuring nsg</span></span>
* <span data-ttu-id="1d3b4-2163">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2163">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1d3b4-2164">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2164">Support managed service identities</span></span>
* <span data-ttu-id="1d3b4-2165">기존 부하 분산 장치가 있는 `cmss create`에 ??이(가) 필요했던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2165">Fixed issue where `cmss create` with an existing load balancer required</span></span> `--backend-pool-name`
* <span data-ttu-id="1d3b4-2166">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2166">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1d3b4-2167">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2167">May 10, 2017</span></span>

<span data-ttu-id="1d3b4-2168">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2168">Version 2.0.6</span></span>

* <span data-ttu-id="1d3b4-2169">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2169">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1d3b4-2170">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2170">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1d3b4-2171">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2171">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="1d3b4-2172">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2172">Include Cognitive Services module</span></span>
* <span data-ttu-id="1d3b4-2173">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2173">Include Service Fabric module</span></span>
* <span data-ttu-id="1d3b4-2174">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2174">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="1d3b4-2175">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2175">Add support for CDN commands</span></span>
* <span data-ttu-id="1d3b4-2176">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2176">Remove Container module</span></span>
* <span data-ttu-id="1d3b4-2177">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2177">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1d3b4-2178">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2178">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1d3b4-2179">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2179">Core</span></span>

* <span data-ttu-id="1d3b4-2180">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2180">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="1d3b4-2181">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2181">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1d3b4-2182">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2182">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1d3b4-2183">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2183">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1d3b4-2184">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2184">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1d3b4-2185">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2185">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1d3b4-2186">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2186">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1d3b4-2187">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2187">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1d3b4-2188">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2188">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1d3b4-2189">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2189">core: Improved performance</span></span>
* <span data-ttu-id="1d3b4-2190">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2190">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1d3b4-2191">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2191">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2192">ACS</span></span>

* <span data-ttu-id="1d3b4-2193">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2193">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1d3b4-2194">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2194">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1d3b4-2195">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2195">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1d3b4-2196">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2196">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2197">AppService</span></span>

* <span data-ttu-id="1d3b4-2198">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2198">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1d3b4-2199">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2199">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1d3b4-2200">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2200">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1d3b4-2201">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2201">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1d3b4-2202">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2202">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1d3b4-2203">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2203">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1d3b4-2204">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2204">support slot swap with preview</span></span>
* <span data-ttu-id="1d3b4-2205">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2205">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1d3b4-2206">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2206">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1d3b4-2207">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2207">CosmosDB</span></span>

* <span data-ttu-id="1d3b4-2208">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2208">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="1d3b4-2209">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2209">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1d3b4-2210">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2210">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1d3b4-2211">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2211">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1d3b4-2212">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2212">Data Lake Analytics</span></span>

* <span data-ttu-id="1d3b4-2213">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2213">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="1d3b4-2214">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2214">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1d3b4-2215">다음을 통해 액세스:</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2215">accessed through:</span></span> `az dla catalog package`
* <span data-ttu-id="1d3b4-2216">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2216">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1d3b4-2217">테이블</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2217">Table</span></span>
  * <span data-ttu-id="1d3b4-2218">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2218">Table valued function</span></span>
  * <span data-ttu-id="1d3b4-2219">보기</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2219">View</span></span>
  * <span data-ttu-id="1d3b4-2220">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2220">Table Statistics.</span></span> <span data-ttu-id="1d3b4-2221">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2221">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1d3b4-2222">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2222">Data Lake Store</span></span>

* <span data-ttu-id="1d3b4-2223">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2223">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="1d3b4-2224">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2224">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1d3b4-2225">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2225">missed help for access show.</span></span> <span data-ttu-id="1d3b4-2226">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2226">adding it.</span></span> <span data-ttu-id="1d3b4-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1d3b4-2228">찾기</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2228">Find</span></span>

* <span data-ttu-id="1d3b4-2229">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2229">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1d3b4-2230">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2230">KeyVault</span></span>

* <span data-ttu-id="1d3b4-2231">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2231">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1d3b4-2232">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2232">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="1d3b4-2233">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2233">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1d3b4-2234">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2234">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="1d3b4-2235">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2235">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1d3b4-2236">랩</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2236">Lab</span></span>

* <span data-ttu-id="1d3b4-2237">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2237">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="1d3b4-2238">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2238">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="1d3b4-2239">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2239">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="1d3b4-2240">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2240">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="1d3b4-2241">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2241">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="1d3b4-2242">모니터</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2242">Monitor</span></span>

* <span data-ttu-id="1d3b4-2243">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2243">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1d3b4-2244">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2244">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1d3b4-2245">네트워크</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2245">Network</span></span>

* <span data-ttu-id="1d3b4-2246">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2246">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="1d3b4-2247">??의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2247">Add support for `--filters` parameter for</span></span> `network watcher packet-capture create`
* <span data-ttu-id="1d3b4-2248">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2248">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="1d3b4-2249">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2249">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="1d3b4-2250">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2250">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="1d3b4-2251">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2251">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="1d3b4-2252">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2252">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="1d3b4-2253">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2253">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="1d3b4-2254">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2254">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="1d3b4-2255">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2255">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1d3b4-2256">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2256">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="1d3b4-2257">BC: ??의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2257">BC: Fix bug in the output of</span></span> `vpn-connection create`
* <span data-ttu-id="1d3b4-2258">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2258">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="1d3b4-2259">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2259">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="1d3b4-2260">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2260">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="1d3b4-2261">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2261">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="1d3b4-2262">프로필</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2262">Profile</span></span>

* <span data-ttu-id="1d3b4-2263">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2263">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1d3b4-2264">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2264">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1d3b4-2265">Redis</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2265">Redis</span></span>

* <span data-ttu-id="1d3b4-2266">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2266">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1d3b4-2267">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2267">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="1d3b4-2268">리소스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2268">Resource</span></span>

* <span data-ttu-id="1d3b4-2269">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2269">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1d3b4-2270">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2270">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1d3b4-2271">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2271">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1d3b4-2272">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2272">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1d3b4-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1d3b4-2274">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2274">Add docs for az lock update.</span></span> <span data-ttu-id="1d3b4-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1d3b4-2276">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2276">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1d3b4-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1d3b4-2278">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2278">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1d3b4-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1d3b4-2280">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2280">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1d3b4-2281">역할</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2281">Role</span></span>

* <span data-ttu-id="1d3b4-2282">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2282">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1d3b4-2283">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2283">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1d3b4-2284">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2284">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1d3b4-2285">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2285">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1d3b4-2286">SQL</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2286">SQL</span></span>

* <span data-ttu-id="1d3b4-2287">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2287">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="1d3b4-2288">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2288">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1d3b4-2289">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2289">Storage</span></span>

* <span data-ttu-id="1d3b4-2290">??의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2290">Default location to resource group location for</span></span> `storage account create`
* <span data-ttu-id="1d3b4-2291">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2291">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1d3b4-2292">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2292">Add support for large block blob upload</span></span>
* <span data-ttu-id="1d3b4-2293">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2293">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-2294">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2294">VM</span></span>

* <span data-ttu-id="1d3b4-2295">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2295">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1d3b4-2296">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2296">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1d3b4-2297">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2297">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1d3b4-2298">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2298">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1d3b4-2299">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2299">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1d3b4-2300">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2300">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1d3b4-2301">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2301">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1d3b4-2302">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2302">April 3, 2017</span></span>

<span data-ttu-id="1d3b4-2303">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2303">Version 2.0.2</span></span>

<span data-ttu-id="1d3b4-2304">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2304">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="1d3b4-2305">코어</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2305">Core</span></span>

* <span data-ttu-id="1d3b4-2306">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2306">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="1d3b4-2307">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2307">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1d3b4-2308">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2308">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1d3b4-2309">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2309">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1d3b4-2310">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2310">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1d3b4-2311">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2311">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1d3b4-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1d3b4-2313">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2313">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1d3b4-2314">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2314">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="1d3b4-2315">ACS</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2315">ACS</span></span>

* <span data-ttu-id="1d3b4-2316">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2316">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1d3b4-2317">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2317">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1d3b4-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1d3b4-2319">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2319">Add support for windows clusters.</span></span> <span data-ttu-id="1d3b4-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1d3b4-2321">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2321">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1d3b4-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="1d3b4-2323">AppService</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2323">AppService</span></span>

* <span data-ttu-id="1d3b4-2324">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2324">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1d3b4-2325">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2325">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1d3b4-2326">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2326">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1d3b4-2327">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2327">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="1d3b4-2328">DataLake</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2328">DataLake</span></span>

* <span data-ttu-id="1d3b4-2329">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2329">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="1d3b4-2330">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2330">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="1d3b4-2331">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2331">DocuemntDB</span></span>

* <span data-ttu-id="1d3b4-2332">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2332">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1d3b4-2333">VM</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2333">VM</span></span>

* <span data-ttu-id="1d3b4-2334">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2334">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1d3b4-2335">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2335">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1d3b4-2336">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2336">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1d3b4-2337">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2337">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1d3b4-2338">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2338">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1d3b4-2339">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2339">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="1d3b4-2340">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2340">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1d3b4-2341">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2341">February 27, 2017</span></span>

<span data-ttu-id="1d3b4-2342">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2342">Version 2.0.0</span></span>

<span data-ttu-id="1d3b4-2343">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2343">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="1d3b4-2344">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2344">Container Service (acs)</span></span>
- <span data-ttu-id="1d3b4-2345">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2345">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1d3b4-2346">네트워킹</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2346">Networking</span></span>
- <span data-ttu-id="1d3b4-2347">Storage</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2347">Storage</span></span>

<span data-ttu-id="1d3b4-2348">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2348">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="1d3b4-2349">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2349">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="1d3b4-2350">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2350">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="1d3b4-2351">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2351">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="1d3b4-2352">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2352">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="1d3b4-2353">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2353">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1d3b4-2354">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2354">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1d3b4-2355">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2355">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="1d3b4-2356">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="1d3b4-2356">Provide feedback from the command line with the `az feedback` command</span></span>


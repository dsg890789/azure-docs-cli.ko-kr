---
title: "Azure CLI 2.0 릴리스 정보"
description: "Azure CLI 2.0 최신 업데이트 알아보기"
keywords: "Azure CLI 2.0, 릴리스 정보"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.contentlocale: ko-KR
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="38266-104">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="38266-104">Azure CLI 2.0 release notes</span></span>

## <a name="may-10-2017"></a><span data-ttu-id="38266-105">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="38266-105">May 10, 2017</span></span>

<span data-ttu-id="38266-106">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="38266-106">Version 2.0.6</span></span>

* <span data-ttu-id="38266-107">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="38266-107">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="38266-108">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="38266-108">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="38266-109">Data Lake Analytics 및 Data Lake Store 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-109">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="38266-110">Cognitive Services 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-110">Include Cognitive Services module.</span></span>
* <span data-ttu-id="38266-111">Service Fabric 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-111">Include Service Fabric module.</span></span>
* <span data-ttu-id="38266-112">대화형 모듈(az-shell 이름 바꾸기)을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-112">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="38266-113">CDN 명령에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-113">Add support for CDN commands.</span></span>
* <span data-ttu-id="38266-114">컨테이너 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-114">Remove Container module.</span></span>
* <span data-ttu-id="38266-115">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="38266-115">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="38266-116">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="38266-116">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="38266-117">코어</span><span class="sxs-lookup"><span data-stu-id="38266-117">Core</span></span>

* <span data-ttu-id="38266-118">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="38266-118">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="38266-119">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="38266-119">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="38266-120">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="38266-120">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="38266-121">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="38266-121">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="38266-122">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="38266-122">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="38266-123">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="38266-123">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="38266-124">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="38266-124">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="38266-125">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="38266-125">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="38266-126">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="38266-126">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="38266-127">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="38266-127">core: Improved performance</span></span>
* <span data-ttu-id="38266-128">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="38266-128">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="38266-129">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="38266-129">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="38266-130">ACS</span><span class="sxs-lookup"><span data-stu-id="38266-130">ACS</span></span>

* <span data-ttu-id="38266-131">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="38266-131">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="38266-132">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="38266-132">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="38266-133">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="38266-133">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="38266-134">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="38266-134">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="38266-135">AppService</span><span class="sxs-lookup"><span data-stu-id="38266-135">AppService</span></span>

* <span data-ttu-id="38266-136">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="38266-136">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="38266-137">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="38266-137">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="38266-138">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="38266-138">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="38266-139">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="38266-139">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="38266-140">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="38266-140">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="38266-141">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="38266-141">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="38266-142">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="38266-142">support slot swap with preview</span></span>
* <span data-ttu-id="38266-143">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="38266-143">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="38266-144">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="38266-144">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="38266-145">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="38266-145">CosmosDB</span></span>

* <span data-ttu-id="38266-146">documentdb 모듈 이름을 cosmosdb로 바꿈</span><span class="sxs-lookup"><span data-stu-id="38266-146">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="38266-147">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="38266-147">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="38266-148">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="38266-148">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="38266-149">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="38266-149">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="38266-150">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="38266-150">Data Lake Analytics</span></span>

* <span data-ttu-id="38266-151">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-151">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="38266-152">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-152">Add support for new catalog item type: package.</span></span> <span data-ttu-id="38266-153">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="38266-153">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="38266-154">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="38266-154">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="38266-155">테이블</span><span class="sxs-lookup"><span data-stu-id="38266-155">Table</span></span>
  * <span data-ttu-id="38266-156">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="38266-156">Table valued function</span></span>
  * <span data-ttu-id="38266-157">보기</span><span class="sxs-lookup"><span data-stu-id="38266-157">View</span></span>
  * <span data-ttu-id="38266-158">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="38266-158">Table Statistics.</span></span> <span data-ttu-id="38266-159">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-159">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="38266-160">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="38266-160">Data Lake Store</span></span>

* <span data-ttu-id="38266-161">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 대해 보다 나은 지원을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-161">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="38266-162">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="38266-162">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="38266-163">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="38266-163">missed help for access show.</span></span> <span data-ttu-id="38266-164">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="38266-164">adding it.</span></span> <span data-ttu-id="38266-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="38266-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="38266-166">찾기</span><span class="sxs-lookup"><span data-stu-id="38266-166">Find</span></span>

* <span data-ttu-id="38266-167">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="38266-167">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="38266-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="38266-168">KeyVault</span></span>

* <span data-ttu-id="38266-169">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="38266-169">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="38266-170">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-170">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="38266-171">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-171">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="38266-172">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-172">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="38266-173">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="38266-173">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="38266-174">랩</span><span class="sxs-lookup"><span data-stu-id="38266-174">Lab</span></span>

* <span data-ttu-id="38266-175">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="38266-175">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="38266-176">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="38266-176">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="38266-177">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-177">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="38266-178">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="38266-178">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="38266-179">랩 내에서 비밀을 관리하는 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-179">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="38266-180">모니터</span><span class="sxs-lookup"><span data-stu-id="38266-180">Monitor</span></span>

* <span data-ttu-id="38266-181">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="38266-181">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="38266-182">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="38266-182">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="38266-183">네트워크</span><span class="sxs-lookup"><span data-stu-id="38266-183">Network</span></span>

* <span data-ttu-id="38266-184">`network watcher test-connectivity` 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-184">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="38266-185">`network watcher packet-capture create`에 대한 `--filters` 매개 변수 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-185">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="38266-186">Application Gateway 연결 드레이닝에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-186">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="38266-187">Application Gateway WAF 규칙 집합 구성에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-187">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="38266-188">ExpressRoute 경로 필터 및 규칙에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-188">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="38266-189">TrafficManager 지리적 라우팅에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-189">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="38266-190">VPN 연결 정책 기반 트래픽 선택기에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-190">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="38266-191">VPN 연결 IPSec 정책에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-191">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="38266-192">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create`를 사용하여 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-192">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="38266-193">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="38266-193">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="38266-194">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="38266-194">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="38266-195">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="38266-195">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="38266-196">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-196">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="38266-197">레코드가 제대로 가져와지지 않는 `dns zone import`의 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-197">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="38266-198">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-198">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="38266-199">'network watcher' 미리 보기 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-199">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="38266-200">프로필</span><span class="sxs-lookup"><span data-stu-id="38266-200">Profile</span></span>

* <span data-ttu-id="38266-201">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="38266-201">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="38266-202">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="38266-202">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="38266-203">Redis</span><span class="sxs-lookup"><span data-stu-id="38266-203">Redis</span></span>

* <span data-ttu-id="38266-204">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="38266-204">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="38266-205">'update-settings' 명령은 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-205">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="38266-206">리소스</span><span class="sxs-lookup"><span data-stu-id="38266-206">Resource</span></span>

* <span data-ttu-id="38266-207">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="38266-207">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="38266-208">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="38266-208">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="38266-209">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="38266-209">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="38266-210">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-210">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="38266-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="38266-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="38266-212">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-212">Add docs for az lock update.</span></span> <span data-ttu-id="38266-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="38266-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="38266-214">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-214">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="38266-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="38266-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="38266-216">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-216">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="38266-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="38266-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="38266-218">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="38266-218">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="38266-219">역할</span><span class="sxs-lookup"><span data-stu-id="38266-219">Role</span></span>

* <span data-ttu-id="38266-220">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="38266-220">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="38266-221">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="38266-221">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="38266-222">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="38266-222">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="38266-223">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="38266-223">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="38266-224">SQL</span><span class="sxs-lookup"><span data-stu-id="38266-224">SQL</span></span>

* <span data-ttu-id="38266-225">az sql server list-usages 및 az sql db list-usages 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-225">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="38266-226">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="38266-226">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="38266-227">저장소</span><span class="sxs-lookup"><span data-stu-id="38266-227">Storage</span></span>

* <span data-ttu-id="38266-228">기본 위치를 `storage account create`에 대한 리소스 그룹 위치로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-228">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="38266-229">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="38266-229">Add support for incremental blob copy</span></span>
* <span data-ttu-id="38266-230">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="38266-230">Add support for large block blob upload</span></span>
* <span data-ttu-id="38266-231">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="38266-231">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="38266-232">VM</span><span class="sxs-lookup"><span data-stu-id="38266-232">VM</span></span>

* <span data-ttu-id="38266-233">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="38266-233">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="38266-234">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="38266-234">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="38266-235">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="38266-235">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="38266-236">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="38266-236">az vm/vmss disk</span></span>
  3. <span data-ttu-id="38266-237">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-237">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="38266-238">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="38266-238">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="38266-239">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="38266-239">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="38266-240">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="38266-240">April 3, 2017</span></span>

<span data-ttu-id="38266-241">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="38266-241">Version 2.0.2</span></span>

<span data-ttu-id="38266-242">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 출시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-242">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="38266-243">코어</span><span class="sxs-lookup"><span data-stu-id="38266-243">Core</span></span>

* <span data-ttu-id="38266-244">기본 목록에 acr, 랩, 모니터 및 찾기 모듈을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-244">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="38266-245">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="38266-245">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="38266-246">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="38266-246">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="38266-247">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="38266-247">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="38266-248">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="38266-248">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="38266-249">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="38266-249">Add prompting for missing template parameters.</span></span> <span data-ttu-id="38266-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="38266-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="38266-251">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="38266-251">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="38266-252">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="38266-252">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="38266-253">ACS</span><span class="sxs-lookup"><span data-stu-id="38266-253">ACS</span></span>

* [<span data-ttu-id="38266-254">ACS] 기본 ACS 클러스터 구성 지원 추가([#2554</span><span class="sxs-lookup"><span data-stu-id="38266-254">ACS] Adding support for configuring a default ACS cluster ([#2554</span></span>](https://github.com/Azure/azure-cli/pull/2554))
* <span data-ttu-id="38266-255">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="38266-255">Add support for ssh key password prompting.</span></span> <span data-ttu-id="38266-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="38266-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="38266-257">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="38266-257">Add support for windows clusters.</span></span> <span data-ttu-id="38266-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="38266-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="38266-259">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="38266-259">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="38266-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="38266-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="38266-261">AppService</span><span class="sxs-lookup"><span data-stu-id="38266-261">AppService</span></span>

* <span data-ttu-id="38266-262">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="38266-262">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="38266-263">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="38266-263">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="38266-264">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="38266-264">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="38266-265">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="38266-265">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="38266-266">DataLake</span><span class="sxs-lookup"><span data-stu-id="38266-266">DataLake</span></span>

* <span data-ttu-id="38266-267">Data Lake Analytics 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="38266-267">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="38266-268">Data Lake Store 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="38266-268">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="38266-269">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="38266-269">DocuemntDB</span></span>

* <span data-ttu-id="38266-270">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="38266-270">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="38266-271">VM</span><span class="sxs-lookup"><span data-stu-id="38266-271">VM</span></span>

* [<span data-ttu-id="38266-272">Compute] 가상 컴퓨터 확장 집합 만들기에 AppGateway 지원 추가([#2570</span><span class="sxs-lookup"><span data-stu-id="38266-272">Compute] Add AppGateway support to virtual machine scale set create ([#2570</span></span>](https://github.com/Azure/azure-cli/pull/2570))
* [<span data-ttu-id="38266-273">VM/VMSS] 향상된 디스크 캐싱 지원([#2522</span><span class="sxs-lookup"><span data-stu-id="38266-273">VM/VMSS] Improved disk caching support ([#2522</span></span>](https://github.com/Azure/azure-cli/pull/2522))
* <span data-ttu-id="38266-274">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="38266-274">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="38266-275">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="38266-275">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="38266-276">가상 컴퓨터 확장 집합: vm의 인스턴스 보기를 나열하는 * 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="38266-276">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="38266-277">VM 및 가상 컴퓨터 확장 집합에 --secrets 추가([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="38266-277">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="38266-278">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="38266-278">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="38266-279">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="38266-279">February 27, 2017</span></span>

<span data-ttu-id="38266-280">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="38266-280">Version 2.0.0</span></span>

<span data-ttu-id="38266-281">Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="38266-281">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="38266-282">일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="38266-282">General availability applies to these command modules:</span></span>
- <span data-ttu-id="38266-283">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="38266-283">Container Service (acs)</span></span>
- <span data-ttu-id="38266-284">Compute(Resource Manager, VM, 가상 컴퓨터 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="38266-284">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="38266-285">네트워킹</span><span class="sxs-lookup"><span data-stu-id="38266-285">Networking</span></span>
- <span data-ttu-id="38266-286">저장소</span><span class="sxs-lookup"><span data-stu-id="38266-286">Storage</span></span>

<span data-ttu-id="38266-287">이러한 명령은 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-287">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="38266-288">Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 개설할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-288">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="38266-289">[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-289">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
<span data-ttu-id="38266-290">`az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-290">You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="38266-291">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="38266-291">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="38266-292">CLI 버전을 확인하려면 `az --version`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-292">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="38266-293">출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="38266-293">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="38266-294">일부 명령 모듈에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-294">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="38266-295">이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="38266-295">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="38266-296">CLI 야간 미리 보기 빌드도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-296">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="38266-297">자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="38266-297">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="38266-298">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38266-298">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="38266-299">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="38266-299">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="38266-300">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.</span><span class="sxs-lookup"><span data-stu-id="38266-300">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="38266-301">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공.</span><span class="sxs-lookup"><span data-stu-id="38266-301">Provide feedback from the command line with the `az feedback` command.</span></span>


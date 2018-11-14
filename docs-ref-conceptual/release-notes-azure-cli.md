---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 51b8b8cad6d25f916006b8e68b8f300587f5d45b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222568"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="0770c-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="0770c-103">Azure CLI release notes</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="0770c-104">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="0770c-104">November 6, 2018</span></span>

<span data-ttu-id="0770c-105">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="0770c-105">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="0770c-106">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-106">Core</span></span>
* <span data-ttu-id="0770c-107">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-107">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-108">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-108">ACR</span></span>
* <span data-ttu-id="0770c-109">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-109">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="0770c-110">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-110">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-111">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-111">ACS</span></span>
* <span data-ttu-id="0770c-112">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-112">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="0770c-113">Advisor</span><span class="sxs-lookup"><span data-stu-id="0770c-113">Advisor</span></span>
* <span data-ttu-id="0770c-114">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-114">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="0770c-115">AMS</span><span class="sxs-lookup"><span data-stu-id="0770c-115">AMS</span></span>
* <span data-ttu-id="0770c-116">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="0770c-116">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="0770c-117">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="0770c-117">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="0770c-118">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-118">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="0770c-119">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="0770c-119">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="0770c-120">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-120">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="0770c-121">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-121">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="0770c-122">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-122">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="0770c-123">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0770c-123">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="0770c-124">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-124">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="0770c-125">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-125">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="0770c-126">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0770c-126">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="0770c-127">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="0770c-127">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="0770c-128">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="0770c-128">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="0770c-129">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="0770c-129">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="0770c-130">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-130">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="0770c-131">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-131">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="0770c-132">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-132">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-133">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-133">AppService</span></span>
* <span data-ttu-id="0770c-134">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-134">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="0770c-135">구성</span><span class="sxs-lookup"><span data-stu-id="0770c-135">Configure</span></span>
* <span data-ttu-id="0770c-136">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-136">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="0770c-137">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-137">Container</span></span>
* <span data-ttu-id="0770c-138">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-138">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="0770c-139">EventHub</span><span class="sxs-lookup"><span data-stu-id="0770c-139">EventHub</span></span>
* <span data-ttu-id="0770c-140">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-140">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-141">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-141">Interactive</span></span>
* <span data-ttu-id="0770c-142">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-142">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-143">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-143">Monitor</span></span>
* <span data-ttu-id="0770c-144">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-144">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="0770c-145">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-145">Network</span></span>
* <span data-ttu-id="0770c-146">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-146">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="0770c-147">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-147">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="0770c-148">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-148">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="0770c-149">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-149">Profile</span></span>
* <span data-ttu-id="0770c-150">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-150">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-151">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-151">RDBMS</span></span>
* <span data-ttu-id="0770c-152">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-152">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-153">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-153">Resource</span></span>
* <span data-ttu-id="0770c-154">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-154">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="0770c-155">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-155">Role</span></span>
* <span data-ttu-id="0770c-156">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-156">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="0770c-157">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-157">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="0770c-158">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-158">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-159">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-159">Storage</span></span>
* <span data-ttu-id="0770c-160">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-160">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-161">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-161">VM</span></span>
* <span data-ttu-id="0770c-162">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-162">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="0770c-163">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-163">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="0770c-164">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-164">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="0770c-165">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-165">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="0770c-166">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="0770c-166">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="0770c-167">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-167">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="0770c-168">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="0770c-168">October 23, 2018</span></span>

<span data-ttu-id="0770c-169">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="0770c-169">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="0770c-170">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-170">Core</span></span>
* <span data-ttu-id="0770c-171">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-171">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="0770c-172">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-172">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-173">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-173">ACR</span></span>
* <span data-ttu-id="0770c-174">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-174">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="0770c-175">CDN</span><span class="sxs-lookup"><span data-stu-id="0770c-175">CDN</span></span>
* <span data-ttu-id="0770c-176">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-176">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="0770c-177">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-177">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="0770c-178">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-178">Container</span></span>
* <span data-ttu-id="0770c-179">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-179">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="0770c-180">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-180">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="0770c-181">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-181">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="0770c-182">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-182">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="0770c-183">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-183">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="0770c-184">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-184">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="0770c-185">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-185">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0770c-186">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0770c-186">CosmosDB</span></span>
* <span data-ttu-id="0770c-187">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-187">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-188">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-188">Interactive</span></span>
* <span data-ttu-id="0770c-189">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-189">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="0770c-190">IoT Central</span><span class="sxs-lookup"><span data-stu-id="0770c-190">IoT Central</span></span>
* <span data-ttu-id="0770c-191">IoT Central 응용 프로그램 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-191">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="0770c-192">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-192">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-193">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-193">Monitor</span></span>
* <span data-ttu-id="0770c-194">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0770c-194">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="0770c-195">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-195">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="0770c-196">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-196">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0770c-197">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-197">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="0770c-198">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-198">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="0770c-199">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-199">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="0770c-200">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0770c-200">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="0770c-201">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-201">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="0770c-202">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-202">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="0770c-203">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-203">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="0770c-204">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-204">Network</span></span>
* <span data-ttu-id="0770c-205">NIC에 응용 프로그램 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-205">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="0770c-206">NIC에 응용 프로그램 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-206">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="0770c-207">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0770c-207">ServiceBus</span></span>
* <span data-ttu-id="0770c-208">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-208">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-209">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-209">SQL</span></span>
* <span data-ttu-id="0770c-210">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-210">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-211">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-211">Storage</span></span>
* <span data-ttu-id="0770c-212">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-212">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="0770c-213">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-213">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-214">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-214">VM</span></span>
* <span data-ttu-id="0770c-215">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-215">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="0770c-216">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-216">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="0770c-217">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-217">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="0770c-218">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="0770c-218">October 16, 2018</span></span>

<span data-ttu-id="0770c-219">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="0770c-219">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-220">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-220">VM</span></span>
* <span data-ttu-id="0770c-221">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-221">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="0770c-222">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="0770c-222">October 9, 2018</span></span>

<span data-ttu-id="0770c-223">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="0770c-223">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="0770c-224">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-224">Core</span></span>
* <span data-ttu-id="0770c-225">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="0770c-225">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-226">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-226">ACR</span></span>
* <span data-ttu-id="0770c-227">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-227">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-228">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-228">ACS</span></span>
* <span data-ttu-id="0770c-229">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="0770c-229">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="0770c-230">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-230">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="0770c-231">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-231">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="0770c-232">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="0770c-232">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="0770c-233">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-233">Container</span></span>
* <span data-ttu-id="0770c-234">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-234">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="0770c-235">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-235">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="0770c-236">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="0770c-236">Event Hub</span></span>
* <span data-ttu-id="0770c-237">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-237">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="0770c-238">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-238">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="0770c-239">확장</span><span class="sxs-lookup"><span data-stu-id="0770c-239">Extensions</span></span>
* <span data-ttu-id="0770c-240">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-240">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="0770c-241">HDInsight</span><span class="sxs-lookup"><span data-stu-id="0770c-241">HDInsight</span></span>
* <span data-ttu-id="0770c-242">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-242">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-243">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-243">IoT</span></span>
* <span data-ttu-id="0770c-244">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-244">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0770c-245">KeyVault</span></span>
* <span data-ttu-id="0770c-246">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-246">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="0770c-247">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-247">Network</span></span>
* <span data-ttu-id="0770c-248">`network dns zone create` 수정: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-248">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="0770c-249">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="0770c-249">See #6052</span></span>
* <span data-ttu-id="0770c-250">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0770c-250">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="0770c-251">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-251">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="0770c-252">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-252">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="0770c-253">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-253">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="0770c-254">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-254">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="0770c-255">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-255">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="0770c-256">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-256">Role</span></span>
* <span data-ttu-id="0770c-257">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-257">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="0770c-258">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-258">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="0770c-259">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-259">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="0770c-260">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-260">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="0770c-261">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0770c-261">Service Bus</span></span>
* <span data-ttu-id="0770c-262">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-262">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-263">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-263">VM</span></span>
* <span data-ttu-id="0770c-264">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-264">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="0770c-265">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-265">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="0770c-266">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-266">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="0770c-267">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-267">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="0770c-268">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-268">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="0770c-269">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-269">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="0770c-270">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="0770c-270">September 21, 2018</span></span>

<span data-ttu-id="0770c-271">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="0770c-271">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-272">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-272">ACR</span></span>
* <span data-ttu-id="0770c-273">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-273">Added ACR Task commands</span></span>
* <span data-ttu-id="0770c-274">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-274">Added quick run command</span></span>
* <span data-ttu-id="0770c-275">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-275">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="0770c-276">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-276">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="0770c-277">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-277">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="0770c-278">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-278">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-279">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-279">ACS</span></span>
* <span data-ttu-id="0770c-280">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-280">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="0770c-281">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-281">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-282">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-282">AppService</span></span>

* <span data-ttu-id="0770c-283">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-283">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="0770c-284">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-284">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="0770c-285">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-285">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="0770c-286">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-286">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-287">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-287">Batch</span></span>
* <span data-ttu-id="0770c-288">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-288">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="0770c-289">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-289">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="0770c-290">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-290">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="0770c-291">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-291">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0770c-292">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0770c-292">Batch AI</span></span> 
* <span data-ttu-id="0770c-293">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-293">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0770c-294">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0770c-294">Cognitive Services</span></span>
* <span data-ttu-id="0770c-295">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-295">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="0770c-296">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-296">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="0770c-297">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-297">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="0770c-298">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-298">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="0770c-299">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-299">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="0770c-300">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-300">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="0770c-301">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-301">Container</span></span>
* <span data-ttu-id="0770c-302">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-302">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="0770c-303">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-303">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="0770c-304">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-304">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="0770c-305">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-305">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="0770c-306">Datalake</span><span class="sxs-lookup"><span data-stu-id="0770c-306">Datalake</span></span>
* <span data-ttu-id="0770c-307">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-307">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="0770c-308">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="0770c-308">Interactive Shell</span></span>
* <span data-ttu-id="0770c-309">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-309">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="0770c-310">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-310">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-311">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-311">IoT</span></span>
* <span data-ttu-id="0770c-312">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-312">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="0770c-313">Key Vault</span><span class="sxs-lookup"><span data-stu-id="0770c-313">Key Vault</span></span>
* <span data-ttu-id="0770c-314">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-314">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="0770c-315">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-315">Network</span></span>
* <span data-ttu-id="0770c-316">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-316">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="0770c-317">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-317">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="0770c-318">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-318">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="0770c-319">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-319">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="0770c-320">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-320">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="0770c-321">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-321">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="0770c-322">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-322">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="0770c-323">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-323">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="0770c-324">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-324">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="0770c-325">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-325">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="0770c-326">`network vnet subnet create/update`: `--delegation` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-326">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="0770c-327">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-327">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="0770c-328">`network traffic-manager profile create/update`: 모니터 구성을 위한 `--interval`, `--timeout` 및 `--max-failures` 지원 추가. `--path`, `--port`, `--protocol`로 인해 `--monitor-path`, `--monitor-port` 및 `--monitor-protocol` 옵션이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-328">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="0770c-329">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하기 위한 논리 수정. 사설 IP 주소가 제공된 경우 할당이 정적이 됨. 사설 IP 주소가 제공되지 않은 경우 사설 IP 주소에 대해 빈 문자열이 제공되고 할당이 동적이 됨.</span><span class="sxs-lookup"><span data-stu-id="0770c-329">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="0770c-330">`dns record-set * create/update`: `--target-resource` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-330">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="0770c-331">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-331">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="0770c-332">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-332">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="0770c-333">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-333">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-334">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-334">RDBMS</span></span>
* <span data-ttu-id="0770c-335">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-335">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="0770c-336">예약</span><span class="sxs-lookup"><span data-stu-id="0770c-336">Reservation</span></span>
* <span data-ttu-id="0770c-337">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-337">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="0770c-338">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-338">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="0770c-339">앱 관리</span><span class="sxs-lookup"><span data-stu-id="0770c-339">Manage App</span></span>
* <span data-ttu-id="0770c-340">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-340">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="0770c-341">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-341">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="0770c-342">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-342">Role</span></span>
* <span data-ttu-id="0770c-343">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-343">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="0770c-344">SignalR</span><span class="sxs-lookup"><span data-stu-id="0770c-344">SignalR</span></span>
* <span data-ttu-id="0770c-345">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-345">First release</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-346">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-346">Storage</span></span>
* <span data-ttu-id="0770c-347">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-347">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="0770c-348">변경할 수 없는 저장소 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-348">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-349">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-349">VM</span></span>
* <span data-ttu-id="0770c-350">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="0770c-350">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="0770c-351">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-351">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="0770c-352">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="0770c-352">August 28, 2018</span></span>

<span data-ttu-id="0770c-353">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="0770c-353">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="0770c-354">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-354">Core</span></span>

* <span data-ttu-id="0770c-355">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-355">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="0770c-356">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-356">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-357">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-357">ACR</span></span>

* <span data-ttu-id="0770c-358">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-358">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="0770c-359">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-359">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-360">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-360">ACS</span></span>

* <span data-ttu-id="0770c-361">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-361">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="0770c-362">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-362">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-363">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-363">AppService</span></span>

* <span data-ttu-id="0770c-364">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-364">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="0770c-365">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-365">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="0770c-366">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-366">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="0770c-367">Backup</span><span class="sxs-lookup"><span data-stu-id="0770c-367">Backup</span></span>

* <span data-ttu-id="0770c-368">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-368">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="0770c-369">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="0770c-369">Bot Service</span></span>

* <span data-ttu-id="0770c-370">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-370">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0770c-371">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0770c-371">Cognitive Services</span></span>

* <span data-ttu-id="0770c-372">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-372">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-373">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-373">IoT</span></span>

* <span data-ttu-id="0770c-374">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-374">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-375">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-375">Monitor</span></span>

* <span data-ttu-id="0770c-376">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-376">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="0770c-377">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="0770c-377">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0770c-378">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-378">Network</span></span>

* <span data-ttu-id="0770c-379">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-379">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-380">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-380">Resource</span></span>

* <span data-ttu-id="0770c-381">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-381">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-382">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-382">Storage</span></span>

* <span data-ttu-id="0770c-383">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-383">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-384">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-384">VM</span></span>

* <span data-ttu-id="0770c-385">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-385">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="0770c-386">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0770c-386">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="0770c-387">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="0770c-387">Auguest 14, 2018</span></span>

<span data-ttu-id="0770c-388">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="0770c-388">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="0770c-389">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-389">Core</span></span>

* <span data-ttu-id="0770c-390">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-390">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="0770c-391">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="0770c-391">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="0770c-392">원격 분석</span><span class="sxs-lookup"><span data-stu-id="0770c-392">Telemetry</span></span>

* <span data-ttu-id="0770c-393">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="0770c-393">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-394">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-394">ACR</span></span>

* <span data-ttu-id="0770c-395">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-395">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="0770c-396">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-396">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-397">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-397">ACS</span></span>

* <span data-ttu-id="0770c-398">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-398">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="0770c-399">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-399">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="0770c-400">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-400">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="0770c-401">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-401">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="0770c-402">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-402">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="0770c-403">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-403">AppService</span></span>

* <span data-ttu-id="0770c-404">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-404">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="0770c-405">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-405">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="0770c-406">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0770c-406">BatchAI</span></span>

* <span data-ttu-id="0770c-407">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-407">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="0770c-408">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-408">Container</span></span>

* <span data-ttu-id="0770c-409">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-409">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="0770c-410">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-410">IoT</span></span>

* <span data-ttu-id="0770c-411">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="0770c-411">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="0770c-412">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-412">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="0770c-413">Iot Central</span><span class="sxs-lookup"><span data-stu-id="0770c-413">Iot Central</span></span>

* <span data-ttu-id="0770c-414">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-414">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-415">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0770c-415">KeyVault</span></span>


* <span data-ttu-id="0770c-416">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-416">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="0770c-417">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-417">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="0770c-418">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-418">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="0770c-419">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-419">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="0770c-420">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-420">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="0770c-421">릴레이</span><span class="sxs-lookup"><span data-stu-id="0770c-421">Relay</span></span>

* <span data-ttu-id="0770c-422">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-422">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-423">Sql</span><span class="sxs-lookup"><span data-stu-id="0770c-423">Sql</span></span>

* <span data-ttu-id="0770c-424">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-424">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-425">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-425">Storage</span></span>

* <span data-ttu-id="0770c-426">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="0770c-426">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="0770c-427">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-427">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="0770c-428">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-428">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="0770c-429">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="0770c-429">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="0770c-430">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-430">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-431">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-431">VM</span></span>

* <span data-ttu-id="0770c-432">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-432">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="0770c-433">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="0770c-433">July 31, 2018</span></span>

<span data-ttu-id="0770c-434">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="0770c-434">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-435">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-435">ACR</span></span>

* <span data-ttu-id="0770c-436">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-436">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="0770c-437">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-437">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-438">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-438">ACS</span></span>

* <span data-ttu-id="0770c-439">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-439">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-440">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-440">Batch</span></span>

* <span data-ttu-id="0770c-441">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-441">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="0770c-442">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-442">Container</span></span>

* <span data-ttu-id="0770c-443">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-443">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="0770c-444">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-444">Network</span></span>

* <span data-ttu-id="0770c-445">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-445">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="0770c-446">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-446">Resource</span></span>

* <span data-ttu-id="0770c-447">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="0770c-447">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="0770c-448">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-448">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="0770c-449">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-449">Role</span></span>

* <span data-ttu-id="0770c-450">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-450">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="0770c-451">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-451">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="0770c-452">검색</span><span class="sxs-lookup"><span data-stu-id="0770c-452">Search</span></span>

* <span data-ttu-id="0770c-453">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-453">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="0770c-454">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0770c-454">Service Bus</span></span>

* <span data-ttu-id="0770c-455">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-455">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="0770c-456">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-456">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="0770c-457">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="0770c-457">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="0770c-458">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="0770c-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-459">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-459">Storage</span></span>

* <span data-ttu-id="0770c-460">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-460">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="0770c-461">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="0770c-461">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-462">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-462">VM</span></span>

* <span data-ttu-id="0770c-463">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-463">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="0770c-464">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-464">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="0770c-465">VM 확장 집합 생성 시 응용 프로그램 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-465">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="0770c-466">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-466">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="0770c-467">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="0770c-467">July 18, 2018</span></span>

<span data-ttu-id="0770c-468">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="0770c-468">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="0770c-469">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-469">Core</span></span>

* <span data-ttu-id="0770c-470">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-470">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="0770c-471">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-471">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="0770c-472">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-472">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-473">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-473">ACR</span></span>

* <span data-ttu-id="0770c-474">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-474">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="0770c-475">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-475">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="0770c-476">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-476">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="0770c-477">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-477">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-478">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-478">ACS</span></span>

* <span data-ttu-id="0770c-479">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-479">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-480">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-480">AppService</span></span>

* <span data-ttu-id="0770c-481">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-481">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-482">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-482">Batch</span></span>

* <span data-ttu-id="0770c-483">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-483">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="0770c-484">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-484">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0770c-485">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0770c-485">Batch AI</span></span>

* <span data-ttu-id="0770c-486">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-486">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="0770c-487">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-487">Container</span></span>

* <span data-ttu-id="0770c-488">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-488">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="0770c-489">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-489">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="0770c-490">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-490">Network</span></span>

* <span data-ttu-id="0770c-491">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-491">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="0770c-492">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-492">Added `network nic wait`</span></span>
* <span data-ttu-id="0770c-493">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-493">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="0770c-494">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-494">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="0770c-495">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-495">Resource</span></span>

* <span data-ttu-id="0770c-496">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-496">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="0770c-497">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-497">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="0770c-498">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-498">Added `deployment wait` command</span></span>
* <span data-ttu-id="0770c-499">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-499">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-500">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-500">SQL</span></span>

* <span data-ttu-id="0770c-501">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-501">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="0770c-502">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-502">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="0770c-503">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="0770c-503">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-504">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-504">Storage</span></span>

* <span data-ttu-id="0770c-505">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-505">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-506">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-506">VM</span></span>

* <span data-ttu-id="0770c-507">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-507">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="0770c-508">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-508">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="0770c-509">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-509">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0770c-510">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="0770c-510">July 3, 2018</span></span>

<span data-ttu-id="0770c-511">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="0770c-511">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="0770c-512">AKS</span><span class="sxs-lookup"><span data-stu-id="0770c-512">AKS</span></span>

* <span data-ttu-id="0770c-513">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-513">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="0770c-514">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="0770c-514">July 3, 2018</span></span>

<span data-ttu-id="0770c-515">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="0770c-515">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="0770c-516">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-516">Core</span></span>

* <span data-ttu-id="0770c-517">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-517">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-518">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-518">ACR</span></span>

* <span data-ttu-id="0770c-519">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-519">Added polling build status</span></span>
* <span data-ttu-id="0770c-520">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-520">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="0770c-521">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-521">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-522">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-522">ACS</span></span>

* <span data-ttu-id="0770c-523">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-523">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="0770c-524">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-524">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="0770c-525">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="0770c-525">Updated options for `aks browse` command.</span></span> <span data-ttu-id="0770c-526">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-526">Added `--listen-port` support</span></span>
* <span data-ttu-id="0770c-527">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="0770c-527">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="0770c-528">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="0770c-528">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="0770c-529">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-529">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-530">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-530">AppService</span></span>

* <span data-ttu-id="0770c-531">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-531">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="0770c-532">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-532">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="0770c-533">Backup</span><span class="sxs-lookup"><span data-stu-id="0770c-533">Backup</span></span>

* <span data-ttu-id="0770c-534">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-534">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="0770c-535">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0770c-535">BatchAI</span></span>

* <span data-ttu-id="0770c-536">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-536">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="0770c-537">클라우드</span><span class="sxs-lookup"><span data-stu-id="0770c-537">Cloud</span></span>

* <span data-ttu-id="0770c-538">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-538">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="0770c-539">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-539">Container</span></span>

* <span data-ttu-id="0770c-540">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-540">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="0770c-541">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-541">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="0770c-542">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-542">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-543">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-543">Extension</span></span>

* <span data-ttu-id="0770c-544">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-544">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="0770c-545">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-545">Network</span></span>

* <span data-ttu-id="0770c-546">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="0770c-546">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-547">Rdbms</span><span class="sxs-lookup"><span data-stu-id="0770c-547">Rdbms</span></span>

* <span data-ttu-id="0770c-548">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-548">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-549">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-549">Resource</span></span>

* <span data-ttu-id="0770c-550">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-550">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-551">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-551">VM</span></span>

* <span data-ttu-id="0770c-552">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-552">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="0770c-553">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="0770c-553">June 25, 2018</span></span>

<span data-ttu-id="0770c-554">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="0770c-554">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="0770c-555">CLI</span><span class="sxs-lookup"><span data-stu-id="0770c-555">CLI</span></span>

* <span data-ttu-id="0770c-556">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-556">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="0770c-557">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="0770c-557">June 19, 2018</span></span>

<span data-ttu-id="0770c-558">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="0770c-558">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="0770c-559">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-559">Core</span></span>

* <span data-ttu-id="0770c-560">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-560">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-561">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-561">ACR</span></span>

* <span data-ttu-id="0770c-562">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-562">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="0770c-563">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-563">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-564">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-564">ACS</span></span>

* <span data-ttu-id="0770c-565">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="0770c-565">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="0770c-566">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-566">Added `--update` support</span></span>
* <span data-ttu-id="0770c-567">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-567">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="0770c-568">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="0770c-568">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="0770c-569">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-569">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="0770c-570">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-570">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="0770c-571">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-571">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="0770c-572">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-572">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-573">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-573">AppService</span></span>

* <span data-ttu-id="0770c-574">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-574">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="0770c-575">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-575">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-576">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-576">Batch</span></span>

* <span data-ttu-id="0770c-577">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-577">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0770c-578">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0770c-578">Batch AI</span></span>

* <span data-ttu-id="0770c-579">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0770c-579">Added support for workspaces.</span></span> <span data-ttu-id="0770c-580">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-580">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="0770c-581">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0770c-581">Added support for experiments.</span></span> <span data-ttu-id="0770c-582">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-582">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="0770c-583">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-583">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="0770c-584">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="0770c-584">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="0770c-585">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-585">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="0770c-586">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-586">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="0770c-587">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="0770c-587">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="0770c-588">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="0770c-588">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="0770c-589">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="0770c-589">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="0770c-590">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="0770c-590">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="0770c-591">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="0770c-591">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="0770c-592">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="0770c-592">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="0770c-593">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="0770c-593">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="0770c-594">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-594">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="0770c-595">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="0770c-595">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="0770c-596">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="0770c-596">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="0770c-597">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0770c-597">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="0770c-598">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0770c-598">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0770c-599">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0770c-599">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="0770c-600">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="0770c-600">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="0770c-601">지도</span><span class="sxs-lookup"><span data-stu-id="0770c-601">Maps</span></span>

* <span data-ttu-id="0770c-602">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-602">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="0770c-603">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-603">Network</span></span>

* <span data-ttu-id="0770c-604">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-604">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="0770c-605">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-605">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="0770c-606">#6502</span><span class="sxs-lookup"><span data-stu-id="0770c-606">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="0770c-607">예약</span><span class="sxs-lookup"><span data-stu-id="0770c-607">Reservations</span></span>

* <span data-ttu-id="0770c-608">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-608">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="0770c-609">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-609">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="0770c-610">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="0770c-610">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="0770c-611">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-611">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="0770c-612">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-612">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="0770c-613">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-613">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="0770c-614">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-614">Role</span></span>

* <span data-ttu-id="0770c-615">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="0770c-615">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-616">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-616">SQL</span></span>

* <span data-ttu-id="0770c-617">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-617">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-618">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-618">Storage</span></span>

* <span data-ttu-id="0770c-619">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="0770c-619">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-620">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-620">VM</span></span>

* <span data-ttu-id="0770c-621">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="0770c-621">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="0770c-622">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-622">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="0770c-623">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-623">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0770c-624">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="0770c-624">June 13, 2018</span></span>

<span data-ttu-id="0770c-625">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="0770c-625">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="0770c-626">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-626">Core</span></span>

* <span data-ttu-id="0770c-627">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="0770c-627">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="0770c-628">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="0770c-628">June 13, 2018</span></span>

<span data-ttu-id="0770c-629">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="0770c-629">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="0770c-630">AKS</span><span class="sxs-lookup"><span data-stu-id="0770c-630">AKS</span></span>

* <span data-ttu-id="0770c-631">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-631">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="0770c-632">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="0770c-632">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="0770c-633">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-633">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="0770c-634">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-634">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="0770c-635">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-635">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-636">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-636">AppService</span></span>

* <span data-ttu-id="0770c-637">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-637">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0770c-638">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="0770c-638">June 5, 2018</span></span>

<span data-ttu-id="0770c-639">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="0770c-639">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-640">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-640">Interactive</span></span>

* <span data-ttu-id="0770c-641">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="0770c-641">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="0770c-642">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="0770c-642">June 5, 2018</span></span>

<span data-ttu-id="0770c-643">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="0770c-643">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="0770c-644">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-644">Core</span></span>

* <span data-ttu-id="0770c-645">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-645">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="0770c-646">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-646">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-647">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-647">ACR</span></span>

* <span data-ttu-id="0770c-648">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-648">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="0770c-649">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-649">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="0770c-650">AKS</span><span class="sxs-lookup"><span data-stu-id="0770c-650">AKS</span></span>

* <span data-ttu-id="0770c-651">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-651">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-652">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-652">Batch</span></span>

* <span data-ttu-id="0770c-653">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="0770c-653">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-654">IOT</span><span class="sxs-lookup"><span data-stu-id="0770c-654">IOT</span></span>

* <span data-ttu-id="0770c-655">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-655">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="0770c-656">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-656">Network</span></span>

* <span data-ttu-id="0770c-657">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="0770c-657">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="0770c-658">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0770c-658">Policy Insights</span></span>

* <span data-ttu-id="0770c-659">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-659">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="0770c-660">ARM</span><span class="sxs-lookup"><span data-stu-id="0770c-660">ARM</span></span>

* <span data-ttu-id="0770c-661">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-661">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-662">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-662">SQL</span></span>

* <span data-ttu-id="0770c-663">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="0770c-663">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="0770c-664">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-664">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="0770c-665">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-665">Storage</span></span>

* <span data-ttu-id="0770c-666">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="0770c-666">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-667">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-667">VM</span></span>

* <span data-ttu-id="0770c-668">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-668">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="0770c-669">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-669">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="0770c-670">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-670">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="0770c-671">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="0770c-671">May 22, 2018</span></span>

<span data-ttu-id="0770c-672">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="0770c-672">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="0770c-673">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-673">Core</span></span>

* <span data-ttu-id="0770c-674">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-674">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-675">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-675">ACS</span></span>

* <span data-ttu-id="0770c-676">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-676">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="0770c-677">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-677">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-678">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-678">AppService</span></span>

* <span data-ttu-id="0770c-679">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-679">Improved generic update commands</span></span>
* <span data-ttu-id="0770c-680">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-680">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="0770c-681">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-681">Container</span></span>

* <span data-ttu-id="0770c-682">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-682">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="0770c-683">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-683">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-684">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-684">Extension</span></span>

* <span data-ttu-id="0770c-685">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-685">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-686">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-686">Interactive</span></span>

* <span data-ttu-id="0770c-687">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-687">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="0770c-688">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="0770c-688">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-689">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0770c-689">KeyVault</span></span>

* <span data-ttu-id="0770c-690">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="0770c-690">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="0770c-691">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-691">Network</span></span>

* <span data-ttu-id="0770c-692">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="0770c-692">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="0770c-693">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-693">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-694">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-694">SQL</span></span>

* <span data-ttu-id="0770c-695">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="0770c-695">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="0770c-696">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="0770c-696">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="0770c-697">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-697">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="0770c-698">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-698">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="0770c-699">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-699">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="0770c-700">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="0770c-700">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="0770c-701">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-701">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="0770c-702">`edition`</span><span class="sxs-lookup"><span data-stu-id="0770c-702">`edition`.</span></span> <span data-ttu-id="0770c-703">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-703">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="0770c-704">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="0770c-704">`elasticPoolName`.</span></span> <span data-ttu-id="0770c-705">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-705">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="0770c-706">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-706">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="0770c-707">`edition`</span><span class="sxs-lookup"><span data-stu-id="0770c-707">`edition`.</span></span> <span data-ttu-id="0770c-708">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="0770c-708">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="0770c-709">`dtu`</span><span class="sxs-lookup"><span data-stu-id="0770c-709">`dtu`.</span></span> <span data-ttu-id="0770c-710">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="0770c-710">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="0770c-711">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="0770c-711">`databaseDtuMin`.</span></span> <span data-ttu-id="0770c-712">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="0770c-712">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="0770c-713">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="0770c-713">`databaseDtuMax`.</span></span> <span data-ttu-id="0770c-714">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="0770c-714">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="0770c-715">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-715">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="0770c-716">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-716">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-717">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-717">Storage</span></span>

* <span data-ttu-id="0770c-718">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-718">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="0770c-719">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-719">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-720">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-720">VM</span></span>

* <span data-ttu-id="0770c-721">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="0770c-721">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="0770c-722">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="0770c-722">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="0770c-723">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="0770c-723">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="0770c-724">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="0770c-724">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="0770c-725">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-725">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="0770c-726">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="0770c-726">May 7, 2018</span></span>

<span data-ttu-id="0770c-727">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="0770c-727">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="0770c-728">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-728">Core</span></span>

* <span data-ttu-id="0770c-729">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-729">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="0770c-730">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-730">Added limited support for positional arguments</span></span>
* <span data-ttu-id="0770c-731">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-731">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="0770c-732">#5591</span><span class="sxs-lookup"><span data-stu-id="0770c-732">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="0770c-733">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-733">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="0770c-734">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-734">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="0770c-735">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-735">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="0770c-736">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-736">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="0770c-737">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-737">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-738">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-738">ACR</span></span>

* <span data-ttu-id="0770c-739">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-739">Added ACR Build commands</span></span>
* <span data-ttu-id="0770c-740">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-740">Improved resource not found error messages</span></span>
* <span data-ttu-id="0770c-741">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-741">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="0770c-742">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-742">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="0770c-743">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-743">Improved repository commands error messages</span></span>
* <span data-ttu-id="0770c-744">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-744">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-745">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-745">ACS</span></span>

* <span data-ttu-id="0770c-746">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-746">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="0770c-747">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-747">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="0770c-748">AMS</span><span class="sxs-lookup"><span data-stu-id="0770c-748">AMS</span></span>

* <span data-ttu-id="0770c-749">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="0770c-749">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-750">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-750">Appservice</span></span>

* <span data-ttu-id="0770c-751">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-751">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="0770c-752">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-752">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="0770c-753">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-753">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="0770c-754">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-754">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="0770c-755">Batch AI</span><span class="sxs-lookup"><span data-stu-id="0770c-755">Batch AI</span></span>

* <span data-ttu-id="0770c-756">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-756">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0770c-757">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0770c-757">Cognitive Services</span></span>

* <span data-ttu-id="0770c-758">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-758">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="0770c-759">Consumption</span><span class="sxs-lookup"><span data-stu-id="0770c-759">Consumption</span></span>

* <span data-ttu-id="0770c-760">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-760">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="0770c-761">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-761">Container</span></span>

* <span data-ttu-id="0770c-762">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-762">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="0770c-763">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0770c-763">Cosmos DB</span></span>

* <span data-ttu-id="0770c-764">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0770c-764">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="0770c-765">DMS</span><span class="sxs-lookup"><span data-stu-id="0770c-765">DMS</span></span>

* <span data-ttu-id="0770c-766">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-766">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-767">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-767">Extension</span></span>

* <span data-ttu-id="0770c-768">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-768">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-769">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-769">Interactive</span></span>

* <span data-ttu-id="0770c-770">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-770">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="0770c-771">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="0770c-771">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="0770c-772">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-772">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="0770c-773">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-773">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="0770c-774">랩</span><span class="sxs-lookup"><span data-stu-id="0770c-774">Lab</span></span>

* <span data-ttu-id="0770c-775">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-775">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="0770c-776">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-776">Network</span></span>

* <span data-ttu-id="0770c-777">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-777">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="0770c-778">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-778">Profile</span></span>

* <span data-ttu-id="0770c-779">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-779">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="0770c-780">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-780">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="0770c-781">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-781">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="0770c-782">Redis</span><span class="sxs-lookup"><span data-stu-id="0770c-782">Redis</span></span>

* <span data-ttu-id="0770c-783">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-783">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="0770c-784">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-784">Deprecated `redis list-all`.</span></span> <span data-ttu-id="0770c-785">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="0770c-785">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="0770c-786">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-786">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="0770c-787">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-787">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="0770c-788">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-788">Role</span></span>

* <span data-ttu-id="0770c-789">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-789">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-790">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-790">Storage</span></span>

* <span data-ttu-id="0770c-791">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-791">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="0770c-792">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="0770c-792">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="0770c-793">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="0770c-793">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="0770c-794">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-794">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="0770c-795">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-795">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-796">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-796">VM</span></span>

* <span data-ttu-id="0770c-797">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-797">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="0770c-798">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-798">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="0770c-799">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="0770c-799">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="0770c-800">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-800">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="0770c-801">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-801">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="0770c-802">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-802">Added write accelerator support</span></span>
* <span data-ttu-id="0770c-803">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-803">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="0770c-804">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-804">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="0770c-805">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-805">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="0770c-806">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="0770c-806">April 10, 2018</span></span>

<span data-ttu-id="0770c-807">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="0770c-807">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-808">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-808">ACR</span></span>

* <span data-ttu-id="0770c-809">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="0770c-809">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-810">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-810">ACS</span></span>

* <span data-ttu-id="0770c-811">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-811">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-812">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-812">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="0770c-814">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-814">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="0770c-815">BatchAI</span><span class="sxs-lookup"><span data-stu-id="0770c-815">BatchAI</span></span>

* <span data-ttu-id="0770c-816">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-816">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="0770c-817">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="0770c-817">Job level mounting</span></span>
  - <span data-ttu-id="0770c-818">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="0770c-818">Environment variables with secret values</span></span>
  - <span data-ttu-id="0770c-819">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-819">Performance counters settings</span></span>
  - <span data-ttu-id="0770c-820">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="0770c-820">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="0770c-821">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-821">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="0770c-822">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="0770c-822">Usage and limits reporting</span></span>
  - <span data-ttu-id="0770c-823">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-823">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="0770c-824">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-824">Support for custom images</span></span>
  - <span data-ttu-id="0770c-825">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-825">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="0770c-826">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-826">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="0770c-827">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-827">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="0770c-828">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-828">National clouds are supported</span></span>
* <span data-ttu-id="0770c-829">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-829">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="0770c-830">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="0770c-830">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="0770c-831">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-831">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="0770c-832">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-832">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="0770c-833">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="0770c-833">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="0770c-834">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="0770c-834">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="0770c-835">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-835">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="0770c-836">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-836">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="0770c-837">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-837">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="0770c-838">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-838">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="0770c-839">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-839">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="0770c-840">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="0770c-840">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="0770c-841">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-841">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="0770c-842">결제</span><span class="sxs-lookup"><span data-stu-id="0770c-842">Billing</span></span>

* <span data-ttu-id="0770c-843">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-843">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="0770c-844">Consumption</span><span class="sxs-lookup"><span data-stu-id="0770c-844">Consumption</span></span>

* <span data-ttu-id="0770c-845">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-845">Added `marketplace` commands</span></span>
* <span data-ttu-id="0770c-846">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-846">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="0770c-847">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-847">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="0770c-848">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-848">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="0770c-849">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-849">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="0770c-850">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-850">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="0770c-851">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-851">Container</span></span>

* <span data-ttu-id="0770c-852">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="0770c-852">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="0770c-853">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="0770c-853">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-854">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-854">Extension</span></span>

* <span data-ttu-id="0770c-855">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-855">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-856">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-856">Interactive</span></span>

* <span data-ttu-id="0770c-857">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-857">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="0770c-858">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-858">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="0770c-859">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-859">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="0770c-860">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-860">Network</span></span>

* <span data-ttu-id="0770c-861">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-861">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="0770c-862">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-862">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="0770c-863">#4910</span><span class="sxs-lookup"><span data-stu-id="0770c-863">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="0770c-864">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-864">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="0770c-865">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="0770c-865">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="0770c-866">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-866">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="0770c-867">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-867">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="0770c-868">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-868">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-869">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-869">Profile</span></span>

* <span data-ttu-id="0770c-870">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-870">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="0770c-871">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-871">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-872">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-872">RDBMS</span></span>

* <span data-ttu-id="0770c-873">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-873">Added `georestore` command</span></span>
* <span data-ttu-id="0770c-874">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-874">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-875">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-875">Resource</span></span>

* <span data-ttu-id="0770c-876">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-876">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="0770c-877">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-877">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-878">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-878">SQL</span></span>

* <span data-ttu-id="0770c-879">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-879">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-880">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-880">Storage</span></span>

* <span data-ttu-id="0770c-881">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-881">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-882">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-882">VM</span></span>

* <span data-ttu-id="0770c-883">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-883">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="0770c-884">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-884">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="0770c-886">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-886">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="0770c-887">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-887">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="0770c-888">#5718</span><span class="sxs-lookup"><span data-stu-id="0770c-888">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="0770c-889">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-889">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="0770c-890">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="0770c-890">March 27, 2018</span></span>

<span data-ttu-id="0770c-891">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="0770c-891">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="0770c-892">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-892">Core</span></span>

* <span data-ttu-id="0770c-893">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="0770c-893">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-894">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-894">ACS</span></span>

* <span data-ttu-id="0770c-895">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-895">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-896">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-896">Appservice</span></span>

* <span data-ttu-id="0770c-897">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-897">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="0770c-898">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-898">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0770c-899">Backup</span><span class="sxs-lookup"><span data-stu-id="0770c-899">Backup</span></span>

* <span data-ttu-id="0770c-900">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-900">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="0770c-901">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-901">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="0770c-902">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-902">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="0770c-903">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-903">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="0770c-904">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-904">Container</span></span>

* <span data-ttu-id="0770c-905">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-905">Added `container exec` command.</span></span> <span data-ttu-id="0770c-906">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-906">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="0770c-907">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-907">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-908">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-908">Extension</span></span>

* <span data-ttu-id="0770c-909">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-909">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="0770c-910">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-910">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="0770c-911">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-911">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-912">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-912">Interactive</span></span>

* <span data-ttu-id="0770c-913">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="0770c-913">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="0770c-914">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-914">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="0770c-915">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="0770c-915">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="0770c-916">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-916">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="0770c-917">랩</span><span class="sxs-lookup"><span data-stu-id="0770c-917">Lab</span></span>

* <span data-ttu-id="0770c-918">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-918">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-919">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-919">Monitor</span></span>

* <span data-ttu-id="0770c-920">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-920">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="0770c-921">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="0770c-921">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="0770c-922">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-922">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="0770c-923">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-923">Network</span></span>

* <span data-ttu-id="0770c-924">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-924">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-925">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-925">Profile</span></span>

* <span data-ttu-id="0770c-926">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-926">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-927">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-927">RDBMS</span></span>

* <span data-ttu-id="0770c-928">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-928">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-929">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-929">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="0770c-931">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-931">Role</span></span>

* <span data-ttu-id="0770c-932">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-932">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="0770c-933">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-933">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="0770c-934">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-934">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="0770c-935">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-935">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="0770c-936">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-936">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-937">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-937">Storage</span></span>

* <span data-ttu-id="0770c-938">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-938">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="0770c-939">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="0770c-939">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-940">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-940">VM</span></span>

* <span data-ttu-id="0770c-941">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-941">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="0770c-942">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-942">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="0770c-943">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-943">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="0770c-944">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-944">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="0770c-945">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="0770c-945">March 13, 2018</span></span>

<span data-ttu-id="0770c-946">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="0770c-946">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-947">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-947">ACR</span></span>

* <span data-ttu-id="0770c-948">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-948">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="0770c-949">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-949">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="0770c-950">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-950">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-951">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-951">ACS</span></span>

* <span data-ttu-id="0770c-952">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-952">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="0770c-953">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-953">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="0770c-954">Advisor</span><span class="sxs-lookup"><span data-stu-id="0770c-954">Advisor</span></span>

* <span data-ttu-id="0770c-955">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-955">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="0770c-956">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-956">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="0770c-957">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-957">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="0770c-958">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-958">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="0770c-959">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-959">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-960">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-960">Appservice</span></span>

* <span data-ttu-id="0770c-961">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-961">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="0770c-962">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-962">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="0770c-963">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="0770c-963">Eventhubs</span></span>

* <span data-ttu-id="0770c-964">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-964">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-965">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-965">Extension</span></span>

* <span data-ttu-id="0770c-966">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-966">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-967">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-967">Interactive</span></span>

* <span data-ttu-id="0770c-968">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="0770c-968">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="0770c-969">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="0770c-969">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="0770c-970">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-970">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="0770c-971">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-971">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-972">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-972">Monitor</span></span>

* <span data-ttu-id="0770c-973">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-973">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="0770c-974">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-974">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="0770c-975">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-975">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="0770c-976">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-976">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="0770c-977">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-977">Network</span></span>

* <span data-ttu-id="0770c-978">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-978">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="0770c-979">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="0770c-979">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="0770c-980">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-980">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="0770c-981">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-981">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-982">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-982">Profile</span></span>

* <span data-ttu-id="0770c-983">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-983">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="0770c-984">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-984">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-985">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-985">RDBMS</span></span>

* <span data-ttu-id="0770c-986">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-986">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="0770c-987">Service Bus</span><span class="sxs-lookup"><span data-stu-id="0770c-987">Service Bus</span></span>

* <span data-ttu-id="0770c-988">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-988">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-989">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-989">Storage</span></span>

* <span data-ttu-id="0770c-990">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-990">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="0770c-991">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-991">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-992">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-992">VM</span></span>

* <span data-ttu-id="0770c-993">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-993">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="0770c-994">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-994">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="0770c-995">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-995">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="0770c-996">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-996">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="0770c-997">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="0770c-997">February 27, 2018</span></span>

<span data-ttu-id="0770c-998">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="0770c-998">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="0770c-999">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-999">Core</span></span>

* <span data-ttu-id="0770c-1000">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1000">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="0770c-1001">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1001">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="0770c-1002">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1002">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1003">ACS</span></span>

* <span data-ttu-id="0770c-1004">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1004">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="0770c-1005">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1005">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="0770c-1006">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1006">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="0770c-1007">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-1007">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1008">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1008">Appservice</span></span>

* <span data-ttu-id="0770c-1009">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="0770c-1009">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="0770c-1010">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1010">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="0770c-1011">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="0770c-1011">Cognitive Services</span></span>

* <span data-ttu-id="0770c-1012">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-1012">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="0770c-1013">Consumption</span><span class="sxs-lookup"><span data-stu-id="0770c-1013">Consumption</span></span>

* <span data-ttu-id="0770c-1014">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1014">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="0770c-1015">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-1015">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1016">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1016">Container</span></span>

* <span data-ttu-id="0770c-1017">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1017">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1018">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1018">Network</span></span>

* <span data-ttu-id="0770c-1019">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1019">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1020">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1020">Resource</span></span>

* <span data-ttu-id="0770c-1021">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1021">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1022">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1022">Role</span></span>

* <span data-ttu-id="0770c-1023">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1023">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1024">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1024">SQL</span></span>

* <span data-ttu-id="0770c-1025">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1025">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1026">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1026">Storage</span></span>

* <span data-ttu-id="0770c-1027">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="0770c-1027">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1028">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1028">VM</span></span>

* <span data-ttu-id="0770c-1029">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1029">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="0770c-1030">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="0770c-1030">February 13, 2018</span></span>

<span data-ttu-id="0770c-1031">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="0770c-1031">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1032">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1032">Core</span></span>

* <span data-ttu-id="0770c-1033">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1033">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1034">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1034">ACS</span></span>

* <span data-ttu-id="0770c-1035">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1035">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="0770c-1036">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1036">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="0770c-1037">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1037">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="0770c-1038">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="0770c-1038">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="0770c-1039">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1039">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="0770c-1040">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="0770c-1040">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="0770c-1041">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1041">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="0770c-1042">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1042">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1043">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1043">Appservice</span></span>

* <span data-ttu-id="0770c-1044">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1044">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="0770c-1045">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1045">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="0770c-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="0770c-1046">CDN</span></span>

* <span data-ttu-id="0770c-1047">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1047">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1048">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1048">Container</span></span>

* <span data-ttu-id="0770c-1049">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1049">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="0770c-1050">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1050">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0770c-1051">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0770c-1051">CosmosDB</span></span>

* <span data-ttu-id="0770c-1052">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1052">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-1053">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-1053">Extension</span></span>

* <span data-ttu-id="0770c-1054">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1054">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="0770c-1055">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1055">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="0770c-1056">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="0770c-1056">Feedback</span></span>

* <span data-ttu-id="0770c-1057">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1057">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-1058">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-1058">Interactive</span></span>

* <span data-ttu-id="0770c-1059">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1059">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="0770c-1060">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1060">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-1061">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-1061">IoT</span></span>

* <span data-ttu-id="0770c-1062">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1062">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0770c-1063">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1063">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="0770c-1064">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1064">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="0770c-1065">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1065">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1066">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1066">Monitor</span></span>

* <span data-ttu-id="0770c-1067">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1067">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1068">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1068">Network</span></span>

* <span data-ttu-id="0770c-1069">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1069">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="0770c-1070">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1070">Profile</span></span>

* <span data-ttu-id="0770c-1071">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1071">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1072">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1072">Resource</span></span>

* <span data-ttu-id="0770c-1073">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1073">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1074">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1074">Role</span></span>

* <span data-ttu-id="0770c-1075">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1075">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1076">SQL</span></span>

* <span data-ttu-id="0770c-1077">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1077">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="0770c-1078">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1078">Added `sql db rename`</span></span>
* <span data-ttu-id="0770c-1079">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1079">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1080">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1080">Storage</span></span>

* <span data-ttu-id="0770c-1081">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1081">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1082">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1082">VM</span></span>

* <span data-ttu-id="0770c-1083">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1083">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="0770c-1084">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1084">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="0770c-1085">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="0770c-1085">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="0770c-1086">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="0770c-1086">January 31, 2018</span></span>

<span data-ttu-id="0770c-1087">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="0770c-1087">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1088">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1088">Core</span></span>

* <span data-ttu-id="0770c-1089">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1089">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="0770c-1090">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-1090">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="0770c-1091">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1091">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="0770c-1092">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="0770c-1092">Use `--verbose` to see</span></span>
* <span data-ttu-id="0770c-1093">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1093">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1094">ACS</span></span>

* <span data-ttu-id="0770c-1095">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1095">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="0770c-1096">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="0770c-1096">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1097">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1097">Appservice</span></span>

* <span data-ttu-id="0770c-1098">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="0770c-1098">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="0770c-1099">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-1099">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="0770c-1100">CDN</span><span class="sxs-lookup"><span data-stu-id="0770c-1100">CDN</span></span>

* <span data-ttu-id="0770c-1101">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1101">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0770c-1102">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0770c-1102">CosmosDB</span></span>

* <span data-ttu-id="0770c-1103">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1103">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-1104">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-1104">Interactive</span></span>

* <span data-ttu-id="0770c-1105">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1105">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1106">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1106">Network</span></span>

* <span data-ttu-id="0770c-1107">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1107">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="0770c-1108">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1108">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="0770c-1109">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1109">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="0770c-1110">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1110">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="0770c-1111">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1111">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="0770c-1112">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="0770c-1112">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="0770c-1113">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1113">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="0770c-1114">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1114">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="0770c-1115">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1115">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="0770c-1116">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="0770c-1116">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1117">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1117">Profile</span></span>

* <span data-ttu-id="0770c-1118">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1118">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1119">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1119">Resource</span></span>

* <span data-ttu-id="0770c-1120">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1120">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1121">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1121">Storage</span></span>

* <span data-ttu-id="0770c-1122">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1122">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="0770c-1123">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1123">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="0770c-1124">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1124">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="0770c-1125">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1125">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="0770c-1126">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1126">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1127">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1127">VM</span></span>

* <span data-ttu-id="0770c-1128">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1128">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="0770c-1129">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1129">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="0770c-1130">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1130">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="0770c-1131">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1131">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="0770c-1132">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="0770c-1132">January 17, 2018</span></span>

<span data-ttu-id="0770c-1133">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="0770c-1133">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-1134">ACR</span></span>

* <span data-ttu-id="0770c-1135">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1135">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="0770c-1136">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1136">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1137">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1137">ACS</span></span>

* <span data-ttu-id="0770c-1138">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1138">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="0770c-1139">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1139">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1140">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1140">Appservice</span></span>

* <span data-ttu-id="0770c-1141">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1141">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="0770c-1142">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1142">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="0770c-1143">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1143">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="0770c-1144">Backup</span><span class="sxs-lookup"><span data-stu-id="0770c-1144">Backup</span></span>

* <span data-ttu-id="0770c-1145">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1145">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="0770c-1146">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1146">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="0770c-1147">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1147">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="0770c-1148">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1148">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="0770c-1149">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1149">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-1150">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-1150">Batch</span></span>

* <span data-ttu-id="0770c-1151">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1151">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="0770c-1152">클라우드</span><span class="sxs-lookup"><span data-stu-id="0770c-1152">Cloud</span></span>

* <span data-ttu-id="0770c-1153">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1153">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="0770c-1154">Consumption</span><span class="sxs-lookup"><span data-stu-id="0770c-1154">Consumption</span></span>

* <span data-ttu-id="0770c-1155">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1155">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="0770c-1156">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0770c-1156">Event Grid</span></span>

* <span data-ttu-id="0770c-1157">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1157">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0770c-1158">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1158">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="0770c-1159">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1159">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="0770c-1160">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="0770c-1160">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="0770c-1161">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1161">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="0770c-1162">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1162">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="0770c-1163">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1163">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="0770c-1164">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1164">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-1165">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-1165">Interactive</span></span>

* <span data-ttu-id="0770c-1166">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1166">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="0770c-1167">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1167">Fixed errors on startup</span></span>
* <span data-ttu-id="0770c-1168">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1168">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-1169">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-1169">IoT</span></span>

* <span data-ttu-id="0770c-1170">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1170">Added support for device provisioning service</span></span>
* <span data-ttu-id="0770c-1171">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1171">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="0770c-1172">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1172">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1173">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1173">Monitor</span></span>

* <span data-ttu-id="0770c-1174">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1174">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="0770c-1175">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="0770c-1175">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="0770c-1176">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1176">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1177">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1177">Network</span></span>

* <span data-ttu-id="0770c-1178">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1178">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="0770c-1179">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1179">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1180">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1180">Profile</span></span>

* <span data-ttu-id="0770c-1181">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1181">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1182">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1182">Role</span></span>

* <span data-ttu-id="0770c-1183">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1183">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0770c-1184">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0770c-1184">Service Fabric</span></span>

* <span data-ttu-id="0770c-1185">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1185">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="0770c-1186">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1186">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1187">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1187">VM</span></span>

* <span data-ttu-id="0770c-1188">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1188">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="0770c-1189">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1189">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="0770c-1190">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1190">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="0770c-1191">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1191">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="0770c-1192">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1192">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="0770c-1193">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1193">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="0770c-1194">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1194">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="0770c-1195">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1195">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="0770c-1196">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="0770c-1196">December 19, 2017</span></span>

<span data-ttu-id="0770c-1197">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="0770c-1197">Version 2.0.23</span></span>

* <span data-ttu-id="0770c-1198">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1198">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1199">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1199">Container</span></span>

* <span data-ttu-id="0770c-1200">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1200">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1201">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1201">Network</span></span>

* <span data-ttu-id="0770c-1202">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1202">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="0770c-1203">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1203">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1204">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1204">Storage</span></span>

* <span data-ttu-id="0770c-1205">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1205">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1206">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1206">VM</span></span>

* <span data-ttu-id="0770c-1207">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1207">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="0770c-1208">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="0770c-1208">December 5, 2017</span></span>

<span data-ttu-id="0770c-1209">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="0770c-1209">Version 2.0.22</span></span>

* <span data-ttu-id="0770c-1210">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1210">Removed `az component` commands.</span></span> <span data-ttu-id="0770c-1211">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="0770c-1211">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1212">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1212">Core</span></span>
* <span data-ttu-id="0770c-1213">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1213">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="0770c-1214">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1214">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1215">ACS</span></span>

* <span data-ttu-id="0770c-1216">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1216">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="0770c-1217">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1217">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="0770c-1218">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1218">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="0770c-1219">Advisor</span><span class="sxs-lookup"><span data-stu-id="0770c-1219">Advisor</span></span>

* <span data-ttu-id="0770c-1220">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1220">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1221">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1221">Appservice</span></span>

* <span data-ttu-id="0770c-1222">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1222">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="0770c-1223">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1223">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="0770c-1224">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1224">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="0770c-1225">Consumption</span><span class="sxs-lookup"><span data-stu-id="0770c-1225">Consumption</span></span>

* <span data-ttu-id="0770c-1226">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1226">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1227">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1227">Container</span></span>

* <span data-ttu-id="0770c-1228">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1228">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1229">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1229">Monitor</span></span>

* <span data-ttu-id="0770c-1230">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1230">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1231">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1231">Resource</span></span>

* <span data-ttu-id="0770c-1232">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1232">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1233">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1233">Role</span></span>

* <span data-ttu-id="0770c-1234">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1234">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="0770c-1235">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1235">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="0770c-1236">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1236">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1237">SQL</span></span>

* <span data-ttu-id="0770c-1238">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1238">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="0770c-1239">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1239">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1240">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1240">VM</span></span>

* <span data-ttu-id="0770c-1241">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1241">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="0770c-1242">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="0770c-1242">November 14, 2017</span></span>

<span data-ttu-id="0770c-1243">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="0770c-1243">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-1244">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-1244">ACR</span></span>

* <span data-ttu-id="0770c-1245">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1245">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="0770c-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1246">ACS</span></span>

* <span data-ttu-id="0770c-1247">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1247">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="0770c-1248">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="0770c-1248">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="0770c-1249">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1249">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="0770c-1250">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1250">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="0770c-1251">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1251">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1252">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1252">Appservice</span></span>

* <span data-ttu-id="0770c-1253">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1253">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="0770c-1254">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1254">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="0770c-1255">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1255">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="0770c-1256">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1256">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="0770c-1257">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1257">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="0770c-1258">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="0770c-1258">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-1259">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-1259">Batch</span></span>

* <span data-ttu-id="0770c-1260">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1260">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="0770c-1261">Batchai</span><span class="sxs-lookup"><span data-stu-id="0770c-1261">Batchai</span></span>

* <span data-ttu-id="0770c-1262">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1262">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="0770c-1263">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1263">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="0770c-1264">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1264">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="0770c-1265">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1265">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="0770c-1266">클라우드</span><span class="sxs-lookup"><span data-stu-id="0770c-1266">Cloud</span></span>

* <span data-ttu-id="0770c-1267">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1267">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1268">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1268">Container</span></span>

* <span data-ttu-id="0770c-1269">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1269">Added support to open multiple ports</span></span>
* <span data-ttu-id="0770c-1270">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1270">Added container group restart policy</span></span>
* <span data-ttu-id="0770c-1271">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1271">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="0770c-1272">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="0770c-1272">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0770c-1273">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0770c-1273">Data Lake Analytics</span></span>

* <span data-ttu-id="0770c-1274">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1274">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0770c-1275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0770c-1275">Data Lake Store</span></span>

* <span data-ttu-id="0770c-1276">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1276">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-1277">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-1277">Extension</span></span>

* <span data-ttu-id="0770c-1278">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1278">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="0770c-1279">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1279">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-1280">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-1280">IoT</span></span>

* <span data-ttu-id="0770c-1281">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1281">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1282">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1282">Monitor</span></span>

* <span data-ttu-id="0770c-1283">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1283">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1284">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1284">Network</span></span>

* <span data-ttu-id="0770c-1285">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1285">Added support for CAA DNS records</span></span>
* <span data-ttu-id="0770c-1286">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1286">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="0770c-1287">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1287">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="0770c-1288">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1288">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="0770c-1289">예약</span><span class="sxs-lookup"><span data-stu-id="0770c-1289">Reservations</span></span>

* <span data-ttu-id="0770c-1290">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1290">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1291">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1291">Resource</span></span>

* <span data-ttu-id="0770c-1292">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1292">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1293">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1293">SQL</span></span>

* <span data-ttu-id="0770c-1294">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1294">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1295">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1295">Storage</span></span>

* <span data-ttu-id="0770c-1296">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1296">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="0770c-1297">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1297">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="0770c-1298">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1298">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="0770c-1299">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="0770c-1299">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="0770c-1300">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1300">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="0770c-1301">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1301">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="0770c-1302">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1302">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1303">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1303">VM</span></span>

* <span data-ttu-id="0770c-1304">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1304">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="0770c-1305">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1305">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="0770c-1306">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1306">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="0770c-1307">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1307">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="0770c-1308">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1308">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="0770c-1309">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="0770c-1309">October 24, 2017</span></span>

<span data-ttu-id="0770c-1310">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="0770c-1310">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1311">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1311">Core</span></span>

* <span data-ttu-id="0770c-1312">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="0770c-1312">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-1313">ACR</span></span>

* <span data-ttu-id="0770c-1314">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="0770c-1314">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="0770c-1315">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-1315">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="0770c-1316">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="0770c-1316">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1317">ACS</span></span>

* <span data-ttu-id="0770c-1318">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1318">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="0770c-1319">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1319">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1320">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1320">Appservice</span></span>

* <span data-ttu-id="0770c-1321">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1321">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="0770c-1322">구성 요소</span><span class="sxs-lookup"><span data-stu-id="0770c-1322">Component</span></span>

* <span data-ttu-id="0770c-1323">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1323">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1324">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1324">Monitor</span></span>

* <span data-ttu-id="0770c-1325">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1325">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1326">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1326">Resource</span></span>

* <span data-ttu-id="0770c-1327">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1327">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="0770c-1328">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1328">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1329">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1329">VM</span></span>

* <span data-ttu-id="0770c-1330">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1330">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="0770c-1331">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="0770c-1331">October 9, 2017</span></span>

<span data-ttu-id="0770c-1332">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="0770c-1332">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1333">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1333">Core</span></span>

* <span data-ttu-id="0770c-1334">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1334">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1335">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1335">Appservice</span></span>

* <span data-ttu-id="0770c-1336">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1336">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-1337">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-1337">Batch</span></span>

* <span data-ttu-id="0770c-1338">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1338">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="0770c-1339">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1339">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="0770c-1340">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1340">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="0770c-1341">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1341">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="0770c-1342">Batchai</span><span class="sxs-lookup"><span data-stu-id="0770c-1342">Batchai</span></span>

* <span data-ttu-id="0770c-1343">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1343">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-1344">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0770c-1344">Keyvault</span></span>

* <span data-ttu-id="0770c-1345">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1345">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="0770c-1346">(#4448)</span><span class="sxs-lookup"><span data-stu-id="0770c-1346">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="0770c-1347">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1347">Network</span></span>

* <span data-ttu-id="0770c-1348">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1348">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="0770c-1349">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1349">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1350">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1350">Resource</span></span>

* <span data-ttu-id="0770c-1351">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1351">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="0770c-1352">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1352">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="0770c-1353">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1353">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="0770c-1354">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1354">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1355">Sql</span><span class="sxs-lookup"><span data-stu-id="0770c-1355">Sql</span></span>

* <span data-ttu-id="0770c-1356">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1356">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="0770c-1357">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1357">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="0770c-1358">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1358">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1359">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1359">Storage</span></span>

* <span data-ttu-id="0770c-1360">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1360">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1361">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1361">Vm</span></span>

* <span data-ttu-id="0770c-1362">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1362">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="0770c-1363">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1363">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="0770c-1364">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1364">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="0770c-1365">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1365">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="0770c-1366">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1366">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="0770c-1367">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="0770c-1367">September 22, 2017</span></span>

<span data-ttu-id="0770c-1368">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="0770c-1368">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1369">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1369">Resource</span></span>

* <span data-ttu-id="0770c-1370">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1370">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="0770c-1371">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1371">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="0770c-1372">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1372">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="0770c-1373">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1373">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1374">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1374">Network</span></span>

* <span data-ttu-id="0770c-1375">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1375">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="0770c-1376">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1376">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="0770c-1377">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1377">Added `asg` application security group commands</span></span>
* <span data-ttu-id="0770c-1378">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1378">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="0770c-1379">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1379">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0770c-1380">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1380">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="0770c-1381">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1381">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1382">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1382">Storage</span></span>

* <span data-ttu-id="0770c-1383">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1383">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="0770c-1384">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0770c-1384">Eventgrid</span></span>

* <span data-ttu-id="0770c-1385">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="0770c-1385">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1386">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1386">SQL</span></span>

* <span data-ttu-id="0770c-1387">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1387">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="0770c-1388">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1388">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="0770c-1389">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1389">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-1390">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0770c-1390">Keyvault</span></span>

* <span data-ttu-id="0770c-1391">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1391">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1392">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1392">VM</span></span>

* <span data-ttu-id="0770c-1393">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1393">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="0770c-1394">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="0770c-1394">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="0770c-1395">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1395">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="0770c-1396">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1396">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="0770c-1397">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1397">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="0770c-1398">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1398">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1399">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1399">ACS</span></span>

* <span data-ttu-id="0770c-1400">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1400">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1401">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1401">Appservice</span></span>

* <span data-ttu-id="0770c-1402">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1402">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="0770c-1403">Backup</span><span class="sxs-lookup"><span data-stu-id="0770c-1403">Backup</span></span>

* <span data-ttu-id="0770c-1404">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1404">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="0770c-1405">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="0770c-1405">September 11, 2017</span></span>

<span data-ttu-id="0770c-1406">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="0770c-1406">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="0770c-1407">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1407">Core</span></span>

* <span data-ttu-id="0770c-1408">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1408">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="0770c-1409">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1409">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1410">Acs</span></span>

* <span data-ttu-id="0770c-1411">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1411">Added `acs list-locations` command</span></span>
* <span data-ttu-id="0770c-1412">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="0770c-1412">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1413">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1413">Appservice</span></span>

* <span data-ttu-id="0770c-1414">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1414">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="0770c-1415">CDN</span><span class="sxs-lookup"><span data-stu-id="0770c-1415">CDN</span></span>

* <span data-ttu-id="0770c-1416">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1416">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="0770c-1417">내선 번호</span><span class="sxs-lookup"><span data-stu-id="0770c-1417">Extension</span></span>

* <span data-ttu-id="0770c-1418">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1418">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-1419">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0770c-1419">Keyvault</span></span>

* <span data-ttu-id="0770c-1420">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1420">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1421">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1421">Network</span></span>

* <span data-ttu-id="0770c-1422">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1422">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0770c-1423">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1423">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="0770c-1424">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1424">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="0770c-1425">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1425">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0770c-1426">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1426">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1427">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1427">Resource</span></span>

* <span data-ttu-id="0770c-1428">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-1428">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="0770c-1429">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-1429">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="0770c-1430">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-1430">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="0770c-1431">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="0770c-1431">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1432">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1432">SQL</span></span>

* <span data-ttu-id="0770c-1433">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1433">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1434">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1434">VM</span></span>

* <span data-ttu-id="0770c-1435">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1435">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="0770c-1436">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="0770c-1436">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="0770c-1437">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1437">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="0770c-1438">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1438">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="0770c-1439">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1439">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="0770c-1440">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="0770c-1440">August 31, 2017</span></span>

<span data-ttu-id="0770c-1441">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="0770c-1441">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-1442">Keyvault</span><span class="sxs-lookup"><span data-stu-id="0770c-1442">Keyvault</span></span>

* <span data-ttu-id="0770c-1443">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1443">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="0770c-1444">Sf</span><span class="sxs-lookup"><span data-stu-id="0770c-1444">Sf</span></span>

* <span data-ttu-id="0770c-1445">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1445">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1446">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1446">Storage</span></span>

* <span data-ttu-id="0770c-1447">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1447">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="0770c-1448">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="0770c-1448">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="0770c-1449">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="0770c-1449">August 28, 2017</span></span>

<span data-ttu-id="0770c-1450">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="0770c-1450">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="0770c-1451">CLI</span><span class="sxs-lookup"><span data-stu-id="0770c-1451">CLI</span></span>

* <span data-ttu-id="0770c-1452">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1452">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1453">ACS</span></span>

* <span data-ttu-id="0770c-1454">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1454">Corrected preview regions</span></span>
* <span data-ttu-id="0770c-1455">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1455">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="0770c-1456">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1456">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1457">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1457">Appservice</span></span>

* <span data-ttu-id="0770c-1458">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1458">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="0770c-1459">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1459">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="0770c-1460">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1460">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="0770c-1461">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1461">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="0770c-1462">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1462">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-1463">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-1463">IoT</span></span>

* <span data-ttu-id="0770c-1464">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1464">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1465">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1465">Network</span></span>

* <span data-ttu-id="0770c-1466">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1466">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="0770c-1467">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1467">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="0770c-1468">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1468">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="0770c-1469">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="0770c-1470">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1470">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1471">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1471">Profile</span></span>

* <span data-ttu-id="0770c-1472">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1472">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0770c-1473">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0770c-1473">Service Fabric</span></span>

* <span data-ttu-id="0770c-1474">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1474">Preview release</span></span>
* <span data-ttu-id="0770c-1475">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1475">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="0770c-1476">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1476">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="0770c-1477">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1477">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1478">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1478">Storage</span></span>

* <span data-ttu-id="0770c-1479">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1479">Enabled setting blob tier</span></span>
* <span data-ttu-id="0770c-1480">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1480">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="0770c-1481">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1481">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="0770c-1482">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1482">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="0770c-1483">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1483">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="0770c-1484">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1484">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1485">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1485">VM</span></span>

* <span data-ttu-id="0770c-1486">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1486">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="0770c-1487">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1487">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="0770c-1488">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1488">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="0770c-1489">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1489">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="0770c-1490">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1490">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="0770c-1491">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1491">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="0770c-1492">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="0770c-1492">August 15, 2017</span></span>

<span data-ttu-id="0770c-1493">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="0770c-1493">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1494">ACS</span></span>

* <span data-ttu-id="0770c-1495">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1495">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1496">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1496">Appservice</span></span>

* <span data-ttu-id="0770c-1497">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1497">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="0770c-1498">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0770c-1498">Event Grid</span></span>

* <span data-ttu-id="0770c-1499">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1499">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="0770c-1500">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="0770c-1500">August 11, 2017</span></span>

<span data-ttu-id="0770c-1501">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="0770c-1501">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1502">ACS</span></span>

* <span data-ttu-id="0770c-1503">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1503">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-1504">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-1504">Batch</span></span>

* <span data-ttu-id="0770c-1505">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1505">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="0770c-1506">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1506">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="0770c-1507">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1507">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="0770c-1508">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1508">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="0770c-1509">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1509">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="0770c-1510">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1510">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="0770c-1511">구성 요소</span><span class="sxs-lookup"><span data-stu-id="0770c-1511">Component</span></span>

* <span data-ttu-id="0770c-1512">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1512">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="0770c-1513">컨테이너</span><span class="sxs-lookup"><span data-stu-id="0770c-1513">Container</span></span>

* <span data-ttu-id="0770c-1514">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1514">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="0770c-1515">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0770c-1515">Data Lake Store</span></span>

* <span data-ttu-id="0770c-1516">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1516">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="0770c-1517">Event Grid</span><span class="sxs-lookup"><span data-stu-id="0770c-1517">Event Grid</span></span>

* <span data-ttu-id="0770c-1518">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1518">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1519">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1519">Network</span></span>

* <span data-ttu-id="0770c-1520">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1520">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="0770c-1521">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1521">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="0770c-1522">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1522">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="0770c-1523">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1523">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1524">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1524">Profile</span></span>

* <span data-ttu-id="0770c-1525">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1525">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1526">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1526">Storage</span></span>

* <span data-ttu-id="0770c-1527">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1527">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1528">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1528">VM</span></span>

* <span data-ttu-id="0770c-1529">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1529">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="0770c-1530">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1530">Exposed `list-skus` command</span></span>
* <span data-ttu-id="0770c-1531">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1531">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="0770c-1532">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1532">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="0770c-1533">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1533">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="0770c-1534">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="0770c-1534">July 28, 2017</span></span>

<span data-ttu-id="0770c-1535">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="0770c-1535">Version 2.0.12</span></span>

* <span data-ttu-id="0770c-1536">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1536">Added container commands</span></span>
* <span data-ttu-id="0770c-1537">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1537">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="0770c-1538">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1538">Core</span></span>

* <span data-ttu-id="0770c-1539">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1539">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="0770c-1540">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1540">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="0770c-1541">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="0770c-1541">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="0770c-1542">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="0770c-1542">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="0770c-1543">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="0770c-1543">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="0770c-1544">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="0770c-1544">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="0770c-1545">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="0770c-1545">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0770c-1546">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="0770c-1546">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="0770c-1547">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="0770c-1547">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="0770c-1548">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="0770c-1548">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="0770c-1549">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="0770c-1549">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="0770c-1550">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="0770c-1550">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="0770c-1551">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1551">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="0770c-1552">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1552">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="0770c-1553">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1553">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="0770c-1554">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="0770c-1554">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="0770c-1555">ACR</span><span class="sxs-lookup"><span data-stu-id="0770c-1555">ACR</span></span>

* <span data-ttu-id="0770c-1556">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1556">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="0770c-1557">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1557">Support SKU update for managed registries</span></span>
* <span data-ttu-id="0770c-1558">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1558">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="0770c-1559">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1559">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="0770c-1560">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1560">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="0770c-1561">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1561">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1562">ACS</span></span>

* <span data-ttu-id="0770c-1563">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1563">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1564">App Service</span><span class="sxs-lookup"><span data-stu-id="0770c-1564">Appservice</span></span>

* <span data-ttu-id="0770c-1565">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1565">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="0770c-1566">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1566">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="0770c-1567">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1567">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="0770c-1568">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="0770c-1568">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="0770c-1569">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="0770c-1569">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="0770c-1570">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="0770c-1570">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="0770c-1571">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="0770c-1571">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="0770c-1572">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="0770c-1572">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="0770c-1573">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1573">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="0770c-1574">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1574">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="0770c-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="0770c-1575">Batch</span></span>

* <span data-ttu-id="0770c-1576">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1576">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="0770c-1577">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1577">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="0770c-1578">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1578">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="0770c-1579">CDN</span><span class="sxs-lookup"><span data-stu-id="0770c-1579">CDN</span></span>

* <span data-ttu-id="0770c-1580">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1580">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="0770c-1581">클라우드</span><span class="sxs-lookup"><span data-stu-id="0770c-1581">Cloud</span></span>

* <span data-ttu-id="0770c-1582">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1582">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="0770c-1583">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1583">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="0770c-1584">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1584">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="0770c-1585">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1585">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="0770c-1586">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1586">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0770c-1587">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0770c-1587">CosmosDB</span></span>

* <span data-ttu-id="0770c-1588">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1588">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="0770c-1589">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1589">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0770c-1590">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0770c-1590">Data Lake Analytics</span></span>

* <span data-ttu-id="0770c-1591">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1591">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="0770c-1592">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1592">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="0770c-1593">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1593">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0770c-1594">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0770c-1594">Data Lake Store</span></span>

* <span data-ttu-id="0770c-1595">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1595">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="0770c-1596">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1596">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="0770c-1597">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1597">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="0770c-1598">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="0770c-1598">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="0770c-1599">대화형</span><span class="sxs-lookup"><span data-stu-id="0770c-1599">Interactive</span></span>

* <span data-ttu-id="0770c-1600">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1600">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="0770c-1601">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1601">Increased test coverage</span></span>
* <span data-ttu-id="0770c-1602">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1602">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="0770c-1603">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="0770c-1603">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="0770c-1604">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="0770c-1604">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="0770c-1605">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="0770c-1605">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="0770c-1606">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="0770c-1606">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="0770c-1607">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1607">Added `--progress` flag</span></span>
* <span data-ttu-id="0770c-1608">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1608">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="0770c-1609">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="0770c-1609">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="0770c-1610">IoT</span><span class="sxs-lookup"><span data-stu-id="0770c-1610">IoT</span></span>

* <span data-ttu-id="0770c-1611">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1611">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="0770c-1612">(#3934)</span><span class="sxs-lookup"><span data-stu-id="0770c-1612">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="0770c-1613">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="0770c-1613">Key vault</span></span>

* <span data-ttu-id="0770c-1614">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="0770c-1614">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="0770c-1615">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0770c-1615">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="0770c-1616">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0770c-1616">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0770c-1617">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0770c-1617">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="0770c-1618">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="0770c-1618">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="0770c-1619">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="0770c-1619">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="0770c-1620">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1620">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="0770c-1621">(#3307)</span><span class="sxs-lookup"><span data-stu-id="0770c-1621">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="0770c-1622">랩</span><span class="sxs-lookup"><span data-stu-id="0770c-1622">Lab</span></span>

* <span data-ttu-id="0770c-1623">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1623">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="0770c-1624">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1624">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1625">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1625">Monitor</span></span>

* <span data-ttu-id="0770c-1626">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="0770c-1626">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="0770c-1627">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1627">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="0770c-1628">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1628">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="0770c-1629">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1629">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="0770c-1630">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1630">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="0770c-1631">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="0770c-1631">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="0770c-1632">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1632">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="0770c-1633">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1633">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="0770c-1634">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1634">`location` no longer required</span></span>
  * <span data-ttu-id="0770c-1635">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1635">Add name and ID support for target</span></span>
  * <span data-ttu-id="0770c-1636">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1636">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="0770c-1637">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1637">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="0770c-1638">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1638">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="0770c-1639">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1639">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="0770c-1640">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1640">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="0770c-1641">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1641">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1642">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1642">Network</span></span>

* <span data-ttu-id="0770c-1643">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1643">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="0770c-1644">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1644">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="0770c-1645">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1645">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="0770c-1646">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1646">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="0770c-1647">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1647">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="0770c-1648">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1648">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="0770c-1649">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="0770c-1649">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="0770c-1650">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="0770c-1650">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="0770c-1651">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="0770c-1651">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="0770c-1652">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0770c-1652">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="0770c-1653">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0770c-1653">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="0770c-1654">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="0770c-1654">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="0770c-1655">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="0770c-1655">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="0770c-1656">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="0770c-1656">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="0770c-1657">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1657">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="0770c-1658">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1658">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="0770c-1659">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1659">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="0770c-1660">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1660">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="0770c-1661">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1661">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="0770c-1662">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1662">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="0770c-1663">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1663">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="0770c-1664">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1664">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="0770c-1665">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1665">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="0770c-1666">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1666">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="0770c-1667">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1667">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="0770c-1668">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1668">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="0770c-1669">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1669">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1670">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1670">Profile</span></span>

* <span data-ttu-id="0770c-1671">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1671">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="0770c-1672">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1672">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="0770c-1673">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1673">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="0770c-1674">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1674">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="0770c-1675">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1675">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="0770c-1676">RDBMS</span><span class="sxs-lookup"><span data-stu-id="0770c-1676">RDBMS</span></span>

* <span data-ttu-id="0770c-1677">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="0770c-1677">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="0770c-1678">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="0770c-1678">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="0770c-1679">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="0770c-1679">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="0770c-1680">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="0770c-1680">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1681">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1681">Resource</span></span>

* <span data-ttu-id="0770c-1682">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1682">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="0770c-1683">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1683">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="0770c-1684">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1684">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="0770c-1685">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1685">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="0770c-1686">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="0770c-1686">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="0770c-1687">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1687">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="0770c-1688">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="0770c-1688">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="0770c-1689">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1689">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1690">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1690">Role</span></span>

* <span data-ttu-id="0770c-1691">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1691">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="0770c-1692">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="0770c-1692">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="0770c-1693">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1693">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="0770c-1694">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1694">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="0770c-1695">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1695">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="0770c-1696">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0770c-1696">Service Fabric</span></span>
* <span data-ttu-id="0770c-1697">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="0770c-1697">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="0770c-1698">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="0770c-1698">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="0770c-1699">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="0770c-1699">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1700">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1700">SQL</span></span>

* <span data-ttu-id="0770c-1701">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1701">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="0770c-1702">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1702">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="0770c-1703">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1703">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1704">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1704">Storage</span></span>

* <span data-ttu-id="0770c-1705">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="0770c-1705">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="0770c-1706">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="0770c-1706">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="0770c-1707">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="0770c-1707">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="0770c-1708">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1708">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="0770c-1709">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="0770c-1709">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="0770c-1710">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="0770c-1710">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1711">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1711">VM</span></span>

* <span data-ttu-id="0770c-1712">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1712">Support configuring nsg</span></span>
* <span data-ttu-id="0770c-1713">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1713">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="0770c-1714">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1714">Support managed service identities</span></span>
* <span data-ttu-id="0770c-1715">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1715">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="0770c-1716">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1716">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="0770c-1717">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="0770c-1717">May 10, 2017</span></span>

<span data-ttu-id="0770c-1718">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="0770c-1718">Version 2.0.6</span></span>

* <span data-ttu-id="0770c-1719">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="0770c-1719">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="0770c-1720">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1720">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="0770c-1721">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0770c-1721">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="0770c-1722">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0770c-1722">Include Cognitive Services module</span></span>
* <span data-ttu-id="0770c-1723">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="0770c-1723">Include Service Fabric module</span></span>
* <span data-ttu-id="0770c-1724">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="0770c-1724">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="0770c-1725">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1725">Add support for CDN commands</span></span>
* <span data-ttu-id="0770c-1726">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-1726">Remove Container module</span></span>
* <span data-ttu-id="0770c-1727">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="0770c-1727">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="0770c-1728">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0770c-1728">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="0770c-1729">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1729">Core</span></span>

* <span data-ttu-id="0770c-1730">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="0770c-1730">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="0770c-1731">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="0770c-1731">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="0770c-1732">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="0770c-1732">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="0770c-1733">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="0770c-1733">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="0770c-1734">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="0770c-1734">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="0770c-1735">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="0770c-1735">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="0770c-1736">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="0770c-1736">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="0770c-1737">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="0770c-1737">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="0770c-1738">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="0770c-1738">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="0770c-1739">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="0770c-1739">core: Improved performance</span></span>
* <span data-ttu-id="0770c-1740">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1740">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="0770c-1741">core: 클라우드 구성 - '관리' 엔드포인트를 설정하지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="0770c-1741">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1742">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1742">ACS</span></span>

* <span data-ttu-id="0770c-1743">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1743">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="0770c-1744">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="0770c-1744">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="0770c-1745">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="0770c-1745">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="0770c-1746">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="0770c-1746">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1747">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-1747">AppService</span></span>

* <span data-ttu-id="0770c-1748">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="0770c-1748">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="0770c-1749">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1749">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="0770c-1750">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="0770c-1750">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="0770c-1751">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="0770c-1751">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="0770c-1752">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="0770c-1752">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="0770c-1753">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="0770c-1753">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="0770c-1754">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1754">support slot swap with preview</span></span>
* <span data-ttu-id="0770c-1755">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="0770c-1755">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="0770c-1756">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="0770c-1756">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="0770c-1757">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="0770c-1757">CosmosDB</span></span>

* <span data-ttu-id="0770c-1758">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="0770c-1758">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="0770c-1759">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1759">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="0770c-1760">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1760">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="0770c-1761">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1761">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="0770c-1762">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="0770c-1762">Data Lake Analytics</span></span>

* <span data-ttu-id="0770c-1763">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1763">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="0770c-1764">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1764">Add support for new catalog item type: package.</span></span> <span data-ttu-id="0770c-1765">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="0770c-1765">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="0770c-1766">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="0770c-1766">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="0770c-1767">테이블</span><span class="sxs-lookup"><span data-stu-id="0770c-1767">Table</span></span>
  * <span data-ttu-id="0770c-1768">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="0770c-1768">Table valued function</span></span>
  * <span data-ttu-id="0770c-1769">보기</span><span class="sxs-lookup"><span data-stu-id="0770c-1769">View</span></span>
  * <span data-ttu-id="0770c-1770">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="0770c-1770">Table Statistics.</span></span> <span data-ttu-id="0770c-1771">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="0770c-1771">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="0770c-1772">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="0770c-1772">Data Lake Store</span></span>

* <span data-ttu-id="0770c-1773">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="0770c-1773">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="0770c-1774">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="0770c-1774">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="0770c-1775">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="0770c-1775">missed help for access show.</span></span> <span data-ttu-id="0770c-1776">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1776">adding it.</span></span> <span data-ttu-id="0770c-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="0770c-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="0770c-1778">찾기</span><span class="sxs-lookup"><span data-stu-id="0770c-1778">Find</span></span>

* <span data-ttu-id="0770c-1779">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="0770c-1779">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="0770c-1780">KeyVault</span><span class="sxs-lookup"><span data-stu-id="0770c-1780">KeyVault</span></span>

* <span data-ttu-id="0770c-1781">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1781">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="0770c-1782">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1782">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="0770c-1783">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1783">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="0770c-1784">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1784">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="0770c-1785">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="0770c-1785">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="0770c-1786">랩</span><span class="sxs-lookup"><span data-stu-id="0770c-1786">Lab</span></span>

* <span data-ttu-id="0770c-1787">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1787">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="0770c-1788">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1788">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="0770c-1789">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="0770c-1789">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="0770c-1790">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="0770c-1790">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="0770c-1791">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1791">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="0770c-1792">모니터</span><span class="sxs-lookup"><span data-stu-id="0770c-1792">Monitor</span></span>

* <span data-ttu-id="0770c-1793">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="0770c-1793">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="0770c-1794">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="0770c-1794">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="0770c-1795">네트워크</span><span class="sxs-lookup"><span data-stu-id="0770c-1795">Network</span></span>

* <span data-ttu-id="0770c-1796">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1796">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="0770c-1797">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1797">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="0770c-1798">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1798">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="0770c-1799">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1799">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="0770c-1800">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1800">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="0770c-1801">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1801">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="0770c-1802">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1802">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="0770c-1803">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1803">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="0770c-1804">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1804">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="0770c-1805">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1805">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="0770c-1806">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="0770c-1806">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="0770c-1807">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1807">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="0770c-1808">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1808">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="0770c-1809">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1809">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="0770c-1810">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="0770c-1810">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="0770c-1811">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1811">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="0770c-1812">프로필</span><span class="sxs-lookup"><span data-stu-id="0770c-1812">Profile</span></span>

* <span data-ttu-id="0770c-1813">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="0770c-1813">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="0770c-1814">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="0770c-1814">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="0770c-1815">Redis</span><span class="sxs-lookup"><span data-stu-id="0770c-1815">Redis</span></span>

* <span data-ttu-id="0770c-1816">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1816">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="0770c-1817">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="0770c-1817">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="0770c-1818">리소스</span><span class="sxs-lookup"><span data-stu-id="0770c-1818">Resource</span></span>

* <span data-ttu-id="0770c-1819">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="0770c-1819">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="0770c-1820">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="0770c-1820">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="0770c-1821">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="0770c-1821">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="0770c-1822">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1822">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="0770c-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="0770c-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="0770c-1824">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1824">Add docs for az lock update.</span></span> <span data-ttu-id="0770c-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="0770c-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="0770c-1826">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1826">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="0770c-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="0770c-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="0770c-1828">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1828">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="0770c-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="0770c-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="0770c-1830">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="0770c-1830">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="0770c-1831">역할</span><span class="sxs-lookup"><span data-stu-id="0770c-1831">Role</span></span>

* <span data-ttu-id="0770c-1832">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="0770c-1832">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="0770c-1833">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="0770c-1833">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="0770c-1834">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="0770c-1834">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="0770c-1835">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="0770c-1835">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="0770c-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="0770c-1836">SQL</span></span>

* <span data-ttu-id="0770c-1837">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="0770c-1837">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="0770c-1838">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="0770c-1838">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="0770c-1839">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1839">Storage</span></span>

* <span data-ttu-id="0770c-1840">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="0770c-1840">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="0770c-1841">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1841">Add support for incremental blob copy</span></span>
* <span data-ttu-id="0770c-1842">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1842">Add support for large block blob upload</span></span>
* <span data-ttu-id="0770c-1843">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="0770c-1843">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1844">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1844">VM</span></span>

* <span data-ttu-id="0770c-1845">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="0770c-1845">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="0770c-1846">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="0770c-1846">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="0770c-1847">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="0770c-1847">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="0770c-1848">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="0770c-1848">az vm/vmss disk</span></span>
  3. <span data-ttu-id="0770c-1849">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1849">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="0770c-1850">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="0770c-1850">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="0770c-1851">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="0770c-1851">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="0770c-1852">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="0770c-1852">April 3, 2017</span></span>

<span data-ttu-id="0770c-1853">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="0770c-1853">Version 2.0.2</span></span>

<span data-ttu-id="0770c-1854">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1854">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="0770c-1855">코어</span><span class="sxs-lookup"><span data-stu-id="0770c-1855">Core</span></span>

* <span data-ttu-id="0770c-1856">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="0770c-1856">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="0770c-1857">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="0770c-1857">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="0770c-1858">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="0770c-1858">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="0770c-1859">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0770c-1859">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0770c-1860">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="0770c-1860">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="0770c-1861">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="0770c-1861">Add prompting for missing template parameters.</span></span> <span data-ttu-id="0770c-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="0770c-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="0770c-1863">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1863">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="0770c-1864">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="0770c-1864">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="0770c-1865">ACS</span><span class="sxs-lookup"><span data-stu-id="0770c-1865">ACS</span></span>

* <span data-ttu-id="0770c-1866">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="0770c-1866">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="0770c-1867">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0770c-1867">Add support for ssh key password prompting.</span></span> <span data-ttu-id="0770c-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="0770c-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="0770c-1869">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="0770c-1869">Add support for windows clusters.</span></span> <span data-ttu-id="0770c-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="0770c-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="0770c-1871">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="0770c-1871">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="0770c-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="0770c-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="0770c-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="0770c-1873">AppService</span></span>

* <span data-ttu-id="0770c-1874">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="0770c-1874">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="0770c-1875">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="0770c-1875">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="0770c-1876">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="0770c-1876">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="0770c-1877">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="0770c-1877">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="0770c-1878">DataLake</span><span class="sxs-lookup"><span data-stu-id="0770c-1878">DataLake</span></span>

* <span data-ttu-id="0770c-1879">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1879">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="0770c-1880">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="0770c-1880">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="0770c-1881">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="0770c-1881">DocuemntDB</span></span>

* <span data-ttu-id="0770c-1882">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="0770c-1882">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="0770c-1883">VM</span><span class="sxs-lookup"><span data-stu-id="0770c-1883">VM</span></span>

* <span data-ttu-id="0770c-1884">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="0770c-1884">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="0770c-1885">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="0770c-1885">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="0770c-1886">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="0770c-1886">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="0770c-1887">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="0770c-1887">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="0770c-1888">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="0770c-1888">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="0770c-1889">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="0770c-1889">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="0770c-1890">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="0770c-1890">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="0770c-1891">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="0770c-1891">February 27, 2017</span></span>

<span data-ttu-id="0770c-1892">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="0770c-1892">Version 2.0.0</span></span>

<span data-ttu-id="0770c-1893">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1893">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="0770c-1894">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="0770c-1894">Container Service (acs)</span></span>
- <span data-ttu-id="0770c-1895">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="0770c-1895">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="0770c-1896">네트워킹</span><span class="sxs-lookup"><span data-stu-id="0770c-1896">Networking</span></span>
- <span data-ttu-id="0770c-1897">Storage</span><span class="sxs-lookup"><span data-stu-id="0770c-1897">Storage</span></span>

<span data-ttu-id="0770c-1898">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1898">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="0770c-1899">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1899">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="0770c-1900">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1900">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="0770c-1901">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1901">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="0770c-1902">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0770c-1902">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="0770c-1903">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0770c-1903">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="0770c-1904">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="0770c-1904">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="0770c-1905">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="0770c-1905">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="0770c-1906">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="0770c-1906">Provide feedback from the command line with the `az feedback` command</span></span>


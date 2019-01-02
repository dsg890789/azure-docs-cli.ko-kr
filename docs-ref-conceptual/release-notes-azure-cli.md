---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/20/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7a2ab41dd6696d658d05ab76e44abf97626761aa
ms.sourcegitcommit: 14aa16beeec59e51890a6cba4906bdc8e19b94d0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/05/2018
ms.locfileid: "52892686"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="290af-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="290af-103">Azure CLI release notes</span></span>
## <a name="december-4-2018"></a><span data-ttu-id="290af-104">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="290af-104">December 4, 2018</span></span>

<span data-ttu-id="290af-105">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="290af-105">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="290af-106">코어</span><span class="sxs-lookup"><span data-stu-id="290af-106">Core</span></span>
* <span data-ttu-id="290af-107">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-107">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="290af-108">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-108">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-109">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-109">Appservice</span></span>
* <span data-ttu-id="290af-110">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-110">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="290af-111">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-111">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="290af-112">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-112">Network</span></span>
* <span data-ttu-id="290af-113">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-113">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="290af-114">역할</span><span class="sxs-lookup"><span data-stu-id="290af-114">Role</span></span>
* <span data-ttu-id="290af-115">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-115">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="290af-116">VM</span><span class="sxs-lookup"><span data-stu-id="290af-116">VM</span></span>
* <span data-ttu-id="290af-117">[사용되지 않음]`vm extension [show|wait] --expand` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-117">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="290af-118">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-118">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="290af-119">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-119">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="290af-120">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-120">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="290af-121">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="290af-121">November 20, 2018</span></span>

<span data-ttu-id="290af-122">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="290af-122">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="290af-123">코어</span><span class="sxs-lookup"><span data-stu-id="290af-123">Core</span></span>
* <span data-ttu-id="290af-124">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="290af-124">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="290af-125">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-125">ACR</span></span>
* <span data-ttu-id="290af-126">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="290af-126">Added context token to task step</span></span>
* <span data-ttu-id="290af-127">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-127">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="290af-128">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="290af-128">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-129">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-129">Appservice</span></span>
* <span data-ttu-id="290af-130">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-130">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="290af-131">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-131">Updated the default `node_version`.</span></span> <span data-ttu-id="290af-132">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-132">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="290af-133">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="290af-133">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="290af-134">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-134">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="290af-135">IotCentral</span><span class="sxs-lookup"><span data-stu-id="290af-135">IotCentral</span></span>
* <span data-ttu-id="290af-136">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="290af-136">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-137">KeyVault</span><span class="sxs-lookup"><span data-stu-id="290af-137">KeyVault</span></span>
* <span data-ttu-id="290af-138">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-138">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="290af-139">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-139">Network</span></span>
* <span data-ttu-id="290af-140">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-140">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="290af-141">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="290af-141">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="290af-142">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-142">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="290af-143">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="290af-143">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-144">Rdbms</span><span class="sxs-lookup"><span data-stu-id="290af-144">Rdbms</span></span>
* <span data-ttu-id="290af-145">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-145">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="290af-146">Rbac</span><span class="sxs-lookup"><span data-stu-id="290af-146">Rbac</span></span>
* <span data-ttu-id="290af-147">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-147">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="290af-148">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-148">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="290af-149">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-149">Storage</span></span>
* <span data-ttu-id="290af-150">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-150">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="290af-151">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-151">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="290af-152">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-152">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="290af-153">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-153">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="290af-154">VM</span><span class="sxs-lookup"><span data-stu-id="290af-154">VM</span></span>
* <span data-ttu-id="290af-155">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-155">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="290af-156">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-156">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="290af-157">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="290af-157">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="290af-158">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-158">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="290af-159">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-159">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="290af-160">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-160">Added `snapshot wait` command</span></span>
* <span data-ttu-id="290af-161">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-161">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="290af-162">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="290af-162">November 6, 2018</span></span>

<span data-ttu-id="290af-163">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="290af-163">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="290af-164">코어</span><span class="sxs-lookup"><span data-stu-id="290af-164">Core</span></span>
* <span data-ttu-id="290af-165">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-165">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="290af-166">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-166">ACR</span></span>
* <span data-ttu-id="290af-167">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-167">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="290af-168">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-168">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="290af-169">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-169">ACS</span></span>
* <span data-ttu-id="290af-170">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-170">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="290af-171">Advisor</span><span class="sxs-lookup"><span data-stu-id="290af-171">Advisor</span></span>
* <span data-ttu-id="290af-172">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-172">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="290af-173">AMS</span><span class="sxs-lookup"><span data-stu-id="290af-173">AMS</span></span>
* <span data-ttu-id="290af-174">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="290af-174">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="290af-175">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="290af-175">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="290af-176">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-176">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="290af-177">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="290af-177">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="290af-178">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-178">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="290af-179">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-179">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="290af-180">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-180">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="290af-181">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="290af-181">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="290af-182">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-182">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="290af-183">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-183">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="290af-184">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="290af-184">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="290af-185">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="290af-185">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="290af-186">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="290af-186">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="290af-187">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="290af-187">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="290af-188">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-188">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="290af-189">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-189">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="290af-190">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-190">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-191">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-191">AppService</span></span>
* <span data-ttu-id="290af-192">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-192">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="290af-193">구성</span><span class="sxs-lookup"><span data-stu-id="290af-193">Configure</span></span>
* <span data-ttu-id="290af-194">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-194">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="290af-195">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-195">Container</span></span>
* <span data-ttu-id="290af-196">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-196">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="290af-197">EventHub</span><span class="sxs-lookup"><span data-stu-id="290af-197">EventHub</span></span>
* <span data-ttu-id="290af-198">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-198">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-199">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-199">Interactive</span></span>
* <span data-ttu-id="290af-200">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="290af-200">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-201">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-201">Monitor</span></span>
* <span data-ttu-id="290af-202">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-202">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="290af-203">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-203">Network</span></span>
* <span data-ttu-id="290af-204">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-204">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="290af-205">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-205">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="290af-206">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-206">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="290af-207">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-207">Profile</span></span>
* <span data-ttu-id="290af-208">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-208">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-209">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-209">RDBMS</span></span>
* <span data-ttu-id="290af-210">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-210">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="290af-211">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-211">Resource</span></span>
* <span data-ttu-id="290af-212">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-212">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="290af-213">역할</span><span class="sxs-lookup"><span data-stu-id="290af-213">Role</span></span>
* <span data-ttu-id="290af-214">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-214">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="290af-215">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-215">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="290af-216">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-216">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="290af-217">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-217">Storage</span></span>
* <span data-ttu-id="290af-218">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-218">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="290af-219">VM</span><span class="sxs-lookup"><span data-stu-id="290af-219">VM</span></span>
* <span data-ttu-id="290af-220">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-220">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="290af-221">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-221">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="290af-222">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-222">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="290af-223">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-223">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="290af-224">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="290af-224">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="290af-225">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-225">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="290af-226">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="290af-226">October 23, 2018</span></span>

<span data-ttu-id="290af-227">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="290af-227">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="290af-228">코어</span><span class="sxs-lookup"><span data-stu-id="290af-228">Core</span></span>
* <span data-ttu-id="290af-229">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-229">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="290af-230">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-230">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="290af-231">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-231">ACR</span></span>
* <span data-ttu-id="290af-232">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-232">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="290af-233">CDN</span><span class="sxs-lookup"><span data-stu-id="290af-233">CDN</span></span>
* <span data-ttu-id="290af-234">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-234">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="290af-235">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-235">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="290af-236">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-236">Container</span></span>
* <span data-ttu-id="290af-237">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-237">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="290af-238">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-238">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="290af-239">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-239">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="290af-240">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-240">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="290af-241">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-241">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="290af-242">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-242">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="290af-243">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-243">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="290af-244">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="290af-244">CosmosDB</span></span>
* <span data-ttu-id="290af-245">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-245">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-246">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-246">Interactive</span></span>
* <span data-ttu-id="290af-247">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-247">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="290af-248">IoT Central</span><span class="sxs-lookup"><span data-stu-id="290af-248">IoT Central</span></span>
* <span data-ttu-id="290af-249">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-249">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="290af-250">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-250">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-251">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-251">Monitor</span></span>
* <span data-ttu-id="290af-252">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="290af-252">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="290af-253">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-253">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="290af-254">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-254">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="290af-255">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-255">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="290af-256">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-256">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="290af-257">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-257">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="290af-258">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="290af-258">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="290af-259">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-259">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="290af-260">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-260">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="290af-261">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-261">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="290af-262">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-262">Network</span></span>
* <span data-ttu-id="290af-263">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-263">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="290af-264">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-264">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="290af-265">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="290af-265">ServiceBus</span></span>
* <span data-ttu-id="290af-266">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-266">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="290af-267">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-267">SQL</span></span>
* <span data-ttu-id="290af-268">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-268">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="290af-269">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-269">Storage</span></span>
* <span data-ttu-id="290af-270">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-270">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="290af-271">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-271">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="290af-272">VM</span><span class="sxs-lookup"><span data-stu-id="290af-272">VM</span></span>
* <span data-ttu-id="290af-273">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-273">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="290af-274">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-274">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="290af-275">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-275">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="290af-276">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="290af-276">October 16, 2018</span></span>

<span data-ttu-id="290af-277">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="290af-277">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="290af-278">VM</span><span class="sxs-lookup"><span data-stu-id="290af-278">VM</span></span>
* <span data-ttu-id="290af-279">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-279">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="290af-280">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="290af-280">October 9, 2018</span></span>

<span data-ttu-id="290af-281">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="290af-281">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="290af-282">코어</span><span class="sxs-lookup"><span data-stu-id="290af-282">Core</span></span>
* <span data-ttu-id="290af-283">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="290af-283">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="290af-284">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-284">ACR</span></span>
* <span data-ttu-id="290af-285">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-285">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="290af-286">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-286">ACS</span></span>
* <span data-ttu-id="290af-287">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="290af-287">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="290af-288">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="290af-288">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="290af-289">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-289">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="290af-290">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="290af-290">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="290af-291">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-291">Container</span></span>
* <span data-ttu-id="290af-292">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-292">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="290af-293">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-293">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="290af-294">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="290af-294">Event Hub</span></span>
* <span data-ttu-id="290af-295">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-295">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="290af-296">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="290af-296">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="290af-297">확장</span><span class="sxs-lookup"><span data-stu-id="290af-297">Extensions</span></span>
* <span data-ttu-id="290af-298">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-298">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="290af-299">HDInsight</span><span class="sxs-lookup"><span data-stu-id="290af-299">HDInsight</span></span>
* <span data-ttu-id="290af-300">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-300">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="290af-301">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-301">IoT</span></span>
* <span data-ttu-id="290af-302">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-302">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-303">KeyVault</span><span class="sxs-lookup"><span data-stu-id="290af-303">KeyVault</span></span>
* <span data-ttu-id="290af-304">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-304">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="290af-305">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-305">Network</span></span>
* <span data-ttu-id="290af-306">`network dns zone create` 수정: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-306">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="290af-307">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="290af-307">See #6052</span></span>
* <span data-ttu-id="290af-308">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="290af-308">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="290af-309">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-309">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="290af-310">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-310">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="290af-311">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-311">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="290af-312">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-312">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="290af-313">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-313">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="290af-314">역할</span><span class="sxs-lookup"><span data-stu-id="290af-314">Role</span></span>
* <span data-ttu-id="290af-315">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-315">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="290af-316">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-316">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="290af-317">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-317">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="290af-318">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-318">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="290af-319">Service Bus</span><span class="sxs-lookup"><span data-stu-id="290af-319">Service Bus</span></span>
* <span data-ttu-id="290af-320">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="290af-320">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="290af-321">VM</span><span class="sxs-lookup"><span data-stu-id="290af-321">VM</span></span>
* <span data-ttu-id="290af-322">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="290af-322">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="290af-323">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-323">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="290af-324">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-324">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="290af-325">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-325">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="290af-326">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-326">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="290af-327">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-327">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="290af-328">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="290af-328">September 21, 2018</span></span>

<span data-ttu-id="290af-329">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="290af-329">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="290af-330">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-330">ACR</span></span>
* <span data-ttu-id="290af-331">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-331">Added ACR Task commands</span></span>
* <span data-ttu-id="290af-332">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-332">Added quick run command</span></span>
* <span data-ttu-id="290af-333">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-333">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="290af-334">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="290af-334">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="290af-335">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-335">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="290af-336">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="290af-336">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="290af-337">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-337">ACS</span></span>
* <span data-ttu-id="290af-338">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="290af-338">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="290af-339">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="290af-339">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-340">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-340">AppService</span></span>

* <span data-ttu-id="290af-341">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-341">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="290af-342">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-342">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="290af-343">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-343">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="290af-344">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-344">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="290af-345">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-345">Batch</span></span>
* <span data-ttu-id="290af-346">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="290af-346">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="290af-347">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-347">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="290af-348">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-348">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="290af-349">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="290af-349">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="290af-350">Batch AI</span><span class="sxs-lookup"><span data-stu-id="290af-350">Batch AI</span></span> 
* <span data-ttu-id="290af-351">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="290af-351">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="290af-352">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="290af-352">Cognitive Services</span></span>
* <span data-ttu-id="290af-353">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="290af-353">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="290af-354">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-354">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="290af-355">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-355">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="290af-356">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-356">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="290af-357">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-357">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="290af-358">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-358">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="290af-359">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-359">Container</span></span>
* <span data-ttu-id="290af-360">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="290af-360">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="290af-361">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-361">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="290af-362">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-362">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="290af-363">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="290af-363">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="290af-364">Datalake</span><span class="sxs-lookup"><span data-stu-id="290af-364">Datalake</span></span>
* <span data-ttu-id="290af-365">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-365">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="290af-366">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="290af-366">Interactive Shell</span></span>
* <span data-ttu-id="290af-367">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="290af-367">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="290af-368">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-368">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="290af-369">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-369">IoT</span></span>
* <span data-ttu-id="290af-370">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-370">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="290af-371">Key Vault</span><span class="sxs-lookup"><span data-stu-id="290af-371">Key Vault</span></span>
* <span data-ttu-id="290af-372">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="290af-372">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="290af-373">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-373">Network</span></span>
* <span data-ttu-id="290af-374">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-374">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="290af-375">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-375">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="290af-376">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-376">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="290af-377">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-377">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="290af-378">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-378">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="290af-379">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-379">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="290af-380">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="290af-380">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="290af-381">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-381">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="290af-382">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="290af-382">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="290af-383">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="290af-383">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="290af-384">`network vnet subnet create/update`: `--delegation` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-384">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="290af-385">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-385">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="290af-386">`network traffic-manager profile create/update`: 모니터 구성을 위한 `--interval`, `--timeout` 및 `--max-failures` 지원 추가. `--path`, `--port`, `--protocol`로 인해 `--monitor-path`, `--monitor-port` 및 `--monitor-protocol` 옵션이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-386">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="290af-387">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하기 위한 논리 수정. 사설 IP 주소가 제공된 경우 할당이 정적이 됨. 사설 IP 주소가 제공되지 않은 경우 사설 IP 주소에 대해 빈 문자열이 제공되고 할당이 동적이 됨.</span><span class="sxs-lookup"><span data-stu-id="290af-387">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="290af-388">`dns record-set * create/update`: `--target-resource` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-388">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="290af-389">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-389">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="290af-390">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-390">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="290af-391">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-391">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-392">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-392">RDBMS</span></span>
* <span data-ttu-id="290af-393">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-393">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="290af-394">예약</span><span class="sxs-lookup"><span data-stu-id="290af-394">Reservation</span></span>
* <span data-ttu-id="290af-395">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="290af-395">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="290af-396">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="290af-396">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="290af-397">앱 관리</span><span class="sxs-lookup"><span data-stu-id="290af-397">Manage App</span></span>
* <span data-ttu-id="290af-398">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="290af-398">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="290af-399">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="290af-399">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="290af-400">역할</span><span class="sxs-lookup"><span data-stu-id="290af-400">Role</span></span>
* <span data-ttu-id="290af-401">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-401">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="290af-402">SignalR</span><span class="sxs-lookup"><span data-stu-id="290af-402">SignalR</span></span>
* <span data-ttu-id="290af-403">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-403">First release</span></span>

### <a name="storage"></a><span data-ttu-id="290af-404">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-404">Storage</span></span>
* <span data-ttu-id="290af-405">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-405">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="290af-406">변경할 수 없는 저장소 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-406">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="290af-407">VM</span><span class="sxs-lookup"><span data-stu-id="290af-407">VM</span></span>
* <span data-ttu-id="290af-408">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="290af-408">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="290af-409">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-409">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="290af-410">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="290af-410">August 28, 2018</span></span>

<span data-ttu-id="290af-411">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="290af-411">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="290af-412">코어</span><span class="sxs-lookup"><span data-stu-id="290af-412">Core</span></span>

* <span data-ttu-id="290af-413">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-413">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="290af-414">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-414">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="290af-415">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-415">ACR</span></span>

* <span data-ttu-id="290af-416">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="290af-416">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="290af-417">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-417">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="290af-418">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-418">ACS</span></span>

* <span data-ttu-id="290af-419">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-419">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="290af-420">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-420">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-421">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-421">AppService</span></span>

* <span data-ttu-id="290af-422">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-422">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="290af-423">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-423">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="290af-424">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-424">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="290af-425">Backup</span><span class="sxs-lookup"><span data-stu-id="290af-425">Backup</span></span>

* <span data-ttu-id="290af-426">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-426">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="290af-427">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="290af-427">Bot Service</span></span>

* <span data-ttu-id="290af-428">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-428">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="290af-429">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="290af-429">Cognitive Services</span></span>

* <span data-ttu-id="290af-430">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-430">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="290af-431">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-431">IoT</span></span>

* <span data-ttu-id="290af-432">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-432">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-433">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-433">Monitor</span></span>

* <span data-ttu-id="290af-434">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-434">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="290af-435">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="290af-435">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="290af-436">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-436">Network</span></span>

* <span data-ttu-id="290af-437">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-437">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="290af-438">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-438">Resource</span></span>

* <span data-ttu-id="290af-439">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-439">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="290af-440">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-440">Storage</span></span>

* <span data-ttu-id="290af-441">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-441">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="290af-442">VM</span><span class="sxs-lookup"><span data-stu-id="290af-442">VM</span></span>

* <span data-ttu-id="290af-443">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-443">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="290af-444">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="290af-444">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="290af-445">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="290af-445">Auguest 14, 2018</span></span>

<span data-ttu-id="290af-446">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="290af-446">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="290af-447">코어</span><span class="sxs-lookup"><span data-stu-id="290af-447">Core</span></span>

* <span data-ttu-id="290af-448">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="290af-448">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="290af-449">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="290af-449">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="290af-450">원격 분석</span><span class="sxs-lookup"><span data-stu-id="290af-450">Telemetry</span></span>

* <span data-ttu-id="290af-451">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="290af-451">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="290af-452">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-452">ACR</span></span>

* <span data-ttu-id="290af-453">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-453">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="290af-454">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-454">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="290af-455">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-455">ACS</span></span>

* <span data-ttu-id="290af-456">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-456">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="290af-457">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-457">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="290af-458">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="290af-458">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="290af-459">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="290af-459">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="290af-460">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-460">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="290af-461">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-461">AppService</span></span>

* <span data-ttu-id="290af-462">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-462">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="290af-463">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="290af-463">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="290af-464">BatchAI</span><span class="sxs-lookup"><span data-stu-id="290af-464">BatchAI</span></span>

* <span data-ttu-id="290af-465">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="290af-465">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="290af-466">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-466">Container</span></span>

* <span data-ttu-id="290af-467">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-467">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="290af-468">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-468">IoT</span></span>

* <span data-ttu-id="290af-469">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="290af-469">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="290af-470">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-470">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="290af-471">Iot Central</span><span class="sxs-lookup"><span data-stu-id="290af-471">Iot Central</span></span>

* <span data-ttu-id="290af-472">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-472">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-473">KeyVault</span><span class="sxs-lookup"><span data-stu-id="290af-473">KeyVault</span></span>


* <span data-ttu-id="290af-474">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-474">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="290af-475">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-475">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="290af-476">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="290af-476">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="290af-477">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-477">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="290af-478">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-478">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="290af-479">릴레이</span><span class="sxs-lookup"><span data-stu-id="290af-479">Relay</span></span>

* <span data-ttu-id="290af-480">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-480">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="290af-481">Sql</span><span class="sxs-lookup"><span data-stu-id="290af-481">Sql</span></span>

* <span data-ttu-id="290af-482">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-482">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="290af-483">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-483">Storage</span></span>

* <span data-ttu-id="290af-484">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="290af-484">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="290af-485">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-485">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="290af-486">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="290af-486">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="290af-487">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="290af-487">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="290af-488">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="290af-488">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="290af-489">VM</span><span class="sxs-lookup"><span data-stu-id="290af-489">VM</span></span>

* <span data-ttu-id="290af-490">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-490">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="290af-491">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="290af-491">July 31, 2018</span></span>

<span data-ttu-id="290af-492">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="290af-492">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="290af-493">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-493">ACR</span></span>

* <span data-ttu-id="290af-494">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-494">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="290af-495">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-495">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="290af-496">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-496">ACS</span></span>

* <span data-ttu-id="290af-497">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-497">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="290af-498">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-498">Batch</span></span>

* <span data-ttu-id="290af-499">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-499">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="290af-500">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-500">Container</span></span>

* <span data-ttu-id="290af-501">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-501">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="290af-502">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-502">Network</span></span>

* <span data-ttu-id="290af-503">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-503">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="290af-504">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-504">Resource</span></span>

* <span data-ttu-id="290af-505">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="290af-505">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="290af-506">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="290af-506">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="290af-507">역할</span><span class="sxs-lookup"><span data-stu-id="290af-507">Role</span></span>

* <span data-ttu-id="290af-508">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-508">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="290af-509">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-509">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="290af-510">검색</span><span class="sxs-lookup"><span data-stu-id="290af-510">Search</span></span>

* <span data-ttu-id="290af-511">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-511">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="290af-512">Service Bus</span><span class="sxs-lookup"><span data-stu-id="290af-512">Service Bus</span></span>

* <span data-ttu-id="290af-513">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-513">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="290af-514">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-514">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="290af-515">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="290af-515">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="290af-516">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="290af-516">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-517">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-517">Storage</span></span>

* <span data-ttu-id="290af-518">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-518">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="290af-519">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="290af-519">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="290af-520">VM</span><span class="sxs-lookup"><span data-stu-id="290af-520">VM</span></span>

* <span data-ttu-id="290af-521">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-521">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="290af-522">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-522">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="290af-523">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-523">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="290af-524">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-524">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="290af-525">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="290af-525">July 18, 2018</span></span>

<span data-ttu-id="290af-526">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="290af-526">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="290af-527">코어</span><span class="sxs-lookup"><span data-stu-id="290af-527">Core</span></span>

* <span data-ttu-id="290af-528">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-528">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="290af-529">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="290af-529">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="290af-530">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-530">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="290af-531">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-531">ACR</span></span>

* <span data-ttu-id="290af-532">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-532">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="290af-533">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-533">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="290af-534">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="290af-534">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="290af-535">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="290af-535">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="290af-536">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-536">ACS</span></span>

* <span data-ttu-id="290af-537">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="290af-537">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-538">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-538">AppService</span></span>

* <span data-ttu-id="290af-539">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-539">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="290af-540">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-540">Batch</span></span>

* <span data-ttu-id="290af-541">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-541">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="290af-542">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-542">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="290af-543">Batch AI</span><span class="sxs-lookup"><span data-stu-id="290af-543">Batch AI</span></span>

* <span data-ttu-id="290af-544">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-544">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="290af-545">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-545">Container</span></span>

* <span data-ttu-id="290af-546">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="290af-546">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="290af-547">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="290af-547">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="290af-548">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-548">Network</span></span>

* <span data-ttu-id="290af-549">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-549">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="290af-550">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-550">Added `network nic wait`</span></span>
* <span data-ttu-id="290af-551">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-551">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="290af-552">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="290af-552">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="290af-553">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-553">Resource</span></span>

* <span data-ttu-id="290af-554">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-554">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="290af-555">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-555">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="290af-556">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-556">Added `deployment wait` command</span></span>
* <span data-ttu-id="290af-557">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-557">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="290af-558">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-558">SQL</span></span>

* <span data-ttu-id="290af-559">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-559">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="290af-560">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="290af-560">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="290af-561">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="290af-561">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="290af-562">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-562">Storage</span></span>

* <span data-ttu-id="290af-563">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="290af-563">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="290af-564">VM</span><span class="sxs-lookup"><span data-stu-id="290af-564">VM</span></span>

* <span data-ttu-id="290af-565">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-565">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="290af-566">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-566">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="290af-567">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-567">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="290af-568">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="290af-568">July 3, 2018</span></span>

<span data-ttu-id="290af-569">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="290af-569">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="290af-570">AKS</span><span class="sxs-lookup"><span data-stu-id="290af-570">AKS</span></span>

* <span data-ttu-id="290af-571">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="290af-571">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="290af-572">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="290af-572">July 3, 2018</span></span>

<span data-ttu-id="290af-573">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="290af-573">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="290af-574">코어</span><span class="sxs-lookup"><span data-stu-id="290af-574">Core</span></span>

* <span data-ttu-id="290af-575">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="290af-575">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="290af-576">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-576">ACR</span></span>

* <span data-ttu-id="290af-577">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="290af-577">Added polling build status</span></span>
* <span data-ttu-id="290af-578">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-578">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="290af-579">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-579">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="290af-580">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-580">ACS</span></span>

* <span data-ttu-id="290af-581">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-581">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="290af-582">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-582">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="290af-583">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="290af-583">Updated options for `aks browse` command.</span></span> <span data-ttu-id="290af-584">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-584">Added `--listen-port` support</span></span>
* <span data-ttu-id="290af-585">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="290af-585">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="290af-586">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="290af-586">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="290af-587">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-587">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-588">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-588">AppService</span></span>

* <span data-ttu-id="290af-589">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-589">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="290af-590">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="290af-590">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="290af-591">Backup</span><span class="sxs-lookup"><span data-stu-id="290af-591">Backup</span></span>

* <span data-ttu-id="290af-592">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-592">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="290af-593">BatchAI</span><span class="sxs-lookup"><span data-stu-id="290af-593">BatchAI</span></span>

* <span data-ttu-id="290af-594">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-594">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="290af-595">클라우드</span><span class="sxs-lookup"><span data-stu-id="290af-595">Cloud</span></span>

* <span data-ttu-id="290af-596">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-596">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="290af-597">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-597">Container</span></span>

* <span data-ttu-id="290af-598">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-598">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="290af-599">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-599">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="290af-600">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="290af-600">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="290af-601">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-601">Extension</span></span>

* <span data-ttu-id="290af-602">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-602">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="290af-603">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-603">Network</span></span>

* <span data-ttu-id="290af-604">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="290af-604">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-605">Rdbms</span><span class="sxs-lookup"><span data-stu-id="290af-605">Rdbms</span></span>

* <span data-ttu-id="290af-606">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-606">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="290af-607">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-607">Resource</span></span>

* <span data-ttu-id="290af-608">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-608">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="290af-609">VM</span><span class="sxs-lookup"><span data-stu-id="290af-609">VM</span></span>

* <span data-ttu-id="290af-610">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-610">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="290af-611">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="290af-611">June 25, 2018</span></span>

<span data-ttu-id="290af-612">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="290af-612">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="290af-613">CLI</span><span class="sxs-lookup"><span data-stu-id="290af-613">CLI</span></span>

* <span data-ttu-id="290af-614">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-614">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="290af-615">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="290af-615">June 19, 2018</span></span>

<span data-ttu-id="290af-616">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="290af-616">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="290af-617">코어</span><span class="sxs-lookup"><span data-stu-id="290af-617">Core</span></span>

* <span data-ttu-id="290af-618">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-618">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="290af-619">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-619">ACR</span></span>

* <span data-ttu-id="290af-620">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-620">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="290af-621">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-621">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="290af-622">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-622">ACS</span></span>

* <span data-ttu-id="290af-623">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="290af-623">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="290af-624">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-624">Added `--update` support</span></span>
* <span data-ttu-id="290af-625">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-625">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="290af-626">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="290af-626">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="290af-627">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="290af-627">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="290af-628">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="290af-628">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="290af-629">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="290af-629">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="290af-630">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="290af-630">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-631">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-631">AppService</span></span>

* <span data-ttu-id="290af-632">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-632">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="290af-633">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-633">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="290af-634">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-634">Batch</span></span>

* <span data-ttu-id="290af-635">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="290af-635">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="290af-636">Batch AI</span><span class="sxs-lookup"><span data-stu-id="290af-636">Batch AI</span></span>

* <span data-ttu-id="290af-637">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="290af-637">Added support for workspaces.</span></span> <span data-ttu-id="290af-638">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="290af-638">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="290af-639">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="290af-639">Added support for experiments.</span></span> <span data-ttu-id="290af-640">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="290af-640">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="290af-641">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-641">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="290af-642">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="290af-642">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="290af-643">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-643">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="290af-644">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-644">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="290af-645">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="290af-645">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="290af-646">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="290af-646">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="290af-647">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="290af-647">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="290af-648">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="290af-648">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="290af-649">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="290af-649">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="290af-650">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="290af-650">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="290af-651">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="290af-651">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="290af-652">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="290af-652">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="290af-653">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="290af-653">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="290af-654">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="290af-654">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="290af-655">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="290af-655">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="290af-656">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="290af-656">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="290af-657">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="290af-657">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="290af-658">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="290af-658">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="290af-659">지도</span><span class="sxs-lookup"><span data-stu-id="290af-659">Maps</span></span>

* <span data-ttu-id="290af-660">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-660">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="290af-661">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-661">Network</span></span>

* <span data-ttu-id="290af-662">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-662">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="290af-663">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-663">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="290af-664">#6502</span><span class="sxs-lookup"><span data-stu-id="290af-664">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="290af-665">예약</span><span class="sxs-lookup"><span data-stu-id="290af-665">Reservations</span></span>

* <span data-ttu-id="290af-666">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-666">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="290af-667">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-667">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="290af-668">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="290af-668">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="290af-669">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-669">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="290af-670">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="290af-670">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="290af-671">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-671">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="290af-672">역할</span><span class="sxs-lookup"><span data-stu-id="290af-672">Role</span></span>

* <span data-ttu-id="290af-673">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="290af-673">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="290af-674">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-674">SQL</span></span>

* <span data-ttu-id="290af-675">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="290af-675">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="290af-676">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-676">Storage</span></span>

* <span data-ttu-id="290af-677">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="290af-677">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="290af-678">VM</span><span class="sxs-lookup"><span data-stu-id="290af-678">VM</span></span>

* <span data-ttu-id="290af-679">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="290af-679">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="290af-680">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="290af-680">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="290af-681">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-681">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="290af-682">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="290af-682">June 13, 2018</span></span>

<span data-ttu-id="290af-683">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="290af-683">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="290af-684">코어</span><span class="sxs-lookup"><span data-stu-id="290af-684">Core</span></span>

* <span data-ttu-id="290af-685">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="290af-685">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="290af-686">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="290af-686">June 13, 2018</span></span>

<span data-ttu-id="290af-687">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="290af-687">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="290af-688">AKS</span><span class="sxs-lookup"><span data-stu-id="290af-688">AKS</span></span>

* <span data-ttu-id="290af-689">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-689">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="290af-690">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="290af-690">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="290af-691">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-691">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="290af-692">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-692">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="290af-693">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-693">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-694">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-694">AppService</span></span>

* <span data-ttu-id="290af-695">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-695">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="290af-696">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="290af-696">June 5, 2018</span></span>

<span data-ttu-id="290af-697">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="290af-697">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-698">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-698">Interactive</span></span>

* <span data-ttu-id="290af-699">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="290af-699">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="290af-700">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="290af-700">June 5, 2018</span></span>

<span data-ttu-id="290af-701">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="290af-701">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="290af-702">코어</span><span class="sxs-lookup"><span data-stu-id="290af-702">Core</span></span>

* <span data-ttu-id="290af-703">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-703">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="290af-704">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-704">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="290af-705">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-705">ACR</span></span>

* <span data-ttu-id="290af-706">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-706">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="290af-707">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-707">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="290af-708">AKS</span><span class="sxs-lookup"><span data-stu-id="290af-708">AKS</span></span>

* <span data-ttu-id="290af-709">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="290af-709">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="290af-710">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-710">Batch</span></span>

* <span data-ttu-id="290af-711">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="290af-711">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="290af-712">IOT</span><span class="sxs-lookup"><span data-stu-id="290af-712">IOT</span></span>

* <span data-ttu-id="290af-713">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-713">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="290af-714">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-714">Network</span></span>

* <span data-ttu-id="290af-715">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="290af-715">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="290af-716">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="290af-716">Policy Insights</span></span>

* <span data-ttu-id="290af-717">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-717">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="290af-718">ARM</span><span class="sxs-lookup"><span data-stu-id="290af-718">ARM</span></span>

* <span data-ttu-id="290af-719">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-719">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="290af-720">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-720">SQL</span></span>

* <span data-ttu-id="290af-721">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="290af-721">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="290af-722">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-722">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="290af-723">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-723">Storage</span></span>

* <span data-ttu-id="290af-724">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="290af-724">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="290af-725">VM</span><span class="sxs-lookup"><span data-stu-id="290af-725">VM</span></span>

* <span data-ttu-id="290af-726">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-726">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="290af-727">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-727">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="290af-728">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-728">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="290af-729">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="290af-729">May 22, 2018</span></span>

<span data-ttu-id="290af-730">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="290af-730">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="290af-731">코어</span><span class="sxs-lookup"><span data-stu-id="290af-731">Core</span></span>

* <span data-ttu-id="290af-732">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-732">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="290af-733">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-733">ACS</span></span>

* <span data-ttu-id="290af-734">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-734">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="290af-735">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="290af-735">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-736">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-736">AppService</span></span>

* <span data-ttu-id="290af-737">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-737">Improved generic update commands</span></span>
* <span data-ttu-id="290af-738">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-738">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="290af-739">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-739">Container</span></span>

* <span data-ttu-id="290af-740">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-740">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="290af-741">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-741">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="290af-742">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-742">Extension</span></span>

* <span data-ttu-id="290af-743">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-743">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-744">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-744">Interactive</span></span>

* <span data-ttu-id="290af-745">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-745">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="290af-746">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="290af-746">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-747">KeyVault</span><span class="sxs-lookup"><span data-stu-id="290af-747">KeyVault</span></span>

* <span data-ttu-id="290af-748">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="290af-748">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="290af-749">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-749">Network</span></span>

* <span data-ttu-id="290af-750">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="290af-750">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="290af-751">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-751">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="290af-752">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-752">SQL</span></span>

* <span data-ttu-id="290af-753">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="290af-753">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="290af-754">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="290af-754">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="290af-755">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="290af-755">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="290af-756">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-756">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="290af-757">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-757">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="290af-758">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="290af-758">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="290af-759">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="290af-759">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="290af-760">`edition`</span><span class="sxs-lookup"><span data-stu-id="290af-760">`edition`.</span></span> <span data-ttu-id="290af-761">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="290af-761">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="290af-762">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="290af-762">`elasticPoolName`.</span></span> <span data-ttu-id="290af-763">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="290af-763">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="290af-764">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-764">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="290af-765">`edition`</span><span class="sxs-lookup"><span data-stu-id="290af-765">`edition`.</span></span> <span data-ttu-id="290af-766">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="290af-766">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="290af-767">`dtu`</span><span class="sxs-lookup"><span data-stu-id="290af-767">`dtu`.</span></span> <span data-ttu-id="290af-768">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="290af-768">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="290af-769">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="290af-769">`databaseDtuMin`.</span></span> <span data-ttu-id="290af-770">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="290af-770">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="290af-771">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="290af-771">`databaseDtuMax`.</span></span> <span data-ttu-id="290af-772">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="290af-772">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="290af-773">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-773">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="290af-774">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-774">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="290af-775">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-775">Storage</span></span>

* <span data-ttu-id="290af-776">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="290af-776">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="290af-777">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-777">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="290af-778">VM</span><span class="sxs-lookup"><span data-stu-id="290af-778">VM</span></span>

* <span data-ttu-id="290af-779">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="290af-779">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="290af-780">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="290af-780">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="290af-781">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="290af-781">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="290af-782">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="290af-782">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="290af-783">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-783">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="290af-784">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="290af-784">May 7, 2018</span></span>

<span data-ttu-id="290af-785">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="290af-785">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="290af-786">코어</span><span class="sxs-lookup"><span data-stu-id="290af-786">Core</span></span>

* <span data-ttu-id="290af-787">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-787">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="290af-788">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-788">Added limited support for positional arguments</span></span>
* <span data-ttu-id="290af-789">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-789">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="290af-790">#5591</span><span class="sxs-lookup"><span data-stu-id="290af-790">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="290af-791">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-791">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="290af-792">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="290af-792">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="290af-793">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-793">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="290af-794">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-794">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="290af-795">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-795">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="290af-796">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-796">ACR</span></span>

* <span data-ttu-id="290af-797">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-797">Added ACR Build commands</span></span>
* <span data-ttu-id="290af-798">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-798">Improved resource not found error messages</span></span>
* <span data-ttu-id="290af-799">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-799">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="290af-800">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-800">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="290af-801">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-801">Improved repository commands error messages</span></span>
* <span data-ttu-id="290af-802">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-802">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="290af-803">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-803">ACS</span></span>

* <span data-ttu-id="290af-804">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-804">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="290af-805">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-805">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="290af-806">AMS</span><span class="sxs-lookup"><span data-stu-id="290af-806">AMS</span></span>

* <span data-ttu-id="290af-807">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="290af-807">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-808">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-808">Appservice</span></span>

* <span data-ttu-id="290af-809">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-809">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="290af-810">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-810">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="290af-811">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-811">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="290af-812">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-812">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="290af-813">Batch AI</span><span class="sxs-lookup"><span data-stu-id="290af-813">Batch AI</span></span>

* <span data-ttu-id="290af-814">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-814">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="290af-815">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="290af-815">Cognitive Services</span></span>

* <span data-ttu-id="290af-816">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-816">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="290af-817">Consumption</span><span class="sxs-lookup"><span data-stu-id="290af-817">Consumption</span></span>

* <span data-ttu-id="290af-818">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-818">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="290af-819">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-819">Container</span></span>

* <span data-ttu-id="290af-820">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-820">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="290af-821">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="290af-821">Cosmos DB</span></span>

* <span data-ttu-id="290af-822">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="290af-822">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="290af-823">DMS</span><span class="sxs-lookup"><span data-stu-id="290af-823">DMS</span></span>

* <span data-ttu-id="290af-824">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-824">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="290af-825">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-825">Extension</span></span>

* <span data-ttu-id="290af-826">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-826">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-827">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-827">Interactive</span></span>

* <span data-ttu-id="290af-828">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-828">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="290af-829">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="290af-829">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="290af-830">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-830">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="290af-831">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-831">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="290af-832">랩</span><span class="sxs-lookup"><span data-stu-id="290af-832">Lab</span></span>

* <span data-ttu-id="290af-833">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-833">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="290af-834">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-834">Network</span></span>

* <span data-ttu-id="290af-835">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-835">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="290af-836">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-836">Profile</span></span>

* <span data-ttu-id="290af-837">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-837">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="290af-838">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-838">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="290af-839">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-839">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="290af-840">Redis</span><span class="sxs-lookup"><span data-stu-id="290af-840">Redis</span></span>

* <span data-ttu-id="290af-841">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-841">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="290af-842">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-842">Deprecated `redis list-all`.</span></span> <span data-ttu-id="290af-843">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="290af-843">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="290af-844">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-844">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="290af-845">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-845">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="290af-846">역할</span><span class="sxs-lookup"><span data-stu-id="290af-846">Role</span></span>

* <span data-ttu-id="290af-847">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-847">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-848">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-848">Storage</span></span>

* <span data-ttu-id="290af-849">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-849">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="290af-850">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="290af-850">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="290af-851">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="290af-851">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="290af-852">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="290af-852">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="290af-853">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-853">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="290af-854">VM</span><span class="sxs-lookup"><span data-stu-id="290af-854">VM</span></span>

* <span data-ttu-id="290af-855">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-855">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="290af-856">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-856">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="290af-857">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="290af-857">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="290af-858">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-858">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="290af-859">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-859">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="290af-860">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-860">Added write accelerator support</span></span>
* <span data-ttu-id="290af-861">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-861">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="290af-862">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-862">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="290af-863">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-863">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="290af-864">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="290af-864">April 10, 2018</span></span>

<span data-ttu-id="290af-865">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="290af-865">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="290af-866">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-866">ACR</span></span>

* <span data-ttu-id="290af-867">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="290af-867">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="290af-868">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-868">ACS</span></span>

* <span data-ttu-id="290af-869">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="290af-869">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-870">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-870">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="290af-872">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-872">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="290af-873">BatchAI</span><span class="sxs-lookup"><span data-stu-id="290af-873">BatchAI</span></span>

* <span data-ttu-id="290af-874">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-874">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="290af-875">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="290af-875">Job level mounting</span></span>
  - <span data-ttu-id="290af-876">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="290af-876">Environment variables with secret values</span></span>
  - <span data-ttu-id="290af-877">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="290af-877">Performance counters settings</span></span>
  - <span data-ttu-id="290af-878">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="290af-878">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="290af-879">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="290af-879">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="290af-880">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="290af-880">Usage and limits reporting</span></span>
  - <span data-ttu-id="290af-881">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-881">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="290af-882">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="290af-882">Support for custom images</span></span>
  - <span data-ttu-id="290af-883">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-883">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="290af-884">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-884">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="290af-885">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-885">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="290af-886">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-886">National clouds are supported</span></span>
* <span data-ttu-id="290af-887">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-887">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="290af-888">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="290af-888">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="290af-889">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="290af-889">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="290af-890">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-890">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="290af-891">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="290af-891">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="290af-892">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="290af-892">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="290af-893">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-893">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="290af-894">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-894">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="290af-895">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-895">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="290af-896">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-896">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="290af-897">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="290af-897">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="290af-898">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="290af-898">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="290af-899">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-899">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="290af-900">결제</span><span class="sxs-lookup"><span data-stu-id="290af-900">Billing</span></span>

* <span data-ttu-id="290af-901">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-901">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="290af-902">Consumption</span><span class="sxs-lookup"><span data-stu-id="290af-902">Consumption</span></span>

* <span data-ttu-id="290af-903">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-903">Added `marketplace` commands</span></span>
* <span data-ttu-id="290af-904">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-904">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="290af-905">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-905">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="290af-906">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-906">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="290af-907">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-907">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="290af-908">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-908">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="290af-909">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-909">Container</span></span>

* <span data-ttu-id="290af-910">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="290af-910">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="290af-911">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="290af-911">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="290af-912">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-912">Extension</span></span>

* <span data-ttu-id="290af-913">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-913">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-914">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-914">Interactive</span></span>

* <span data-ttu-id="290af-915">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-915">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="290af-916">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="290af-916">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="290af-917">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="290af-917">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="290af-918">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-918">Network</span></span>

* <span data-ttu-id="290af-919">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-919">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="290af-920">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-920">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="290af-921">#4910</span><span class="sxs-lookup"><span data-stu-id="290af-921">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="290af-922">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-922">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="290af-923">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="290af-923">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="290af-924">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-924">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="290af-925">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-925">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="290af-926">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-926">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="290af-927">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-927">Profile</span></span>

* <span data-ttu-id="290af-928">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-928">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="290af-929">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-929">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-930">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-930">RDBMS</span></span>

* <span data-ttu-id="290af-931">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-931">Added `georestore` command</span></span>
* <span data-ttu-id="290af-932">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-932">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="290af-933">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-933">Resource</span></span>

* <span data-ttu-id="290af-934">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-934">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="290af-935">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-935">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="290af-936">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-936">SQL</span></span>

* <span data-ttu-id="290af-937">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-937">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-938">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-938">Storage</span></span>

* <span data-ttu-id="290af-939">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-939">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="290af-940">VM</span><span class="sxs-lookup"><span data-stu-id="290af-940">VM</span></span>

* <span data-ttu-id="290af-941">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-941">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="290af-942">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-942">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="290af-944">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-944">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="290af-945">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-945">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="290af-946">#5718</span><span class="sxs-lookup"><span data-stu-id="290af-946">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="290af-947">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-947">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="290af-948">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="290af-948">March 27, 2018</span></span>

<span data-ttu-id="290af-949">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="290af-949">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="290af-950">코어</span><span class="sxs-lookup"><span data-stu-id="290af-950">Core</span></span>

* <span data-ttu-id="290af-951">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="290af-951">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="290af-952">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-952">ACS</span></span>

* <span data-ttu-id="290af-953">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="290af-953">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-954">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-954">Appservice</span></span>

* <span data-ttu-id="290af-955">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-955">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="290af-956">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-956">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="290af-957">Backup</span><span class="sxs-lookup"><span data-stu-id="290af-957">Backup</span></span>

* <span data-ttu-id="290af-958">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-958">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="290af-959">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-959">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="290af-960">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-960">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="290af-961">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-961">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="290af-962">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-962">Container</span></span>

* <span data-ttu-id="290af-963">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-963">Added `container exec` command.</span></span> <span data-ttu-id="290af-964">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-964">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="290af-965">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="290af-965">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="290af-966">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-966">Extension</span></span>

* <span data-ttu-id="290af-967">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-967">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="290af-968">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-968">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="290af-969">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-969">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-970">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-970">Interactive</span></span>

* <span data-ttu-id="290af-971">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="290af-971">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="290af-972">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-972">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="290af-973">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="290af-973">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="290af-974">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-974">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="290af-975">랩</span><span class="sxs-lookup"><span data-stu-id="290af-975">Lab</span></span>

* <span data-ttu-id="290af-976">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-976">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-977">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-977">Monitor</span></span>

* <span data-ttu-id="290af-978">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-978">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="290af-979">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="290af-979">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="290af-980">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-980">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="290af-981">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-981">Network</span></span>

* <span data-ttu-id="290af-982">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-982">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="290af-983">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-983">Profile</span></span>

* <span data-ttu-id="290af-984">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-984">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-985">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-985">RDBMS</span></span>

* <span data-ttu-id="290af-986">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-986">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="290af-987">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-987">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="290af-989">역할</span><span class="sxs-lookup"><span data-stu-id="290af-989">Role</span></span>

* <span data-ttu-id="290af-990">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-990">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="290af-991">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-991">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="290af-992">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-992">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="290af-993">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-993">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="290af-994">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-994">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-995">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-995">Storage</span></span>

* <span data-ttu-id="290af-996">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-996">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="290af-997">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="290af-997">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="290af-998">VM</span><span class="sxs-lookup"><span data-stu-id="290af-998">VM</span></span>

* <span data-ttu-id="290af-999">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-999">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="290af-1000">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1000">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="290af-1001">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1001">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="290af-1002">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1002">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="290af-1003">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="290af-1003">March 13, 2018</span></span>

<span data-ttu-id="290af-1004">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="290af-1004">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="290af-1005">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-1005">ACR</span></span>

* <span data-ttu-id="290af-1006">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1006">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="290af-1007">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1007">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="290af-1008">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1008">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1009">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1009">ACS</span></span>

* <span data-ttu-id="290af-1010">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1010">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="290af-1011">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1011">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="290af-1012">Advisor</span><span class="sxs-lookup"><span data-stu-id="290af-1012">Advisor</span></span>

* <span data-ttu-id="290af-1013">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1013">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="290af-1014">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1014">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="290af-1015">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1015">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="290af-1016">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1016">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="290af-1017">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1017">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1018">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1018">Appservice</span></span>

* <span data-ttu-id="290af-1019">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1019">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="290af-1020">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1020">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="290af-1021">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="290af-1021">Eventhubs</span></span>

* <span data-ttu-id="290af-1022">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1022">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="290af-1023">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-1023">Extension</span></span>

* <span data-ttu-id="290af-1024">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1024">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-1025">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-1025">Interactive</span></span>

* <span data-ttu-id="290af-1026">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="290af-1026">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="290af-1027">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="290af-1027">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="290af-1028">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1028">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="290af-1029">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1029">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1030">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1030">Monitor</span></span>

* <span data-ttu-id="290af-1031">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1031">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="290af-1032">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1032">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="290af-1033">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1033">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="290af-1034">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1034">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="290af-1035">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1035">Network</span></span>

* <span data-ttu-id="290af-1036">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1036">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="290af-1037">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="290af-1037">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="290af-1038">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1038">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="290af-1039">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1039">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1040">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1040">Profile</span></span>

* <span data-ttu-id="290af-1041">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1041">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="290af-1042">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1042">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-1043">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-1043">RDBMS</span></span>

* <span data-ttu-id="290af-1044">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1044">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="290af-1045">Service Bus</span><span class="sxs-lookup"><span data-stu-id="290af-1045">Service Bus</span></span>

* <span data-ttu-id="290af-1046">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1046">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1047">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1047">Storage</span></span>

* <span data-ttu-id="290af-1048">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1048">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="290af-1049">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1049">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1050">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1050">VM</span></span>

* <span data-ttu-id="290af-1051">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1051">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="290af-1052">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1052">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="290af-1053">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1053">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="290af-1054">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1054">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="290af-1055">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="290af-1055">February 27, 2018</span></span>

<span data-ttu-id="290af-1056">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="290af-1056">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="290af-1057">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1057">Core</span></span>

* <span data-ttu-id="290af-1058">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1058">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="290af-1059">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1059">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="290af-1060">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1060">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1061">ACS</span></span>

* <span data-ttu-id="290af-1062">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1062">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="290af-1063">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1063">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="290af-1064">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1064">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="290af-1065">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="290af-1065">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1066">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1066">Appservice</span></span>

* <span data-ttu-id="290af-1067">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="290af-1067">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="290af-1068">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1068">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="290af-1069">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="290af-1069">Cognitive Services</span></span>

* <span data-ttu-id="290af-1070">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-1070">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="290af-1071">Consumption</span><span class="sxs-lookup"><span data-stu-id="290af-1071">Consumption</span></span>

* <span data-ttu-id="290af-1072">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1072">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="290af-1073">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-1073">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="290af-1074">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1074">Container</span></span>

* <span data-ttu-id="290af-1075">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1075">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="290af-1076">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1076">Network</span></span>

* <span data-ttu-id="290af-1077">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1077">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1078">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1078">Resource</span></span>

* <span data-ttu-id="290af-1079">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1079">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="290af-1080">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1080">Role</span></span>

* <span data-ttu-id="290af-1081">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1081">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1082">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1082">SQL</span></span>

* <span data-ttu-id="290af-1083">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1083">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1084">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1084">Storage</span></span>

* <span data-ttu-id="290af-1085">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="290af-1085">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1086">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1086">VM</span></span>

* <span data-ttu-id="290af-1087">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1087">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="290af-1088">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="290af-1088">February 13, 2018</span></span>

<span data-ttu-id="290af-1089">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="290af-1089">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="290af-1090">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1090">Core</span></span>

* <span data-ttu-id="290af-1091">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1091">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1092">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1092">ACS</span></span>

* <span data-ttu-id="290af-1093">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1093">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="290af-1094">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1094">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="290af-1095">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1095">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="290af-1096">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="290af-1096">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="290af-1097">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1097">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="290af-1098">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="290af-1098">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="290af-1099">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1099">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="290af-1100">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1100">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1101">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1101">Appservice</span></span>

* <span data-ttu-id="290af-1102">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1102">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="290af-1103">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1103">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="290af-1104">CDN</span><span class="sxs-lookup"><span data-stu-id="290af-1104">CDN</span></span>

* <span data-ttu-id="290af-1105">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1105">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="290af-1106">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1106">Container</span></span>

* <span data-ttu-id="290af-1107">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1107">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="290af-1108">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1108">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="290af-1109">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="290af-1109">CosmosDB</span></span>

* <span data-ttu-id="290af-1110">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1110">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="290af-1111">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-1111">Extension</span></span>

* <span data-ttu-id="290af-1112">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1112">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="290af-1113">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1113">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="290af-1114">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="290af-1114">Feedback</span></span>

* <span data-ttu-id="290af-1115">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1115">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-1116">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-1116">Interactive</span></span>

* <span data-ttu-id="290af-1117">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1117">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="290af-1118">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1118">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="290af-1119">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-1119">IoT</span></span>

* <span data-ttu-id="290af-1120">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1120">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="290af-1121">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1121">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="290af-1122">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1122">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="290af-1123">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1123">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1124">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1124">Monitor</span></span>

* <span data-ttu-id="290af-1125">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1125">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="290af-1126">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1126">Network</span></span>

* <span data-ttu-id="290af-1127">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1127">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="290af-1128">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1128">Profile</span></span>

* <span data-ttu-id="290af-1129">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1129">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1130">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1130">Resource</span></span>

* <span data-ttu-id="290af-1131">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1131">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="290af-1132">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1132">Role</span></span>

* <span data-ttu-id="290af-1133">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1133">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1134">SQL</span></span>

* <span data-ttu-id="290af-1135">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1135">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="290af-1136">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1136">Added `sql db rename`</span></span>
* <span data-ttu-id="290af-1137">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1137">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1138">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1138">Storage</span></span>

* <span data-ttu-id="290af-1139">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1139">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1140">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1140">VM</span></span>

* <span data-ttu-id="290af-1141">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1141">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="290af-1142">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1142">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="290af-1143">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="290af-1143">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="290af-1144">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="290af-1144">January 31, 2018</span></span>

<span data-ttu-id="290af-1145">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="290af-1145">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="290af-1146">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1146">Core</span></span>

* <span data-ttu-id="290af-1147">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1147">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="290af-1148">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="290af-1148">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="290af-1149">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1149">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="290af-1150">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="290af-1150">Use `--verbose` to see</span></span>
* <span data-ttu-id="290af-1151">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1151">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1152">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1152">ACS</span></span>

* <span data-ttu-id="290af-1153">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1153">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="290af-1154">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="290af-1154">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1155">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1155">Appservice</span></span>

* <span data-ttu-id="290af-1156">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="290af-1156">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="290af-1157">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="290af-1157">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="290af-1158">CDN</span><span class="sxs-lookup"><span data-stu-id="290af-1158">CDN</span></span>

* <span data-ttu-id="290af-1159">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1159">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="290af-1160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="290af-1160">CosmosDB</span></span>

* <span data-ttu-id="290af-1161">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1161">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-1162">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-1162">Interactive</span></span>

* <span data-ttu-id="290af-1163">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1163">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="290af-1164">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1164">Network</span></span>

* <span data-ttu-id="290af-1165">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1165">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="290af-1166">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1166">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="290af-1167">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1167">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="290af-1168">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1168">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="290af-1169">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1169">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="290af-1170">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="290af-1170">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="290af-1171">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1171">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="290af-1172">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1172">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="290af-1173">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1173">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="290af-1174">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="290af-1174">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1175">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1175">Profile</span></span>

* <span data-ttu-id="290af-1176">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1176">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1177">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1177">Resource</span></span>

* <span data-ttu-id="290af-1178">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1178">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1179">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1179">Storage</span></span>

* <span data-ttu-id="290af-1180">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1180">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="290af-1181">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1181">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="290af-1182">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1182">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="290af-1183">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1183">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="290af-1184">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1184">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1185">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1185">VM</span></span>

* <span data-ttu-id="290af-1186">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1186">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="290af-1187">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1187">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="290af-1188">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1188">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="290af-1189">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1189">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="290af-1190">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="290af-1190">January 17, 2018</span></span>

<span data-ttu-id="290af-1191">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="290af-1191">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="290af-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-1192">ACR</span></span>

* <span data-ttu-id="290af-1193">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1193">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="290af-1194">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1194">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1195">ACS</span></span>

* <span data-ttu-id="290af-1196">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1196">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="290af-1197">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1197">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1198">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1198">Appservice</span></span>

* <span data-ttu-id="290af-1199">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1199">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="290af-1200">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1200">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="290af-1201">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1201">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="290af-1202">Backup</span><span class="sxs-lookup"><span data-stu-id="290af-1202">Backup</span></span>

* <span data-ttu-id="290af-1203">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1203">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="290af-1204">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1204">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="290af-1205">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1205">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="290af-1206">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1206">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="290af-1207">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1207">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="290af-1208">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-1208">Batch</span></span>

* <span data-ttu-id="290af-1209">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1209">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="290af-1210">클라우드</span><span class="sxs-lookup"><span data-stu-id="290af-1210">Cloud</span></span>

* <span data-ttu-id="290af-1211">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1211">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="290af-1212">Consumption</span><span class="sxs-lookup"><span data-stu-id="290af-1212">Consumption</span></span>

* <span data-ttu-id="290af-1213">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1213">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="290af-1214">Event Grid</span><span class="sxs-lookup"><span data-stu-id="290af-1214">Event Grid</span></span>

* <span data-ttu-id="290af-1215">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="290af-1215">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="290af-1216">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="290af-1216">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="290af-1217">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1217">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="290af-1218">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="290af-1218">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="290af-1219">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1219">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="290af-1220">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1220">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="290af-1221">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1221">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="290af-1222">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1222">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-1223">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-1223">Interactive</span></span>

* <span data-ttu-id="290af-1224">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1224">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="290af-1225">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1225">Fixed errors on startup</span></span>
* <span data-ttu-id="290af-1226">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1226">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="290af-1227">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-1227">IoT</span></span>

* <span data-ttu-id="290af-1228">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1228">Added support for device provisioning service</span></span>
* <span data-ttu-id="290af-1229">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1229">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="290af-1230">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1230">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1231">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1231">Monitor</span></span>

* <span data-ttu-id="290af-1232">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1232">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="290af-1233">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="290af-1233">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="290af-1234">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1234">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="290af-1235">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1235">Network</span></span>

* <span data-ttu-id="290af-1236">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1236">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="290af-1237">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1237">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1238">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1238">Profile</span></span>

* <span data-ttu-id="290af-1239">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1239">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="290af-1240">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1240">Role</span></span>

* <span data-ttu-id="290af-1241">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1241">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="290af-1242">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="290af-1242">Service Fabric</span></span>

* <span data-ttu-id="290af-1243">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1243">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="290af-1244">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1244">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1245">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1245">VM</span></span>

* <span data-ttu-id="290af-1246">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1246">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="290af-1247">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1247">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="290af-1248">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1248">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="290af-1249">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1249">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="290af-1250">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1250">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="290af-1251">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1251">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="290af-1252">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1252">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="290af-1253">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1253">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="290af-1254">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="290af-1254">December 19, 2017</span></span>

<span data-ttu-id="290af-1255">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="290af-1255">Version 2.0.23</span></span>

* <span data-ttu-id="290af-1256">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1256">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="290af-1257">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1257">Container</span></span>

* <span data-ttu-id="290af-1258">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1258">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="290af-1259">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1259">Network</span></span>

* <span data-ttu-id="290af-1260">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1260">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="290af-1261">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1261">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1262">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1262">Storage</span></span>

* <span data-ttu-id="290af-1263">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1263">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1264">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1264">VM</span></span>

* <span data-ttu-id="290af-1265">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1265">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="290af-1266">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="290af-1266">December 5, 2017</span></span>

<span data-ttu-id="290af-1267">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="290af-1267">Version 2.0.22</span></span>

* <span data-ttu-id="290af-1268">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1268">Removed `az component` commands.</span></span> <span data-ttu-id="290af-1269">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="290af-1269">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="290af-1270">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1270">Core</span></span>
* <span data-ttu-id="290af-1271">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1271">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="290af-1272">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1272">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1273">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1273">ACS</span></span>

* <span data-ttu-id="290af-1274">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1274">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="290af-1275">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-1275">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="290af-1276">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1276">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="290af-1277">Advisor</span><span class="sxs-lookup"><span data-stu-id="290af-1277">Advisor</span></span>

* <span data-ttu-id="290af-1278">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1278">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1279">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1279">Appservice</span></span>

* <span data-ttu-id="290af-1280">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1280">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="290af-1281">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1281">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="290af-1282">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1282">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="290af-1283">Consumption</span><span class="sxs-lookup"><span data-stu-id="290af-1283">Consumption</span></span>

* <span data-ttu-id="290af-1284">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1284">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="290af-1285">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1285">Container</span></span>

* <span data-ttu-id="290af-1286">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1286">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1287">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1287">Monitor</span></span>

* <span data-ttu-id="290af-1288">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1288">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1289">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1289">Resource</span></span>

* <span data-ttu-id="290af-1290">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1290">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="290af-1291">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1291">Role</span></span>

* <span data-ttu-id="290af-1292">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1292">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="290af-1293">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1293">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="290af-1294">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="290af-1294">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1295">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1295">SQL</span></span>

* <span data-ttu-id="290af-1296">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1296">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="290af-1297">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1297">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1298">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1298">VM</span></span>

* <span data-ttu-id="290af-1299">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1299">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="290af-1300">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="290af-1300">November 14, 2017</span></span>

<span data-ttu-id="290af-1301">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="290af-1301">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="290af-1302">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-1302">ACR</span></span>

* <span data-ttu-id="290af-1303">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1303">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="290af-1304">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1304">ACS</span></span>

* <span data-ttu-id="290af-1305">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1305">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="290af-1306">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="290af-1306">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="290af-1307">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1307">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="290af-1308">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1308">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="290af-1309">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1309">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1310">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1310">Appservice</span></span>

* <span data-ttu-id="290af-1311">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1311">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="290af-1312">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1312">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="290af-1313">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1313">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="290af-1314">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1314">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="290af-1315">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1315">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="290af-1316">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="290af-1316">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="290af-1317">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-1317">Batch</span></span>

* <span data-ttu-id="290af-1318">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1318">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="290af-1319">Batchai</span><span class="sxs-lookup"><span data-stu-id="290af-1319">Batchai</span></span>

* <span data-ttu-id="290af-1320">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1320">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="290af-1321">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1321">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="290af-1322">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1322">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="290af-1323">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1323">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="290af-1324">클라우드</span><span class="sxs-lookup"><span data-stu-id="290af-1324">Cloud</span></span>

* <span data-ttu-id="290af-1325">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1325">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="290af-1326">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1326">Container</span></span>

* <span data-ttu-id="290af-1327">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1327">Added support to open multiple ports</span></span>
* <span data-ttu-id="290af-1328">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1328">Added container group restart policy</span></span>
* <span data-ttu-id="290af-1329">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1329">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="290af-1330">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="290af-1330">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="290af-1331">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="290af-1331">Data Lake Analytics</span></span>

* <span data-ttu-id="290af-1332">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1332">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="290af-1333">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="290af-1333">Data Lake Store</span></span>

* <span data-ttu-id="290af-1334">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1334">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="290af-1335">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-1335">Extension</span></span>

* <span data-ttu-id="290af-1336">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1336">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="290af-1337">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1337">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="290af-1338">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-1338">IoT</span></span>

* <span data-ttu-id="290af-1339">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1339">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1340">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1340">Monitor</span></span>

* <span data-ttu-id="290af-1341">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1341">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="290af-1342">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1342">Network</span></span>

* <span data-ttu-id="290af-1343">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1343">Added support for CAA DNS records</span></span>
* <span data-ttu-id="290af-1344">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1344">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="290af-1345">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1345">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="290af-1346">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1346">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="290af-1347">예약</span><span class="sxs-lookup"><span data-stu-id="290af-1347">Reservations</span></span>

* <span data-ttu-id="290af-1348">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1348">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1349">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1349">Resource</span></span>

* <span data-ttu-id="290af-1350">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1350">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1351">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1351">SQL</span></span>

* <span data-ttu-id="290af-1352">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1352">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1353">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1353">Storage</span></span>

* <span data-ttu-id="290af-1354">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1354">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="290af-1355">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1355">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="290af-1356">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1356">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="290af-1357">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="290af-1357">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="290af-1358">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1358">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="290af-1359">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1359">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="290af-1360">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1360">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1361">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1361">VM</span></span>

* <span data-ttu-id="290af-1362">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1362">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="290af-1363">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1363">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="290af-1364">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1364">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="290af-1365">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1365">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="290af-1366">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1366">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="290af-1367">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="290af-1367">October 24, 2017</span></span>

<span data-ttu-id="290af-1368">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="290af-1368">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="290af-1369">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1369">Core</span></span>

* <span data-ttu-id="290af-1370">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="290af-1370">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="290af-1371">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-1371">ACR</span></span>

* <span data-ttu-id="290af-1372">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="290af-1372">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="290af-1373">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-1373">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="290af-1374">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="290af-1374">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1375">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1375">ACS</span></span>

* <span data-ttu-id="290af-1376">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1376">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="290af-1377">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1377">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1378">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1378">Appservice</span></span>

* <span data-ttu-id="290af-1379">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1379">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="290af-1380">구성 요소</span><span class="sxs-lookup"><span data-stu-id="290af-1380">Component</span></span>

* <span data-ttu-id="290af-1381">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1381">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1382">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1382">Monitor</span></span>

* <span data-ttu-id="290af-1383">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1383">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1384">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1384">Resource</span></span>

* <span data-ttu-id="290af-1385">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1385">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="290af-1386">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1386">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1387">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1387">VM</span></span>

* <span data-ttu-id="290af-1388">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1388">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="290af-1389">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="290af-1389">October 9, 2017</span></span>

<span data-ttu-id="290af-1390">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="290af-1390">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="290af-1391">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1391">Core</span></span>

* <span data-ttu-id="290af-1392">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1392">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1393">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1393">Appservice</span></span>

* <span data-ttu-id="290af-1394">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1394">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="290af-1395">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-1395">Batch</span></span>

* <span data-ttu-id="290af-1396">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1396">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="290af-1397">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1397">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="290af-1398">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1398">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="290af-1399">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1399">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="290af-1400">Batchai</span><span class="sxs-lookup"><span data-stu-id="290af-1400">Batchai</span></span>

* <span data-ttu-id="290af-1401">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1401">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-1402">Keyvault</span><span class="sxs-lookup"><span data-stu-id="290af-1402">Keyvault</span></span>

* <span data-ttu-id="290af-1403">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1403">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="290af-1404">(#4448)</span><span class="sxs-lookup"><span data-stu-id="290af-1404">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="290af-1405">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1405">Network</span></span>

* <span data-ttu-id="290af-1406">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1406">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="290af-1407">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1407">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1408">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1408">Resource</span></span>

* <span data-ttu-id="290af-1409">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1409">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="290af-1410">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1410">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="290af-1411">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1411">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="290af-1412">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1412">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1413">Sql</span><span class="sxs-lookup"><span data-stu-id="290af-1413">Sql</span></span>

* <span data-ttu-id="290af-1414">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1414">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="290af-1415">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1415">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="290af-1416">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1416">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1417">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1417">Storage</span></span>

* <span data-ttu-id="290af-1418">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1418">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1419">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1419">Vm</span></span>

* <span data-ttu-id="290af-1420">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1420">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="290af-1421">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1421">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="290af-1422">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1422">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="290af-1423">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1423">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="290af-1424">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1424">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="290af-1425">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="290af-1425">September 22, 2017</span></span>

<span data-ttu-id="290af-1426">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="290af-1426">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1427">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1427">Resource</span></span>

* <span data-ttu-id="290af-1428">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1428">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="290af-1429">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1429">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="290af-1430">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1430">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="290af-1431">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1431">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="290af-1432">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1432">Network</span></span>

* <span data-ttu-id="290af-1433">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1433">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="290af-1434">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1434">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="290af-1435">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1435">Added `asg` application security group commands</span></span>
* <span data-ttu-id="290af-1436">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1436">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="290af-1437">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1437">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="290af-1438">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1438">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="290af-1439">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1439">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1440">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1440">Storage</span></span>

* <span data-ttu-id="290af-1441">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1441">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="290af-1442">Event Grid</span><span class="sxs-lookup"><span data-stu-id="290af-1442">Eventgrid</span></span>

* <span data-ttu-id="290af-1443">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="290af-1443">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1444">SQL</span></span>

* <span data-ttu-id="290af-1445">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1445">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="290af-1446">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="290af-1446">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="290af-1447">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1447">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-1448">Keyvault</span><span class="sxs-lookup"><span data-stu-id="290af-1448">Keyvault</span></span>

* <span data-ttu-id="290af-1449">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1449">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1450">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1450">VM</span></span>

* <span data-ttu-id="290af-1451">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1451">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="290af-1452">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="290af-1452">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="290af-1453">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1453">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="290af-1454">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1454">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="290af-1455">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1455">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="290af-1456">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1456">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1457">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1457">ACS</span></span>

* <span data-ttu-id="290af-1458">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1458">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1459">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1459">Appservice</span></span>

* <span data-ttu-id="290af-1460">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1460">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="290af-1461">Backup</span><span class="sxs-lookup"><span data-stu-id="290af-1461">Backup</span></span>

* <span data-ttu-id="290af-1462">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1462">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="290af-1463">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="290af-1463">September 11, 2017</span></span>

<span data-ttu-id="290af-1464">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="290af-1464">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="290af-1465">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1465">Core</span></span>

* <span data-ttu-id="290af-1466">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1466">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="290af-1467">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1467">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1468">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1468">Acs</span></span>

* <span data-ttu-id="290af-1469">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1469">Added `acs list-locations` command</span></span>
* <span data-ttu-id="290af-1470">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="290af-1470">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1471">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1471">Appservice</span></span>

* <span data-ttu-id="290af-1472">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1472">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="290af-1473">CDN</span><span class="sxs-lookup"><span data-stu-id="290af-1473">CDN</span></span>

* <span data-ttu-id="290af-1474">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1474">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="290af-1475">내선 번호</span><span class="sxs-lookup"><span data-stu-id="290af-1475">Extension</span></span>

* <span data-ttu-id="290af-1476">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1476">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-1477">Keyvault</span><span class="sxs-lookup"><span data-stu-id="290af-1477">Keyvault</span></span>

* <span data-ttu-id="290af-1478">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1478">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="290af-1479">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1479">Network</span></span>

* <span data-ttu-id="290af-1480">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1480">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="290af-1481">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1481">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="290af-1482">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1482">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="290af-1483">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1483">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="290af-1484">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1484">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1485">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1485">Resource</span></span>

* <span data-ttu-id="290af-1486">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-1486">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="290af-1487">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-1487">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="290af-1488">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="290af-1488">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="290af-1489">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="290af-1489">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1490">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1490">SQL</span></span>

* <span data-ttu-id="290af-1491">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1491">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1492">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1492">VM</span></span>

* <span data-ttu-id="290af-1493">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1493">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="290af-1494">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="290af-1494">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="290af-1495">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1495">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="290af-1496">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1496">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="290af-1497">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1497">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="290af-1498">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="290af-1498">August 31, 2017</span></span>

<span data-ttu-id="290af-1499">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="290af-1499">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-1500">Keyvault</span><span class="sxs-lookup"><span data-stu-id="290af-1500">Keyvault</span></span>

* <span data-ttu-id="290af-1501">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1501">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="290af-1502">Sf</span><span class="sxs-lookup"><span data-stu-id="290af-1502">Sf</span></span>

* <span data-ttu-id="290af-1503">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1503">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1504">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1504">Storage</span></span>

* <span data-ttu-id="290af-1505">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1505">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="290af-1506">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="290af-1506">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="290af-1507">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="290af-1507">August 28, 2017</span></span>

<span data-ttu-id="290af-1508">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="290af-1508">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="290af-1509">CLI</span><span class="sxs-lookup"><span data-stu-id="290af-1509">CLI</span></span>

* <span data-ttu-id="290af-1510">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1510">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1511">ACS</span></span>

* <span data-ttu-id="290af-1512">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1512">Corrected preview regions</span></span>
* <span data-ttu-id="290af-1513">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1513">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="290af-1514">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="290af-1514">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1515">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1515">Appservice</span></span>

* <span data-ttu-id="290af-1516">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1516">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="290af-1517">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1517">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="290af-1518">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1518">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="290af-1519">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1519">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="290af-1520">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1520">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="290af-1521">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-1521">IoT</span></span>

* <span data-ttu-id="290af-1522">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1522">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="290af-1523">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1523">Network</span></span>

* <span data-ttu-id="290af-1524">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1524">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="290af-1525">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1525">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="290af-1526">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1526">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="290af-1527">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1527">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="290af-1528">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1528">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1529">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1529">Profile</span></span>

* <span data-ttu-id="290af-1530">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1530">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="290af-1531">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="290af-1531">Service Fabric</span></span>

* <span data-ttu-id="290af-1532">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1532">Preview release</span></span>
* <span data-ttu-id="290af-1533">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="290af-1533">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="290af-1534">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1534">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="290af-1535">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1535">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1536">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1536">Storage</span></span>

* <span data-ttu-id="290af-1537">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1537">Enabled setting blob tier</span></span>
* <span data-ttu-id="290af-1538">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1538">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="290af-1539">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1539">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="290af-1540">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1540">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="290af-1541">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1541">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="290af-1542">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1542">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1543">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1543">VM</span></span>

* <span data-ttu-id="290af-1544">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1544">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="290af-1545">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1545">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="290af-1546">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1546">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="290af-1547">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1547">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="290af-1548">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1548">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="290af-1549">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1549">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="290af-1550">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="290af-1550">August 15, 2017</span></span>

<span data-ttu-id="290af-1551">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="290af-1551">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1552">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1552">ACS</span></span>

* <span data-ttu-id="290af-1553">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1553">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1554">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1554">Appservice</span></span>

* <span data-ttu-id="290af-1555">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1555">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="290af-1556">Event Grid</span><span class="sxs-lookup"><span data-stu-id="290af-1556">Event Grid</span></span>

* <span data-ttu-id="290af-1557">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1557">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="290af-1558">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="290af-1558">August 11, 2017</span></span>

<span data-ttu-id="290af-1559">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="290af-1559">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1560">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1560">ACS</span></span>

* <span data-ttu-id="290af-1561">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1561">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="290af-1562">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-1562">Batch</span></span>

* <span data-ttu-id="290af-1563">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1563">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="290af-1564">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1564">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="290af-1565">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1565">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="290af-1566">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1566">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="290af-1567">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1567">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="290af-1568">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1568">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="290af-1569">구성 요소</span><span class="sxs-lookup"><span data-stu-id="290af-1569">Component</span></span>

* <span data-ttu-id="290af-1570">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1570">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="290af-1571">컨테이너</span><span class="sxs-lookup"><span data-stu-id="290af-1571">Container</span></span>

* <span data-ttu-id="290af-1572">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1572">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="290af-1573">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="290af-1573">Data Lake Store</span></span>

* <span data-ttu-id="290af-1574">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1574">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="290af-1575">Event Grid</span><span class="sxs-lookup"><span data-stu-id="290af-1575">Event Grid</span></span>

* <span data-ttu-id="290af-1576">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1576">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="290af-1577">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1577">Network</span></span>

* <span data-ttu-id="290af-1578">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1578">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="290af-1579">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1579">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="290af-1580">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1580">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="290af-1581">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1581">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1582">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1582">Profile</span></span>

* <span data-ttu-id="290af-1583">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1583">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1584">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1584">Storage</span></span>

* <span data-ttu-id="290af-1585">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1585">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1586">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1586">VM</span></span>

* <span data-ttu-id="290af-1587">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1587">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="290af-1588">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1588">Exposed `list-skus` command</span></span>
* <span data-ttu-id="290af-1589">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1589">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="290af-1590">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1590">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="290af-1591">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1591">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="290af-1592">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="290af-1592">July 28, 2017</span></span>

<span data-ttu-id="290af-1593">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="290af-1593">Version 2.0.12</span></span>

* <span data-ttu-id="290af-1594">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1594">Added container commands</span></span>
* <span data-ttu-id="290af-1595">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1595">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="290af-1596">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1596">Core</span></span>

* <span data-ttu-id="290af-1597">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="290af-1597">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="290af-1598">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="290af-1598">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="290af-1599">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="290af-1599">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="290af-1600">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="290af-1600">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="290af-1601">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="290af-1601">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="290af-1602">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="290af-1602">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="290af-1603">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="290af-1603">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="290af-1604">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="290af-1604">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="290af-1605">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="290af-1605">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="290af-1606">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="290af-1606">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="290af-1607">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="290af-1607">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="290af-1608">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="290af-1608">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="290af-1609">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1609">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="290af-1610">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1610">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="290af-1611">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1611">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="290af-1612">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="290af-1612">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="290af-1613">ACR</span><span class="sxs-lookup"><span data-stu-id="290af-1613">ACR</span></span>

* <span data-ttu-id="290af-1614">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1614">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="290af-1615">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1615">Support SKU update for managed registries</span></span>
* <span data-ttu-id="290af-1616">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1616">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="290af-1617">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1617">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="290af-1618">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1618">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="290af-1619">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1619">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1620">ACS</span></span>

* <span data-ttu-id="290af-1621">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1621">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1622">App Service</span><span class="sxs-lookup"><span data-stu-id="290af-1622">Appservice</span></span>

* <span data-ttu-id="290af-1623">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1623">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="290af-1624">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1624">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="290af-1625">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1625">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="290af-1626">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="290af-1626">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="290af-1627">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="290af-1627">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="290af-1628">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="290af-1628">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="290af-1629">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="290af-1629">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="290af-1630">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="290af-1630">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="290af-1631">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1631">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="290af-1632">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1632">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="290af-1633">Batch</span><span class="sxs-lookup"><span data-stu-id="290af-1633">Batch</span></span>

* <span data-ttu-id="290af-1634">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1634">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="290af-1635">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1635">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="290af-1636">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1636">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="290af-1637">CDN</span><span class="sxs-lookup"><span data-stu-id="290af-1637">CDN</span></span>

* <span data-ttu-id="290af-1638">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="290af-1638">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="290af-1639">클라우드</span><span class="sxs-lookup"><span data-stu-id="290af-1639">Cloud</span></span>

* <span data-ttu-id="290af-1640">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1640">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="290af-1641">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1641">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="290af-1642">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1642">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="290af-1643">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="290af-1643">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="290af-1644">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="290af-1644">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="290af-1645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="290af-1645">CosmosDB</span></span>

* <span data-ttu-id="290af-1646">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1646">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="290af-1647">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1647">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="290af-1648">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="290af-1648">Data Lake Analytics</span></span>

* <span data-ttu-id="290af-1649">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1649">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="290af-1650">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1650">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="290af-1651">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1651">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="290af-1652">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="290af-1652">Data Lake Store</span></span>

* <span data-ttu-id="290af-1653">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1653">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="290af-1654">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1654">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="290af-1655">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1655">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="290af-1656">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="290af-1656">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="290af-1657">대화형</span><span class="sxs-lookup"><span data-stu-id="290af-1657">Interactive</span></span>

* <span data-ttu-id="290af-1658">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1658">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="290af-1659">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1659">Increased test coverage</span></span>
* <span data-ttu-id="290af-1660">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1660">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="290af-1661">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="290af-1661">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="290af-1662">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="290af-1662">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="290af-1663">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="290af-1663">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="290af-1664">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="290af-1664">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="290af-1665">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1665">Added `--progress` flag</span></span>
* <span data-ttu-id="290af-1666">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1666">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="290af-1667">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="290af-1667">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="290af-1668">IoT</span><span class="sxs-lookup"><span data-stu-id="290af-1668">IoT</span></span>

* <span data-ttu-id="290af-1669">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1669">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="290af-1670">(#3934)</span><span class="sxs-lookup"><span data-stu-id="290af-1670">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="290af-1671">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="290af-1671">Key vault</span></span>

* <span data-ttu-id="290af-1672">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="290af-1672">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="290af-1673">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="290af-1673">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="290af-1674">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="290af-1674">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="290af-1675">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="290af-1675">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="290af-1676">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="290af-1676">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="290af-1677">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="290af-1677">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="290af-1678">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="290af-1678">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="290af-1679">(#3307)</span><span class="sxs-lookup"><span data-stu-id="290af-1679">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="290af-1680">랩</span><span class="sxs-lookup"><span data-stu-id="290af-1680">Lab</span></span>

* <span data-ttu-id="290af-1681">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1681">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="290af-1682">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1682">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1683">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1683">Monitor</span></span>

* <span data-ttu-id="290af-1684">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="290af-1684">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="290af-1685">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1685">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="290af-1686">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1686">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="290af-1687">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1687">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="290af-1688">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="290af-1688">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="290af-1689">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="290af-1689">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="290af-1690">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1690">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="290af-1691">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1691">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="290af-1692">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1692">`location` no longer required</span></span>
  * <span data-ttu-id="290af-1693">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1693">Add name and ID support for target</span></span>
  * <span data-ttu-id="290af-1694">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1694">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="290af-1695">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1695">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="290af-1696">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1696">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="290af-1697">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1697">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="290af-1698">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1698">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="290af-1699">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1699">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="290af-1700">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1700">Network</span></span>

* <span data-ttu-id="290af-1701">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1701">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="290af-1702">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1702">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="290af-1703">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1703">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="290af-1704">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1704">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="290af-1705">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1705">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="290af-1706">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1706">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="290af-1707">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="290af-1707">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="290af-1708">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="290af-1708">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="290af-1709">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="290af-1709">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="290af-1710">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="290af-1710">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="290af-1711">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="290af-1711">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="290af-1712">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="290af-1712">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="290af-1713">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="290af-1713">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="290af-1714">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="290af-1714">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="290af-1715">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1715">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="290af-1716">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1716">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="290af-1717">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1717">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="290af-1718">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1718">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="290af-1719">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1719">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="290af-1720">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1720">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="290af-1721">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1721">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="290af-1722">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1722">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="290af-1723">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1723">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="290af-1724">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1724">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="290af-1725">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1725">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="290af-1726">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1726">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="290af-1727">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="290af-1727">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1728">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1728">Profile</span></span>

* <span data-ttu-id="290af-1729">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1729">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="290af-1730">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1730">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="290af-1731">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="290af-1731">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="290af-1732">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1732">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="290af-1733">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1733">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="290af-1734">RDBMS</span><span class="sxs-lookup"><span data-stu-id="290af-1734">RDBMS</span></span>

* <span data-ttu-id="290af-1735">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="290af-1735">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="290af-1736">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="290af-1736">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="290af-1737">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="290af-1737">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="290af-1738">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="290af-1738">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1739">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1739">Resource</span></span>

* <span data-ttu-id="290af-1740">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1740">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="290af-1741">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="290af-1741">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="290af-1742">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1742">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="290af-1743">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1743">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="290af-1744">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="290af-1744">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="290af-1745">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1745">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="290af-1746">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="290af-1746">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="290af-1747">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1747">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="290af-1748">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1748">Role</span></span>

* <span data-ttu-id="290af-1749">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1749">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="290af-1750">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="290af-1750">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="290af-1751">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="290af-1751">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="290af-1752">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="290af-1752">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="290af-1753">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1753">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="290af-1754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="290af-1754">Service Fabric</span></span>
* <span data-ttu-id="290af-1755">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="290af-1755">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="290af-1756">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="290af-1756">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="290af-1757">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="290af-1757">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1758">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1758">SQL</span></span>

* <span data-ttu-id="290af-1759">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1759">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="290af-1760">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="290af-1760">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="290af-1761">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1761">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1762">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1762">Storage</span></span>

* <span data-ttu-id="290af-1763">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="290af-1763">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="290af-1764">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="290af-1764">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="290af-1765">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="290af-1765">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="290af-1766">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1766">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="290af-1767">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="290af-1767">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="290af-1768">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="290af-1768">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1769">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1769">VM</span></span>

* <span data-ttu-id="290af-1770">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1770">Support configuring nsg</span></span>
* <span data-ttu-id="290af-1771">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1771">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="290af-1772">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="290af-1772">Support managed service identities</span></span>
* <span data-ttu-id="290af-1773">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="290af-1773">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="290af-1774">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="290af-1774">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="290af-1775">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="290af-1775">May 10, 2017</span></span>

<span data-ttu-id="290af-1776">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="290af-1776">Version 2.0.6</span></span>

* <span data-ttu-id="290af-1777">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="290af-1777">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="290af-1778">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1778">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="290af-1779">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="290af-1779">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="290af-1780">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="290af-1780">Include Cognitive Services module</span></span>
* <span data-ttu-id="290af-1781">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="290af-1781">Include Service Fabric module</span></span>
* <span data-ttu-id="290af-1782">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="290af-1782">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="290af-1783">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1783">Add support for CDN commands</span></span>
* <span data-ttu-id="290af-1784">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="290af-1784">Remove Container module</span></span>
* <span data-ttu-id="290af-1785">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="290af-1785">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="290af-1786">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="290af-1786">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="290af-1787">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1787">Core</span></span>

* <span data-ttu-id="290af-1788">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="290af-1788">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="290af-1789">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="290af-1789">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="290af-1790">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="290af-1790">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="290af-1791">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="290af-1791">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="290af-1792">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="290af-1792">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="290af-1793">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="290af-1793">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="290af-1794">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="290af-1794">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="290af-1795">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="290af-1795">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="290af-1796">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="290af-1796">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="290af-1797">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="290af-1797">core: Improved performance</span></span>
* <span data-ttu-id="290af-1798">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1798">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="290af-1799">core: 클라우드 구성 - '관리' 엔드포인트를 설정하지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="290af-1799">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1800">ACS</span></span>

* <span data-ttu-id="290af-1801">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1801">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="290af-1802">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="290af-1802">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="290af-1803">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="290af-1803">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="290af-1804">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="290af-1804">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-1805">AppService</span></span>

* <span data-ttu-id="290af-1806">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="290af-1806">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="290af-1807">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1807">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="290af-1808">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="290af-1808">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="290af-1809">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="290af-1809">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="290af-1810">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="290af-1810">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="290af-1811">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="290af-1811">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="290af-1812">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1812">support slot swap with preview</span></span>
* <span data-ttu-id="290af-1813">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="290af-1813">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="290af-1814">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="290af-1814">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="290af-1815">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="290af-1815">CosmosDB</span></span>

* <span data-ttu-id="290af-1816">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="290af-1816">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="290af-1817">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1817">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="290af-1818">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1818">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="290af-1819">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1819">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="290af-1820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="290af-1820">Data Lake Analytics</span></span>

* <span data-ttu-id="290af-1821">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1821">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="290af-1822">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1822">Add support for new catalog item type: package.</span></span> <span data-ttu-id="290af-1823">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="290af-1823">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="290af-1824">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="290af-1824">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="290af-1825">테이블</span><span class="sxs-lookup"><span data-stu-id="290af-1825">Table</span></span>
  * <span data-ttu-id="290af-1826">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="290af-1826">Table valued function</span></span>
  * <span data-ttu-id="290af-1827">보기</span><span class="sxs-lookup"><span data-stu-id="290af-1827">View</span></span>
  * <span data-ttu-id="290af-1828">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="290af-1828">Table Statistics.</span></span> <span data-ttu-id="290af-1829">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="290af-1829">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="290af-1830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="290af-1830">Data Lake Store</span></span>

* <span data-ttu-id="290af-1831">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="290af-1831">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="290af-1832">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="290af-1832">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="290af-1833">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="290af-1833">missed help for access show.</span></span> <span data-ttu-id="290af-1834">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1834">adding it.</span></span> <span data-ttu-id="290af-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="290af-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="290af-1836">찾기</span><span class="sxs-lookup"><span data-stu-id="290af-1836">Find</span></span>

* <span data-ttu-id="290af-1837">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="290af-1837">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="290af-1838">KeyVault</span><span class="sxs-lookup"><span data-stu-id="290af-1838">KeyVault</span></span>

* <span data-ttu-id="290af-1839">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1839">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="290af-1840">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1840">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="290af-1841">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1841">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="290af-1842">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1842">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="290af-1843">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="290af-1843">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="290af-1844">랩</span><span class="sxs-lookup"><span data-stu-id="290af-1844">Lab</span></span>

* <span data-ttu-id="290af-1845">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1845">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="290af-1846">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1846">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="290af-1847">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="290af-1847">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="290af-1848">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="290af-1848">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="290af-1849">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1849">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="290af-1850">모니터</span><span class="sxs-lookup"><span data-stu-id="290af-1850">Monitor</span></span>

* <span data-ttu-id="290af-1851">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="290af-1851">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="290af-1852">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="290af-1852">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="290af-1853">네트워크</span><span class="sxs-lookup"><span data-stu-id="290af-1853">Network</span></span>

* <span data-ttu-id="290af-1854">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1854">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="290af-1855">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1855">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="290af-1856">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1856">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="290af-1857">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1857">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="290af-1858">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1858">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="290af-1859">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1859">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="290af-1860">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1860">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="290af-1861">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1861">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="290af-1862">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1862">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="290af-1863">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1863">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="290af-1864">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="290af-1864">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="290af-1865">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1865">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="290af-1866">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1866">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="290af-1867">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1867">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="290af-1868">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="290af-1868">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="290af-1869">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1869">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="290af-1870">프로필</span><span class="sxs-lookup"><span data-stu-id="290af-1870">Profile</span></span>

* <span data-ttu-id="290af-1871">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="290af-1871">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="290af-1872">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="290af-1872">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="290af-1873">Redis</span><span class="sxs-lookup"><span data-stu-id="290af-1873">Redis</span></span>

* <span data-ttu-id="290af-1874">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1874">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="290af-1875">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="290af-1875">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="290af-1876">리소스</span><span class="sxs-lookup"><span data-stu-id="290af-1876">Resource</span></span>

* <span data-ttu-id="290af-1877">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="290af-1877">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="290af-1878">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="290af-1878">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="290af-1879">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="290af-1879">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="290af-1880">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1880">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="290af-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="290af-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="290af-1882">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1882">Add docs for az lock update.</span></span> <span data-ttu-id="290af-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="290af-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="290af-1884">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1884">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="290af-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="290af-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="290af-1886">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1886">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="290af-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="290af-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="290af-1888">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="290af-1888">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="290af-1889">역할</span><span class="sxs-lookup"><span data-stu-id="290af-1889">Role</span></span>

* <span data-ttu-id="290af-1890">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="290af-1890">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="290af-1891">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="290af-1891">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="290af-1892">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="290af-1892">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="290af-1893">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="290af-1893">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="290af-1894">SQL</span><span class="sxs-lookup"><span data-stu-id="290af-1894">SQL</span></span>

* <span data-ttu-id="290af-1895">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="290af-1895">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="290af-1896">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="290af-1896">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="290af-1897">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1897">Storage</span></span>

* <span data-ttu-id="290af-1898">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="290af-1898">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="290af-1899">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1899">Add support for incremental blob copy</span></span>
* <span data-ttu-id="290af-1900">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1900">Add support for large block blob upload</span></span>
* <span data-ttu-id="290af-1901">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="290af-1901">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1902">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1902">VM</span></span>

* <span data-ttu-id="290af-1903">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="290af-1903">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="290af-1904">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="290af-1904">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="290af-1905">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="290af-1905">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="290af-1906">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="290af-1906">az vm/vmss disk</span></span>
  3. <span data-ttu-id="290af-1907">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1907">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="290af-1908">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="290af-1908">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="290af-1909">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="290af-1909">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="290af-1910">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="290af-1910">April 3, 2017</span></span>

<span data-ttu-id="290af-1911">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="290af-1911">Version 2.0.2</span></span>

<span data-ttu-id="290af-1912">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1912">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="290af-1913">코어</span><span class="sxs-lookup"><span data-stu-id="290af-1913">Core</span></span>

* <span data-ttu-id="290af-1914">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="290af-1914">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="290af-1915">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="290af-1915">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="290af-1916">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="290af-1916">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="290af-1917">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="290af-1917">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="290af-1918">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="290af-1918">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="290af-1919">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="290af-1919">Add prompting for missing template parameters.</span></span> <span data-ttu-id="290af-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="290af-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="290af-1921">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1921">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="290af-1922">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="290af-1922">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="290af-1923">ACS</span><span class="sxs-lookup"><span data-stu-id="290af-1923">ACS</span></span>

* <span data-ttu-id="290af-1924">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="290af-1924">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="290af-1925">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="290af-1925">Add support for ssh key password prompting.</span></span> <span data-ttu-id="290af-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="290af-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="290af-1927">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="290af-1927">Add support for windows clusters.</span></span> <span data-ttu-id="290af-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="290af-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="290af-1929">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="290af-1929">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="290af-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="290af-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="290af-1931">AppService</span><span class="sxs-lookup"><span data-stu-id="290af-1931">AppService</span></span>

* <span data-ttu-id="290af-1932">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="290af-1932">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="290af-1933">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="290af-1933">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="290af-1934">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="290af-1934">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="290af-1935">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="290af-1935">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="290af-1936">DataLake</span><span class="sxs-lookup"><span data-stu-id="290af-1936">DataLake</span></span>

* <span data-ttu-id="290af-1937">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1937">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="290af-1938">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="290af-1938">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="290af-1939">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="290af-1939">DocuemntDB</span></span>

* <span data-ttu-id="290af-1940">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="290af-1940">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="290af-1941">VM</span><span class="sxs-lookup"><span data-stu-id="290af-1941">VM</span></span>

* <span data-ttu-id="290af-1942">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="290af-1942">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="290af-1943">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="290af-1943">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="290af-1944">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="290af-1944">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="290af-1945">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="290af-1945">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="290af-1946">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="290af-1946">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="290af-1947">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="290af-1947">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="290af-1948">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="290af-1948">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="290af-1949">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="290af-1949">February 27, 2017</span></span>

<span data-ttu-id="290af-1950">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="290af-1950">Version 2.0.0</span></span>

<span data-ttu-id="290af-1951">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1951">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="290af-1952">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="290af-1952">Container Service (acs)</span></span>
- <span data-ttu-id="290af-1953">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="290af-1953">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="290af-1954">네트워킹</span><span class="sxs-lookup"><span data-stu-id="290af-1954">Networking</span></span>
- <span data-ttu-id="290af-1955">Storage</span><span class="sxs-lookup"><span data-stu-id="290af-1955">Storage</span></span>

<span data-ttu-id="290af-1956">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1956">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="290af-1957">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1957">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="290af-1958">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1958">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="290af-1959">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1959">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="290af-1960">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="290af-1960">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="290af-1961">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="290af-1961">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="290af-1962">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="290af-1962">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="290af-1963">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="290af-1963">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="290af-1964">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="290af-1964">Provide feedback from the command line with the `az feedback` command</span></span>


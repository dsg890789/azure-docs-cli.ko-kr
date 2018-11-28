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
ms.openlocfilehash: 36b57d52a5851275fd317240e5c2c95171a99e7e
ms.sourcegitcommit: 22b73d56602c1c4e647ed2c5af3d596a2f6a7ed5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2018
ms.locfileid: "52267333"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="55d74-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="55d74-103">Azure CLI release notes</span></span>
## <a name="november-20-2018"></a><span data-ttu-id="55d74-104">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="55d74-104">November 20, 2018</span></span>

<span data-ttu-id="55d74-105">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="55d74-105">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="55d74-106">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-106">Core</span></span>
* <span data-ttu-id="55d74-107">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-107">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-108">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-108">ACR</span></span>
* <span data-ttu-id="55d74-109">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-109">Added context token to task step</span></span>
* <span data-ttu-id="55d74-110">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-110">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="55d74-111">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="55d74-111">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-112">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-112">Appservice</span></span>
* <span data-ttu-id="55d74-113">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-113">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="55d74-114">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-114">Updated the default `node_version`.</span></span> <span data-ttu-id="55d74-115">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-115">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="55d74-116">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-116">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="55d74-117">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-117">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="55d74-118">IotCentral</span><span class="sxs-lookup"><span data-stu-id="55d74-118">IotCentral</span></span>
* <span data-ttu-id="55d74-119">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-119">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-120">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55d74-120">KeyVault</span></span>
* <span data-ttu-id="55d74-121">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-121">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="55d74-122">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-122">Network</span></span>
* <span data-ttu-id="55d74-123">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-123">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="55d74-124">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="55d74-124">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="55d74-125">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-125">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="55d74-126">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="55d74-126">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="55d74-127">Rdbms</span></span>
* <span data-ttu-id="55d74-128">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-128">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="55d74-129">Rbac</span><span class="sxs-lookup"><span data-stu-id="55d74-129">Rbac</span></span>
* <span data-ttu-id="55d74-130">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-130">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="55d74-131">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-131">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="55d74-132">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-132">Storage</span></span>
* <span data-ttu-id="55d74-133">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-133">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="55d74-134">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-134">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="55d74-135">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-135">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="55d74-136">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-136">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-137">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-137">VM</span></span>
* <span data-ttu-id="55d74-138">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-138">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="55d74-139">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-139">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="55d74-140">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="55d74-140">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="55d74-141">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-141">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="55d74-142">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-142">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="55d74-143">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-143">Added `snapshot wait` command</span></span>
* <span data-ttu-id="55d74-144">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-144">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="55d74-145">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="55d74-145">November 6, 2018</span></span>

<span data-ttu-id="55d74-146">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="55d74-146">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="55d74-147">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-147">Core</span></span>
* <span data-ttu-id="55d74-148">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-148">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-149">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-149">ACR</span></span>
* <span data-ttu-id="55d74-150">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-150">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="55d74-151">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-151">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-152">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-152">ACS</span></span>
* <span data-ttu-id="55d74-153">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-153">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="55d74-154">Advisor</span><span class="sxs-lookup"><span data-stu-id="55d74-154">Advisor</span></span>
* <span data-ttu-id="55d74-155">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-155">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="55d74-156">AMS</span><span class="sxs-lookup"><span data-stu-id="55d74-156">AMS</span></span>
* <span data-ttu-id="55d74-157">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="55d74-157">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="55d74-158">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="55d74-158">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="55d74-159">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-159">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="55d74-160">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="55d74-160">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="55d74-161">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-161">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="55d74-162">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-162">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="55d74-163">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-163">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="55d74-164">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="55d74-164">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="55d74-165">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-165">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="55d74-166">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-166">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="55d74-167">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="55d74-167">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="55d74-168">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="55d74-168">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="55d74-169">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="55d74-169">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="55d74-170">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="55d74-170">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="55d74-171">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-171">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="55d74-172">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-172">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="55d74-173">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-173">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-174">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-174">AppService</span></span>
* <span data-ttu-id="55d74-175">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-175">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="55d74-176">구성</span><span class="sxs-lookup"><span data-stu-id="55d74-176">Configure</span></span>
* <span data-ttu-id="55d74-177">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-177">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="55d74-178">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-178">Container</span></span>
* <span data-ttu-id="55d74-179">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-179">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="55d74-180">EventHub</span><span class="sxs-lookup"><span data-stu-id="55d74-180">EventHub</span></span>
* <span data-ttu-id="55d74-181">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-181">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-182">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-182">Interactive</span></span>
* <span data-ttu-id="55d74-183">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-183">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-184">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-184">Monitor</span></span>
* <span data-ttu-id="55d74-185">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-185">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="55d74-186">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-186">Network</span></span>
* <span data-ttu-id="55d74-187">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-187">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="55d74-188">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-188">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="55d74-189">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-189">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="55d74-190">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-190">Profile</span></span>
* <span data-ttu-id="55d74-191">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-191">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-192">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-192">RDBMS</span></span>
* <span data-ttu-id="55d74-193">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-193">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-194">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-194">Resource</span></span>
* <span data-ttu-id="55d74-195">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-195">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="55d74-196">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-196">Role</span></span>
* <span data-ttu-id="55d74-197">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-197">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="55d74-198">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-198">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="55d74-199">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-199">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-200">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-200">Storage</span></span>
* <span data-ttu-id="55d74-201">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-201">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-202">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-202">VM</span></span>
* <span data-ttu-id="55d74-203">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-203">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="55d74-204">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-204">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="55d74-205">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-205">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="55d74-206">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-206">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="55d74-207">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="55d74-207">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="55d74-208">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-208">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="55d74-209">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="55d74-209">October 23, 2018</span></span>

<span data-ttu-id="55d74-210">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="55d74-210">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="55d74-211">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-211">Core</span></span>
* <span data-ttu-id="55d74-212">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-212">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="55d74-213">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-213">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-214">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-214">ACR</span></span>
* <span data-ttu-id="55d74-215">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-215">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="55d74-216">CDN</span><span class="sxs-lookup"><span data-stu-id="55d74-216">CDN</span></span>
* <span data-ttu-id="55d74-217">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-217">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="55d74-218">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-218">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="55d74-219">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-219">Container</span></span>
* <span data-ttu-id="55d74-220">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-220">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="55d74-221">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-221">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="55d74-222">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-222">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="55d74-223">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-223">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="55d74-224">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-224">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="55d74-225">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-225">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="55d74-226">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-226">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55d74-227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55d74-227">CosmosDB</span></span>
* <span data-ttu-id="55d74-228">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-228">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-229">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-229">Interactive</span></span>
* <span data-ttu-id="55d74-230">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-230">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="55d74-231">IoT Central</span><span class="sxs-lookup"><span data-stu-id="55d74-231">IoT Central</span></span>
* <span data-ttu-id="55d74-232">IoT Central 응용 프로그램 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-232">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="55d74-233">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-233">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-234">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-234">Monitor</span></span>
* <span data-ttu-id="55d74-235">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="55d74-235">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="55d74-236">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-236">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="55d74-237">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-237">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="55d74-238">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-238">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="55d74-239">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-239">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="55d74-240">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-240">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="55d74-241">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="55d74-241">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="55d74-242">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-242">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="55d74-243">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-243">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="55d74-244">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-244">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="55d74-245">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-245">Network</span></span>
* <span data-ttu-id="55d74-246">NIC에 응용 프로그램 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-246">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="55d74-247">NIC에 응용 프로그램 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-247">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="55d74-248">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55d74-248">ServiceBus</span></span>
* <span data-ttu-id="55d74-249">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-249">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-250">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-250">SQL</span></span>
* <span data-ttu-id="55d74-251">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-251">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-252">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-252">Storage</span></span>
* <span data-ttu-id="55d74-253">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-253">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="55d74-254">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-254">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-255">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-255">VM</span></span>
* <span data-ttu-id="55d74-256">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-256">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="55d74-257">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-257">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="55d74-258">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-258">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="55d74-259">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="55d74-259">October 16, 2018</span></span>

<span data-ttu-id="55d74-260">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="55d74-260">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-261">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-261">VM</span></span>
* <span data-ttu-id="55d74-262">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-262">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="55d74-263">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="55d74-263">October 9, 2018</span></span>

<span data-ttu-id="55d74-264">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="55d74-264">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="55d74-265">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-265">Core</span></span>
* <span data-ttu-id="55d74-266">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="55d74-266">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-267">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-267">ACR</span></span>
* <span data-ttu-id="55d74-268">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-268">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-269">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-269">ACS</span></span>
* <span data-ttu-id="55d74-270">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="55d74-270">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="55d74-271">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-271">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="55d74-272">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-272">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="55d74-273">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="55d74-273">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="55d74-274">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-274">Container</span></span>
* <span data-ttu-id="55d74-275">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-275">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="55d74-276">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-276">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="55d74-277">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="55d74-277">Event Hub</span></span>
* <span data-ttu-id="55d74-278">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-278">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="55d74-279">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-279">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="55d74-280">확장</span><span class="sxs-lookup"><span data-stu-id="55d74-280">Extensions</span></span>
* <span data-ttu-id="55d74-281">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-281">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="55d74-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="55d74-282">HDInsight</span></span>
* <span data-ttu-id="55d74-283">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-283">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-284">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-284">IoT</span></span>
* <span data-ttu-id="55d74-285">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-285">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55d74-286">KeyVault</span></span>
* <span data-ttu-id="55d74-287">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-287">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="55d74-288">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-288">Network</span></span>
* <span data-ttu-id="55d74-289">`network dns zone create` 수정: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-289">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="55d74-290">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="55d74-290">See #6052</span></span>
* <span data-ttu-id="55d74-291">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="55d74-291">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="55d74-292">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-292">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="55d74-293">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-293">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="55d74-294">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-294">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="55d74-295">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-295">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="55d74-296">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-296">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="55d74-297">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-297">Role</span></span>
* <span data-ttu-id="55d74-298">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-298">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="55d74-299">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-299">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="55d74-300">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-300">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="55d74-301">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-301">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="55d74-302">Service Bus</span><span class="sxs-lookup"><span data-stu-id="55d74-302">Service Bus</span></span>
* <span data-ttu-id="55d74-303">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-303">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-304">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-304">VM</span></span>
* <span data-ttu-id="55d74-305">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-305">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="55d74-306">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-306">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="55d74-307">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-307">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="55d74-308">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-308">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="55d74-309">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-309">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="55d74-310">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-310">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="55d74-311">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="55d74-311">September 21, 2018</span></span>

<span data-ttu-id="55d74-312">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="55d74-312">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-313">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-313">ACR</span></span>
* <span data-ttu-id="55d74-314">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-314">Added ACR Task commands</span></span>
* <span data-ttu-id="55d74-315">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-315">Added quick run command</span></span>
* <span data-ttu-id="55d74-316">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-316">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="55d74-317">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-317">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="55d74-318">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-318">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="55d74-319">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-319">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-320">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-320">ACS</span></span>
* <span data-ttu-id="55d74-321">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-321">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="55d74-322">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-322">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-323">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-323">AppService</span></span>

* <span data-ttu-id="55d74-324">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-324">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="55d74-325">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-325">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="55d74-326">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-326">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="55d74-327">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-327">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-328">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-328">Batch</span></span>
* <span data-ttu-id="55d74-329">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-329">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="55d74-330">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-330">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="55d74-331">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-331">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="55d74-332">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-332">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="55d74-333">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55d74-333">Batch AI</span></span> 
* <span data-ttu-id="55d74-334">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-334">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55d74-335">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55d74-335">Cognitive Services</span></span>
* <span data-ttu-id="55d74-336">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-336">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="55d74-337">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-337">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="55d74-338">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-338">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="55d74-339">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-339">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="55d74-340">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-340">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="55d74-341">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-341">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="55d74-342">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-342">Container</span></span>
* <span data-ttu-id="55d74-343">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-343">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="55d74-344">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-344">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="55d74-345">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-345">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="55d74-346">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-346">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="55d74-347">Datalake</span><span class="sxs-lookup"><span data-stu-id="55d74-347">Datalake</span></span>
* <span data-ttu-id="55d74-348">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-348">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="55d74-349">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="55d74-349">Interactive Shell</span></span>
* <span data-ttu-id="55d74-350">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-350">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="55d74-351">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-351">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-352">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-352">IoT</span></span>
* <span data-ttu-id="55d74-353">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-353">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="55d74-354">Key Vault</span><span class="sxs-lookup"><span data-stu-id="55d74-354">Key Vault</span></span>
* <span data-ttu-id="55d74-355">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-355">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="55d74-356">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-356">Network</span></span>
* <span data-ttu-id="55d74-357">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-357">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="55d74-358">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-358">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="55d74-359">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-359">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="55d74-360">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-360">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="55d74-361">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-361">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="55d74-362">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-362">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="55d74-363">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-363">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="55d74-364">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-364">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="55d74-365">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-365">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="55d74-366">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-366">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="55d74-367">`network vnet subnet create/update`: `--delegation` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-367">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="55d74-368">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-368">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="55d74-369">`network traffic-manager profile create/update`: 모니터 구성을 위한 `--interval`, `--timeout` 및 `--max-failures` 지원 추가. `--path`, `--port`, `--protocol`로 인해 `--monitor-path`, `--monitor-port` 및 `--monitor-protocol` 옵션이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-369">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="55d74-370">`network lb frontend-ip create/update`: 사설 IP 할당 방법을 설정하기 위한 논리 수정. 사설 IP 주소가 제공된 경우 할당이 정적이 됨. 사설 IP 주소가 제공되지 않은 경우 사설 IP 주소에 대해 빈 문자열이 제공되고 할당이 동적이 됨.</span><span class="sxs-lookup"><span data-stu-id="55d74-370">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="55d74-371">`dns record-set * create/update`: `--target-resource` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-371">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="55d74-372">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-372">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="55d74-373">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-373">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="55d74-374">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-374">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-375">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-375">RDBMS</span></span>
* <span data-ttu-id="55d74-376">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-376">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="55d74-377">예약</span><span class="sxs-lookup"><span data-stu-id="55d74-377">Reservation</span></span>
* <span data-ttu-id="55d74-378">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-378">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="55d74-379">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-379">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="55d74-380">앱 관리</span><span class="sxs-lookup"><span data-stu-id="55d74-380">Manage App</span></span>
* <span data-ttu-id="55d74-381">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-381">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="55d74-382">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-382">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="55d74-383">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-383">Role</span></span>
* <span data-ttu-id="55d74-384">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-384">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="55d74-385">SignalR</span><span class="sxs-lookup"><span data-stu-id="55d74-385">SignalR</span></span>
* <span data-ttu-id="55d74-386">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-386">First release</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-387">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-387">Storage</span></span>
* <span data-ttu-id="55d74-388">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-388">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="55d74-389">변경할 수 없는 저장소 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-389">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-390">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-390">VM</span></span>
* <span data-ttu-id="55d74-391">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 개인 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="55d74-391">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="55d74-392">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-392">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="55d74-393">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="55d74-393">August 28, 2018</span></span>

<span data-ttu-id="55d74-394">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="55d74-394">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="55d74-395">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-395">Core</span></span>

* <span data-ttu-id="55d74-396">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-396">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="55d74-397">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-397">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-398">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-398">ACR</span></span>

* <span data-ttu-id="55d74-399">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-399">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="55d74-400">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-400">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-401">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-401">ACS</span></span>

* <span data-ttu-id="55d74-402">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-402">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="55d74-403">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-403">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-404">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-404">AppService</span></span>

* <span data-ttu-id="55d74-405">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-405">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="55d74-406">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-406">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="55d74-407">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-407">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="55d74-408">Backup</span><span class="sxs-lookup"><span data-stu-id="55d74-408">Backup</span></span>

* <span data-ttu-id="55d74-409">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-409">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="55d74-410">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="55d74-410">Bot Service</span></span>

* <span data-ttu-id="55d74-411">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-411">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55d74-412">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55d74-412">Cognitive Services</span></span>

* <span data-ttu-id="55d74-413">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-413">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-414">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-414">IoT</span></span>

* <span data-ttu-id="55d74-415">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-415">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-416">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-416">Monitor</span></span>

* <span data-ttu-id="55d74-417">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-417">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="55d74-418">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="55d74-418">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="55d74-419">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-419">Network</span></span>

* <span data-ttu-id="55d74-420">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-420">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-421">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-421">Resource</span></span>

* <span data-ttu-id="55d74-422">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-422">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-423">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-423">Storage</span></span>

* <span data-ttu-id="55d74-424">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-424">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-425">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-425">VM</span></span>

* <span data-ttu-id="55d74-426">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-426">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="55d74-427">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="55d74-427">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="55d74-428">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="55d74-428">Auguest 14, 2018</span></span>

<span data-ttu-id="55d74-429">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="55d74-429">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="55d74-430">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-430">Core</span></span>

* <span data-ttu-id="55d74-431">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-431">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="55d74-432">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="55d74-432">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="55d74-433">원격 분석</span><span class="sxs-lookup"><span data-stu-id="55d74-433">Telemetry</span></span>

* <span data-ttu-id="55d74-434">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="55d74-434">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-435">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-435">ACR</span></span>

* <span data-ttu-id="55d74-436">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-436">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="55d74-437">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-437">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-438">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-438">ACS</span></span>

* <span data-ttu-id="55d74-439">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-439">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="55d74-440">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-440">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="55d74-441">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-441">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="55d74-442">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-442">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="55d74-443">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-443">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="55d74-444">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-444">AppService</span></span>

* <span data-ttu-id="55d74-445">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-445">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="55d74-446">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-446">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="55d74-447">BatchAI</span><span class="sxs-lookup"><span data-stu-id="55d74-447">BatchAI</span></span>

* <span data-ttu-id="55d74-448">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-448">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="55d74-449">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-449">Container</span></span>

* <span data-ttu-id="55d74-450">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-450">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="55d74-451">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-451">IoT</span></span>

* <span data-ttu-id="55d74-452">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="55d74-452">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="55d74-453">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-453">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="55d74-454">Iot Central</span><span class="sxs-lookup"><span data-stu-id="55d74-454">Iot Central</span></span>

* <span data-ttu-id="55d74-455">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-455">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-456">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55d74-456">KeyVault</span></span>


* <span data-ttu-id="55d74-457">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-457">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="55d74-458">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-458">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="55d74-459">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-459">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="55d74-460">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-460">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="55d74-461">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-461">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="55d74-462">릴레이</span><span class="sxs-lookup"><span data-stu-id="55d74-462">Relay</span></span>

* <span data-ttu-id="55d74-463">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-463">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-464">Sql</span><span class="sxs-lookup"><span data-stu-id="55d74-464">Sql</span></span>

* <span data-ttu-id="55d74-465">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-465">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-466">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-466">Storage</span></span>

* <span data-ttu-id="55d74-467">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="55d74-467">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="55d74-468">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-468">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="55d74-469">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-469">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="55d74-470">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="55d74-470">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="55d74-471">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-471">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-472">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-472">VM</span></span>

* <span data-ttu-id="55d74-473">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-473">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="55d74-474">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="55d74-474">July 31, 2018</span></span>

<span data-ttu-id="55d74-475">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="55d74-475">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-476">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-476">ACR</span></span>

* <span data-ttu-id="55d74-477">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-477">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="55d74-478">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-478">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-479">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-479">ACS</span></span>

* <span data-ttu-id="55d74-480">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-480">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-481">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-481">Batch</span></span>

* <span data-ttu-id="55d74-482">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-482">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="55d74-483">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-483">Container</span></span>

* <span data-ttu-id="55d74-484">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-484">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="55d74-485">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-485">Network</span></span>

* <span data-ttu-id="55d74-486">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-486">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="55d74-487">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-487">Resource</span></span>

* <span data-ttu-id="55d74-488">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="55d74-488">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="55d74-489">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-489">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="55d74-490">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-490">Role</span></span>

* <span data-ttu-id="55d74-491">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-491">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="55d74-492">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-492">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="55d74-493">검색</span><span class="sxs-lookup"><span data-stu-id="55d74-493">Search</span></span>

* <span data-ttu-id="55d74-494">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-494">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="55d74-495">Service Bus</span><span class="sxs-lookup"><span data-stu-id="55d74-495">Service Bus</span></span>

* <span data-ttu-id="55d74-496">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-496">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="55d74-497">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-497">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="55d74-498">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="55d74-498">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="55d74-499">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="55d74-499">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-500">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-500">Storage</span></span>

* <span data-ttu-id="55d74-501">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-501">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="55d74-502">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="55d74-502">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-503">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-503">VM</span></span>

* <span data-ttu-id="55d74-504">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-504">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="55d74-505">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-505">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="55d74-506">VM 확장 집합 생성 시 응용 프로그램 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-506">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="55d74-507">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-507">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="55d74-508">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="55d74-508">July 18, 2018</span></span>

<span data-ttu-id="55d74-509">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="55d74-509">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="55d74-510">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-510">Core</span></span>

* <span data-ttu-id="55d74-511">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-511">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="55d74-512">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-512">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="55d74-513">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-513">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-514">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-514">ACR</span></span>

* <span data-ttu-id="55d74-515">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-515">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="55d74-516">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-516">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="55d74-517">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-517">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="55d74-518">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-518">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-519">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-519">ACS</span></span>

* <span data-ttu-id="55d74-520">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-520">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-521">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-521">AppService</span></span>

* <span data-ttu-id="55d74-522">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-522">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-523">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-523">Batch</span></span>

* <span data-ttu-id="55d74-524">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-524">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="55d74-525">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-525">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="55d74-526">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55d74-526">Batch AI</span></span>

* <span data-ttu-id="55d74-527">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-527">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="55d74-528">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-528">Container</span></span>

* <span data-ttu-id="55d74-529">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-529">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="55d74-530">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-530">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="55d74-531">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-531">Network</span></span>

* <span data-ttu-id="55d74-532">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-532">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="55d74-533">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-533">Added `network nic wait`</span></span>
* <span data-ttu-id="55d74-534">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-534">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="55d74-535">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-535">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="55d74-536">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-536">Resource</span></span>

* <span data-ttu-id="55d74-537">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-537">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="55d74-538">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-538">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="55d74-539">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-539">Added `deployment wait` command</span></span>
* <span data-ttu-id="55d74-540">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-540">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-541">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-541">SQL</span></span>

* <span data-ttu-id="55d74-542">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-542">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="55d74-543">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-543">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="55d74-544">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="55d74-544">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-545">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-545">Storage</span></span>

* <span data-ttu-id="55d74-546">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-546">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-547">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-547">VM</span></span>

* <span data-ttu-id="55d74-548">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-548">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="55d74-549">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-549">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="55d74-550">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-550">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="55d74-551">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="55d74-551">July 3, 2018</span></span>

<span data-ttu-id="55d74-552">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="55d74-552">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="55d74-553">AKS</span><span class="sxs-lookup"><span data-stu-id="55d74-553">AKS</span></span>

* <span data-ttu-id="55d74-554">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-554">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="55d74-555">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="55d74-555">July 3, 2018</span></span>

<span data-ttu-id="55d74-556">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="55d74-556">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="55d74-557">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-557">Core</span></span>

* <span data-ttu-id="55d74-558">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-558">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-559">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-559">ACR</span></span>

* <span data-ttu-id="55d74-560">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-560">Added polling build status</span></span>
* <span data-ttu-id="55d74-561">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-561">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="55d74-562">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-562">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-563">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-563">ACS</span></span>

* <span data-ttu-id="55d74-564">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-564">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="55d74-565">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-565">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="55d74-566">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="55d74-566">Updated options for `aks browse` command.</span></span> <span data-ttu-id="55d74-567">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-567">Added `--listen-port` support</span></span>
* <span data-ttu-id="55d74-568">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트 </span><span class="sxs-lookup"><span data-stu-id="55d74-568">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="55d74-569">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="55d74-569">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="55d74-570">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-570">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-571">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-571">AppService</span></span>

* <span data-ttu-id="55d74-572">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-572">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="55d74-573">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-573">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="55d74-574">Backup</span><span class="sxs-lookup"><span data-stu-id="55d74-574">Backup</span></span>

* <span data-ttu-id="55d74-575">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-575">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="55d74-576">BatchAI</span><span class="sxs-lookup"><span data-stu-id="55d74-576">BatchAI</span></span>

* <span data-ttu-id="55d74-577">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-577">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="55d74-578">클라우드</span><span class="sxs-lookup"><span data-stu-id="55d74-578">Cloud</span></span>

* <span data-ttu-id="55d74-579">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-579">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="55d74-580">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-580">Container</span></span>

* <span data-ttu-id="55d74-581">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-581">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="55d74-582">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-582">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="55d74-583">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-583">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-584">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-584">Extension</span></span>

* <span data-ttu-id="55d74-585">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-585">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="55d74-586">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-586">Network</span></span>

* <span data-ttu-id="55d74-587">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="55d74-587">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-588">Rdbms</span><span class="sxs-lookup"><span data-stu-id="55d74-588">Rdbms</span></span>

* <span data-ttu-id="55d74-589">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-589">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-590">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-590">Resource</span></span>

* <span data-ttu-id="55d74-591">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-591">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-592">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-592">VM</span></span>

* <span data-ttu-id="55d74-593">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-593">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="55d74-594">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="55d74-594">June 25, 2018</span></span>

<span data-ttu-id="55d74-595">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="55d74-595">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="55d74-596">CLI</span><span class="sxs-lookup"><span data-stu-id="55d74-596">CLI</span></span>

* <span data-ttu-id="55d74-597">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-597">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="55d74-598">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="55d74-598">June 19, 2018</span></span>

<span data-ttu-id="55d74-599">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="55d74-599">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="55d74-600">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-600">Core</span></span>

* <span data-ttu-id="55d74-601">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-601">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-602">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-602">ACR</span></span>

* <span data-ttu-id="55d74-603">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-603">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="55d74-604">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-604">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-605">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-605">ACS</span></span>

* <span data-ttu-id="55d74-606">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="55d74-606">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="55d74-607">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-607">Added `--update` support</span></span>
* <span data-ttu-id="55d74-608">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-608">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="55d74-609">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="55d74-609">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="55d74-610">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-610">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="55d74-611">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-611">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="55d74-612">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-612">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="55d74-613">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-613">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-614">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-614">AppService</span></span>

* <span data-ttu-id="55d74-615">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-615">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="55d74-616">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-616">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-617">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-617">Batch</span></span>

* <span data-ttu-id="55d74-618">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-618">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="55d74-619">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55d74-619">Batch AI</span></span>

* <span data-ttu-id="55d74-620">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="55d74-620">Added support for workspaces.</span></span> <span data-ttu-id="55d74-621">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-621">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="55d74-622">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="55d74-622">Added support for experiments.</span></span> <span data-ttu-id="55d74-623">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-623">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="55d74-624">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-624">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="55d74-625">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="55d74-625">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="55d74-626">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-626">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="55d74-627">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-627">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="55d74-628">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="55d74-628">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="55d74-629">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="55d74-629">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="55d74-630">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="55d74-630">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="55d74-631">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="55d74-631">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="55d74-632">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="55d74-632">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="55d74-633">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="55d74-633">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="55d74-634">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="55d74-634">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="55d74-635">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-635">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="55d74-636">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="55d74-636">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="55d74-637">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="55d74-637">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="55d74-638">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="55d74-638">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="55d74-639">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="55d74-639">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="55d74-640">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="55d74-640">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="55d74-641">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="55d74-641">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="55d74-642">지도</span><span class="sxs-lookup"><span data-stu-id="55d74-642">Maps</span></span>

* <span data-ttu-id="55d74-643">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-643">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="55d74-644">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-644">Network</span></span>

* <span data-ttu-id="55d74-645">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-645">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="55d74-646">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-646">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="55d74-647">#6502</span><span class="sxs-lookup"><span data-stu-id="55d74-647">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="55d74-648">예약</span><span class="sxs-lookup"><span data-stu-id="55d74-648">Reservations</span></span>

* <span data-ttu-id="55d74-649">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-649">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="55d74-650">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-650">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="55d74-651">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="55d74-651">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="55d74-652">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-652">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="55d74-653">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-653">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="55d74-654">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-654">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="55d74-655">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-655">Role</span></span>

* <span data-ttu-id="55d74-656">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="55d74-656">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-657">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-657">SQL</span></span>

* <span data-ttu-id="55d74-658">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-658">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-659">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-659">Storage</span></span>

* <span data-ttu-id="55d74-660">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경 </span><span class="sxs-lookup"><span data-stu-id="55d74-660">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-661">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-661">VM</span></span>

* <span data-ttu-id="55d74-662">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="55d74-662">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="55d74-663">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-663">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="55d74-664">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-664">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="55d74-665">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="55d74-665">June 13, 2018</span></span>

<span data-ttu-id="55d74-666">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="55d74-666">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="55d74-667">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-667">Core</span></span>

* <span data-ttu-id="55d74-668">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="55d74-668">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="55d74-669">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="55d74-669">June 13, 2018</span></span>

<span data-ttu-id="55d74-670">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="55d74-670">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="55d74-671">AKS</span><span class="sxs-lookup"><span data-stu-id="55d74-671">AKS</span></span>

* <span data-ttu-id="55d74-672">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-672">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="55d74-673">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="55d74-673">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="55d74-674">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-674">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="55d74-675">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-675">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="55d74-676">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-676">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-677">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-677">AppService</span></span>

* <span data-ttu-id="55d74-678">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-678">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="55d74-679">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="55d74-679">June 5, 2018</span></span>

<span data-ttu-id="55d74-680">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="55d74-680">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-681">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-681">Interactive</span></span>

* <span data-ttu-id="55d74-682">대화형 모드의 종속성에 제한 추가 </span><span class="sxs-lookup"><span data-stu-id="55d74-682">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="55d74-683">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="55d74-683">June 5, 2018</span></span>

<span data-ttu-id="55d74-684">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="55d74-684">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="55d74-685">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-685">Core</span></span>

* <span data-ttu-id="55d74-686">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-686">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="55d74-687">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-687">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-688">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-688">ACR</span></span>

* <span data-ttu-id="55d74-689">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-689">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="55d74-690">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-690">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="55d74-691">AKS</span><span class="sxs-lookup"><span data-stu-id="55d74-691">AKS</span></span>

* <span data-ttu-id="55d74-692">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-692">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-693">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-693">Batch</span></span>

* <span data-ttu-id="55d74-694">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="55d74-694">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-695">IOT</span><span class="sxs-lookup"><span data-stu-id="55d74-695">IOT</span></span>

* <span data-ttu-id="55d74-696">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-696">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="55d74-697">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-697">Network</span></span>

* <span data-ttu-id="55d74-698">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="55d74-698">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="55d74-699">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="55d74-699">Policy Insights</span></span>

* <span data-ttu-id="55d74-700">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-700">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="55d74-701">ARM</span><span class="sxs-lookup"><span data-stu-id="55d74-701">ARM</span></span>

* <span data-ttu-id="55d74-702">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-702">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-703">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-703">SQL</span></span>

* <span data-ttu-id="55d74-704">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="55d74-704">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="55d74-705">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-705">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="55d74-706">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-706">Storage</span></span>

* <span data-ttu-id="55d74-707">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="55d74-707">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-708">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-708">VM</span></span>

* <span data-ttu-id="55d74-709">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-709">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="55d74-710">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-710">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="55d74-711">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-711">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="55d74-712">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="55d74-712">May 22, 2018</span></span>

<span data-ttu-id="55d74-713">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="55d74-713">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="55d74-714">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-714">Core</span></span>

* <span data-ttu-id="55d74-715">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-715">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-716">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-716">ACS</span></span>

* <span data-ttu-id="55d74-717">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-717">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="55d74-718">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-718">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-719">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-719">AppService</span></span>

* <span data-ttu-id="55d74-720">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-720">Improved generic update commands</span></span>
* <span data-ttu-id="55d74-721">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-721">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="55d74-722">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-722">Container</span></span>

* <span data-ttu-id="55d74-723">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-723">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="55d74-724">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-724">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-725">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-725">Extension</span></span>

* <span data-ttu-id="55d74-726">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-726">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-727">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-727">Interactive</span></span>

* <span data-ttu-id="55d74-728">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-728">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="55d74-729">잘못된 도움말 캐시의 처리가 향상됨 </span><span class="sxs-lookup"><span data-stu-id="55d74-729">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55d74-730">KeyVault</span></span>

* <span data-ttu-id="55d74-731">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="55d74-731">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="55d74-732">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-732">Network</span></span>

* <span data-ttu-id="55d74-733">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결 </span><span class="sxs-lookup"><span data-stu-id="55d74-733">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="55d74-734">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-734">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-735">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-735">SQL</span></span>

* <span data-ttu-id="55d74-736">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="55d74-736">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="55d74-737">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈 </span><span class="sxs-lookup"><span data-stu-id="55d74-737">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="55d74-738">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-738">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="55d74-739">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-739">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="55d74-740">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-740">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="55d74-741">`requestedServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="55d74-741">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="55d74-742">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-742">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="55d74-743">`edition`</span><span class="sxs-lookup"><span data-stu-id="55d74-743">`edition`.</span></span> <span data-ttu-id="55d74-744">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-744">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="55d74-745">`elasticPoolName`</span><span class="sxs-lookup"><span data-stu-id="55d74-745">`elasticPoolName`.</span></span> <span data-ttu-id="55d74-746">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-746">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="55d74-747">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-747">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="55d74-748">`edition`</span><span class="sxs-lookup"><span data-stu-id="55d74-748">`edition`.</span></span> <span data-ttu-id="55d74-749">업데이트하려면 `--edition` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="55d74-749">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="55d74-750">`dtu`</span><span class="sxs-lookup"><span data-stu-id="55d74-750">`dtu`.</span></span> <span data-ttu-id="55d74-751">업데이트하려면 `--capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="55d74-751">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="55d74-752">`databaseDtuMin`</span><span class="sxs-lookup"><span data-stu-id="55d74-752">`databaseDtuMin`.</span></span> <span data-ttu-id="55d74-753">업데이트하려면 `--db-min-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="55d74-753">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="55d74-754">`databaseDtuMax`</span><span class="sxs-lookup"><span data-stu-id="55d74-754">`databaseDtuMax`.</span></span> <span data-ttu-id="55d74-755">업데이트하려면 `--db-max-capacity` 매개 변수를 사용 </span><span class="sxs-lookup"><span data-stu-id="55d74-755">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="55d74-756">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-756">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="55d74-757">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-757">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-758">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-758">Storage</span></span>

* <span data-ttu-id="55d74-759">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-759">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="55d74-760">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-760">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-761">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-761">VM</span></span>

* <span data-ttu-id="55d74-762">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="55d74-762">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="55d74-763">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="55d74-763">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="55d74-764">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정 </span><span class="sxs-lookup"><span data-stu-id="55d74-764">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="55d74-765">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가 </span><span class="sxs-lookup"><span data-stu-id="55d74-765">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="55d74-766">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-766">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="55d74-767">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="55d74-767">May 7, 2018</span></span>

<span data-ttu-id="55d74-768">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="55d74-768">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="55d74-769">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-769">Core</span></span>

* <span data-ttu-id="55d74-770">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-770">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="55d74-771">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-771">Added limited support for positional arguments</span></span>
* <span data-ttu-id="55d74-772">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-772">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="55d74-773">#5591</span><span class="sxs-lookup"><span data-stu-id="55d74-773">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="55d74-774">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-774">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="55d74-775">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-775">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="55d74-776">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-776">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="55d74-777">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-777">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="55d74-778">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-778">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-779">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-779">ACR</span></span>

* <span data-ttu-id="55d74-780">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-780">Added ACR Build commands</span></span>
* <span data-ttu-id="55d74-781">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-781">Improved resource not found error messages</span></span>
* <span data-ttu-id="55d74-782">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-782">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="55d74-783">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-783">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="55d74-784">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-784">Improved repository commands error messages</span></span>
* <span data-ttu-id="55d74-785">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-785">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-786">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-786">ACS</span></span>

* <span data-ttu-id="55d74-787">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-787">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="55d74-788">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-788">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="55d74-789">AMS</span><span class="sxs-lookup"><span data-stu-id="55d74-789">AMS</span></span>

* <span data-ttu-id="55d74-790">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="55d74-790">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-791">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-791">Appservice</span></span>

* <span data-ttu-id="55d74-792">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-792">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="55d74-793">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-793">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="55d74-794">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-794">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="55d74-795">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-795">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="55d74-796">Batch AI</span><span class="sxs-lookup"><span data-stu-id="55d74-796">Batch AI</span></span>

* <span data-ttu-id="55d74-797">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-797">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55d74-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55d74-798">Cognitive Services</span></span>

* <span data-ttu-id="55d74-799">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-799">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="55d74-800">Consumption</span><span class="sxs-lookup"><span data-stu-id="55d74-800">Consumption</span></span>

* <span data-ttu-id="55d74-801">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-801">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="55d74-802">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-802">Container</span></span>

* <span data-ttu-id="55d74-803">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-803">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="55d74-804">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="55d74-804">Cosmos DB</span></span>

* <span data-ttu-id="55d74-805">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="55d74-805">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="55d74-806">DMS</span><span class="sxs-lookup"><span data-stu-id="55d74-806">DMS</span></span>

* <span data-ttu-id="55d74-807">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-807">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-808">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-808">Extension</span></span>

* <span data-ttu-id="55d74-809">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-809">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-810">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-810">Interactive</span></span>

* <span data-ttu-id="55d74-811">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-811">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="55d74-812">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="55d74-812">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="55d74-813">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-813">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="55d74-814">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-814">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="55d74-815">랩</span><span class="sxs-lookup"><span data-stu-id="55d74-815">Lab</span></span>

* <span data-ttu-id="55d74-816">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-816">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="55d74-817">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-817">Network</span></span>

* <span data-ttu-id="55d74-818">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-818">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="55d74-819">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-819">Profile</span></span>

* <span data-ttu-id="55d74-820">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-820">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="55d74-821">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-821">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="55d74-822">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-822">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="55d74-823">Redis</span><span class="sxs-lookup"><span data-stu-id="55d74-823">Redis</span></span>

* <span data-ttu-id="55d74-824">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-824">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="55d74-825">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-825">Deprecated `redis list-all`.</span></span> <span data-ttu-id="55d74-826">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="55d74-826">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="55d74-827">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-827">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="55d74-828">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-828">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="55d74-829">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-829">Role</span></span>

* <span data-ttu-id="55d74-830">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-830">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-831">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-831">Storage</span></span>

* <span data-ttu-id="55d74-832">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-832">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="55d74-833">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="55d74-833">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="55d74-834">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="55d74-834">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="55d74-835">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-835">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="55d74-836">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-836">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-837">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-837">VM</span></span>

* <span data-ttu-id="55d74-838">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-838">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="55d74-839">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-839">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="55d74-840">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="55d74-840">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="55d74-841">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-841">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="55d74-842">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-842">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="55d74-843">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-843">Added write accelerator support</span></span>
* <span data-ttu-id="55d74-844">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-844">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="55d74-845">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-845">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="55d74-846">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-846">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="55d74-847">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="55d74-847">April 10, 2018</span></span>

<span data-ttu-id="55d74-848">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="55d74-848">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-849">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-849">ACR</span></span>

* <span data-ttu-id="55d74-850">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="55d74-850">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-851">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-851">ACS</span></span>

* <span data-ttu-id="55d74-852">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-852">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-853">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-853">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="55d74-855">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-855">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="55d74-856">BatchAI</span><span class="sxs-lookup"><span data-stu-id="55d74-856">BatchAI</span></span>

* <span data-ttu-id="55d74-857">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-857">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="55d74-858">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="55d74-858">Job level mounting</span></span>
  - <span data-ttu-id="55d74-859">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="55d74-859">Environment variables with secret values</span></span>
  - <span data-ttu-id="55d74-860">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-860">Performance counters settings</span></span>
  - <span data-ttu-id="55d74-861">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="55d74-861">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="55d74-862">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-862">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="55d74-863">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="55d74-863">Usage and limits reporting</span></span>
  - <span data-ttu-id="55d74-864">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-864">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="55d74-865">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-865">Support for custom images</span></span>
  - <span data-ttu-id="55d74-866">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-866">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="55d74-867">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-867">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="55d74-868">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-868">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="55d74-869">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-869">National clouds are supported</span></span>
* <span data-ttu-id="55d74-870">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-870">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="55d74-871">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="55d74-871">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="55d74-872">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-872">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="55d74-873">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-873">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="55d74-874">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 저장소 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(저장소 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="55d74-874">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="55d74-875">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="55d74-875">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="55d74-876">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-876">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="55d74-877">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-877">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="55d74-878">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-878">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="55d74-879">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-879">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="55d74-880">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-880">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="55d74-881">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="55d74-881">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="55d74-882">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-882">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="55d74-883">결제</span><span class="sxs-lookup"><span data-stu-id="55d74-883">Billing</span></span>

* <span data-ttu-id="55d74-884">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-884">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="55d74-885">Consumption</span><span class="sxs-lookup"><span data-stu-id="55d74-885">Consumption</span></span>

* <span data-ttu-id="55d74-886">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-886">Added `marketplace` commands</span></span>
* <span data-ttu-id="55d74-887">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-887">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="55d74-888">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-888">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="55d74-889">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-889">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="55d74-890">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-890">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="55d74-891">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-891">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="55d74-892">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-892">Container</span></span>

* <span data-ttu-id="55d74-893">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="55d74-893">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="55d74-894">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="55d74-894">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-895">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-895">Extension</span></span>

* <span data-ttu-id="55d74-896">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-896">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-897">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-897">Interactive</span></span>

* <span data-ttu-id="55d74-898">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-898">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="55d74-899">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-899">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="55d74-900">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-900">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="55d74-901">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-901">Network</span></span>

* <span data-ttu-id="55d74-902">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-902">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="55d74-903">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-903">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="55d74-904">#4910</span><span class="sxs-lookup"><span data-stu-id="55d74-904">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="55d74-905">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-905">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="55d74-906">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="55d74-906">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="55d74-907">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-907">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="55d74-908">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-908">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="55d74-909">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-909">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-910">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-910">Profile</span></span>

* <span data-ttu-id="55d74-911">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-911">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="55d74-912">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-912">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-913">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-913">RDBMS</span></span>

* <span data-ttu-id="55d74-914">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-914">Added `georestore` command</span></span>
* <span data-ttu-id="55d74-915">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-915">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-916">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-916">Resource</span></span>

* <span data-ttu-id="55d74-917">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-917">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="55d74-918">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-918">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-919">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-919">SQL</span></span>

* <span data-ttu-id="55d74-920">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-920">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-921">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-921">Storage</span></span>

* <span data-ttu-id="55d74-922">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-922">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-923">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-923">VM</span></span>

* <span data-ttu-id="55d74-924">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-924">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="55d74-925">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-925">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="55d74-927">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-927">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="55d74-928">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-928">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="55d74-929">#5718</span><span class="sxs-lookup"><span data-stu-id="55d74-929">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="55d74-930">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-930">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="55d74-931">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="55d74-931">March 27, 2018</span></span>

<span data-ttu-id="55d74-932">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="55d74-932">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="55d74-933">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-933">Core</span></span>

* <span data-ttu-id="55d74-934">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="55d74-934">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-935">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-935">ACS</span></span>

* <span data-ttu-id="55d74-936">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-936">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-937">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-937">Appservice</span></span>

* <span data-ttu-id="55d74-938">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-938">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="55d74-939">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-939">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="55d74-940">Backup</span><span class="sxs-lookup"><span data-stu-id="55d74-940">Backup</span></span>

* <span data-ttu-id="55d74-941">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-941">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="55d74-942">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-942">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="55d74-943">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-943">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="55d74-944">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-944">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="55d74-945">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-945">Container</span></span>

* <span data-ttu-id="55d74-946">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-946">Added `container exec` command.</span></span> <span data-ttu-id="55d74-947">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-947">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="55d74-948">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-948">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-949">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-949">Extension</span></span>

* <span data-ttu-id="55d74-950">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-950">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="55d74-951">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-951">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="55d74-952">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-952">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-953">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-953">Interactive</span></span>

* <span data-ttu-id="55d74-954">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="55d74-954">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="55d74-955">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-955">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="55d74-956">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="55d74-956">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="55d74-957">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-957">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="55d74-958">랩</span><span class="sxs-lookup"><span data-stu-id="55d74-958">Lab</span></span>

* <span data-ttu-id="55d74-959">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-959">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-960">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-960">Monitor</span></span>

* <span data-ttu-id="55d74-961">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-961">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="55d74-962">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 공백으로 구분된 메트릭 목록을 수락하여 검색</span><span class="sxs-lookup"><span data-stu-id="55d74-962">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="55d74-963">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-963">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="55d74-964">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-964">Network</span></span>

* <span data-ttu-id="55d74-965">사설 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-965">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-966">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-966">Profile</span></span>

* <span data-ttu-id="55d74-967">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-967">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-968">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-968">RDBMS</span></span>

* <span data-ttu-id="55d74-969">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-969">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-970">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-970">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="55d74-972">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-972">Role</span></span>

* <span data-ttu-id="55d74-973">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-973">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="55d74-974">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-974">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="55d74-975">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-975">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="55d74-976">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-976">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="55d74-977">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-977">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-978">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-978">Storage</span></span>

* <span data-ttu-id="55d74-979">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-979">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="55d74-980">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하고 blob 업로드 추가 관련 문제</span><span class="sxs-lookup"><span data-stu-id="55d74-980">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-981">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-981">VM</span></span>

* <span data-ttu-id="55d74-982">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-982">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="55d74-983">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-983">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="55d74-984">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-984">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="55d74-985">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-985">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="55d74-986">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="55d74-986">March 13, 2018</span></span>

<span data-ttu-id="55d74-987">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="55d74-987">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-988">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-988">ACR</span></span>

* <span data-ttu-id="55d74-989">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-989">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="55d74-990">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-990">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="55d74-991">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-991">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-992">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-992">ACS</span></span>

* <span data-ttu-id="55d74-993">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-993">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="55d74-994">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-994">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="55d74-995">Advisor</span><span class="sxs-lookup"><span data-stu-id="55d74-995">Advisor</span></span>

* <span data-ttu-id="55d74-996">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-996">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="55d74-997">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-997">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="55d74-998">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-998">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="55d74-999">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-999">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="55d74-1000">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1000">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1001">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1001">Appservice</span></span>

* <span data-ttu-id="55d74-1002">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1002">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="55d74-1003">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1003">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="55d74-1004">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="55d74-1004">Eventhubs</span></span>

* <span data-ttu-id="55d74-1005">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1005">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-1006">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-1006">Extension</span></span>

* <span data-ttu-id="55d74-1007">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1007">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-1008">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-1008">Interactive</span></span>

* <span data-ttu-id="55d74-1009">[#5625](https://github.com/Azure/azure-cli/issues/5625) 해결: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="55d74-1009">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="55d74-1010">[#3016](https://github.com/Azure/azure-cli/issues/3016) 해결: 범위에 있는 동안 기록되지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="55d74-1010">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="55d74-1011">[#5688](https://github.com/Azure/azure-cli/issues/5688) 해결: 명령 테이블 로드에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1011">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="55d74-1012">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1012">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1013">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1013">Monitor</span></span>

* <span data-ttu-id="55d74-1014">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1014">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="55d74-1015">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1015">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="55d74-1016">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1016">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="55d74-1017">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1017">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1018">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1018">Network</span></span>

* <span data-ttu-id="55d74-1019">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1019">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="55d74-1020">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="55d74-1020">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="55d74-1021">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1021">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="55d74-1022">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1022">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1023">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1023">Profile</span></span>

* <span data-ttu-id="55d74-1024">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1024">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="55d74-1025">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1025">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-1026">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-1026">RDBMS</span></span>

* <span data-ttu-id="55d74-1027">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1027">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="55d74-1028">Service Bus</span><span class="sxs-lookup"><span data-stu-id="55d74-1028">Service Bus</span></span>

* <span data-ttu-id="55d74-1029">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1029">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1030">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1030">Storage</span></span>

* <span data-ttu-id="55d74-1031">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1031">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="55d74-1032">[#5286](https://github.com/Azure/azure-cli/issues/5286) 해결: `storage blob [delete-batch|download-batch|upload-batch]` 명령 일괄 처리하여 더 이상 사전 조건 실패 시 오류를 throw하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1032">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1033">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1033">VM</span></span>

* <span data-ttu-id="55d74-1034">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1034">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="55d74-1035">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1035">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="55d74-1036">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1036">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="55d74-1037">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1037">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="55d74-1038">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="55d74-1038">February 27, 2018</span></span>

<span data-ttu-id="55d74-1039">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="55d74-1039">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1040">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1040">Core</span></span>

* <span data-ttu-id="55d74-1041">[#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1041">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="55d74-1042">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1042">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="55d74-1043">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1043">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1044">ACS</span></span>

* <span data-ttu-id="55d74-1045">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1045">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="55d74-1046">문제: ACI 컨테이너 그룹을 만들기 위해 서비스 주체에 대한 사용 권한 부족 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1046">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="55d74-1047">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1047">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="55d74-1048">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-1048">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1049">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1049">Appservice</span></span>

* <span data-ttu-id="55d74-1050">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="55d74-1050">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="55d74-1051">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1051">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="55d74-1052">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="55d74-1052">Cognitive Services</span></span>

* <span data-ttu-id="55d74-1053">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-1053">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="55d74-1054">Consumption</span><span class="sxs-lookup"><span data-stu-id="55d74-1054">Consumption</span></span>

* <span data-ttu-id="55d74-1055">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1055">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="55d74-1056">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-1056">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1057">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1057">Container</span></span>

* <span data-ttu-id="55d74-1058">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1058">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1059">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1059">Network</span></span>

* <span data-ttu-id="55d74-1060">[#5559](https://github.com/Azure/azure-cli/issues/5559): `network vnet-gateway vpn-client generate`에서 누락된 클라이언트 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1060">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1061">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1061">Resource</span></span>

* <span data-ttu-id="55d74-1062">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1062">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1063">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1063">Role</span></span>

* <span data-ttu-id="55d74-1064">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1064">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1065">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1065">SQL</span></span>

* <span data-ttu-id="55d74-1066">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1066">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1067">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1067">Storage</span></span>

* <span data-ttu-id="55d74-1068">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="55d74-1068">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1069">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1069">VM</span></span>

* <span data-ttu-id="55d74-1070">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1070">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="55d74-1071">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="55d74-1071">February 13, 2018</span></span>

<span data-ttu-id="55d74-1072">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="55d74-1072">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1073">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1073">Core</span></span>

* <span data-ttu-id="55d74-1074">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1074">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1075">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1075">ACS</span></span>

* <span data-ttu-id="55d74-1076">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1076">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="55d74-1077">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1077">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="55d74-1078">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1078">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="55d74-1079">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="55d74-1079">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="55d74-1080">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1080">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="55d74-1081">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="55d74-1081">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="55d74-1082">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1082">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="55d74-1083">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1083">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1084">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1084">Appservice</span></span>

* <span data-ttu-id="55d74-1085">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1085">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="55d74-1086">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1086">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="55d74-1087">CDN</span><span class="sxs-lookup"><span data-stu-id="55d74-1087">CDN</span></span>

* <span data-ttu-id="55d74-1088">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1088">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1089">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1089">Container</span></span>

* <span data-ttu-id="55d74-1090">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1090">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="55d74-1091">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1091">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55d74-1092">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55d74-1092">CosmosDB</span></span>

* <span data-ttu-id="55d74-1093">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1093">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-1094">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-1094">Extension</span></span>

* <span data-ttu-id="55d74-1095">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1095">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="55d74-1096">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1096">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="55d74-1097">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="55d74-1097">Feedback</span></span>

* <span data-ttu-id="55d74-1098">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1098">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-1099">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-1099">Interactive</span></span>

* <span data-ttu-id="55d74-1100">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1100">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="55d74-1101">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1101">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-1102">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-1102">IoT</span></span>

* <span data-ttu-id="55d74-1103">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1103">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="55d74-1104">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1104">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="55d74-1105">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1105">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="55d74-1106">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1106">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1107">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1107">Monitor</span></span>

* <span data-ttu-id="55d74-1108">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1108">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1109">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1109">Network</span></span>

* <span data-ttu-id="55d74-1110">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1110">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="55d74-1111">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1111">Profile</span></span>

* <span data-ttu-id="55d74-1112">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1112">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1113">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1113">Resource</span></span>

* <span data-ttu-id="55d74-1114">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1114">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1115">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1115">Role</span></span>

* <span data-ttu-id="55d74-1116">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1116">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1117">SQL</span></span>

* <span data-ttu-id="55d74-1118">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1118">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="55d74-1119">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1119">Added `sql db rename`</span></span>
* <span data-ttu-id="55d74-1120">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1120">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1121">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1121">Storage</span></span>

* <span data-ttu-id="55d74-1122">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1122">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1123">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1123">VM</span></span>

* <span data-ttu-id="55d74-1124">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1124">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="55d74-1125">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1125">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="55d74-1126">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="55d74-1126">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="55d74-1127">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="55d74-1127">January 31, 2018</span></span>

<span data-ttu-id="55d74-1128">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="55d74-1128">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1129">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1129">Core</span></span>

* <span data-ttu-id="55d74-1130">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1130">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="55d74-1131">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-1131">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="55d74-1132">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1132">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="55d74-1133">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="55d74-1133">Use `--verbose` to see</span></span>
* <span data-ttu-id="55d74-1134">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1134">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1135">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1135">ACS</span></span>

* <span data-ttu-id="55d74-1136">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1136">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="55d74-1137">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="55d74-1137">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1138">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1138">Appservice</span></span>

* <span data-ttu-id="55d74-1139">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="55d74-1139">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="55d74-1140">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-1140">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="55d74-1141">CDN</span><span class="sxs-lookup"><span data-stu-id="55d74-1141">CDN</span></span>

* <span data-ttu-id="55d74-1142">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1142">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55d74-1143">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55d74-1143">CosmosDB</span></span>

* <span data-ttu-id="55d74-1144">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1144">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-1145">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-1145">Interactive</span></span>

* <span data-ttu-id="55d74-1146">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1146">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1147">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1147">Network</span></span>

* <span data-ttu-id="55d74-1148">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1148">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="55d74-1149">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1149">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="55d74-1150">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1150">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="55d74-1151">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1151">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="55d74-1152">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1152">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="55d74-1153">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="55d74-1153">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="55d74-1154">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1154">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="55d74-1155">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1155">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="55d74-1156">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1156">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="55d74-1157">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="55d74-1157">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1158">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1158">Profile</span></span>

* <span data-ttu-id="55d74-1159">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1159">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1160">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1160">Resource</span></span>

* <span data-ttu-id="55d74-1161">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1161">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1162">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1162">Storage</span></span>

* <span data-ttu-id="55d74-1163">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1163">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="55d74-1164">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1164">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="55d74-1165">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1165">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="55d74-1166">`blob [list|show]`에 대한 테이블 출력에 'snapshot' 열 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1166">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="55d74-1167">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1167">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1168">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1168">VM</span></span>

* <span data-ttu-id="55d74-1169">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1169">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="55d74-1170">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1170">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="55d74-1171">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1171">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="55d74-1172">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1172">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="55d74-1173">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="55d74-1173">January 17, 2018</span></span>

<span data-ttu-id="55d74-1174">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="55d74-1174">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-1175">ACR</span></span>

* <span data-ttu-id="55d74-1176">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1176">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="55d74-1177">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1177">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1178">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1178">ACS</span></span>

* <span data-ttu-id="55d74-1179">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1179">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="55d74-1180">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1180">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1181">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1181">Appservice</span></span>

* <span data-ttu-id="55d74-1182">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1182">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="55d74-1183">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1183">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="55d74-1184">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1184">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="55d74-1185">Backup</span><span class="sxs-lookup"><span data-stu-id="55d74-1185">Backup</span></span>

* <span data-ttu-id="55d74-1186">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1186">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="55d74-1187">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1187">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="55d74-1188">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1188">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="55d74-1189">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1189">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="55d74-1190">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1190">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-1191">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-1191">Batch</span></span>

* <span data-ttu-id="55d74-1192">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1192">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="55d74-1193">클라우드</span><span class="sxs-lookup"><span data-stu-id="55d74-1193">Cloud</span></span>

* <span data-ttu-id="55d74-1194">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1194">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="55d74-1195">Consumption</span><span class="sxs-lookup"><span data-stu-id="55d74-1195">Consumption</span></span>

* <span data-ttu-id="55d74-1196">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1196">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="55d74-1197">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55d74-1197">Event Grid</span></span>

* <span data-ttu-id="55d74-1198">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1198">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="55d74-1199">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1199">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="55d74-1200">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1200">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="55d74-1201">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="55d74-1201">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="55d74-1202">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1202">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="55d74-1203">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1203">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="55d74-1204">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1204">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="55d74-1205">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1205">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-1206">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-1206">Interactive</span></span>

* <span data-ttu-id="55d74-1207">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1207">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="55d74-1208">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1208">Fixed errors on startup</span></span>
* <span data-ttu-id="55d74-1209">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1209">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-1210">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-1210">IoT</span></span>

* <span data-ttu-id="55d74-1211">장치 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1211">Added support for device provisioning service</span></span>
* <span data-ttu-id="55d74-1212">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1212">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="55d74-1213">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1213">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1214">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1214">Monitor</span></span>

* <span data-ttu-id="55d74-1215">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1215">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="55d74-1216">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="55d74-1216">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="55d74-1217">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1217">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1218">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1218">Network</span></span>

* <span data-ttu-id="55d74-1219">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1219">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="55d74-1220">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1220">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1221">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1221">Profile</span></span>

* <span data-ttu-id="55d74-1222">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1222">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1223">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1223">Role</span></span>

* <span data-ttu-id="55d74-1224">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1224">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55d74-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55d74-1225">Service Fabric</span></span>

* <span data-ttu-id="55d74-1226">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1226">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="55d74-1227">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1227">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1228">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1228">VM</span></span>

* <span data-ttu-id="55d74-1229">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1229">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="55d74-1230">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1230">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="55d74-1231">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1231">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="55d74-1232">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1232">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="55d74-1233">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1233">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="55d74-1234">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1234">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="55d74-1235">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1235">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="55d74-1236">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1236">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="55d74-1237">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="55d74-1237">December 19, 2017</span></span>

<span data-ttu-id="55d74-1238">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="55d74-1238">Version 2.0.23</span></span>

* <span data-ttu-id="55d74-1239">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1239">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1240">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1240">Container</span></span>

* <span data-ttu-id="55d74-1241">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1241">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1242">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1242">Network</span></span>

* <span data-ttu-id="55d74-1243">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1243">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="55d74-1244">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1244">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1245">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1245">Storage</span></span>

* <span data-ttu-id="55d74-1246">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1246">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1247">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1247">VM</span></span>

* <span data-ttu-id="55d74-1248">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1248">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="55d74-1249">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="55d74-1249">December 5, 2017</span></span>

<span data-ttu-id="55d74-1250">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="55d74-1250">Version 2.0.22</span></span>

* <span data-ttu-id="55d74-1251">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1251">Removed `az component` commands.</span></span> <span data-ttu-id="55d74-1252">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="55d74-1252">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1253">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1253">Core</span></span>
* <span data-ttu-id="55d74-1254">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1254">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="55d74-1255">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1255">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1256">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1256">ACS</span></span>

* <span data-ttu-id="55d74-1257">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1257">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="55d74-1258">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1258">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="55d74-1259">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1259">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="55d74-1260">Advisor</span><span class="sxs-lookup"><span data-stu-id="55d74-1260">Advisor</span></span>

* <span data-ttu-id="55d74-1261">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1261">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1262">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1262">Appservice</span></span>

* <span data-ttu-id="55d74-1263">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1263">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="55d74-1264">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1264">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="55d74-1265">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1265">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="55d74-1266">Consumption</span><span class="sxs-lookup"><span data-stu-id="55d74-1266">Consumption</span></span>

* <span data-ttu-id="55d74-1267">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1267">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1268">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1268">Container</span></span>

* <span data-ttu-id="55d74-1269">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1269">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1270">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1270">Monitor</span></span>

* <span data-ttu-id="55d74-1271">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1271">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1272">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1272">Resource</span></span>

* <span data-ttu-id="55d74-1273">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1273">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1274">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1274">Role</span></span>

* <span data-ttu-id="55d74-1275">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1275">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="55d74-1276">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1276">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="55d74-1277">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1277">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1278">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1278">SQL</span></span>

* <span data-ttu-id="55d74-1279">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1279">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="55d74-1280">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1280">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1281">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1281">VM</span></span>

* <span data-ttu-id="55d74-1282">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1282">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="55d74-1283">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="55d74-1283">November 14, 2017</span></span>

<span data-ttu-id="55d74-1284">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="55d74-1284">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-1285">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-1285">ACR</span></span>

* <span data-ttu-id="55d74-1286">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1286">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="55d74-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1287">ACS</span></span>

* <span data-ttu-id="55d74-1288">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1288">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="55d74-1289">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="55d74-1289">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="55d74-1290">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1290">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="55d74-1291">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1291">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="55d74-1292">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1292">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1293">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1293">Appservice</span></span>

* <span data-ttu-id="55d74-1294">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1294">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="55d74-1295">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1295">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="55d74-1296">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1296">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="55d74-1297">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1297">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="55d74-1298">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1298">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="55d74-1299">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="55d74-1299">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-1300">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-1300">Batch</span></span>

* <span data-ttu-id="55d74-1301">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1301">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="55d74-1302">Batchai</span><span class="sxs-lookup"><span data-stu-id="55d74-1302">Batchai</span></span>

* <span data-ttu-id="55d74-1303">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1303">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="55d74-1304">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1304">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="55d74-1305">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1305">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="55d74-1306">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1306">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="55d74-1307">클라우드</span><span class="sxs-lookup"><span data-stu-id="55d74-1307">Cloud</span></span>

* <span data-ttu-id="55d74-1308">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1308">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1309">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1309">Container</span></span>

* <span data-ttu-id="55d74-1310">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1310">Added support to open multiple ports</span></span>
* <span data-ttu-id="55d74-1311">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1311">Added container group restart policy</span></span>
* <span data-ttu-id="55d74-1312">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1312">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="55d74-1313">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="55d74-1313">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55d74-1314">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55d74-1314">Data Lake Analytics</span></span>

* <span data-ttu-id="55d74-1315">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1315">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55d74-1316">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55d74-1316">Data Lake Store</span></span>

* <span data-ttu-id="55d74-1317">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1317">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-1318">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-1318">Extension</span></span>

* <span data-ttu-id="55d74-1319">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1319">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="55d74-1320">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1320">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-1321">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-1321">IoT</span></span>

* <span data-ttu-id="55d74-1322">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1322">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1323">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1323">Monitor</span></span>

* <span data-ttu-id="55d74-1324">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1324">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1325">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1325">Network</span></span>

* <span data-ttu-id="55d74-1326">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1326">Added support for CAA DNS records</span></span>
* <span data-ttu-id="55d74-1327">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1327">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="55d74-1328">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1328">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="55d74-1329">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1329">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="55d74-1330">예약</span><span class="sxs-lookup"><span data-stu-id="55d74-1330">Reservations</span></span>

* <span data-ttu-id="55d74-1331">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1331">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1332">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1332">Resource</span></span>

* <span data-ttu-id="55d74-1333">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1333">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1334">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1334">SQL</span></span>

* <span data-ttu-id="55d74-1335">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1335">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1336">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1336">Storage</span></span>

* <span data-ttu-id="55d74-1337">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1337">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="55d74-1338">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1338">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="55d74-1339">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1339">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="55d74-1340">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="55d74-1340">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="55d74-1341">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1341">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="55d74-1342">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1342">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="55d74-1343">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1343">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1344">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1344">VM</span></span>

* <span data-ttu-id="55d74-1345">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1345">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="55d74-1346">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1346">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="55d74-1347">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1347">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="55d74-1348">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1348">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="55d74-1349">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1349">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="55d74-1350">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="55d74-1350">October 24, 2017</span></span>

<span data-ttu-id="55d74-1351">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="55d74-1351">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1352">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1352">Core</span></span>

* <span data-ttu-id="55d74-1353">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="55d74-1353">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-1354">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-1354">ACR</span></span>

* <span data-ttu-id="55d74-1355">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="55d74-1355">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="55d74-1356">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-1356">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="55d74-1357">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="55d74-1357">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1358">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1358">ACS</span></span>

* <span data-ttu-id="55d74-1359">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1359">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="55d74-1360">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1360">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1361">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1361">Appservice</span></span>

* <span data-ttu-id="55d74-1362">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1362">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="55d74-1363">구성 요소</span><span class="sxs-lookup"><span data-stu-id="55d74-1363">Component</span></span>

* <span data-ttu-id="55d74-1364">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1364">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1365">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1365">Monitor</span></span>

* <span data-ttu-id="55d74-1366">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1366">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1367">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1367">Resource</span></span>

* <span data-ttu-id="55d74-1368">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1368">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="55d74-1369">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1369">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1370">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1370">VM</span></span>

* <span data-ttu-id="55d74-1371">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1371">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="55d74-1372">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="55d74-1372">October 9, 2017</span></span>

<span data-ttu-id="55d74-1373">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="55d74-1373">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1374">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1374">Core</span></span>

* <span data-ttu-id="55d74-1375">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1375">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1376">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1376">Appservice</span></span>

* <span data-ttu-id="55d74-1377">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1377">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-1378">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-1378">Batch</span></span>

* <span data-ttu-id="55d74-1379">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1379">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="55d74-1380">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1380">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="55d74-1381">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1381">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="55d74-1382">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1382">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="55d74-1383">Batchai</span><span class="sxs-lookup"><span data-stu-id="55d74-1383">Batchai</span></span>

* <span data-ttu-id="55d74-1384">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1384">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-1385">Keyvault</span><span class="sxs-lookup"><span data-stu-id="55d74-1385">Keyvault</span></span>

* <span data-ttu-id="55d74-1386">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1386">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="55d74-1387">(#4448)</span><span class="sxs-lookup"><span data-stu-id="55d74-1387">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="55d74-1388">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1388">Network</span></span>

* <span data-ttu-id="55d74-1389">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1389">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="55d74-1390">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1390">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1391">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1391">Resource</span></span>

* <span data-ttu-id="55d74-1392">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1392">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="55d74-1393">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1393">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="55d74-1394">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1394">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="55d74-1395">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1395">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1396">Sql</span><span class="sxs-lookup"><span data-stu-id="55d74-1396">Sql</span></span>

* <span data-ttu-id="55d74-1397">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1397">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="55d74-1398">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1398">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="55d74-1399">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1399">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1400">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1400">Storage</span></span>

* <span data-ttu-id="55d74-1401">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1401">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1402">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1402">Vm</span></span>

* <span data-ttu-id="55d74-1403">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1403">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="55d74-1404">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1404">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="55d74-1405">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1405">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="55d74-1406">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1406">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="55d74-1407">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1407">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="55d74-1408">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="55d74-1408">September 22, 2017</span></span>

<span data-ttu-id="55d74-1409">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="55d74-1409">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1410">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1410">Resource</span></span>

* <span data-ttu-id="55d74-1411">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1411">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="55d74-1412">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1412">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="55d74-1413">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1413">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="55d74-1414">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1414">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1415">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1415">Network</span></span>

* <span data-ttu-id="55d74-1416">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1416">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="55d74-1417">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1417">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="55d74-1418">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1418">Added `asg` application security group commands</span></span>
* <span data-ttu-id="55d74-1419">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1419">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="55d74-1420">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1420">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="55d74-1421">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1421">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="55d74-1422">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1422">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1423">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1423">Storage</span></span>

* <span data-ttu-id="55d74-1424">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1424">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="55d74-1425">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55d74-1425">Eventgrid</span></span>

* <span data-ttu-id="55d74-1426">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="55d74-1426">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1427">SQL</span></span>

* <span data-ttu-id="55d74-1428">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1428">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="55d74-1429">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1429">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="55d74-1430">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1430">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-1431">Keyvault</span><span class="sxs-lookup"><span data-stu-id="55d74-1431">Keyvault</span></span>

* <span data-ttu-id="55d74-1432">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1432">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1433">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1433">VM</span></span>

* <span data-ttu-id="55d74-1434">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1434">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="55d74-1435">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="55d74-1435">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="55d74-1436">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1436">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="55d74-1437">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1437">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="55d74-1438">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1438">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="55d74-1439">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1439">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1440">ACS</span></span>

* <span data-ttu-id="55d74-1441">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1441">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1442">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1442">Appservice</span></span>

* <span data-ttu-id="55d74-1443">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1443">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="55d74-1444">Backup</span><span class="sxs-lookup"><span data-stu-id="55d74-1444">Backup</span></span>

* <span data-ttu-id="55d74-1445">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1445">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="55d74-1446">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="55d74-1446">September 11, 2017</span></span>

<span data-ttu-id="55d74-1447">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="55d74-1447">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="55d74-1448">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1448">Core</span></span>

* <span data-ttu-id="55d74-1449">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1449">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="55d74-1450">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1450">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1451">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1451">Acs</span></span>

* <span data-ttu-id="55d74-1452">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1452">Added `acs list-locations` command</span></span>
* <span data-ttu-id="55d74-1453">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="55d74-1453">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1454">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1454">Appservice</span></span>

* <span data-ttu-id="55d74-1455">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1455">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="55d74-1456">CDN</span><span class="sxs-lookup"><span data-stu-id="55d74-1456">CDN</span></span>

* <span data-ttu-id="55d74-1457">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1457">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="55d74-1458">내선 번호</span><span class="sxs-lookup"><span data-stu-id="55d74-1458">Extension</span></span>

* <span data-ttu-id="55d74-1459">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1459">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-1460">Keyvault</span><span class="sxs-lookup"><span data-stu-id="55d74-1460">Keyvault</span></span>

* <span data-ttu-id="55d74-1461">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1461">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1462">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1462">Network</span></span>

* <span data-ttu-id="55d74-1463">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1463">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="55d74-1464">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1464">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="55d74-1465">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1465">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="55d74-1466">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1466">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="55d74-1467">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1467">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1468">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1468">Resource</span></span>

* <span data-ttu-id="55d74-1469">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-1469">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="55d74-1470">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-1470">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="55d74-1471">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-1471">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="55d74-1472">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="55d74-1472">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1473">SQL</span></span>

* <span data-ttu-id="55d74-1474">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1474">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1475">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1475">VM</span></span>

* <span data-ttu-id="55d74-1476">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1476">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="55d74-1477">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="55d74-1477">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="55d74-1478">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1478">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="55d74-1479">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1479">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="55d74-1480">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1480">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="55d74-1481">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="55d74-1481">August 31, 2017</span></span>

<span data-ttu-id="55d74-1482">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="55d74-1482">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-1483">Keyvault</span><span class="sxs-lookup"><span data-stu-id="55d74-1483">Keyvault</span></span>

* <span data-ttu-id="55d74-1484">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1484">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="55d74-1485">Sf</span><span class="sxs-lookup"><span data-stu-id="55d74-1485">Sf</span></span>

* <span data-ttu-id="55d74-1486">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1486">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1487">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1487">Storage</span></span>

* <span data-ttu-id="55d74-1488">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1488">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="55d74-1489">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="55d74-1489">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="55d74-1490">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="55d74-1490">August 28, 2017</span></span>

<span data-ttu-id="55d74-1491">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="55d74-1491">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="55d74-1492">CLI</span><span class="sxs-lookup"><span data-stu-id="55d74-1492">CLI</span></span>

* <span data-ttu-id="55d74-1493">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1493">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1494">ACS</span></span>

* <span data-ttu-id="55d74-1495">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1495">Corrected preview regions</span></span>
* <span data-ttu-id="55d74-1496">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1496">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="55d74-1497">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1497">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1498">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1498">Appservice</span></span>

* <span data-ttu-id="55d74-1499">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1499">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="55d74-1500">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1500">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="55d74-1501">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1501">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="55d74-1502">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1502">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="55d74-1503">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1503">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-1504">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-1504">IoT</span></span>

* <span data-ttu-id="55d74-1505">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1505">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1506">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1506">Network</span></span>

* <span data-ttu-id="55d74-1507">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1507">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="55d74-1508">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1508">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="55d74-1509">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1509">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="55d74-1510">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1510">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="55d74-1511">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1511">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1512">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1512">Profile</span></span>

* <span data-ttu-id="55d74-1513">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1513">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55d74-1514">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55d74-1514">Service Fabric</span></span>

* <span data-ttu-id="55d74-1515">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1515">Preview release</span></span>
* <span data-ttu-id="55d74-1516">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1516">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="55d74-1517">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1517">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="55d74-1518">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1518">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1519">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1519">Storage</span></span>

* <span data-ttu-id="55d74-1520">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1520">Enabled setting blob tier</span></span>
* <span data-ttu-id="55d74-1521">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1521">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="55d74-1522">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1522">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="55d74-1523">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1523">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="55d74-1524">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1524">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="55d74-1525">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1525">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1526">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1526">VM</span></span>

* <span data-ttu-id="55d74-1527">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1527">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="55d74-1528">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1528">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="55d74-1529">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1529">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="55d74-1530">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1530">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="55d74-1531">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1531">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="55d74-1532">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1532">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="55d74-1533">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="55d74-1533">August 15, 2017</span></span>

<span data-ttu-id="55d74-1534">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="55d74-1534">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1535">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1535">ACS</span></span>

* <span data-ttu-id="55d74-1536">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1536">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1537">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1537">Appservice</span></span>

* <span data-ttu-id="55d74-1538">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1538">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="55d74-1539">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55d74-1539">Event Grid</span></span>

* <span data-ttu-id="55d74-1540">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1540">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="55d74-1541">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="55d74-1541">August 11, 2017</span></span>

<span data-ttu-id="55d74-1542">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="55d74-1542">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1543">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1543">ACS</span></span>

* <span data-ttu-id="55d74-1544">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1544">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-1545">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-1545">Batch</span></span>

* <span data-ttu-id="55d74-1546">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1546">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="55d74-1547">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1547">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="55d74-1548">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1548">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="55d74-1549">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1549">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="55d74-1550">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1550">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="55d74-1551">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1551">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="55d74-1552">구성 요소</span><span class="sxs-lookup"><span data-stu-id="55d74-1552">Component</span></span>

* <span data-ttu-id="55d74-1553">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1553">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="55d74-1554">컨테이너</span><span class="sxs-lookup"><span data-stu-id="55d74-1554">Container</span></span>

* <span data-ttu-id="55d74-1555">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1555">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="55d74-1556">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55d74-1556">Data Lake Store</span></span>

* <span data-ttu-id="55d74-1557">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1557">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="55d74-1558">Event Grid</span><span class="sxs-lookup"><span data-stu-id="55d74-1558">Event Grid</span></span>

* <span data-ttu-id="55d74-1559">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1559">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1560">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1560">Network</span></span>

* <span data-ttu-id="55d74-1561">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1561">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="55d74-1562">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1562">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="55d74-1563">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1563">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="55d74-1564">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1564">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1565">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1565">Profile</span></span>

* <span data-ttu-id="55d74-1566">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1566">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1567">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1567">Storage</span></span>

* <span data-ttu-id="55d74-1568">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1568">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1569">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1569">VM</span></span>

* <span data-ttu-id="55d74-1570">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1570">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="55d74-1571">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1571">Exposed `list-skus` command</span></span>
* <span data-ttu-id="55d74-1572">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1572">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="55d74-1573">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1573">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="55d74-1574">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1574">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="55d74-1575">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="55d74-1575">July 28, 2017</span></span>

<span data-ttu-id="55d74-1576">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="55d74-1576">Version 2.0.12</span></span>

* <span data-ttu-id="55d74-1577">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1577">Added container commands</span></span>
* <span data-ttu-id="55d74-1578">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1578">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="55d74-1579">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1579">Core</span></span>

* <span data-ttu-id="55d74-1580">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1580">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="55d74-1581">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1581">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="55d74-1582">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="55d74-1582">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="55d74-1583">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="55d74-1583">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="55d74-1584">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="55d74-1584">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="55d74-1585">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="55d74-1585">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="55d74-1586">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="55d74-1586">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="55d74-1587">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="55d74-1587">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="55d74-1588">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="55d74-1588">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="55d74-1589">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="55d74-1589">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="55d74-1590">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="55d74-1590">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="55d74-1591">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="55d74-1591">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="55d74-1592">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1592">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="55d74-1593">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1593">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="55d74-1594">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1594">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="55d74-1595">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="55d74-1595">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="55d74-1596">ACR</span><span class="sxs-lookup"><span data-stu-id="55d74-1596">ACR</span></span>

* <span data-ttu-id="55d74-1597">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1597">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="55d74-1598">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1598">Support SKU update for managed registries</span></span>
* <span data-ttu-id="55d74-1599">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1599">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="55d74-1600">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1600">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="55d74-1601">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1601">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="55d74-1602">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1602">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1603">ACS</span></span>

* <span data-ttu-id="55d74-1604">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1604">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1605">App Service</span><span class="sxs-lookup"><span data-stu-id="55d74-1605">Appservice</span></span>

* <span data-ttu-id="55d74-1606">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1606">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="55d74-1607">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1607">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="55d74-1608">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1608">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="55d74-1609">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="55d74-1609">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="55d74-1610">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="55d74-1610">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="55d74-1611">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="55d74-1611">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="55d74-1612">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="55d74-1612">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="55d74-1613">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="55d74-1613">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="55d74-1614">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1614">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="55d74-1615">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1615">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="55d74-1616">Batch</span><span class="sxs-lookup"><span data-stu-id="55d74-1616">Batch</span></span>

* <span data-ttu-id="55d74-1617">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1617">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="55d74-1618">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1618">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="55d74-1619">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1619">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="55d74-1620">CDN</span><span class="sxs-lookup"><span data-stu-id="55d74-1620">CDN</span></span>

* <span data-ttu-id="55d74-1621">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1621">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="55d74-1622">클라우드</span><span class="sxs-lookup"><span data-stu-id="55d74-1622">Cloud</span></span>

* <span data-ttu-id="55d74-1623">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1623">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="55d74-1624">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1624">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="55d74-1625">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1625">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="55d74-1626">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1626">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="55d74-1627">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1627">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55d74-1628">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55d74-1628">CosmosDB</span></span>

* <span data-ttu-id="55d74-1629">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1629">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="55d74-1630">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1630">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55d74-1631">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55d74-1631">Data Lake Analytics</span></span>

* <span data-ttu-id="55d74-1632">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1632">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="55d74-1633">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1633">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="55d74-1634">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1634">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55d74-1635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55d74-1635">Data Lake Store</span></span>

* <span data-ttu-id="55d74-1636">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1636">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="55d74-1637">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1637">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="55d74-1638">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1638">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="55d74-1639">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="55d74-1639">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="55d74-1640">대화형</span><span class="sxs-lookup"><span data-stu-id="55d74-1640">Interactive</span></span>

* <span data-ttu-id="55d74-1641">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1641">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="55d74-1642">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1642">Increased test coverage</span></span>
* <span data-ttu-id="55d74-1643">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1643">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="55d74-1644">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="55d74-1644">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="55d74-1645">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="55d74-1645">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="55d74-1646">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="55d74-1646">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="55d74-1647">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="55d74-1647">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="55d74-1648">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1648">Added `--progress` flag</span></span>
* <span data-ttu-id="55d74-1649">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1649">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="55d74-1650">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="55d74-1650">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="55d74-1651">IoT</span><span class="sxs-lookup"><span data-stu-id="55d74-1651">IoT</span></span>

* <span data-ttu-id="55d74-1652">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1652">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="55d74-1653">(#3934)</span><span class="sxs-lookup"><span data-stu-id="55d74-1653">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="55d74-1654">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="55d74-1654">Key vault</span></span>

* <span data-ttu-id="55d74-1655">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="55d74-1655">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="55d74-1656">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55d74-1656">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="55d74-1657">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55d74-1657">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="55d74-1658">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55d74-1658">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="55d74-1659">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="55d74-1659">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="55d74-1660">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="55d74-1660">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="55d74-1661">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1661">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="55d74-1662">(#3307)</span><span class="sxs-lookup"><span data-stu-id="55d74-1662">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="55d74-1663">랩</span><span class="sxs-lookup"><span data-stu-id="55d74-1663">Lab</span></span>

* <span data-ttu-id="55d74-1664">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1664">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="55d74-1665">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1665">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1666">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1666">Monitor</span></span>

* <span data-ttu-id="55d74-1667">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="55d74-1667">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="55d74-1668">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1668">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="55d74-1669">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1669">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="55d74-1670">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1670">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="55d74-1671">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1671">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="55d74-1672">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="55d74-1672">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="55d74-1673">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1673">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="55d74-1674">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1674">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="55d74-1675">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1675">`location` no longer required</span></span>
  * <span data-ttu-id="55d74-1676">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1676">Add name and ID support for target</span></span>
  * <span data-ttu-id="55d74-1677">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1677">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="55d74-1678">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1678">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="55d74-1679">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1679">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="55d74-1680">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1680">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="55d74-1681">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1681">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="55d74-1682">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1682">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1683">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1683">Network</span></span>

* <span data-ttu-id="55d74-1684">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1684">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="55d74-1685">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1685">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="55d74-1686">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1686">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="55d74-1687">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1687">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="55d74-1688">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1688">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="55d74-1689">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1689">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="55d74-1690">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="55d74-1690">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="55d74-1691">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="55d74-1691">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="55d74-1692">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="55d74-1692">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="55d74-1693">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="55d74-1693">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="55d74-1694">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="55d74-1694">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="55d74-1695">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="55d74-1695">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="55d74-1696">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="55d74-1696">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="55d74-1697">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="55d74-1697">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="55d74-1698">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1698">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="55d74-1699">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1699">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="55d74-1700">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1700">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="55d74-1701">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1701">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="55d74-1702">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1702">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="55d74-1703">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1703">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="55d74-1704">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1704">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="55d74-1705">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1705">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="55d74-1706">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1706">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="55d74-1707">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1707">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="55d74-1708">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1708">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="55d74-1709">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1709">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="55d74-1710">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1710">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1711">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1711">Profile</span></span>

* <span data-ttu-id="55d74-1712">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1712">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="55d74-1713">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1713">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="55d74-1714">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1714">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="55d74-1715">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1715">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="55d74-1716">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1716">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="55d74-1717">RDBMS</span><span class="sxs-lookup"><span data-stu-id="55d74-1717">RDBMS</span></span>

* <span data-ttu-id="55d74-1718">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="55d74-1718">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="55d74-1719">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="55d74-1719">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="55d74-1720">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="55d74-1720">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="55d74-1721">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="55d74-1721">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1722">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1722">Resource</span></span>

* <span data-ttu-id="55d74-1723">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1723">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="55d74-1724">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1724">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="55d74-1725">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1725">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="55d74-1726">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1726">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="55d74-1727">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="55d74-1727">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="55d74-1728">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1728">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="55d74-1729">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="55d74-1729">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="55d74-1730">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1730">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1731">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1731">Role</span></span>

* <span data-ttu-id="55d74-1732">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1732">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="55d74-1733">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="55d74-1733">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="55d74-1734">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1734">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="55d74-1735">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1735">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="55d74-1736">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1736">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="55d74-1737">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="55d74-1737">Service Fabric</span></span>
* <span data-ttu-id="55d74-1738">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="55d74-1738">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="55d74-1739">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="55d74-1739">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="55d74-1740">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="55d74-1740">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1741">SQL</span></span>

* <span data-ttu-id="55d74-1742">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1742">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="55d74-1743">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1743">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="55d74-1744">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1744">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1745">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1745">Storage</span></span>

* <span data-ttu-id="55d74-1746">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="55d74-1746">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="55d74-1747">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="55d74-1747">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="55d74-1748">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="55d74-1748">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="55d74-1749">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1749">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="55d74-1750">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="55d74-1750">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="55d74-1751">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="55d74-1751">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1752">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1752">VM</span></span>

* <span data-ttu-id="55d74-1753">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1753">Support configuring nsg</span></span>
* <span data-ttu-id="55d74-1754">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1754">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="55d74-1755">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1755">Support managed service identities</span></span>
* <span data-ttu-id="55d74-1756">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1756">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="55d74-1757">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1757">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="55d74-1758">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="55d74-1758">May 10, 2017</span></span>

<span data-ttu-id="55d74-1759">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="55d74-1759">Version 2.0.6</span></span>

* <span data-ttu-id="55d74-1760">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="55d74-1760">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="55d74-1761">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1761">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="55d74-1762">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="55d74-1762">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="55d74-1763">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="55d74-1763">Include Cognitive Services module</span></span>
* <span data-ttu-id="55d74-1764">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="55d74-1764">Include Service Fabric module</span></span>
* <span data-ttu-id="55d74-1765">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="55d74-1765">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="55d74-1766">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1766">Add support for CDN commands</span></span>
* <span data-ttu-id="55d74-1767">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-1767">Remove Container module</span></span>
* <span data-ttu-id="55d74-1768">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="55d74-1768">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="55d74-1769">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="55d74-1769">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="55d74-1770">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1770">Core</span></span>

* <span data-ttu-id="55d74-1771">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="55d74-1771">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="55d74-1772">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="55d74-1772">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="55d74-1773">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="55d74-1773">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="55d74-1774">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="55d74-1774">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="55d74-1775">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="55d74-1775">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="55d74-1776">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="55d74-1776">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="55d74-1777">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="55d74-1777">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="55d74-1778">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="55d74-1778">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="55d74-1779">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="55d74-1779">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="55d74-1780">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="55d74-1780">core: Improved performance</span></span>
* <span data-ttu-id="55d74-1781">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1781">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="55d74-1782">core: 클라우드 구성 - '관리' 엔드포인트를 설정하지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="55d74-1782">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1783">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1783">ACS</span></span>

* <span data-ttu-id="55d74-1784">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1784">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="55d74-1785">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="55d74-1785">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="55d74-1786">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="55d74-1786">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="55d74-1787">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="55d74-1787">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-1788">AppService</span></span>

* <span data-ttu-id="55d74-1789">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="55d74-1789">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="55d74-1790">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1790">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="55d74-1791">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="55d74-1791">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="55d74-1792">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="55d74-1792">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="55d74-1793">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="55d74-1793">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="55d74-1794">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="55d74-1794">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="55d74-1795">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1795">support slot swap with preview</span></span>
* <span data-ttu-id="55d74-1796">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="55d74-1796">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="55d74-1797">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="55d74-1797">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="55d74-1798">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="55d74-1798">CosmosDB</span></span>

* <span data-ttu-id="55d74-1799">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="55d74-1799">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="55d74-1800">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1800">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="55d74-1801">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1801">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="55d74-1802">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1802">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="55d74-1803">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="55d74-1803">Data Lake Analytics</span></span>

* <span data-ttu-id="55d74-1804">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1804">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="55d74-1805">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1805">Add support for new catalog item type: package.</span></span> <span data-ttu-id="55d74-1806">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="55d74-1806">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="55d74-1807">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="55d74-1807">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="55d74-1808">테이블</span><span class="sxs-lookup"><span data-stu-id="55d74-1808">Table</span></span>
  * <span data-ttu-id="55d74-1809">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="55d74-1809">Table valued function</span></span>
  * <span data-ttu-id="55d74-1810">보기</span><span class="sxs-lookup"><span data-stu-id="55d74-1810">View</span></span>
  * <span data-ttu-id="55d74-1811">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="55d74-1811">Table Statistics.</span></span> <span data-ttu-id="55d74-1812">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="55d74-1812">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="55d74-1813">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="55d74-1813">Data Lake Store</span></span>

* <span data-ttu-id="55d74-1814">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="55d74-1814">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="55d74-1815">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="55d74-1815">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="55d74-1816">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="55d74-1816">missed help for access show.</span></span> <span data-ttu-id="55d74-1817">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1817">adding it.</span></span> <span data-ttu-id="55d74-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="55d74-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="55d74-1819">찾기</span><span class="sxs-lookup"><span data-stu-id="55d74-1819">Find</span></span>

* <span data-ttu-id="55d74-1820">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="55d74-1820">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="55d74-1821">KeyVault</span><span class="sxs-lookup"><span data-stu-id="55d74-1821">KeyVault</span></span>

* <span data-ttu-id="55d74-1822">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1822">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="55d74-1823">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1823">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="55d74-1824">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1824">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="55d74-1825">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1825">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="55d74-1826">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="55d74-1826">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="55d74-1827">랩</span><span class="sxs-lookup"><span data-stu-id="55d74-1827">Lab</span></span>

* <span data-ttu-id="55d74-1828">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1828">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="55d74-1829">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1829">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="55d74-1830">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="55d74-1830">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="55d74-1831">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="55d74-1831">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="55d74-1832">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1832">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="55d74-1833">모니터</span><span class="sxs-lookup"><span data-stu-id="55d74-1833">Monitor</span></span>

* <span data-ttu-id="55d74-1834">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="55d74-1834">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="55d74-1835">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="55d74-1835">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="55d74-1836">네트워크</span><span class="sxs-lookup"><span data-stu-id="55d74-1836">Network</span></span>

* <span data-ttu-id="55d74-1837">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1837">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="55d74-1838">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1838">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="55d74-1839">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1839">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="55d74-1840">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1840">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="55d74-1841">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1841">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="55d74-1842">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1842">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="55d74-1843">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1843">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="55d74-1844">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1844">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="55d74-1845">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1845">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="55d74-1846">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1846">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="55d74-1847">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="55d74-1847">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="55d74-1848">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1848">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="55d74-1849">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1849">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="55d74-1850">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1850">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="55d74-1851">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="55d74-1851">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="55d74-1852">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1852">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="55d74-1853">프로필</span><span class="sxs-lookup"><span data-stu-id="55d74-1853">Profile</span></span>

* <span data-ttu-id="55d74-1854">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="55d74-1854">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="55d74-1855">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="55d74-1855">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="55d74-1856">Redis</span><span class="sxs-lookup"><span data-stu-id="55d74-1856">Redis</span></span>

* <span data-ttu-id="55d74-1857">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1857">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="55d74-1858">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="55d74-1858">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="55d74-1859">리소스</span><span class="sxs-lookup"><span data-stu-id="55d74-1859">Resource</span></span>

* <span data-ttu-id="55d74-1860">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="55d74-1860">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="55d74-1861">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="55d74-1861">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="55d74-1862">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="55d74-1862">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="55d74-1863">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1863">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="55d74-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="55d74-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="55d74-1865">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1865">Add docs for az lock update.</span></span> <span data-ttu-id="55d74-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="55d74-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="55d74-1867">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1867">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="55d74-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="55d74-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="55d74-1869">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1869">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="55d74-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="55d74-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="55d74-1871">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="55d74-1871">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="55d74-1872">역할</span><span class="sxs-lookup"><span data-stu-id="55d74-1872">Role</span></span>

* <span data-ttu-id="55d74-1873">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="55d74-1873">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="55d74-1874">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="55d74-1874">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="55d74-1875">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="55d74-1875">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="55d74-1876">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="55d74-1876">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="55d74-1877">SQL</span><span class="sxs-lookup"><span data-stu-id="55d74-1877">SQL</span></span>

* <span data-ttu-id="55d74-1878">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="55d74-1878">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="55d74-1879">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="55d74-1879">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="55d74-1880">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1880">Storage</span></span>

* <span data-ttu-id="55d74-1881">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="55d74-1881">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="55d74-1882">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1882">Add support for incremental blob copy</span></span>
* <span data-ttu-id="55d74-1883">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1883">Add support for large block blob upload</span></span>
* <span data-ttu-id="55d74-1884">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="55d74-1884">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1885">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1885">VM</span></span>

* <span data-ttu-id="55d74-1886">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="55d74-1886">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="55d74-1887">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="55d74-1887">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="55d74-1888">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="55d74-1888">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="55d74-1889">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="55d74-1889">az vm/vmss disk</span></span>
  3. <span data-ttu-id="55d74-1890">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1890">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="55d74-1891">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="55d74-1891">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="55d74-1892">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="55d74-1892">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="55d74-1893">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="55d74-1893">April 3, 2017</span></span>

<span data-ttu-id="55d74-1894">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="55d74-1894">Version 2.0.2</span></span>

<span data-ttu-id="55d74-1895">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1895">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="55d74-1896">코어</span><span class="sxs-lookup"><span data-stu-id="55d74-1896">Core</span></span>

* <span data-ttu-id="55d74-1897">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="55d74-1897">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="55d74-1898">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="55d74-1898">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="55d74-1899">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="55d74-1899">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="55d74-1900">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="55d74-1900">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="55d74-1901">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="55d74-1901">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="55d74-1902">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="55d74-1902">Add prompting for missing template parameters.</span></span> <span data-ttu-id="55d74-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="55d74-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="55d74-1904">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1904">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="55d74-1905">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="55d74-1905">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="55d74-1906">ACS</span><span class="sxs-lookup"><span data-stu-id="55d74-1906">ACS</span></span>

* <span data-ttu-id="55d74-1907">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="55d74-1907">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="55d74-1908">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="55d74-1908">Add support for ssh key password prompting.</span></span> <span data-ttu-id="55d74-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="55d74-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="55d74-1910">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="55d74-1910">Add support for windows clusters.</span></span> <span data-ttu-id="55d74-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="55d74-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="55d74-1912">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="55d74-1912">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="55d74-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="55d74-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="55d74-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="55d74-1914">AppService</span></span>

* <span data-ttu-id="55d74-1915">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="55d74-1915">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="55d74-1916">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="55d74-1916">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="55d74-1917">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="55d74-1917">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="55d74-1918">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="55d74-1918">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="55d74-1919">DataLake</span><span class="sxs-lookup"><span data-stu-id="55d74-1919">DataLake</span></span>

* <span data-ttu-id="55d74-1920">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1920">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="55d74-1921">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="55d74-1921">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="55d74-1922">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="55d74-1922">DocuemntDB</span></span>

* <span data-ttu-id="55d74-1923">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="55d74-1923">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="55d74-1924">VM</span><span class="sxs-lookup"><span data-stu-id="55d74-1924">VM</span></span>

* <span data-ttu-id="55d74-1925">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="55d74-1925">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="55d74-1926">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="55d74-1926">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="55d74-1927">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="55d74-1927">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="55d74-1928">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="55d74-1928">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="55d74-1929">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="55d74-1929">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="55d74-1930">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="55d74-1930">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="55d74-1931">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="55d74-1931">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="55d74-1932">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="55d74-1932">February 27, 2017</span></span>

<span data-ttu-id="55d74-1933">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="55d74-1933">Version 2.0.0</span></span>

<span data-ttu-id="55d74-1934">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1934">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="55d74-1935">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="55d74-1935">Container Service (acs)</span></span>
- <span data-ttu-id="55d74-1936">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="55d74-1936">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="55d74-1937">네트워킹</span><span class="sxs-lookup"><span data-stu-id="55d74-1937">Networking</span></span>
- <span data-ttu-id="55d74-1938">Storage</span><span class="sxs-lookup"><span data-stu-id="55d74-1938">Storage</span></span>

<span data-ttu-id="55d74-1939">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1939">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="55d74-1940">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1940">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="55d74-1941">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1941">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="55d74-1942">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1942">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="55d74-1943">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="55d74-1943">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="55d74-1944">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55d74-1944">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="55d74-1945">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="55d74-1945">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="55d74-1946">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="55d74-1946">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="55d74-1947">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="55d74-1947">Provide feedback from the command line with the `az feedback` command</span></span>


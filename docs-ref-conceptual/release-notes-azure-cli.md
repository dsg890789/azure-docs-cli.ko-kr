---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 0eb1ccccdeff8c3d9b97167ee74f3380d983a552
ms.sourcegitcommit: e99b39e2f14a38c9bcae1b2b5921c6d8b464ef31
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/17/2019
ms.locfileid: "72549692"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="7a6b8-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="7a6b8-103">Azure CLI release notes</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="7a6b8-104">2019년 10월 15일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-104">October 15, 2019</span></span>

<span data-ttu-id="7a6b8-105">버전 2.0.75</span><span class="sxs-lookup"><span data-stu-id="7a6b8-105">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-106">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-106">AKS</span></span>

* <span data-ttu-id="7a6b8-107">Kubernetes 버전에서 지원되는 경우 `--load-balancer-sku` 기본값이 `standard`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-107">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="7a6b8-108">Kubernetes 버전에서 지원되는 경우 `--vm-set-type` 기본값이 `virtualmachinescalesets`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-108">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-109">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-109">AMS</span></span>

* <span data-ttu-id="7a6b8-110">[주요 변경 사항] `job start`의 이름이 `job create`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-110">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="7a6b8-111">[주요 변경 사항] UTF8 대신 32자 16진수 문자열을 사용하도록 `content-key-policy create`의 `--ask` 매개 변수가 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-111">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-112">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-112">AppService</span></span>

* <span data-ttu-id="7a6b8-113">`webapp config access-restriction show|set|add|remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-113">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="7a6b8-114">`webapp up`에 더 나은 오류 처리 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-114">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="7a6b8-115">`Isolated` SKU에 대한 지원이 `appservice plan update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-115">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="7a6b8-116">ARM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-116">ARM</span></span>

* <span data-ttu-id="7a6b8-117">json 템플릿에서 여러 줄과 주석을 지원하기 위해 `--handle-extended-json-format` 매개 변수가 `deployment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-117">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="7a6b8-118">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="7a6b8-118">Compute</span></span>

* <span data-ttu-id="7a6b8-119">`--enable-agent` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-119">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="7a6b8-120">영역 사용 시 표준 공용 IP SKU를 자동으로 사용하도록 `vm create`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-120">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="7a6b8-121">VM에 대해 유효한 컴퓨터 이름을 자동으로 만들도록 `vm create`이 변경됨(제공되지 않은 경우)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-121">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="7a6b8-122">VMSS에서 가상 머신의 사용자 지정 컴퓨터 이름 접두사를 지원하기 위해 `vmss create`에 `--computer-name-prefix` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-122">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="7a6b8-123">로그 분석 작업 영역을 자동으로 사용하도록 `vm create`에 `--workspace` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-123">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="7a6b8-124">갤러리 API 버전이 2019-07-01로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-124">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-125">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-125">Core</span></span>

* <span data-ttu-id="7a6b8-126">일반 업데이트 명령에 `--set` 매개 변수에 대한 구문 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-126">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-127">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-127">IoT</span></span>

* <span data-ttu-id="7a6b8-128">`iot hub show`에서 "리소스를 찾을 수 없음" 오류가 잘못 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-128">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-129">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-129">Monitor</span></span>

* <span data-ttu-id="7a6b8-130">CRUD에 대한 지원이 `monitor log-analytics workspace`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-130">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-131">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-131">Network</span></span>

* <span data-ttu-id="7a6b8-132">교차 테넌트 가상 연결에 대한 지원이 `network private-dns link vnet [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-132">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="7a6b8-133">[주요 변경 사항] `--resource-group` 및 `--vnet-name` 매개 변수가 필수 매개 변수가 되도록 `network vnet subnet list`가 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-133">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-134">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-134">SQL</span></span>

* <span data-ttu-id="7a6b8-135">관리형 인스턴스에서 AAD 관리자 설정을 지원하는 명령이 `sql mi ad-admin`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-135">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-136">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-136">Storage</span></span>

* <span data-ttu-id="7a6b8-137">서비스에서 서비스로 복사하는 동안 액세스 계층을 유지하기 위해 `storage copy`에 `--preserve-s2s-access-tier` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-137">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="7a6b8-138">스토리지 계정에 대한 대용량 파일 공유를 지원하기 위해 `storage account [create|update]`에 `--enable-large-file-share` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-138">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="7a6b8-139">2019년 9월 24일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-139">September 24, 2019</span></span>

<span data-ttu-id="7a6b8-140">버전 2.0.74</span><span class="sxs-lookup"><span data-stu-id="7a6b8-140">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-141">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-141">ACR</span></span>

* <span data-ttu-id="7a6b8-142">`acr config retention update`에 필수 `--type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-142">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="7a6b8-143">[주요 변경 사항] `--name -n` 매개 변수가 `acr config` 명령 그룹에 대한 `--registry -r `로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-143">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-144">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-144">AKS</span></span>

* <span data-ttu-id="7a6b8-145">`aks create` 명령에 `--load-balancer-sku` 매개 변수가 추가되어 SLB로 AKS 클러스터를 만들 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-145">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="7a6b8-146">`aks [create|update]` 명령에 `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` 및 `--load-balancer-outbound-ip-prefixes` 매개 변수가 추가되어 SLB로 AKS 클러스터의 부하 분산 장치 프로필을 업데이트할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-146">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="7a6b8-147">`aks create` 명령에 `--vm-set-type` 매개 변수가 추가되어 AKS 클러스터의 vm 유형을 지정할 수 있게 되었습니다(vmas 또는 vmss).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-147">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="7a6b8-148">ARM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-148">ARM</span></span>

* <span data-ttu-id="7a6b8-149">json 템플릿에서 여러 줄과 주석을 지원할 수 있도록 `group deployment create` 명령에 `--handle-extended-json-format` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-149">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="7a6b8-150">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="7a6b8-150">Compute</span></span>

* <span data-ttu-id="7a6b8-151">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss [create|update]` 명령에 `--terminate-notification-time` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-151">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="7a6b8-152">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss update` 명령에 `--enable-terminate-notification` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-152">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="7a6b8-153">`[vm|vmss] create` 명령에 `--priority,` `--eviction-policy,` `--max-billing` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-153">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="7a6b8-154">디스크 업로드의 정확한 크기를 지정할 수 있도록 `disk create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-154">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="7a6b8-155">관리 디스크의 증분 스냅샷에 대한 지원이 `snapshot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-155">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7a6b8-156">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-156">Cosmos DB</span></span>

* <span data-ttu-id="7a6b8-157">키, 읽기 전용 키 또는 연결 문자열을 표시하도록 `cosmosdb keys list` 명령에 `--type <key-type>` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-157">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="7a6b8-158">`cosmosdb keys regenerate` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-158">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="7a6b8-159">[사용 되지 않음] `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` 및 `cosmosdb list-read-only-keys` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-159">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7a6b8-160">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-160">EventGrid</span></span>

* <span data-ttu-id="7a6b8-161">오른쪽 매개 변수를 참조하도록 엔드포인트 도움말 텍스트가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-161">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="7a6b8-162">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-162">Key Vault</span></span>

* <span data-ttu-id="7a6b8-163">테넌트(`login -t`)로 로그인하면 `keyvault create`가 실패할 수 있는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-163">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-164">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-164">Monitor</span></span>

* <span data-ttu-id="7a6b8-165">`--condition` 인수에서 `:` 문자가 허용되지 않아 `monitor metrics alert create` 할 수 없는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-165">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="7a6b8-166">정책</span><span class="sxs-lookup"><span data-stu-id="7a6b8-166">Policy</span></span>

* <span data-ttu-id="7a6b8-167">정책 API 버전 2019-06-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-167">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="7a6b8-168">`policy assignment create` 명령에 `--enforcement-mode` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-168">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-169">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-169">Storage</span></span>

* <span data-ttu-id="7a6b8-170">`az storage copy` 명령에 `--blob-type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-170">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="7a6b8-171">2019년 9월 10일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-171">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-172">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-172">ACR</span></span>

* <span data-ttu-id="7a6b8-173">보존 정책을 구성하는 `acr config retention` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-173">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-174">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-174">AKS</span></span>

* <span data-ttu-id="7a6b8-175">다음 명령을 통해 ACR 통합 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-175">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="7a6b8-176">AKS 클러스터에 ACR을 연결하는 `--attach-acr` 매개 변수가 `aks [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-176">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="7a6b8-177">AKS 클러스터에서 ACR을 분리하는 `--detach-acr` 매개 변수가 `aks update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-177">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="7a6b8-178">ARM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-178">ARM</span></span>

* <span data-ttu-id="7a6b8-179">2019-05-10 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-179">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-180">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-180">Batch</span></span>

* <span data-ttu-id="7a6b8-181">`batch pool create`에 대한 `--json-file`에 새 JSON 구성 설정이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-181">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="7a6b8-182">파일 시스템을 탑재하기 위한 `MountConfigurations`가 추가됨(자세한 내용은 https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-182">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="7a6b8-183">`NetworkConfiguration`에 풀의 공용 IP에 대한 선택적 속성 `publicIPs`가 추가됨(자세한 내용은 https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-183">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="7a6b8-184">공유 이미지 갤러리에 대한 지원이 `--image`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-184">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="7a6b8-185">[주요 변경 사항] `batch pool create`의 기본값 `--start-task-wait-for-success`가 `true`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-185">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="7a6b8-186">[주요 변경 사항] `AutoUserSpecification`의 `Scope` 기본값이 항상 풀이 되도록 변경됨(Windows 노드에서는 `Task`, Linux 노드에서는 `Pool`이었음)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-186">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="7a6b8-187">이 인수는 `--json-file`을 사용하여 JSON 구성에서만 설정 가능</span><span class="sxs-lookup"><span data-stu-id="7a6b8-187">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-188">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-188">HDInsight</span></span>

* <span data-ttu-id="7a6b8-189">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-189">GA release</span></span>
* <span data-ttu-id="7a6b8-190">[주요 변경 사항] `az hdinsight resize`의 `--workernode-count/-c` 매개 변수가 필수 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-190">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="7a6b8-191">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-191">Key Vault</span></span>

* <span data-ttu-id="7a6b8-192">네트워크 규칙에서 서브넷을 삭제할 수 없는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-192">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="7a6b8-193">중복 서브넷 및 IP 주소를 네트워크 규칙에 추가할 수 있는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-193">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-194">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-194">Network</span></span>

* <span data-ttu-id="7a6b8-195">트래픽 분석 간격 값을 설정하는 `--interval` 매개 변수가 `network watcher flow-log`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-195">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="7a6b8-196">게이트웨이 ID를 관리하는 `network application-gateway identity`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-196">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="7a6b8-197">Key Vault ID 설정 지원이 `network application-gateway ssl-cert`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-197">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="7a6b8-198">`network express-route peering peer-connection [show|list]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-198">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="7a6b8-199">정책</span><span class="sxs-lookup"><span data-stu-id="7a6b8-199">Policy</span></span>

* <span data-ttu-id="7a6b8-200">2019-01-01 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-200">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="7a6b8-201">2019년 8월 27일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-201">August 27, 2019</span></span>

<span data-ttu-id="7a6b8-202">버전 2.0.72</span><span class="sxs-lookup"><span data-stu-id="7a6b8-202">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-203">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-203">ACR</span></span>

* <span data-ttu-id="7a6b8-204">[주요 변경 사항] `classic` SKU 지원이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-204">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="7a6b8-205">API Management</span><span class="sxs-lookup"><span data-stu-id="7a6b8-205">API Management</span></span>

* <span data-ttu-id="7a6b8-206">[미리 보기] `apim` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-206">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-207">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-207">AppService</span></span>

* <span data-ttu-id="7a6b8-208">슬롯 지정 시의 `webapp webjob continuous start` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-208">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="7a6b8-209">`env` 폴더를 검색하고 배포에 사용된 파일에서 제거하도록 `webapp up`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-209">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-210">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-210">Keyvault</span></span>

* <span data-ttu-id="7a6b8-211">`--expires` 인수를 무시한 `keyvault secret set`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-211">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-212">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-212">Network</span></span>

* <span data-ttu-id="7a6b8-213">`--private-ip-address-version` 인수에 IPv6 주소 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-213">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="7a6b8-214">프라이빗 엔드포인트를 관리하기 위한 새 `network private-endpoint [create|update|list-types]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-214">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="7a6b8-215">`network private-link-service` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-215">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="7a6b8-216">`--private-endpoint-network-policies` 및 `--private-link-service-network-policies` 인수를 `network vnet subnet update`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-216">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="7a6b8-217">RBAC</span><span class="sxs-lookup"><span data-stu-id="7a6b8-217">RBAC</span></span>

* <span data-ttu-id="7a6b8-218">홈페이지가 업데이트되지 않는 `ad app update --homepage` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-218">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7a6b8-219">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-219">ServiceFabric</span></span>

* <span data-ttu-id="7a6b8-220">대/소문자가 혼합된 Key Vault 이름 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-220">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="7a6b8-221">Key Vault에서 인증서를 사용할 때 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-221">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="7a6b8-222">PFX 인증서 파일의 사용 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-222">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="7a6b8-223">Key Vault 리소스 그룹이 지정되지 않은 `sf cluster certificate add` 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-223">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="7a6b8-224">`sf cluster set`가 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-224">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="7a6b8-225">SignalR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-225">SignalR</span></span>

* <span data-ttu-id="7a6b8-226">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-226">Added new commands:</span></span>
  * <span data-ttu-id="7a6b8-227">`signalr cors`: SignalR CORS 관리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-227">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="7a6b8-228">`signalr restart`: SignalR Service 다시 시작</span><span class="sxs-lookup"><span data-stu-id="7a6b8-228">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="7a6b8-229">`signalr update`: SignalR Service 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-229">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="7a6b8-230">`--service-mode` 인수를 `signalr create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-230">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-231">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-231">Storage</span></span>

* <span data-ttu-id="7a6b8-232">`storage account revoke-delegation-keys` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-232">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="7a6b8-233">2019년 8월 13일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-233">August 13, 2019</span></span>

<span data-ttu-id="7a6b8-234">버전 2.0.71</span><span class="sxs-lookup"><span data-stu-id="7a6b8-234">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-235">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-235">AppService</span></span>

* <span data-ttu-id="7a6b8-236">슬롯에 대해 `webapp webjob continuous` 명령이 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-236">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-237">BotService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-237">BotService</span></span>

* <span data-ttu-id="7a6b8-238">[주요 변경 사항] v3 SDK 봇 만들기에 대한 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-238">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="7a6b8-239">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7a6b8-239">CognitiveServices</span></span>

* <span data-ttu-id="7a6b8-240">`cognitiveservices account network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-240">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7a6b8-241">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-241">Cosmos DB</span></span>

* <span data-ttu-id="7a6b8-242">여러 쓰기 위치 업데이트 시의 경고가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-242">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="7a6b8-243">CosmosDB SQL, MongoDB, Cassandra, Gremlin 및 Table 리소스 및 리소스 처리량에 대한 CRUD 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-243">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-244">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-244">HDInsight</span></span>

<span data-ttu-id="7a6b8-245">이 릴리스에는 호환성이 손상되는 변경이 많이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-245">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="7a6b8-246">[주요 변경 사항] `hdinsight create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-246">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="7a6b8-247">이름이 `--storage-default-container`에서 `--storage-container`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-247">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="7a6b8-248">이름이 `--storage-default-filesystem`에서 `--storage-filesystem`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-248">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="7a6b8-249">[주요 변경 사항] `application create`의 `--name` 인수에서 클러스터 이름 대신 애플리케이션 이름을 나타내도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-249">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="7a6b8-250">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 `application create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-250">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="7a6b8-251">[주요 변경 사항] `application create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-251">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="7a6b8-252">이름이 `--application-type`에서 `--type`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-252">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="7a6b8-253">이름이 `--marketplace-identifier`에서 `--marketplace-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-253">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="7a6b8-254">이름이 `--https-endpoint-access-mode`에서 `--access-mode`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-254">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="7a6b8-255">이름이 `--https-endpoint-destination-port`에서 `--destination-port`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-255">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="7a6b8-256">[주요 변경 사항] `application create`에 대한 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-256">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="7a6b8-257">[호환성이 손상되는 변경] `hdinsight resize`에 대한 이름이 `--target-instance-count`에서 `--workernode-count`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-257">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="7a6b8-258">[주요 변경 사항] `hdinsight script-action` 그룹의 모든 명령에서 `--name` 매개 변수를 스크립트 작업 이름으로 사용하도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-258">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="7a6b8-259">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 모든 `hdinsight script-action` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-259">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="7a6b8-260">[주요 변경 사항] 모든 `hdinsight script-action` 명령에 대한 이름이 `--script-execution-id`에서 `--execution-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-260">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="7a6b8-261">[주요 변경 사항] `hdinsight script-action show`에서 `hdinsight script-action show-execution-details`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-261">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="7a6b8-262">[호환성이 손상되는 변경] `hdinsight script-action execute --roles`의 매개 변수에서 쉼표로 구분하는 대신 공백으로 구분하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-262">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="7a6b8-263">[주요 변경 사항] `hdinsight script-action list`의 `--persisted` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-263">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="7a6b8-264">`hdinsight create --cluster-configurations` 매개 변수에서 로컬 JSON 파일 또는 JSON 문자열에 대한 경로를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-264">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="7a6b8-265">명령 `hdinsight script-action list-execution-history` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-265">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="7a6b8-266">`hdinsight monitor enable --workspace`에서 Log Analytics 작업 영역 ID 또는 작업 영역 이름을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-266">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="7a6b8-267">작업 영역 ID가 매개 변수로 제공되는 경우 필요한 `hdinsight monitor enable --primary-key` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-267">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="7a6b8-268">도움말 메시지에 대한 추가 예제 및 업데이트된 설명이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-268">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-269">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-269">Interactive</span></span>

* <span data-ttu-id="7a6b8-270">로드 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-270">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="7a6b8-271">kubernetes</span><span class="sxs-lookup"><span data-stu-id="7a6b8-271">Kubernetes</span></span>

* <span data-ttu-id="7a6b8-272">대시보드 컨테이너 포트에서 `https`를 사용하는 경우 `https`를 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-272">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-273">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-273">Network</span></span>

* <span data-ttu-id="7a6b8-274">`--yes` 인수가 `network dns record-set cname delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-274">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-275">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-275">Profile</span></span>

* <span data-ttu-id="7a6b8-276">리소스 액세스 토큰을 가져오기 위해 `--resource-type` 인수가 `account get-access-token`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-276">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="7a6b8-277">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-277">ServiceFabric</span></span>

* <span data-ttu-id="7a6b8-278">sf 클러스터를 만드는 데 지원되는 모든 os 버전이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-278">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="7a6b8-279">기본 인증서 유효성 검사 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-279">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-280">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-280">Storage</span></span>

* <span data-ttu-id="7a6b8-281">명령 `storage copy` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-281">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="7a6b8-282">2019년 7월 30일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-282">July 30, 2019</span></span>

<span data-ttu-id="7a6b8-283">버전 2.0.70</span><span class="sxs-lookup"><span data-stu-id="7a6b8-283">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-284">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-284">ACR</span></span>

* <span data-ttu-id="7a6b8-285">#9952 문제(`acr pack build` 명령의 회귀)가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-285">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="7a6b8-286">`acr pack build`의 기본 작성기 이미지 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-286">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-287">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-287">Appservice</span></span>

* <span data-ttu-id="7a6b8-288">리소스를 찾을 수 없는 경우 메시지를 표시 하도록 `webapp config ssl`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-288">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="7a6b8-289">`functionapp create`에서 `Standard_RAGRS` 스토리지 계정 유형을 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-289">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="7a6b8-290">이전 버전의 python을 사용하여 실행할 경우 `webapp up`이(가) 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-290">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-291">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-291">Network</span></span>

* <span data-ttu-id="7a6b8-292">`network nic ip-config add`에서 잘못된 매개 변수 `--ids` 제거됨(#9861 수정)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-292">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="7a6b8-293">#9604 수정.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-293">Fixes #9604.</span></span> <span data-ttu-id="7a6b8-294">사용자가 신뢰할 수 있는 루트 인증서를 연결할 수 있도록 `network application-gateway http-settings [create|update]`에 `--root-certs` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-294">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="7a6b8-295">`network dns record-set ns create`(#9965)에 대해 인수 `--subscription`을 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-295">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="7a6b8-296">RBAC</span><span class="sxs-lookup"><span data-stu-id="7a6b8-296">RBAC</span></span>

* <span data-ttu-id="7a6b8-297">`user update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-297">Added `user update` command</span></span>
* <span data-ttu-id="7a6b8-298">[사용 되지 않음] 사용자 관련 명령 중 `--upn-or-object-id`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-298">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="7a6b8-299">대체 인수 `--id` 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-299">Use replacement argument `--id`</span></span>
* <span data-ttu-id="7a6b8-300">사용자 관련 명령에 `--id` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-300">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-301">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-301">SQL</span></span>

* <span data-ttu-id="7a6b8-302">관리형 인스턴스 키 및 TDE 보호기에 대한 관리 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-302">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-303">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-303">Storage</span></span>

* <span data-ttu-id="7a6b8-304">`storage remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-304">Added `storage remove` command</span></span>
* <span data-ttu-id="7a6b8-305">`storage blob update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-305">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-306">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-306">VM</span></span>

* <span data-ttu-id="7a6b8-307">새로운 API 버전을 사용하여 영역 세부 정보를 출력하도록 `list-skus`를 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-307">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="7a6b8-308">`vmss create`에 대한 `--single-placement-group`의 기본값을 `false`로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-308">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="7a6b8-309">`[snapshot|disk] create`에 대한 ZRS 스토리지 SKU를 선택하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-309">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="7a6b8-310">전용 호스트를 지원하는 새로운 명령 그룹 `vm host`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-310">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="7a6b8-311">VM 전용 호스트를 설정하기 위해 `vm create`에 매개 변수 `--host` 및 `--host-group` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-311">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="7a6b8-312">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-312">July 16, 2019</span></span>

<span data-ttu-id="7a6b8-313">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="7a6b8-313">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-314">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-314">Appservice</span></span>

* <span data-ttu-id="7a6b8-315">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-315">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="7a6b8-316">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-316">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="7a6b8-317">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-317">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-318">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-318">Core</span></span>

* <span data-ttu-id="7a6b8-319">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-319">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-320">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-320">Batch</span></span>

* <span data-ttu-id="7a6b8-321">[주요 변경 사항] `batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="7a6b8-321">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="7a6b8-322">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-322">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="7a6b8-323">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-323">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="7a6b8-324">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-324">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7a6b8-325">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7a6b8-325">Eventhubs</span></span>

* <span data-ttu-id="7a6b8-326">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-326">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-327">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-327">RDBMS</span></span>

* <span data-ttu-id="7a6b8-328">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-328">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="7a6b8-329">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-329">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="7a6b8-330">릴레이</span><span class="sxs-lookup"><span data-stu-id="7a6b8-330">Relay</span></span>

* <span data-ttu-id="7a6b8-331">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-331">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="7a6b8-332">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-332">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7a6b8-333">Servicebus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-333">Servicebus</span></span>

* <span data-ttu-id="7a6b8-334">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-334">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-335">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-335">Storage</span></span>

* <span data-ttu-id="7a6b8-336">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-336">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="7a6b8-337">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-337">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="7a6b8-338">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-338">July 2, 2019</span></span>

<span data-ttu-id="7a6b8-339">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="7a6b8-339">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-340">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-340">Core</span></span>

* <span data-ttu-id="7a6b8-341">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-341">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="7a6b8-342">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-342">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="7a6b8-343">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-343">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-344">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-344">ACR</span></span>

* <span data-ttu-id="7a6b8-345">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-345">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-346">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-346">Appservice</span></span>

* <span data-ttu-id="7a6b8-347">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-347">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="7a6b8-348">[주요 변경 사항] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-348">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="7a6b8-349">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-349">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="7a6b8-350">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-350">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7a6b8-351">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-351">Cosmos DB</span></span>

* <span data-ttu-id="7a6b8-352">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-352">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="7a6b8-353">DLS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-353">DLS</span></span>

* <span data-ttu-id="7a6b8-354">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-354">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="7a6b8-355">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="7a6b8-355">Feedback</span></span>

* <span data-ttu-id="7a6b8-356">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-356">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-357">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-357">HDInsight</span></span>

* <span data-ttu-id="7a6b8-358">[주요 변경 사항] `oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-358">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="7a6b8-359">[주요 변경 사항] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-359">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="7a6b8-360">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-360">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="7a6b8-361">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-361">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="7a6b8-362">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-362">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="7a6b8-363">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-363">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="7a6b8-364">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-364">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="7a6b8-365">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-365">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="7a6b8-366">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-366">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="7a6b8-367">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-367">Managed Services</span></span>

* <span data-ttu-id="7a6b8-368">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="7a6b8-368">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-369">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-369">Profile</span></span>
* <span data-ttu-id="7a6b8-370">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-370">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="7a6b8-371">RBAC</span><span class="sxs-lookup"><span data-stu-id="7a6b8-371">RBAC</span></span>

* <span data-ttu-id="7a6b8-372">[주요 변경 사항] `create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-372">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="7a6b8-373">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-373">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="7a6b8-374">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-374">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="7a6b8-375">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-375">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-376">RDBMS</span></span>

* <span data-ttu-id="7a6b8-377">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-377">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-378">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-378">SQL</span></span>

* <span data-ttu-id="7a6b8-379">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-379">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-380">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-380">Storage</span></span>

* <span data-ttu-id="7a6b8-381">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-381">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="7a6b8-382">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-382">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="7a6b8-383">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-383">VM</span></span>

* <span data-ttu-id="7a6b8-384">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-384">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="7a6b8-385">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-385">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="7a6b8-386">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-386">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="7a6b8-387">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-387">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="7a6b8-388">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-388">June 18, 2019</span></span>

<span data-ttu-id="7a6b8-389">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="7a6b8-389">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-390">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-390">Core</span></span>

<span data-ttu-id="7a6b8-391">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-391">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="7a6b8-392">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-392">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="7a6b8-393">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-393">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="7a6b8-394">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-394">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="7a6b8-395">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-395">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="7a6b8-396">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-396">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="7a6b8-397">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-397">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-398">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-398">ACR</span></span>
* <span data-ttu-id="7a6b8-399">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-399">Added 'acr check-health' command</span></span>
* <span data-ttu-id="7a6b8-400">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="7a6b8-400">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-401">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-401">ACS</span></span>
* <span data-ttu-id="7a6b8-402">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="7a6b8-402">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-403">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-403">AMS</span></span>
* <span data-ttu-id="7a6b8-404">[주요 변경 사항] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-404">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-405">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-405">AppService</span></span>
* <span data-ttu-id="7a6b8-406">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-406">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="7a6b8-407">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-407">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="7a6b8-408">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-408">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="7a6b8-409">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-409">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="7a6b8-410">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-410">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="7a6b8-411">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-411">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-412">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-412">Batch</span></span>
* <span data-ttu-id="7a6b8-413">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-413">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-414">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-414">BatchAI</span></span>
* <span data-ttu-id="7a6b8-415">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-415">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-416">BotService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-416">BotService</span></span>
* <span data-ttu-id="7a6b8-417">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-417">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-418">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-418">CosmosDB</span></span>
* <span data-ttu-id="7a6b8-419">[사용 되지 않음] `cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-419">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="7a6b8-420">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="7a6b8-420">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="7a6b8-421">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-421">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="7a6b8-422">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-422">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7a6b8-423">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-423">EventGrid</span></span>
* <span data-ttu-id="7a6b8-424">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-424">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="7a6b8-425">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-425">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="7a6b8-426">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-426">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="7a6b8-427">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-427">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="7a6b8-428">[주요 변경 사항] `eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-428">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-429">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-429">HDInsight</span></span>
* <span data-ttu-id="7a6b8-430">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-430">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-431">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-431">IoT</span></span>
* <span data-ttu-id="7a6b8-432">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-432">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="7a6b8-433">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-433">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-434">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-434">Network</span></span>
* <span data-ttu-id="7a6b8-435">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-435">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="7a6b8-436">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-436">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="7a6b8-437">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-437">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="7a6b8-438">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-438">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-439">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-439">Resource</span></span>
* <span data-ttu-id="7a6b8-440">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-440">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="7a6b8-441">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-441">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="7a6b8-442">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-442">ServiceBus</span></span>
* <span data-ttu-id="7a6b8-443">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-443">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-444">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-444">SQL</span></span>
* <span data-ttu-id="7a6b8-445">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-445">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="7a6b8-446">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-446">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="7a6b8-447">SQLVm</span><span class="sxs-lookup"><span data-stu-id="7a6b8-447">SQLVm</span></span>
* <span data-ttu-id="7a6b8-448">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-448">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="7a6b8-449">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-449">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-450">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-450">Storage</span></span>
* <span data-ttu-id="7a6b8-451">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-451">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="7a6b8-452">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-452">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-453">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-453">VM</span></span>
* <span data-ttu-id="7a6b8-454">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-454">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="7a6b8-455">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-455">June 4, 2019</span></span>

<span data-ttu-id="7a6b8-456">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="7a6b8-456">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-457">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-457">Core</span></span>
* <span data-ttu-id="7a6b8-458">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-458">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-459">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-459">ACR</span></span>
* <span data-ttu-id="7a6b8-460">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-460">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-461">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-461">ACS</span></span>
* <span data-ttu-id="7a6b8-462">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-462">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="7a6b8-463">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-463">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-464">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-464">Batch</span></span>
* <span data-ttu-id="7a6b8-465">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-465">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-466">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-466">IoT</span></span>
* <span data-ttu-id="7a6b8-467">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-467">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-468">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-468">Network</span></span>
* <span data-ttu-id="7a6b8-469">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-469">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="7a6b8-470">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-470">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="7a6b8-471">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-471">Resource</span></span>
* <span data-ttu-id="7a6b8-472">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-472">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-473">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-473">Role</span></span>
* <span data-ttu-id="7a6b8-474">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-474">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="7a6b8-475">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="7a6b8-475">Compute</span></span>
* <span data-ttu-id="7a6b8-476">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-476">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="7a6b8-477">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-477">May 21, 2019</span></span>

<span data-ttu-id="7a6b8-478">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="7a6b8-478">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-479">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-479">Core</span></span>
* <span data-ttu-id="7a6b8-480">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-480">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="7a6b8-481">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-481">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="7a6b8-482">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-482">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-483">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-483">ACR</span></span>
* <span data-ttu-id="7a6b8-484">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-484">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-485">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-485">ACS</span></span>
* <span data-ttu-id="7a6b8-486">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-486">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-487">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-487">AppService</span></span>
* <span data-ttu-id="7a6b8-488">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-488">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="7a6b8-489">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-489">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="7a6b8-490">[주요 변경 사항] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-490">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="7a6b8-491">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-491">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="7a6b8-492">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-492">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="7a6b8-493">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-493">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="7a6b8-494">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-494">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-495">BotService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-495">BotService</span></span>
* <span data-ttu-id="7a6b8-496">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-496">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="7a6b8-497">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-497">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-498">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-498">Consumption</span></span>
* <span data-ttu-id="7a6b8-499">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-499">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-500">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-500">IoT</span></span>
* <span data-ttu-id="7a6b8-501">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-501">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-502">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-502">Network</span></span>
* [주요 변경 사항]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="7a6b8-504">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-504">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="7a6b8-505">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-505">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-506">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-506">RDBMS</span></span>
* <span data-ttu-id="7a6b8-507">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-507">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="7a6b8-508">RBAC</span><span class="sxs-lookup"><span data-stu-id="7a6b8-508">RBAC</span></span>
* <span data-ttu-id="7a6b8-509">`role assignment`에 관리 그룹 범위 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-509">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-510">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-510">Storage</span></span>
* <span data-ttu-id="7a6b8-511">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-511">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="7a6b8-512">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="7a6b8-512">Compute</span></span>
* <span data-ttu-id="7a6b8-513">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-513">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="7a6b8-514">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-514">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="7a6b8-515">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-515">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="7a6b8-516">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-516">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="7a6b8-517">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-517">May 6, 2019</span></span>

<span data-ttu-id="7a6b8-518">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="7a6b8-518">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-519">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-519">ACS</span></span>
* <span data-ttu-id="7a6b8-520">[주요 변경 사항] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-520">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="7a6b8-521">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-521">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="7a6b8-522">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-522">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="7a6b8-523">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-523">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-524">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-524">Appservice</span></span>
* <span data-ttu-id="7a6b8-525">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-525">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="7a6b8-526">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-526">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="7a6b8-527">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-527">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="7a6b8-528">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-528">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="7a6b8-529">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-529">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="7a6b8-530">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-530">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="7a6b8-531">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-531">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="7a6b8-532">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-532">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="7a6b8-533">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-533">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="7a6b8-534">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-534">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-535">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-535">Batch</span></span>
* <span data-ttu-id="7a6b8-536">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-536">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-537">Botservice</span><span class="sxs-lookup"><span data-stu-id="7a6b8-537">Botservice</span></span>
* <span data-ttu-id="7a6b8-538">[주요 변경 사항] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-538">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="7a6b8-539">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-539">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="7a6b8-540">[주요 변경 사항] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-540">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="7a6b8-541">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-541">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="7a6b8-542">[주요 변경 사항] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-542">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="7a6b8-543">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-543">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="7a6b8-544">[주요 변경 사항] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-544">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="7a6b8-545">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-545">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="7a6b8-546">[주요 변경 사항] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-546">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="7a6b8-547">[주요 변경 사항] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-547">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="7a6b8-548">[주요 변경 사항] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-548">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="7a6b8-549">[주요 변경 사항] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-549">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="7a6b8-550">[주요 변경 사항] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-550">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="7a6b8-551">[주요 변경 사항] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-551">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="7a6b8-552">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-552">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="7a6b8-553">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-553">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="7a6b8-554">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-554">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7a6b8-555">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-555">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="7a6b8-556">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-556">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="7a6b8-557">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-557">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="7a6b8-558">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-558">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="7a6b8-559">구성</span><span class="sxs-lookup"><span data-stu-id="7a6b8-559">Configure</span></span>
* <span data-ttu-id="7a6b8-560">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-560">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7a6b8-561">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7a6b8-561">Eventhubs</span></span>
* <span data-ttu-id="7a6b8-562">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-562">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7a6b8-563">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-563">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-564">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-564">Network</span></span>
* <span data-ttu-id="7a6b8-565">[주요 변경 사항] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="7a6b8-565">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="7a6b8-566">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="7a6b8-566">Policy Insights</span></span>
* <span data-ttu-id="7a6b8-567">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-567">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-568">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-568">Role</span></span>
* <span data-ttu-id="7a6b8-569">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-569">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="7a6b8-570">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-570">Service Bus</span></span>
* <span data-ttu-id="7a6b8-571">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-571">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="7a6b8-572">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-572">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="7a6b8-573">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-573">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-574">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-574">SQL</span></span>
* <span data-ttu-id="7a6b8-575">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-575">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-576">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-576">VM</span></span>
* <span data-ttu-id="7a6b8-577">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-577">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="7a6b8-578">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-578">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="7a6b8-579">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-579">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="7a6b8-580">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-580">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="7a6b8-581">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-581">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="7a6b8-582">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-582">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="7a6b8-583">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-583">April 23, 2019</span></span>

<span data-ttu-id="7a6b8-584">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="7a6b8-584">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-585">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-585">ACS</span></span>
* <span data-ttu-id="7a6b8-586">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-586">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="7a6b8-587">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-587">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-588">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-588">AMS</span></span>
* <span data-ttu-id="7a6b8-589">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-589">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-590">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-590">AppService</span></span>
* <span data-ttu-id="7a6b8-591">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-591">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="7a6b8-592">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-592">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="7a6b8-593">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-593">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="7a6b8-594">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-594">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="7a6b8-595">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-595">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="7a6b8-596">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-596">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="7a6b8-597">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-597">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="7a6b8-598">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-598">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="7a6b8-599">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-599">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="7a6b8-600">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="7a6b8-600">Deployment Manager</span></span>
* <span data-ttu-id="7a6b8-601">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-601">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="7a6b8-602">랩</span><span class="sxs-lookup"><span data-stu-id="7a6b8-602">Lab</span></span>
* <span data-ttu-id="7a6b8-603">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-603">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-604">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-604">Network</span></span>
* <span data-ttu-id="7a6b8-605">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-605">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-606">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-606">Resource</span></span>
* <span data-ttu-id="7a6b8-607">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="7a6b8-607">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="7a6b8-608">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-608">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="7a6b8-609">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-609">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="7a6b8-610">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-610">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-611">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-611">SQL</span></span>
* <span data-ttu-id="7a6b8-612">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-612">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="7a6b8-613">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-613">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="7a6b8-614">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-614">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="7a6b8-615">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-615">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-616">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-616">Storage</span></span>
* <span data-ttu-id="7a6b8-617">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-617">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-618">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-618">VM</span></span>
* <span data-ttu-id="7a6b8-619">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-619">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="7a6b8-620">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-620">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="7a6b8-621">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-621">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="7a6b8-622">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-622">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-623">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-623">Core</span></span>
* <span data-ttu-id="7a6b8-624">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-624">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-625">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-625">ACR</span></span>
* <span data-ttu-id="7a6b8-626">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-626">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-627">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-627">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="7a6b8-630">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-630">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="7a6b8-631">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-631">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-632">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-632">AppService</span></span>
* <span data-ttu-id="7a6b8-633">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-633">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="7a6b8-634">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-634">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="7a6b8-635">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="7a6b8-635">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="7a6b8-636">[주요 변경 사항] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-636">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="7a6b8-637">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-637">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="7a6b8-638">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-638">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="7a6b8-639">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-639">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-640">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-640">CDN</span></span>
* <span data-ttu-id="7a6b8-641">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-641">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="7a6b8-642">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="7a6b8-642">Feedback</span></span>
* <span data-ttu-id="7a6b8-643">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-643">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="7a6b8-644">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-644">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="7a6b8-645">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-645">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-646">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-646">Monitor</span></span>
* <span data-ttu-id="7a6b8-647">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-647">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="7a6b8-648">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-648">Network</span></span>
* <span data-ttu-id="7a6b8-649">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-649">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="7a6b8-650">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-650">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="7a6b8-651">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-651">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="7a6b8-652">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-652">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="7a6b8-653">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-653">PrivateDNS</span></span>
* <span data-ttu-id="7a6b8-654">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-654">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-655">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-655">Resource</span></span>
* <span data-ttu-id="7a6b8-656">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-656">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-657">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-657">Role</span></span>
* <span data-ttu-id="7a6b8-658">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-658">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="7a6b8-659">[주요 변경 사항] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-659">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-660">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-660">SQL</span></span>
* <span data-ttu-id="7a6b8-661">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-661">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-662">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-662">Storage</span></span>
* <span data-ttu-id="7a6b8-663">[주요 변경 사항] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-663">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="7a6b8-664">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-664">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="7a6b8-665">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-665">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="7a6b8-666">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-666">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="7a6b8-667">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-667">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="7a6b8-668">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-668">Core</span></span>
* <span data-ttu-id="7a6b8-669">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-669">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="7a6b8-670">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-670">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="7a6b8-671">클라우드</span><span class="sxs-lookup"><span data-stu-id="7a6b8-671">Cloud</span></span>
* <span data-ttu-id="7a6b8-672">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-672">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-673">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-673">ACR</span></span>
* <span data-ttu-id="7a6b8-674">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-674">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="7a6b8-675">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-675">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="7a6b8-676">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-676">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="7a6b8-677">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-677">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-678">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-678">AppService</span></span>
* <span data-ttu-id="7a6b8-679">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-679">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="7a6b8-680">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-680">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="7a6b8-681">BOT Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-681">BOT Service</span></span>
* <span data-ttu-id="7a6b8-682">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-682">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="7a6b8-683">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-683">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="7a6b8-684">[주요 변경 사항] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-684">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="7a6b8-685">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-685">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-686">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-686">CDN</span></span>
* <span data-ttu-id="7a6b8-687">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-687">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [주요 변경 사항]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="7a6b8-689">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-689">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7a6b8-690">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-690">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-691">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="7a6b8-691">Cosmosdb</span></span>
* <span data-ttu-id="7a6b8-692">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-692">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="7a6b8-693">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-693">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-694">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-694">Interactive</span></span>
* <span data-ttu-id="7a6b8-695">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-695">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-696">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-696">Monitor</span></span>
* <span data-ttu-id="7a6b8-697">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-697">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-698">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-698">Network</span></span>
* <span data-ttu-id="7a6b8-699">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-699">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-700">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-700">Profile</span></span>
* <span data-ttu-id="7a6b8-701">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-701">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="7a6b8-702">Postgres</span><span class="sxs-lookup"><span data-stu-id="7a6b8-702">Postgres</span></span> 
* <span data-ttu-id="7a6b8-703">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-703">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="7a6b8-704">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-704">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-705">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-705">Resource</span></span>
* <span data-ttu-id="7a6b8-706">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-706">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="7a6b8-707">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-707">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="7a6b8-708">그래프</span><span class="sxs-lookup"><span data-stu-id="7a6b8-708">Graph</span></span>
* <span data-ttu-id="7a6b8-709">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-709">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="7a6b8-710">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-710">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="7a6b8-711">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-711">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="7a6b8-712">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-712">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="7a6b8-713">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-713">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-714">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-714">storage</span></span>
* <span data-ttu-id="7a6b8-715">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-715">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="7a6b8-716">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-716">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="7a6b8-717">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-717">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="7a6b8-718">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-718">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-719">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-719">VM</span></span>
* <span data-ttu-id="7a6b8-720">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-720">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="7a6b8-721">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-721">March 12, 2019</span></span>

<span data-ttu-id="7a6b8-722">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="7a6b8-722">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-723">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-723">Core</span></span>

* <span data-ttu-id="7a6b8-724">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-724">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-725">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-725">ACR</span></span>

* <span data-ttu-id="7a6b8-726">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-726">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-727">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-727">ACS</span></span>

* <span data-ttu-id="7a6b8-728">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-728">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="7a6b8-729">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-729">AppService</span></span>

* <span data-ttu-id="7a6b8-730">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-730">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="7a6b8-731">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-731">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="7a6b8-732">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-732">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="7a6b8-733">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-733">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-734">Botservice</span><span class="sxs-lookup"><span data-stu-id="7a6b8-734">Botservice</span></span>

* <span data-ttu-id="7a6b8-735">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-735">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7a6b8-736">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-736">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="7a6b8-737">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-737">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="7a6b8-738">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-738">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-739">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-739">Container</span></span>

* <span data-ttu-id="7a6b8-740">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-740">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="7a6b8-741">EventHub</span><span class="sxs-lookup"><span data-stu-id="7a6b8-741">EventHub</span></span>

* <span data-ttu-id="7a6b8-742">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-742">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="7a6b8-743">찾기</span><span class="sxs-lookup"><span data-stu-id="7a6b8-743">Find</span></span>

* <span data-ttu-id="7a6b8-744">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-744">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-745">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-745">HDInsight</span></span>

* <span data-ttu-id="7a6b8-746">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-746">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-747">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-747">Network</span></span>

* <span data-ttu-id="7a6b8-748">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-748">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-749">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7a6b8-749">Rdbms</span></span>

* <span data-ttu-id="7a6b8-750">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-750">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-751">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-751">Role</span></span>

* <span data-ttu-id="7a6b8-752">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-752">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="7a6b8-753">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-753">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7a6b8-754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-754">Service Fabric</span></span>

* <span data-ttu-id="7a6b8-755">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-755">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="7a6b8-756">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-756">February 26, 2019</span></span>

<span data-ttu-id="7a6b8-757">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="7a6b8-757">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-758">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-758">Core</span></span>

* <span data-ttu-id="7a6b8-759">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-759">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-760">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-760">ACR</span></span>

* <span data-ttu-id="7a6b8-761">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-761">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="7a6b8-762">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-762">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-763">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-763">ACS</span></span>

* <span data-ttu-id="7a6b8-764">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-764">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-765">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-765">AppService</span></span>

* <span data-ttu-id="7a6b8-766">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-766">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-767">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-767">Batch</span></span>
* <span data-ttu-id="7a6b8-768">[주요 변경 사항] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-768">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="7a6b8-769">[주요 변경 사항] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-769">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="7a6b8-770">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-770">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="7a6b8-771">[주요 변경 사항] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-771">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="7a6b8-772">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-772">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="7a6b8-773">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-773">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-774">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-774">CosmosDB</span></span>

* <span data-ttu-id="7a6b8-775">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-775">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="7a6b8-776">Kusto</span><span class="sxs-lookup"><span data-stu-id="7a6b8-776">Kusto</span></span>

* <span data-ttu-id="7a6b8-777">[주요 변경 사항] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-777">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-778">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-778">Network</span></span>

* <span data-ttu-id="7a6b8-779">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-779">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="7a6b8-780">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-780">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="7a6b8-781">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-781">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="7a6b8-782">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-782">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="7a6b8-783">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-783">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="7a6b8-784">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-784">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="7a6b8-785">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-785">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-786">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-786">Resource</span></span>

* <span data-ttu-id="7a6b8-787">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-787">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="7a6b8-788">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-788">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="7a6b8-789">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-789">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="7a6b8-790">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-790">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="7a6b8-791">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-791">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-792">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-792">Role</span></span>

* <span data-ttu-id="7a6b8-793">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-793">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-794">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-794">VM</span></span>

* <span data-ttu-id="7a6b8-795">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-795">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="7a6b8-796">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-796">February 12, 2019</span></span>

<span data-ttu-id="7a6b8-797">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="7a6b8-797">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-798">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-798">Core</span></span>

* <span data-ttu-id="7a6b8-799">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-799">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="7a6b8-800">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-800">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-801">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-801">ACR</span></span>
* <span data-ttu-id="7a6b8-802">[주요 변경 사항] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-802">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="7a6b8-803">[주요 변경 사항] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-803">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-804">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-804">ACS</span></span>
* <span data-ttu-id="7a6b8-805">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-805">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="7a6b8-806">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-806">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="7a6b8-807">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-807">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-808">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-808">AMS</span></span>
* <span data-ttu-id="7a6b8-809">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-809">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="7a6b8-810">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-810">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-811">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-811">Appservice</span></span>
* <span data-ttu-id="7a6b8-812">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-812">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="7a6b8-813">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-813">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="7a6b8-814">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-814">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="7a6b8-815">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-815">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="7a6b8-816">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-816">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-817">Botservice</span><span class="sxs-lookup"><span data-stu-id="7a6b8-817">Botservice</span></span>
* <span data-ttu-id="7a6b8-818">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-818">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="7a6b8-819">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-819">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="7a6b8-820">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-820">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="7a6b8-821">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-821">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="7a6b8-822">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-822">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="7a6b8-823">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-823">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="7a6b8-824">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-824">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="7a6b8-825">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-825">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="7a6b8-826">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-826">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="7a6b8-827">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-827">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="7a6b8-828">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-828">Key Vault</span></span>
* <span data-ttu-id="7a6b8-829">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-829">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-830">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-830">Monitor</span></span>
* <span data-ttu-id="7a6b8-831">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-831">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-832">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-832">Network</span></span>
* <span data-ttu-id="7a6b8-833">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-833">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="7a6b8-834">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-834">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="7a6b8-835">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-835">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="7a6b8-836">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-836">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7a6b8-837">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="7a6b8-837">Policy Insights</span></span>
* <span data-ttu-id="7a6b8-838">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-838">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-839">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-839">RDBMS</span></span>
* <span data-ttu-id="7a6b8-840">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-840">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="7a6b8-841">Redis</span><span class="sxs-lookup"><span data-stu-id="7a6b8-841">Redis</span></span>
* <span data-ttu-id="7a6b8-842">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-842">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="7a6b8-843">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-843">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="7a6b8-844">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-844">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="7a6b8-845">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-845">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="7a6b8-846">[주요 변경 사항] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-846">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="7a6b8-847">[주요 변경 사항] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-847">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="7a6b8-848">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-848">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-849">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-849">Role</span></span>
* <span data-ttu-id="7a6b8-850">[주요 변경 사항] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-850">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="7a6b8-851">SQL VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-851">SQL VM</span></span>
* <span data-ttu-id="7a6b8-852">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-852">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-853">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-853">VM</span></span>
* <span data-ttu-id="7a6b8-854">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-854">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="7a6b8-855">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-855">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="7a6b8-856">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-856">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="7a6b8-857">[주요 변경 사항] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-857">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="7a6b8-858">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-858">January 31, 2019</span></span>

<span data-ttu-id="7a6b8-859">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="7a6b8-859">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-860">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-860">Core</span></span>

* <span data-ttu-id="7a6b8-861">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-861">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="7a6b8-862">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-862">January 28, 2019</span></span>

<span data-ttu-id="7a6b8-863">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="7a6b8-863">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-864">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-864">ACR</span></span>
* <span data-ttu-id="7a6b8-865">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-865">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-866">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-866">ACS</span></span>
* <span data-ttu-id="7a6b8-867">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-867">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7a6b8-868">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-868">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="7a6b8-869">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-869">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-870">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-870">AMS</span></span>
* <span data-ttu-id="7a6b8-871">[주요 변경 사항] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-871">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="7a6b8-872">[주요 변경 사항] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-872">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-873">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-873">Appservice</span></span>
* <span data-ttu-id="7a6b8-874">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-874">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="7a6b8-875">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-875">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="7a6b8-876">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-876">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-877">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-877">Container</span></span>
* <span data-ttu-id="7a6b8-878">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-878">Added `container start` command</span></span>
* <span data-ttu-id="7a6b8-879">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-879">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7a6b8-880">EventGrid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-880">EventGrid</span></span>
* <span data-ttu-id="7a6b8-881">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-881">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="7a6b8-882">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-882">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="7a6b8-883">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-883">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="7a6b8-884">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-884">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="7a6b8-885">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-885">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-886">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-886">HDInsight</span></span>
* <span data-ttu-id="7a6b8-887">[주요 변경 사항] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-887">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="7a6b8-888">[주요 변경 사항] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-888">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="7a6b8-889">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-889">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="7a6b8-890">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-890">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="7a6b8-891">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-891">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="7a6b8-892">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-892">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-893">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-893">IoT</span></span>
* <span data-ttu-id="7a6b8-894">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-894">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="7a6b8-895">Kusto</span><span class="sxs-lookup"><span data-stu-id="7a6b8-895">Kusto</span></span>
* <span data-ttu-id="7a6b8-896">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-896">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-897">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-897">Monitor</span></span>
* <span data-ttu-id="7a6b8-898">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-898">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-899">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-899">Profile</span></span>
* <span data-ttu-id="7a6b8-900">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-900">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-901">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-901">Network</span></span>
* <span data-ttu-id="7a6b8-902">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-902">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="7a6b8-903">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-903">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-904">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-904">Resource</span></span>
* <span data-ttu-id="7a6b8-905">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-905">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="7a6b8-906">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-906">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="7a6b8-907">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="7a6b8-907">SQL Virtual Machine</span></span>
* <span data-ttu-id="7a6b8-908">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-908">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-909">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-909">Storage</span></span>
* <span data-ttu-id="7a6b8-910">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-910">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="7a6b8-911">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-911">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-912">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-912">VM</span></span>
* <span data-ttu-id="7a6b8-913">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-913">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="7a6b8-914">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-914">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="7a6b8-915">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-915">January 15, 2019</span></span>

<span data-ttu-id="7a6b8-916">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="7a6b8-916">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-917">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-917">ACR</span></span>
* <span data-ttu-id="7a6b8-918">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-918">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="7a6b8-919">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-919">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="7a6b8-920">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-920">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="7a6b8-921">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-921">ACS</span></span>
* <span data-ttu-id="7a6b8-922">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-922">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-923">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-923">Appservice</span></span>
* <span data-ttu-id="7a6b8-924">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-924">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="7a6b8-925">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-925">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="7a6b8-926">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-926">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="7a6b8-927">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-927">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-928">Botservice</span><span class="sxs-lookup"><span data-stu-id="7a6b8-928">Botservice</span></span>
* <span data-ttu-id="7a6b8-929">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-929">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="7a6b8-930">구성</span><span class="sxs-lookup"><span data-stu-id="7a6b8-930">Configure</span></span>
* <span data-ttu-id="7a6b8-931">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-931">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-932">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-932">CosmosDB</span></span>
* <span data-ttu-id="7a6b8-933">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-933">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-934">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-934">HDInsight</span></span>
* <span data-ttu-id="7a6b8-935">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-935">Added commands for managing applications</span></span>
* <span data-ttu-id="7a6b8-936">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-936">Added commands for managing script actions</span></span>
* <span data-ttu-id="7a6b8-937">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-937">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="7a6b8-938">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-938">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="7a6b8-939">[주요 변경 사항] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-939">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-940">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-940">Network</span></span>
* <span data-ttu-id="7a6b8-941">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-941">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="7a6b8-942">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-942">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="7a6b8-943">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-943">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="7a6b8-944">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-944">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-945">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-945">Role</span></span>
* <span data-ttu-id="7a6b8-946">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-946">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="7a6b8-947">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-947">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="7a6b8-948">보안</span><span class="sxs-lookup"><span data-stu-id="7a6b8-948">Security</span></span>
* <span data-ttu-id="7a6b8-949">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-949">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-950">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-950">Storage</span></span>
* <span data-ttu-id="7a6b8-951">[주요 변경 사항] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-951">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="7a6b8-952">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-952">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="7a6b8-953">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-953">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="7a6b8-954">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-954">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="7a6b8-955">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-955">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-956">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-956">VM</span></span>
* <span data-ttu-id="7a6b8-957">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-957">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="7a6b8-958">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-958">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7a6b8-959">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-959">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="7a6b8-960">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-960">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="7a6b8-961">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-961">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="7a6b8-962">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-962">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="7a6b8-963">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-963">December 20, 2018</span></span>

<span data-ttu-id="7a6b8-964">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="7a6b8-964">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="7a6b8-965">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-965">Appservice</span></span>
* <span data-ttu-id="7a6b8-966">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-966">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="7a6b8-967">웹앱 스냅샷 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-967">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="7a6b8-968">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-968">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7a6b8-969">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="7a6b8-969">IoTCentral</span></span>
* <span data-ttu-id="7a6b8-970">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-970">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-971">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-971">Role</span></span>
* <span data-ttu-id="7a6b8-972">[주요 변경 사항] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-972">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-973">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-973">SQL</span></span>
* <span data-ttu-id="7a6b8-974">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-974">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-975">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-975">VM</span></span>
* <span data-ttu-id="7a6b8-976">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-976">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="7a6b8-977">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-977">December 18, 2018</span></span>

<span data-ttu-id="7a6b8-978">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="7a6b8-978">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="7a6b8-979">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-979">ACR</span></span>
* <span data-ttu-id="7a6b8-980">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-980">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="7a6b8-981">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-981">Condensed the table layout for task list</span></span>
* <span data-ttu-id="7a6b8-982">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-982">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-983">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-983">ACS</span></span>
* <span data-ttu-id="7a6b8-984">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-984">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="7a6b8-985">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-985">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="7a6b8-986">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-986">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="7a6b8-987">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-987">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="7a6b8-988">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-988">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="7a6b8-989">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-989">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-990">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-990">Appservice</span></span>
* <span data-ttu-id="7a6b8-991">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-991">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="7a6b8-992">Botservice</span><span class="sxs-lookup"><span data-stu-id="7a6b8-992">Botservice</span></span>
* <span data-ttu-id="7a6b8-993">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-993">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="7a6b8-994">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-994">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="7a6b8-995">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-995">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="7a6b8-996">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-996">Reduced Kudu network calls</span></span>
* <span data-ttu-id="7a6b8-997">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-997">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-998">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-998">Consumption</span></span>
* <span data-ttu-id="7a6b8-999">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-999">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-1000">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1000">CosmosDB</span></span>
* <span data-ttu-id="7a6b8-1001">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1001">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="7a6b8-1002">지도</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1002">Maps</span></span>
* <span data-ttu-id="7a6b8-1003">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1003">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1004">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1004">Network</span></span>
* <span data-ttu-id="7a6b8-1005">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1005">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="7a6b8-1006">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1006">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1007">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1007">Resource</span></span>
* <span data-ttu-id="7a6b8-1008">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1008">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="7a6b8-1009">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1009">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1010">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1010">Storage</span></span>
*  <span data-ttu-id="7a6b8-1011">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1011">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1012">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1012">VM</span></span>
* <span data-ttu-id="7a6b8-1013">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1013">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="7a6b8-1014">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1014">December 4, 2018</span></span>

<span data-ttu-id="7a6b8-1015">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1015">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="7a6b8-1016">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1016">Core</span></span>
* <span data-ttu-id="7a6b8-1017">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1017">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="7a6b8-1018">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1018">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1019">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1019">Appservice</span></span>
* <span data-ttu-id="7a6b8-1020">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1020">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="7a6b8-1021">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1021">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1022">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1022">Network</span></span>
* <span data-ttu-id="7a6b8-1023">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1023">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1024">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1024">Role</span></span>
* <span data-ttu-id="7a6b8-1025">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1025">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="7a6b8-1026">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1026">VM</span></span>
* <span data-ttu-id="7a6b8-1027">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1027">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="7a6b8-1028">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1028">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="7a6b8-1029">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1029">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="7a6b8-1030">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1030">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="7a6b8-1031">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1031">November 20, 2018</span></span>

<span data-ttu-id="7a6b8-1032">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1032">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="7a6b8-1033">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1033">Core</span></span>
* <span data-ttu-id="7a6b8-1034">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1034">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1035">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1035">ACR</span></span>
* <span data-ttu-id="7a6b8-1036">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1036">Added context token to task step</span></span>
* <span data-ttu-id="7a6b8-1037">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1037">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="7a6b8-1038">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1038">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1039">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1039">Appservice</span></span>
* <span data-ttu-id="7a6b8-1040">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1040">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="7a6b8-1041">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1041">Updated the default `node_version`.</span></span> <span data-ttu-id="7a6b8-1042">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1042">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="7a6b8-1043">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1043">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="7a6b8-1044">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1044">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="7a6b8-1045">IotCentral</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1045">IotCentral</span></span>
* <span data-ttu-id="7a6b8-1046">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1046">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-1047">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1047">KeyVault</span></span>
* <span data-ttu-id="7a6b8-1048">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1048">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1049">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1049">Network</span></span>
* <span data-ttu-id="7a6b8-1050">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1050">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="7a6b8-1051">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1051">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="7a6b8-1052">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1052">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="7a6b8-1053">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1053">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1054">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1054">Rdbms</span></span>
* <span data-ttu-id="7a6b8-1055">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1055">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="7a6b8-1056">Rbac</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1056">Rbac</span></span>
* <span data-ttu-id="7a6b8-1057">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1057">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="7a6b8-1058">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1058">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="7a6b8-1059">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1059">Storage</span></span>
* <span data-ttu-id="7a6b8-1060">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1060">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="7a6b8-1061">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1061">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="7a6b8-1062">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1062">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="7a6b8-1063">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1063">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1064">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1064">VM</span></span>
* <span data-ttu-id="7a6b8-1065">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1065">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="7a6b8-1066">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1066">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="7a6b8-1067">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1067">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="7a6b8-1068">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1068">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="7a6b8-1069">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1069">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="7a6b8-1070">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1070">Added `snapshot wait` command</span></span>
* <span data-ttu-id="7a6b8-1071">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1071">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="7a6b8-1072">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1072">November 6, 2018</span></span>

<span data-ttu-id="7a6b8-1073">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1073">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1074">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1074">Core</span></span>
* <span data-ttu-id="7a6b8-1075">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1075">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1076">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1076">ACR</span></span>
* <span data-ttu-id="7a6b8-1077">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1077">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="7a6b8-1078">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1078">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1079">ACS</span></span>
* <span data-ttu-id="7a6b8-1080">[주요 변경 사항] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1080">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="7a6b8-1081">Advisor</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1081">Advisor</span></span>
* <span data-ttu-id="7a6b8-1082">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1082">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-1083">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1083">AMS</span></span>
* <span data-ttu-id="7a6b8-1084">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1084">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="7a6b8-1085">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1085">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="7a6b8-1086">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1086">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="7a6b8-1087">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1087">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="7a6b8-1088">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1088">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="7a6b8-1089">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1089">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="7a6b8-1090">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1090">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="7a6b8-1091">[주요 변경 사항] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1091">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="7a6b8-1092">[주요 변경 사항] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1092">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="7a6b8-1093">[주요 변경 사항] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1093">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="7a6b8-1094">[주요 변경 사항] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1094">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="7a6b8-1095">[주요 변경 사항] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1095">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="7a6b8-1096">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1096">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="7a6b8-1097">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1097">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="7a6b8-1098">[주요 변경 사항] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1098">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="7a6b8-1099">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1099">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="7a6b8-1100">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1100">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1101">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1101">AppService</span></span>
* <span data-ttu-id="7a6b8-1102">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1102">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="7a6b8-1103">구성</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1103">Configure</span></span>
* <span data-ttu-id="7a6b8-1104">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1104">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1105">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1105">Container</span></span>
* <span data-ttu-id="7a6b8-1106">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1106">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="7a6b8-1107">EventHub</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1107">EventHub</span></span>
* <span data-ttu-id="7a6b8-1108">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1108">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1109">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1109">Interactive</span></span>
* <span data-ttu-id="7a6b8-1110">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1110">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-1111">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1111">Monitor</span></span>
* <span data-ttu-id="7a6b8-1112">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1112">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1113">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1113">Network</span></span>
* <span data-ttu-id="7a6b8-1114">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1114">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="7a6b8-1115">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1115">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="7a6b8-1116">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1116">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="7a6b8-1117">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1117">Profile</span></span>
* <span data-ttu-id="7a6b8-1118">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1118">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1119">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1119">RDBMS</span></span>
* <span data-ttu-id="7a6b8-1120">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1120">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1121">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1121">Resource</span></span>
* <span data-ttu-id="7a6b8-1122">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1122">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1123">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1123">Role</span></span>
* <span data-ttu-id="7a6b8-1124">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1124">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="7a6b8-1125">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1125">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="7a6b8-1126">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1126">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1127">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1127">Storage</span></span>
* <span data-ttu-id="7a6b8-1128">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1128">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1129">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1129">VM</span></span>
* <span data-ttu-id="7a6b8-1130">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1130">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="7a6b8-1131">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1131">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="7a6b8-1132">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1132">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="7a6b8-1133">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1133">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="7a6b8-1134">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1134">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="7a6b8-1135">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1135">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="7a6b8-1136">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1136">October 23, 2018</span></span>

<span data-ttu-id="7a6b8-1137">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1137">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1138">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1138">Core</span></span>
* <span data-ttu-id="7a6b8-1139">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1139">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="7a6b8-1140">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1140">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1141">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1141">ACR</span></span>
* <span data-ttu-id="7a6b8-1142">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1142">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-1143">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1143">CDN</span></span>
* <span data-ttu-id="7a6b8-1144">[주요 변경 사항] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1144">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="7a6b8-1145">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1145">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1146">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1146">Container</span></span>
* <span data-ttu-id="7a6b8-1147">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1147">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="7a6b8-1148">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1148">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="7a6b8-1149">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1149">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="7a6b8-1150">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1150">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="7a6b8-1151">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1151">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="7a6b8-1152">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1152">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="7a6b8-1153">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1153">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-1154">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1154">CosmosDB</span></span>
* <span data-ttu-id="7a6b8-1155">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1155">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1156">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1156">Interactive</span></span>
* <span data-ttu-id="7a6b8-1157">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1157">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="7a6b8-1158">IoT Central</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1158">IoT Central</span></span>
* <span data-ttu-id="7a6b8-1159">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1159">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="7a6b8-1160">[주요 변경 사항] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1160">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-1161">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1161">Monitor</span></span>
* <span data-ttu-id="7a6b8-1162">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1162">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="7a6b8-1163">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1163">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="7a6b8-1164">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1164">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7a6b8-1165">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1165">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="7a6b8-1166">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1166">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="7a6b8-1167">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1167">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="7a6b8-1168">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1168">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="7a6b8-1169">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1169">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="7a6b8-1170">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1170">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="7a6b8-1171">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1171">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1172">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1172">Network</span></span>
* <span data-ttu-id="7a6b8-1173">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1173">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="7a6b8-1174">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1174">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="7a6b8-1175">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1175">ServiceBus</span></span>
* <span data-ttu-id="7a6b8-1176">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1176">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1177">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1177">SQL</span></span>
* <span data-ttu-id="7a6b8-1178">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1178">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1179">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1179">Storage</span></span>
* <span data-ttu-id="7a6b8-1180">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1180">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="7a6b8-1181">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1181">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1182">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1182">VM</span></span>
* <span data-ttu-id="7a6b8-1183">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1183">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="7a6b8-1184">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1184">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="7a6b8-1185">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1185">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="7a6b8-1186">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1186">October 16, 2018</span></span>

<span data-ttu-id="7a6b8-1187">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1187">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1188">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1188">VM</span></span>
* <span data-ttu-id="7a6b8-1189">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1189">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="7a6b8-1190">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1190">October 9, 2018</span></span>

<span data-ttu-id="7a6b8-1191">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1191">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1192">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1192">Core</span></span>
* <span data-ttu-id="7a6b8-1193">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1193">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1194">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1194">ACR</span></span>
* <span data-ttu-id="7a6b8-1195">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1195">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1196">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1196">ACS</span></span>
* <span data-ttu-id="7a6b8-1197">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1197">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="7a6b8-1198">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1198">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="7a6b8-1199">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1199">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="7a6b8-1200">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1200">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1201">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1201">Container</span></span>
* <span data-ttu-id="7a6b8-1202">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1202">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="7a6b8-1203">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1203">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="7a6b8-1204">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1204">Event Hub</span></span>
* <span data-ttu-id="7a6b8-1205">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1205">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="7a6b8-1206">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1206">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="7a6b8-1207">확장</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1207">Extensions</span></span>
* <span data-ttu-id="7a6b8-1208">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1208">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="7a6b8-1209">HDInsight</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1209">HDInsight</span></span>
* <span data-ttu-id="7a6b8-1210">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1210">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-1211">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1211">IoT</span></span>
* <span data-ttu-id="7a6b8-1212">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1212">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-1213">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1213">KeyVault</span></span>
* <span data-ttu-id="7a6b8-1214">최신 API 프로필에 keyvault 스토리지 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1214">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1215">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1215">Network</span></span>
* <span data-ttu-id="7a6b8-1216">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1216">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="7a6b8-1217">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1217">See #6052</span></span>
* <span data-ttu-id="7a6b8-1218">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1218">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="7a6b8-1219">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1219">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="7a6b8-1220">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1220">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="7a6b8-1221">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1221">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="7a6b8-1222">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1222">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="7a6b8-1223">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1223">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1224">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1224">Role</span></span>
* <span data-ttu-id="7a6b8-1225">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1225">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="7a6b8-1226">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1226">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="7a6b8-1227">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1227">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="7a6b8-1228">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1228">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="7a6b8-1229">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1229">Service Bus</span></span>
* <span data-ttu-id="7a6b8-1230">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1230">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1231">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1231">VM</span></span>
* <span data-ttu-id="7a6b8-1232">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1232">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="7a6b8-1233">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1233">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="7a6b8-1234">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1234">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="7a6b8-1235">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1235">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="7a6b8-1236">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1236">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="7a6b8-1237">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1237">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="7a6b8-1238">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1238">September 21, 2018</span></span>

<span data-ttu-id="7a6b8-1239">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1239">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1240">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1240">ACR</span></span>
* <span data-ttu-id="7a6b8-1241">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1241">Added ACR Task commands</span></span>
* <span data-ttu-id="7a6b8-1242">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1242">Added quick run command</span></span>
* <span data-ttu-id="7a6b8-1243">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1243">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="7a6b8-1244">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1244">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="7a6b8-1245">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1245">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="7a6b8-1246">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1246">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1247">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1247">ACS</span></span>
* <span data-ttu-id="7a6b8-1248">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1248">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="7a6b8-1249">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1249">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1250">AppService</span></span>

* <span data-ttu-id="7a6b8-1251">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1251">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="7a6b8-1252">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1252">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="7a6b8-1253">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1253">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="7a6b8-1254">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1254">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-1255">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1255">Batch</span></span>
* <span data-ttu-id="7a6b8-1256">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1256">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="7a6b8-1257">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1257">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="7a6b8-1258">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1258">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="7a6b8-1259">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1259">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7a6b8-1260">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1260">Batch AI</span></span> 
* <span data-ttu-id="7a6b8-1261">`batchai cluster create` 명령에서 자동 스토리지 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1261">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7a6b8-1262">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1262">Cognitive Services</span></span>
* <span data-ttu-id="7a6b8-1263">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1263">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="7a6b8-1264">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1264">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="7a6b8-1265">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1265">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="7a6b8-1266">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1266">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="7a6b8-1267">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1267">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="7a6b8-1268">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1268">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1269">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1269">Container</span></span>
* <span data-ttu-id="7a6b8-1270">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1270">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="7a6b8-1271">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1271">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="7a6b8-1272">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1272">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="7a6b8-1273">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1273">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="7a6b8-1274">Datalake</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1274">Datalake</span></span>
* <span data-ttu-id="7a6b8-1275">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1275">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="7a6b8-1276">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1276">Interactive Shell</span></span>
* <span data-ttu-id="7a6b8-1277">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1277">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="7a6b8-1278">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1278">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-1279">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1279">IoT</span></span>
* <span data-ttu-id="7a6b8-1280">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1280">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="7a6b8-1281">Key Vault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1281">Key Vault</span></span>
* <span data-ttu-id="7a6b8-1282">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1282">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1283">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1283">Network</span></span>
* <span data-ttu-id="7a6b8-1284">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1284">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="7a6b8-1285">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1285">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="7a6b8-1286">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1286">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="7a6b8-1287">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1287">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="7a6b8-1288">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1288">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="7a6b8-1289">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1289">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="7a6b8-1290">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1290">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="7a6b8-1291">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1291">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="7a6b8-1292">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1292">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="7a6b8-1293">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1293">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="7a6b8-1294">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1294">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="7a6b8-1295">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1295">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="7a6b8-1296">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1296">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="7a6b8-1297">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1297">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="7a6b8-1298">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1298">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="7a6b8-1299">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1299">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="7a6b8-1300">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1300">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="7a6b8-1301">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1301">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1302">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1302">RDBMS</span></span>
* <span data-ttu-id="7a6b8-1303">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1303">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="7a6b8-1304">예약</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1304">Reservation</span></span>
* <span data-ttu-id="7a6b8-1305">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1305">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="7a6b8-1306">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1306">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="7a6b8-1307">앱 관리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1307">Manage App</span></span>
* <span data-ttu-id="7a6b8-1308">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1308">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="7a6b8-1309">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1309">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1310">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1310">Role</span></span>
* <span data-ttu-id="7a6b8-1311">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1311">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="7a6b8-1312">SignalR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1312">SignalR</span></span>
* <span data-ttu-id="7a6b8-1313">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1313">First release</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1314">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1314">Storage</span></span>
* <span data-ttu-id="7a6b8-1315">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1315">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="7a6b8-1316">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1316">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1317">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1317">VM</span></span>
* <span data-ttu-id="7a6b8-1318">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1318">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="7a6b8-1319">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1319">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="7a6b8-1320">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1320">August 28, 2018</span></span>

<span data-ttu-id="7a6b8-1321">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1321">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1322">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1322">Core</span></span>

* <span data-ttu-id="7a6b8-1323">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1323">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="7a6b8-1324">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1324">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1325">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1325">ACR</span></span>

* <span data-ttu-id="7a6b8-1326">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1326">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="7a6b8-1327">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1327">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1328">ACS</span></span>

* <span data-ttu-id="7a6b8-1329">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1329">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="7a6b8-1330">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1330">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1331">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1331">AppService</span></span>

* <span data-ttu-id="7a6b8-1332">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1332">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="7a6b8-1333">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1333">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="7a6b8-1334">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1334">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="7a6b8-1335">Backup</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1335">Backup</span></span>

* <span data-ttu-id="7a6b8-1336">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1336">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="7a6b8-1337">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1337">Bot Service</span></span>

* <span data-ttu-id="7a6b8-1338">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1338">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7a6b8-1339">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1339">Cognitive Services</span></span>

* <span data-ttu-id="7a6b8-1340">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1340">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-1341">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1341">IoT</span></span>

* <span data-ttu-id="7a6b8-1342">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1342">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-1343">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1343">Monitor</span></span>

* <span data-ttu-id="7a6b8-1344">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1344">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="7a6b8-1345">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1345">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1346">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1346">Network</span></span>

* <span data-ttu-id="7a6b8-1347">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1347">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1348">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1348">Resource</span></span>

* <span data-ttu-id="7a6b8-1349">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1349">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1350">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1350">Storage</span></span>

* <span data-ttu-id="7a6b8-1351">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1351">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1352">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1352">VM</span></span>

* <span data-ttu-id="7a6b8-1353">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1353">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="7a6b8-1354">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1354">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="7a6b8-1355">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1355">Auguest 14, 2018</span></span>

<span data-ttu-id="7a6b8-1356">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1356">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1357">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1357">Core</span></span>

* <span data-ttu-id="7a6b8-1358">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1358">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="7a6b8-1359">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1359">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="7a6b8-1360">원격 분석</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1360">Telemetry</span></span>

* <span data-ttu-id="7a6b8-1361">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1361">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1362">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1362">ACR</span></span>

* <span data-ttu-id="7a6b8-1363">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1363">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="7a6b8-1364">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1364">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1365">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1365">ACS</span></span>

* <span data-ttu-id="7a6b8-1366">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1366">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="7a6b8-1367">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1367">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="7a6b8-1368">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1368">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="7a6b8-1369">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1369">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="7a6b8-1370">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1370">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="7a6b8-1371">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1371">AppService</span></span>

* <span data-ttu-id="7a6b8-1372">외부 리소스 그룹에 스토리지 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1372">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="7a6b8-1373">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1373">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-1374">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1374">BatchAI</span></span>

* <span data-ttu-id="7a6b8-1375">자동 스토리지 계정 만들기가 &quot;리소스 *그룹*&quot;을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1375">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="7a6b8-1376">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1376">Container</span></span>

* <span data-ttu-id="7a6b8-1377">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1377">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="7a6b8-1378">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1378">IoT</span></span>

* <span data-ttu-id="7a6b8-1379">[주요 변경 사항] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1379">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="7a6b8-1380">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1380">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="7a6b8-1381">Iot Central</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1381">Iot Central</span></span>

* <span data-ttu-id="7a6b8-1382">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1382">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-1383">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1383">KeyVault</span></span>


* <span data-ttu-id="7a6b8-1384">스토리지 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1384">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="7a6b8-1385">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1385">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="7a6b8-1386">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1386">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="7a6b8-1387">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1387">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="7a6b8-1388">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1388">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="7a6b8-1389">릴레이</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1389">Relay</span></span>

* <span data-ttu-id="7a6b8-1390">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1390">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1391">Sql</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1391">Sql</span></span>

* <span data-ttu-id="7a6b8-1392">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1392">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1393">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1393">Storage</span></span>

* <span data-ttu-id="7a6b8-1394">[주요 변경 사항] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1394">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="7a6b8-1395">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1395">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="7a6b8-1396">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1396">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="7a6b8-1397">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1397">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="7a6b8-1398">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1398">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1399">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1399">VM</span></span>

* <span data-ttu-id="7a6b8-1400">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1400">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="7a6b8-1401">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1401">July 31, 2018</span></span>

<span data-ttu-id="7a6b8-1402">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1402">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1403">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1403">ACR</span></span>

* <span data-ttu-id="7a6b8-1404">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1404">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="7a6b8-1405">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1405">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1406">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1406">ACS</span></span>

* <span data-ttu-id="7a6b8-1407">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1407">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-1408">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1408">Batch</span></span>

* <span data-ttu-id="7a6b8-1409">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1409">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1410">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1410">Container</span></span>

* <span data-ttu-id="7a6b8-1411">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1411">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1412">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1412">Network</span></span>

* <span data-ttu-id="7a6b8-1413">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1413">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="7a6b8-1414">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1414">Resource</span></span>

* <span data-ttu-id="7a6b8-1415">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1415">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="7a6b8-1416">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1416">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1417">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1417">Role</span></span>

* <span data-ttu-id="7a6b8-1418">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1418">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="7a6b8-1419">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1419">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="7a6b8-1420">검색</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1420">Search</span></span>

* <span data-ttu-id="7a6b8-1421">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1421">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="7a6b8-1422">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1422">Service Bus</span></span>

* <span data-ttu-id="7a6b8-1423">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1423">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="7a6b8-1424">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1424">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="7a6b8-1425">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1425">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="7a6b8-1426">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1426">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1427">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1427">Storage</span></span>

* <span data-ttu-id="7a6b8-1428">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1428">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="7a6b8-1429">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1429">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1430">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1430">VM</span></span>

* <span data-ttu-id="7a6b8-1431">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1431">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="7a6b8-1432">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1432">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="7a6b8-1433">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1433">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="7a6b8-1434">[주요 변경 사항] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1434">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="7a6b8-1435">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1435">July 18, 2018</span></span>

<span data-ttu-id="7a6b8-1436">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1436">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1437">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1437">Core</span></span>

* <span data-ttu-id="7a6b8-1438">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1438">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="7a6b8-1439">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1439">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="7a6b8-1440">[주요 변경 사항] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1440">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1441">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1441">ACR</span></span>

* <span data-ttu-id="7a6b8-1442">[주요 변경 사항] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1442">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="7a6b8-1443">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1443">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="7a6b8-1444">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1444">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="7a6b8-1445">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1445">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1446">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1446">ACS</span></span>

* <span data-ttu-id="7a6b8-1447">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1447">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1448">AppService</span></span>

* <span data-ttu-id="7a6b8-1449">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1449">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-1450">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1450">Batch</span></span>

* <span data-ttu-id="7a6b8-1451">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1451">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="7a6b8-1452">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1452">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7a6b8-1453">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1453">Batch AI</span></span>

* <span data-ttu-id="7a6b8-1454">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1454">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1455">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1455">Container</span></span>

* <span data-ttu-id="7a6b8-1456">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1456">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="7a6b8-1457">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1457">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1458">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1458">Network</span></span>

* <span data-ttu-id="7a6b8-1459">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1459">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="7a6b8-1460">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1460">Added `network nic wait`</span></span>
* <span data-ttu-id="7a6b8-1461">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1461">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="7a6b8-1462">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1462">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="7a6b8-1463">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1463">Resource</span></span>

* <span data-ttu-id="7a6b8-1464">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1464">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="7a6b8-1465">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1465">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="7a6b8-1466">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1466">Added `deployment wait` command</span></span>
* <span data-ttu-id="7a6b8-1467">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1467">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1468">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1468">SQL</span></span>

* <span data-ttu-id="7a6b8-1469">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1469">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="7a6b8-1470">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1470">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="7a6b8-1471">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1471">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1472">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1472">Storage</span></span>

* <span data-ttu-id="7a6b8-1473">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1473">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1474">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1474">VM</span></span>

* <span data-ttu-id="7a6b8-1475">[주요 변경 사항] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1475">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="7a6b8-1476">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1476">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="7a6b8-1477">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1477">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7a6b8-1478">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1478">July 3, 2018</span></span>

<span data-ttu-id="7a6b8-1479">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1479">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-1480">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1480">AKS</span></span>

* <span data-ttu-id="7a6b8-1481">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1481">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="7a6b8-1482">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1482">July 3, 2018</span></span>

<span data-ttu-id="7a6b8-1483">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1483">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1484">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1484">Core</span></span>

* <span data-ttu-id="7a6b8-1485">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1485">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1486">ACR</span></span>

* <span data-ttu-id="7a6b8-1487">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1487">Added polling build status</span></span>
* <span data-ttu-id="7a6b8-1488">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1488">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="7a6b8-1489">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1489">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1490">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1490">ACS</span></span>

* <span data-ttu-id="7a6b8-1491">[주요 변경 사항]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1491">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="7a6b8-1492">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1492">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="7a6b8-1493">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1493">Updated options for `aks browse` command.</span></span> <span data-ttu-id="7a6b8-1494">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1494">Added `--listen-port` support</span></span>
* <span data-ttu-id="7a6b8-1495">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1495">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="7a6b8-1496">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1496">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="7a6b8-1497">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1497">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1498">AppService</span></span>

* <span data-ttu-id="7a6b8-1499">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1499">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="7a6b8-1500">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1500">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="7a6b8-1501">Backup</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1501">Backup</span></span>

* <span data-ttu-id="7a6b8-1502">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1502">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-1503">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1503">BatchAI</span></span>

* <span data-ttu-id="7a6b8-1504">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1504">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="7a6b8-1505">클라우드</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1505">Cloud</span></span>

* <span data-ttu-id="7a6b8-1506">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1506">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1507">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1507">Container</span></span>

* <span data-ttu-id="7a6b8-1508">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1508">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="7a6b8-1509">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1509">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="7a6b8-1510">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1510">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1511">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1511">Extension</span></span>

* <span data-ttu-id="7a6b8-1512">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1512">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1513">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1513">Network</span></span>

* <span data-ttu-id="7a6b8-1514">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1514">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1515">Rdbms</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1515">Rdbms</span></span>

* <span data-ttu-id="7a6b8-1516">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1516">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1517">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1517">Resource</span></span>

* <span data-ttu-id="7a6b8-1518">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1518">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1519">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1519">VM</span></span>

* <span data-ttu-id="7a6b8-1520">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1520">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="7a6b8-1521">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1521">June 25, 2018</span></span>

<span data-ttu-id="7a6b8-1522">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1522">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="7a6b8-1523">CLI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1523">CLI</span></span>

* <span data-ttu-id="7a6b8-1524">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1524">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="7a6b8-1525">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1525">June 19, 2018</span></span>

<span data-ttu-id="7a6b8-1526">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1526">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1527">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1527">Core</span></span>

* <span data-ttu-id="7a6b8-1528">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1528">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1529">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1529">ACR</span></span>

* <span data-ttu-id="7a6b8-1530">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1530">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="7a6b8-1531">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1531">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1532">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1532">ACS</span></span>

* <span data-ttu-id="7a6b8-1533">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1533">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="7a6b8-1534">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1534">Added `--update` support</span></span>
* <span data-ttu-id="7a6b8-1535">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1535">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="7a6b8-1536">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1536">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="7a6b8-1537">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1537">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="7a6b8-1538">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1538">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="7a6b8-1539">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1539">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="7a6b8-1540">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1540">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1541">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1541">AppService</span></span>

* <span data-ttu-id="7a6b8-1542">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1542">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="7a6b8-1543">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1543">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-1544">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1544">Batch</span></span>

* <span data-ttu-id="7a6b8-1545">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1545">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7a6b8-1546">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1546">Batch AI</span></span>

* <span data-ttu-id="7a6b8-1547">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1547">Added support for workspaces.</span></span> <span data-ttu-id="7a6b8-1548">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1548">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="7a6b8-1549">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1549">Added support for experiments.</span></span> <span data-ttu-id="7a6b8-1550">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1550">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="7a6b8-1551">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1551">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="7a6b8-1552">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1552">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="7a6b8-1553">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1553">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="7a6b8-1554">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1554">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="7a6b8-1555">[주요 변경 사항] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1555">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="7a6b8-1556">[주요 변경 사항] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1556">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="7a6b8-1557">[주요 변경 사항] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1557">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="7a6b8-1558">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1558">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="7a6b8-1559">[주요 변경 사항] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1559">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="7a6b8-1560">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1560">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="7a6b8-1561">[주요 변경 사항] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1561">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="7a6b8-1562">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1562">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="7a6b8-1563">[주요 변경 사항] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1563">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="7a6b8-1564">[주요 변경 사항] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1564">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="7a6b8-1565">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1565">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="7a6b8-1566">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1566">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7a6b8-1567">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1567">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="7a6b8-1568">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1568">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="7a6b8-1569">지도</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1569">Maps</span></span>

* <span data-ttu-id="7a6b8-1570">[주요 변경 사항] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1570">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1571">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1571">Network</span></span>

* <span data-ttu-id="7a6b8-1572">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1572">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="7a6b8-1573">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1573">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="7a6b8-1574">#6502</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1574">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="7a6b8-1575">예약</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1575">Reservations</span></span>

* <span data-ttu-id="7a6b8-1576">[주요 변경 사항] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1576">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="7a6b8-1577">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1577">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="7a6b8-1578">[주요 변경 사항] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1578">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="7a6b8-1579">[주요 변경 사항] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1579">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="7a6b8-1580">[주요 변경 사항] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1580">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="7a6b8-1581">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1581">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1582">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1582">Role</span></span>

* <span data-ttu-id="7a6b8-1583">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1583">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1584">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1584">SQL</span></span>

* <span data-ttu-id="7a6b8-1585">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1585">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1586">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1586">Storage</span></span>

* <span data-ttu-id="7a6b8-1587">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1587">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1588">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1588">VM</span></span>

* <span data-ttu-id="7a6b8-1589">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1589">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="7a6b8-1590">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1590">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="7a6b8-1591">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1591">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7a6b8-1592">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1592">June 13, 2018</span></span>

<span data-ttu-id="7a6b8-1593">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1593">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1594">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1594">Core</span></span>

* <span data-ttu-id="7a6b8-1595">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1595">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="7a6b8-1596">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1596">June 13, 2018</span></span>

<span data-ttu-id="7a6b8-1597">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1597">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-1598">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1598">AKS</span></span>

* <span data-ttu-id="7a6b8-1599">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1599">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="7a6b8-1600">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1600">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="7a6b8-1601">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1601">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="7a6b8-1602">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1602">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="7a6b8-1603">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1603">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1604">AppService</span></span>

* <span data-ttu-id="7a6b8-1605">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1605">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7a6b8-1606">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1606">June 5, 2018</span></span>

<span data-ttu-id="7a6b8-1607">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1607">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1608">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1608">Interactive</span></span>

* <span data-ttu-id="7a6b8-1609">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1609">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="7a6b8-1610">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1610">June 5, 2018</span></span>

<span data-ttu-id="7a6b8-1611">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1611">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1612">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1612">Core</span></span>

* <span data-ttu-id="7a6b8-1613">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1613">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="7a6b8-1614">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1614">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1615">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1615">ACR</span></span>

* <span data-ttu-id="7a6b8-1616">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1616">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="7a6b8-1617">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1617">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="7a6b8-1618">AKS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1618">AKS</span></span>

* <span data-ttu-id="7a6b8-1619">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1619">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-1620">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1620">Batch</span></span>

* <span data-ttu-id="7a6b8-1621">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1621">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-1622">IOT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1622">IOT</span></span>

* <span data-ttu-id="7a6b8-1623">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1623">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1624">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1624">Network</span></span>

* <span data-ttu-id="7a6b8-1625">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1625">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="7a6b8-1626">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1626">Policy Insights</span></span>

* <span data-ttu-id="7a6b8-1627">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1627">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="7a6b8-1628">ARM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1628">ARM</span></span>

* <span data-ttu-id="7a6b8-1629">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1629">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1630">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1630">SQL</span></span>

* <span data-ttu-id="7a6b8-1631">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1631">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="7a6b8-1632">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1632">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="7a6b8-1633">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1633">Storage</span></span>

* <span data-ttu-id="7a6b8-1634">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1634">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1635">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1635">VM</span></span>

* <span data-ttu-id="7a6b8-1636">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1636">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="7a6b8-1637">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1637">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="7a6b8-1638">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1638">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="7a6b8-1639">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1639">May 22, 2018</span></span>

<span data-ttu-id="7a6b8-1640">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1640">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1641">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1641">Core</span></span>

* <span data-ttu-id="7a6b8-1642">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1642">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1643">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1643">ACS</span></span>

* <span data-ttu-id="7a6b8-1644">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1644">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="7a6b8-1645">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1645">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1646">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1646">AppService</span></span>

* <span data-ttu-id="7a6b8-1647">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1647">Improved generic update commands</span></span>
* <span data-ttu-id="7a6b8-1648">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1648">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1649">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1649">Container</span></span>

* <span data-ttu-id="7a6b8-1650">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1650">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="7a6b8-1651">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1651">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1652">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1652">Extension</span></span>

* <span data-ttu-id="7a6b8-1653">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1653">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1654">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1654">Interactive</span></span>

* <span data-ttu-id="7a6b8-1655">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1655">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="7a6b8-1656">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1656">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-1657">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1657">KeyVault</span></span>

* <span data-ttu-id="7a6b8-1658">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1658">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1659">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1659">Network</span></span>

* <span data-ttu-id="7a6b8-1660">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1660">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="7a6b8-1661">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1661">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1662">SQL</span></span>

* <span data-ttu-id="7a6b8-1663">[주요 변경 사항] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1663">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="7a6b8-1664">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1664">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="7a6b8-1665">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1665">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="7a6b8-1666">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1666">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="7a6b8-1667">[주요 변경 사항] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1667">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="7a6b8-1668">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1668">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="7a6b8-1669">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1669">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="7a6b8-1670">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1670">`edition`.</span></span> <span data-ttu-id="7a6b8-1671">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1671">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="7a6b8-1672">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1672">`elasticPoolName`.</span></span> <span data-ttu-id="7a6b8-1673">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1673">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="7a6b8-1674">[주요 변경 사항] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1674">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="7a6b8-1675">`edition`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1675">`edition`.</span></span> <span data-ttu-id="7a6b8-1676">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1676">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="7a6b8-1677">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1677">`dtu`.</span></span> <span data-ttu-id="7a6b8-1678">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1678">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="7a6b8-1679">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1679">`databaseDtuMin`.</span></span> <span data-ttu-id="7a6b8-1680">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1680">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="7a6b8-1681">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1681">`databaseDtuMax`.</span></span> <span data-ttu-id="7a6b8-1682">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1682">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="7a6b8-1683">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1683">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="7a6b8-1684">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1684">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1685">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1685">Storage</span></span>

* <span data-ttu-id="7a6b8-1686">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1686">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="7a6b8-1687">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1687">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1688">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1688">VM</span></span>

* <span data-ttu-id="7a6b8-1689">[주요 변경 사항] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1689">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="7a6b8-1690">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1690">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="7a6b8-1691">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1691">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="7a6b8-1692">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1692">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="7a6b8-1693">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1693">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="7a6b8-1694">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1694">May 7, 2018</span></span>

<span data-ttu-id="7a6b8-1695">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1695">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1696">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1696">Core</span></span>

* <span data-ttu-id="7a6b8-1697">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1697">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="7a6b8-1698">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1698">Added limited support for positional arguments</span></span>
* <span data-ttu-id="7a6b8-1699">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1699">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="7a6b8-1700">#5591</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1700">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="7a6b8-1701">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1701">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="7a6b8-1702">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1702">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="7a6b8-1703">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1703">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="7a6b8-1704">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1704">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="7a6b8-1705">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1705">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1706">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1706">ACR</span></span>

* <span data-ttu-id="7a6b8-1707">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1707">Added ACR Build commands</span></span>
* <span data-ttu-id="7a6b8-1708">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1708">Improved resource not found error messages</span></span>
* <span data-ttu-id="7a6b8-1709">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1709">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="7a6b8-1710">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1710">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="7a6b8-1711">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1711">Improved repository commands error messages</span></span>
* <span data-ttu-id="7a6b8-1712">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1712">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1713">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1713">ACS</span></span>

* <span data-ttu-id="7a6b8-1714">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1714">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="7a6b8-1715">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1715">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="7a6b8-1716">AMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1716">AMS</span></span>

* <span data-ttu-id="7a6b8-1717">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1717">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1718">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1718">Appservice</span></span>

* <span data-ttu-id="7a6b8-1719">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1719">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="7a6b8-1720">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1720">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="7a6b8-1721">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1721">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="7a6b8-1722">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1722">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="7a6b8-1723">Batch AI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1723">Batch AI</span></span>

* <span data-ttu-id="7a6b8-1724">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1724">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7a6b8-1725">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1725">Cognitive Services</span></span>

* <span data-ttu-id="7a6b8-1726">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1726">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-1727">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1727">Consumption</span></span>

* <span data-ttu-id="7a6b8-1728">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1728">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1729">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1729">Container</span></span>

* <span data-ttu-id="7a6b8-1730">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1730">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="7a6b8-1731">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1731">Cosmos DB</span></span>

* <span data-ttu-id="7a6b8-1732">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1732">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="7a6b8-1733">DMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1733">DMS</span></span>

* <span data-ttu-id="7a6b8-1734">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1734">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1735">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1735">Extension</span></span>

* <span data-ttu-id="7a6b8-1736">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1736">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1737">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1737">Interactive</span></span>

* <span data-ttu-id="7a6b8-1738">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1738">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="7a6b8-1739">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1739">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="7a6b8-1740">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1740">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="7a6b8-1741">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1741">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="7a6b8-1742">랩</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1742">Lab</span></span>

* <span data-ttu-id="7a6b8-1743">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1743">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1744">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1744">Network</span></span>

* <span data-ttu-id="7a6b8-1745">[주요 변경 사항] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1745">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="7a6b8-1746">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1746">Profile</span></span>

* <span data-ttu-id="7a6b8-1747">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1747">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="7a6b8-1748">[주요 변경 사항] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1748">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="7a6b8-1749">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1749">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="7a6b8-1750">Redis</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1750">Redis</span></span>

* <span data-ttu-id="7a6b8-1751">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1751">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="7a6b8-1752">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1752">Deprecated `redis list-all`.</span></span> <span data-ttu-id="7a6b8-1753">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1753">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="7a6b8-1754">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1754">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="7a6b8-1755">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1755">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1756">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1756">Role</span></span>

* <span data-ttu-id="7a6b8-1757">[주요 변경 사항] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1757">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1758">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1758">Storage</span></span>

* <span data-ttu-id="7a6b8-1759">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1759">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="7a6b8-1760">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1760">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="7a6b8-1761">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1761">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="7a6b8-1762">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1762">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="7a6b8-1763">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1763">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1764">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1764">VM</span></span>

* <span data-ttu-id="7a6b8-1765">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1765">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="7a6b8-1766">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1766">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="7a6b8-1767">[주요 변경 사항] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1767">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="7a6b8-1768">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1768">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="7a6b8-1769">[주요 변경 사항] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1769">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="7a6b8-1770">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1770">Added write accelerator support</span></span>
* <span data-ttu-id="7a6b8-1771">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1771">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="7a6b8-1772">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1772">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="7a6b8-1773">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1773">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="7a6b8-1774">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1774">April 10, 2018</span></span>

<span data-ttu-id="7a6b8-1775">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1775">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1776">ACR</span></span>

* <span data-ttu-id="7a6b8-1777">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1777">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1778">ACS</span></span>

* <span data-ttu-id="7a6b8-1779">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1779">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1780">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1780">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="7a6b8-1782">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1782">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-1783">BatchAI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1783">BatchAI</span></span>

* <span data-ttu-id="7a6b8-1784">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1784">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="7a6b8-1785">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1785">Job level mounting</span></span>
  - <span data-ttu-id="7a6b8-1786">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1786">Environment variables with secret values</span></span>
  - <span data-ttu-id="7a6b8-1787">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1787">Performance counters settings</span></span>
  - <span data-ttu-id="7a6b8-1788">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1788">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="7a6b8-1789">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1789">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="7a6b8-1790">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1790">Usage and limits reporting</span></span>
  - <span data-ttu-id="7a6b8-1791">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1791">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="7a6b8-1792">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1792">Support for custom images</span></span>
  - <span data-ttu-id="7a6b8-1793">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1793">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="7a6b8-1794">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1794">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="7a6b8-1795">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1795">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="7a6b8-1796">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1796">National clouds are supported</span></span>
* <span data-ttu-id="7a6b8-1797">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1797">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="7a6b8-1798">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1798">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="7a6b8-1799">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1799">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="7a6b8-1800">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1800">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="7a6b8-1801">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1801">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="7a6b8-1802">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1802">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="7a6b8-1803">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1803">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="7a6b8-1804">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1804">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="7a6b8-1805">이 옵션을 사용하면 보다 쉽게 스토리지 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1805">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="7a6b8-1806">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1806">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="7a6b8-1807">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1807">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="7a6b8-1808">[주요 변경 사항] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1808">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="7a6b8-1809">[주요 변경 사항] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1809">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="7a6b8-1810">결제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1810">Billing</span></span>

* <span data-ttu-id="7a6b8-1811">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1811">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-1812">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1812">Consumption</span></span>

* <span data-ttu-id="7a6b8-1813">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1813">Added `marketplace` commands</span></span>
* <span data-ttu-id="7a6b8-1814">[주요 변경 사항] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1814">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="7a6b8-1815">[주요 변경 사항] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1815">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="7a6b8-1816">[주요 변경 사항] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1816">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="7a6b8-1817">[주요 변경 사항] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1817">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="7a6b8-1818">[주요 변경 사항] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1818">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1819">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1819">Container</span></span>

* <span data-ttu-id="7a6b8-1820">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1820">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="7a6b8-1821">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1821">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1822">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1822">Extension</span></span>

* <span data-ttu-id="7a6b8-1823">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1823">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1824">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1824">Interactive</span></span>

* <span data-ttu-id="7a6b8-1825">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1825">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="7a6b8-1826">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1826">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="7a6b8-1827">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1827">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1828">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1828">Network</span></span>

* <span data-ttu-id="7a6b8-1829">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1829">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="7a6b8-1830">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1830">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="7a6b8-1831">#4910</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1831">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="7a6b8-1832">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1832">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="7a6b8-1833">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1833">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="7a6b8-1834">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1834">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="7a6b8-1835">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1835">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="7a6b8-1836">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1836">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-1837">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1837">Profile</span></span>

* <span data-ttu-id="7a6b8-1838">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1838">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="7a6b8-1839">[주요 변경 사항] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1839">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1840">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1840">RDBMS</span></span>

* <span data-ttu-id="7a6b8-1841">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1841">Added `georestore` command</span></span>
* <span data-ttu-id="7a6b8-1842">`create` 명령에서 스토리지 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1842">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1843">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1843">Resource</span></span>

* <span data-ttu-id="7a6b8-1844">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1844">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="7a6b8-1845">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1845">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1846">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1846">SQL</span></span>

* <span data-ttu-id="7a6b8-1847">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1847">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1848">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1848">Storage</span></span>

* <span data-ttu-id="7a6b8-1849">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1849">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1850">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1850">VM</span></span>

* <span data-ttu-id="7a6b8-1851">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1851">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="7a6b8-1852">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1852">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="7a6b8-1854">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1854">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="7a6b8-1855">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1855">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="7a6b8-1856">#5718</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1856">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="7a6b8-1857">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1857">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="7a6b8-1858">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1858">March 27, 2018</span></span>

<span data-ttu-id="7a6b8-1859">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1859">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1860">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1860">Core</span></span>

* <span data-ttu-id="7a6b8-1861">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1861">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1862">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1862">ACS</span></span>

* <span data-ttu-id="7a6b8-1863">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1863">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1864">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1864">Appservice</span></span>

* <span data-ttu-id="7a6b8-1865">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1865">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="7a6b8-1866">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1866">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7a6b8-1867">Backup</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1867">Backup</span></span>

* <span data-ttu-id="7a6b8-1868">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1868">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="7a6b8-1869">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1869">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="7a6b8-1870">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1870">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="7a6b8-1871">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1871">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1872">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1872">Container</span></span>

* <span data-ttu-id="7a6b8-1873">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1873">Added `container exec` command.</span></span> <span data-ttu-id="7a6b8-1874">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1874">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="7a6b8-1875">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1875">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1876">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1876">Extension</span></span>

* <span data-ttu-id="7a6b8-1877">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1877">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="7a6b8-1878">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1878">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="7a6b8-1879">[주요 변경 사항] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1879">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1880">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1880">Interactive</span></span>

* <span data-ttu-id="7a6b8-1881">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1881">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="7a6b8-1882">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1882">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="7a6b8-1883">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1883">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="7a6b8-1884">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1884">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="7a6b8-1885">랩</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1885">Lab</span></span>

* <span data-ttu-id="7a6b8-1886">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1886">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-1887">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1887">Monitor</span></span>

* <span data-ttu-id="7a6b8-1888">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1888">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="7a6b8-1889">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1889">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="7a6b8-1890">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1890">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1891">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1891">Network</span></span>

* <span data-ttu-id="7a6b8-1892">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1892">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-1893">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1893">Profile</span></span>

* <span data-ttu-id="7a6b8-1894">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1894">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1895">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1895">RDBMS</span></span>

* <span data-ttu-id="7a6b8-1896">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1896">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1897">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1897">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="7a6b8-1899">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1899">Role</span></span>

* <span data-ttu-id="7a6b8-1900">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1900">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="7a6b8-1901">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1901">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="7a6b8-1902">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1902">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="7a6b8-1903">[주요 변경 사항] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1903">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="7a6b8-1904">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1904">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1905">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1905">Storage</span></span>

* <span data-ttu-id="7a6b8-1906">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1906">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="7a6b8-1907">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1907">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1908">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1908">VM</span></span>

* <span data-ttu-id="7a6b8-1909">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1909">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="7a6b8-1910">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1910">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="7a6b8-1911">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1911">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="7a6b8-1912">[주요 변경 사항] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1912">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7a6b8-1913">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1913">March 13, 2018</span></span>

<span data-ttu-id="7a6b8-1914">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1914">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-1915">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1915">ACR</span></span>

* <span data-ttu-id="7a6b8-1916">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1916">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7a6b8-1917">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1917">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7a6b8-1918">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1918">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1919">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1919">ACS</span></span>

* <span data-ttu-id="7a6b8-1920">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1920">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7a6b8-1921">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1921">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7a6b8-1922">Advisor</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1922">Advisor</span></span>

* <span data-ttu-id="7a6b8-1923">[주요 변경 사항] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1923">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7a6b8-1924">[주요 변경 사항] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1924">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7a6b8-1925">[주요 변경 사항] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1925">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="7a6b8-1926">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1926">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7a6b8-1927">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1927">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1928">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1928">Appservice</span></span>

* <span data-ttu-id="7a6b8-1929">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1929">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7a6b8-1930">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1930">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7a6b8-1931">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1931">Eventhubs</span></span>

* <span data-ttu-id="7a6b8-1932">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1932">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-1933">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1933">Extension</span></span>

* <span data-ttu-id="7a6b8-1934">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1934">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-1935">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1935">Interactive</span></span>

* <span data-ttu-id="7a6b8-1936">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1936">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7a6b8-1937">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1937">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7a6b8-1938">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1938">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7a6b8-1939">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1939">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-1940">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1940">Monitor</span></span>

* <span data-ttu-id="7a6b8-1941">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1941">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7a6b8-1942">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1942">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7a6b8-1943">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1943">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7a6b8-1944">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1944">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1945">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1945">Network</span></span>

* <span data-ttu-id="7a6b8-1946">[주요 변경 사항] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1946">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7a6b8-1947">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1947">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7a6b8-1948">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1948">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7a6b8-1949">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1949">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-1950">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1950">Profile</span></span>

* <span data-ttu-id="7a6b8-1951">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1951">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7a6b8-1952">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1952">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-1953">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1953">RDBMS</span></span>

* <span data-ttu-id="7a6b8-1954">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1954">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7a6b8-1955">Service Bus</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1955">Service Bus</span></span>

* <span data-ttu-id="7a6b8-1956">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1956">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1957">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1957">Storage</span></span>

* <span data-ttu-id="7a6b8-1958">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1958">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="7a6b8-1959">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1959">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1960">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1960">VM</span></span>

* <span data-ttu-id="7a6b8-1961">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1961">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7a6b8-1962">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1962">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7a6b8-1963">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1963">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7a6b8-1964">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1964">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7a6b8-1965">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1965">February 27, 2018</span></span>

<span data-ttu-id="7a6b8-1966">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1966">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-1967">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1967">Core</span></span>

* <span data-ttu-id="7a6b8-1968">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1968">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7a6b8-1969">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1969">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7a6b8-1970">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1970">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-1971">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1971">ACS</span></span>

* <span data-ttu-id="7a6b8-1972">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1972">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7a6b8-1973">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1973">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7a6b8-1974">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1974">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7a6b8-1975">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1975">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-1976">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1976">Appservice</span></span>

* <span data-ttu-id="7a6b8-1977">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1977">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7a6b8-1978">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1978">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7a6b8-1979">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1979">Cognitive Services</span></span>

* <span data-ttu-id="7a6b8-1980">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1980">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-1981">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1981">Consumption</span></span>

* <span data-ttu-id="7a6b8-1982">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1982">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7a6b8-1983">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1983">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-1984">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1984">Container</span></span>

* <span data-ttu-id="7a6b8-1985">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1985">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-1986">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1986">Network</span></span>

* <span data-ttu-id="7a6b8-1987">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1987">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-1988">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1988">Resource</span></span>

* <span data-ttu-id="7a6b8-1989">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1989">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-1990">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1990">Role</span></span>

* <span data-ttu-id="7a6b8-1991">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1991">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-1992">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1992">SQL</span></span>

* <span data-ttu-id="7a6b8-1993">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1993">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-1994">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1994">Storage</span></span>

* <span data-ttu-id="7a6b8-1995">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1995">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-1996">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1996">VM</span></span>

* <span data-ttu-id="7a6b8-1997">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1997">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7a6b8-1998">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1998">February 13, 2018</span></span>

<span data-ttu-id="7a6b8-1999">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7a6b8-1999">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2000">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2000">Core</span></span>

* <span data-ttu-id="7a6b8-2001">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2001">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2002">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2002">ACS</span></span>

* <span data-ttu-id="7a6b8-2003">[주요 변경 사항] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2003">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7a6b8-2004">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2004">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7a6b8-2005">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2005">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7a6b8-2006">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2006">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7a6b8-2007">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2007">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7a6b8-2008">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2008">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7a6b8-2009">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2009">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7a6b8-2010">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2010">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2011">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2011">Appservice</span></span>

* <span data-ttu-id="7a6b8-2012">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2012">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7a6b8-2013">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2013">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-2014">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2014">CDN</span></span>

* <span data-ttu-id="7a6b8-2015">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2015">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-2016">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2016">Container</span></span>

* <span data-ttu-id="7a6b8-2017">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2017">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7a6b8-2018">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2018">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-2019">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2019">CosmosDB</span></span>

* <span data-ttu-id="7a6b8-2020">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2020">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-2021">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2021">Extension</span></span>

* <span data-ttu-id="7a6b8-2022">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2022">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7a6b8-2023">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2023">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7a6b8-2024">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2024">Feedback</span></span>

* <span data-ttu-id="7a6b8-2025">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2025">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-2026">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2026">Interactive</span></span>

* <span data-ttu-id="7a6b8-2027">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2027">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7a6b8-2028">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2028">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-2029">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2029">IoT</span></span>

* <span data-ttu-id="7a6b8-2030">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2030">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7a6b8-2031">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2031">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="7a6b8-2032">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2032">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2033">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2033">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2034">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2034">Monitor</span></span>

* <span data-ttu-id="7a6b8-2035">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2035">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2036">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2036">Network</span></span>

* <span data-ttu-id="7a6b8-2037">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2037">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7a6b8-2038">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2038">Profile</span></span>

* <span data-ttu-id="7a6b8-2039">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2039">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2040">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2040">Resource</span></span>

* <span data-ttu-id="7a6b8-2041">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2041">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-2042">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2042">Role</span></span>

* <span data-ttu-id="7a6b8-2043">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2043">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2044">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2044">SQL</span></span>

* <span data-ttu-id="7a6b8-2045">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2045">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7a6b8-2046">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2046">Added `sql db rename`</span></span>
* <span data-ttu-id="7a6b8-2047">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2047">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2048">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2048">Storage</span></span>

* <span data-ttu-id="7a6b8-2049">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2049">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2050">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2050">VM</span></span>

* <span data-ttu-id="7a6b8-2051">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2051">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7a6b8-2052">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2052">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7a6b8-2053">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2053">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7a6b8-2054">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2054">January 31, 2018</span></span>

<span data-ttu-id="7a6b8-2055">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2055">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2056">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2056">Core</span></span>

* <span data-ttu-id="7a6b8-2057">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2057">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7a6b8-2058">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2058">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7a6b8-2059">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2059">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7a6b8-2060">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2060">Use `--verbose` to see</span></span>
* <span data-ttu-id="7a6b8-2061">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2061">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2062">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2062">ACS</span></span>

* <span data-ttu-id="7a6b8-2063">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2063">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7a6b8-2064">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2064">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2065">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2065">Appservice</span></span>

* <span data-ttu-id="7a6b8-2066">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2066">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7a6b8-2067">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2067">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-2068">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2068">CDN</span></span>

* <span data-ttu-id="7a6b8-2069">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2069">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-2070">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2070">CosmosDB</span></span>

* <span data-ttu-id="7a6b8-2071">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2071">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-2072">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2072">Interactive</span></span>

* <span data-ttu-id="7a6b8-2073">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2073">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2074">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2074">Network</span></span>

* <span data-ttu-id="7a6b8-2075">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2075">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7a6b8-2076">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2076">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7a6b8-2077">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2077">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7a6b8-2078">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2078">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7a6b8-2079">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2079">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7a6b8-2080">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2080">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7a6b8-2081">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2081">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7a6b8-2082">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2082">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7a6b8-2083">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2083">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="7a6b8-2084">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2084">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2085">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2085">Profile</span></span>

* <span data-ttu-id="7a6b8-2086">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2086">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2087">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2087">Resource</span></span>

* <span data-ttu-id="7a6b8-2088">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2088">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2089">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2089">Storage</span></span>

* <span data-ttu-id="7a6b8-2090">스토리지 V1 계정을 스토리지 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2090">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7a6b8-2091">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2091">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7a6b8-2092">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2092">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="7a6b8-2093">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2093">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7a6b8-2094">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2094">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2095">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2095">VM</span></span>

* <span data-ttu-id="7a6b8-2096">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2096">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7a6b8-2097">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2097">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7a6b8-2098">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2098">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7a6b8-2099">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2099">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7a6b8-2100">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2100">January 17, 2018</span></span>

<span data-ttu-id="7a6b8-2101">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2101">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-2102">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2102">ACR</span></span>

* <span data-ttu-id="7a6b8-2103">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2103">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7a6b8-2104">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2104">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2105">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2105">ACS</span></span>

* <span data-ttu-id="7a6b8-2106">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2106">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7a6b8-2107">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2107">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2108">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2108">Appservice</span></span>

* <span data-ttu-id="7a6b8-2109">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2109">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7a6b8-2110">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2110">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7a6b8-2111">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2111">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7a6b8-2112">Backup</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2112">Backup</span></span>

* <span data-ttu-id="7a6b8-2113">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2113">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7a6b8-2114">`backup restore restore-disks`에 스토리지 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2114">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7a6b8-2115">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2115">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7a6b8-2116">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2116">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7a6b8-2117">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2117">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-2118">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2118">Batch</span></span>

* <span data-ttu-id="7a6b8-2119">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2119">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7a6b8-2120">클라우드</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2120">Cloud</span></span>

* <span data-ttu-id="7a6b8-2121">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2121">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-2122">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2122">Consumption</span></span>

* <span data-ttu-id="7a6b8-2123">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2123">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7a6b8-2124">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2124">Event Grid</span></span>

* <span data-ttu-id="7a6b8-2125">[주요 변경 사항] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2125">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7a6b8-2126">[주요 변경 사항] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2126">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7a6b8-2127">[주요 변경 사항] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2127">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7a6b8-2128">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2128">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7a6b8-2129">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2129">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7a6b8-2130">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2130">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7a6b8-2131">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2131">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7a6b8-2132">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2132">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-2133">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2133">Interactive</span></span>

* <span data-ttu-id="7a6b8-2134">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2134">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7a6b8-2135">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2135">Fixed errors on startup</span></span>
* <span data-ttu-id="7a6b8-2136">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2136">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-2137">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2137">IoT</span></span>

* <span data-ttu-id="7a6b8-2138">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2138">Added support for device provisioning service</span></span>
* <span data-ttu-id="7a6b8-2139">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2139">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7a6b8-2140">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2140">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2141">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2141">Monitor</span></span>

* <span data-ttu-id="7a6b8-2142">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2142">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7a6b8-2143">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2143">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7a6b8-2144">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2144">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2145">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2145">Network</span></span>

* <span data-ttu-id="7a6b8-2146">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2146">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7a6b8-2147">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2147">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2148">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2148">Profile</span></span>

* <span data-ttu-id="7a6b8-2149">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2149">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-2150">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2150">Role</span></span>

* <span data-ttu-id="7a6b8-2151">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2151">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7a6b8-2152">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2152">Service Fabric</span></span>

* <span data-ttu-id="7a6b8-2153">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2153">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7a6b8-2154">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2154">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2155">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2155">VM</span></span>

* <span data-ttu-id="7a6b8-2156">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2156">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7a6b8-2157">[주요 변경 사항] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2157">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7a6b8-2158">[주요 변경 사항] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2158">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7a6b8-2159">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2159">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7a6b8-2160">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2160">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7a6b8-2161">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2161">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7a6b8-2162">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2162">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7a6b8-2163">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2163">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7a6b8-2164">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2164">December 19, 2017</span></span>

<span data-ttu-id="7a6b8-2165">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2165">Version 2.0.23</span></span>

* <span data-ttu-id="7a6b8-2166">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2166">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-2167">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2167">Container</span></span>

* <span data-ttu-id="7a6b8-2168">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2168">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2169">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2169">Network</span></span>

* <span data-ttu-id="7a6b8-2170">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2170">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2171">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2171">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2172">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2172">Storage</span></span>

* <span data-ttu-id="7a6b8-2173">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2173">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2174">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2174">VM</span></span>

* <span data-ttu-id="7a6b8-2175">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2175">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7a6b8-2176">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2176">December 5, 2017</span></span>

<span data-ttu-id="7a6b8-2177">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2177">Version 2.0.22</span></span>

* <span data-ttu-id="7a6b8-2178">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2178">Removed `az component` commands.</span></span> <span data-ttu-id="7a6b8-2179">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2179">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2180">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2180">Core</span></span>
* <span data-ttu-id="7a6b8-2181">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2181">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7a6b8-2182">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2182">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2183">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2183">ACS</span></span>

* <span data-ttu-id="7a6b8-2184">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2184">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7a6b8-2185">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2185">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7a6b8-2186">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2186">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7a6b8-2187">Advisor</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2187">Advisor</span></span>

* <span data-ttu-id="7a6b8-2188">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2188">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2189">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2189">Appservice</span></span>

* <span data-ttu-id="7a6b8-2190">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2190">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7a6b8-2191">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2191">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7a6b8-2192">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2192">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7a6b8-2193">Consumption</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2193">Consumption</span></span>

* <span data-ttu-id="7a6b8-2194">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2194">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-2195">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2195">Container</span></span>

* <span data-ttu-id="7a6b8-2196">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2196">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2197">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2197">Monitor</span></span>

* <span data-ttu-id="7a6b8-2198">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2198">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2199">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2199">Resource</span></span>

* <span data-ttu-id="7a6b8-2200">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2200">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-2201">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2201">Role</span></span>

* <span data-ttu-id="7a6b8-2202">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2202">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7a6b8-2203">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2203">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7a6b8-2204">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2204">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2205">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2205">SQL</span></span>

* <span data-ttu-id="7a6b8-2206">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2206">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7a6b8-2207">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2207">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2208">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2208">VM</span></span>

* <span data-ttu-id="7a6b8-2209">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2209">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7a6b8-2210">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2210">November 14, 2017</span></span>

<span data-ttu-id="7a6b8-2211">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2211">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-2212">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2212">ACR</span></span>

* <span data-ttu-id="7a6b8-2213">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2213">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7a6b8-2214">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2214">ACS</span></span>

* <span data-ttu-id="7a6b8-2215">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2215">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7a6b8-2216">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2216">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7a6b8-2217">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2217">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7a6b8-2218">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2218">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7a6b8-2219">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2219">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2220">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2220">Appservice</span></span>

* <span data-ttu-id="7a6b8-2221">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2221">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7a6b8-2222">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2222">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7a6b8-2223">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2223">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7a6b8-2224">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2224">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7a6b8-2225">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2225">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7a6b8-2226">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2226">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-2227">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2227">Batch</span></span>

* <span data-ttu-id="7a6b8-2228">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2228">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-2229">Batchai</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2229">Batchai</span></span>

* <span data-ttu-id="7a6b8-2230">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2230">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7a6b8-2231">스토리지 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2231">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7a6b8-2232">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2232">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7a6b8-2233">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2233">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7a6b8-2234">클라우드</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2234">Cloud</span></span>

* <span data-ttu-id="7a6b8-2235">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2235">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-2236">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2236">Container</span></span>

* <span data-ttu-id="7a6b8-2237">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2237">Added support to open multiple ports</span></span>
* <span data-ttu-id="7a6b8-2238">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2238">Added container group restart policy</span></span>
* <span data-ttu-id="7a6b8-2239">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2239">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7a6b8-2240">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2240">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7a6b8-2241">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2241">Data Lake Analytics</span></span>

* <span data-ttu-id="7a6b8-2242">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2242">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7a6b8-2243">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2243">Data Lake Store</span></span>

* <span data-ttu-id="7a6b8-2244">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2244">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-2245">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2245">Extension</span></span>

* <span data-ttu-id="7a6b8-2246">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2246">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7a6b8-2247">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2247">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-2248">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2248">IoT</span></span>

* <span data-ttu-id="7a6b8-2249">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2249">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2250">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2250">Monitor</span></span>

* <span data-ttu-id="7a6b8-2251">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2251">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2252">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2252">Network</span></span>

* <span data-ttu-id="7a6b8-2253">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2253">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7a6b8-2254">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2254">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7a6b8-2255">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2255">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7a6b8-2256">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2256">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7a6b8-2257">예약</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2257">Reservations</span></span>

* <span data-ttu-id="7a6b8-2258">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2258">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2259">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2259">Resource</span></span>

* <span data-ttu-id="7a6b8-2260">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2260">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2261">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2261">SQL</span></span>

* <span data-ttu-id="7a6b8-2262">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2262">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2263">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2263">Storage</span></span>

* <span data-ttu-id="7a6b8-2264">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2264">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7a6b8-2265">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2265">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7a6b8-2266">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2266">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7a6b8-2267">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2267">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7a6b8-2268">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2268">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7a6b8-2269">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2269">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7a6b8-2270">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2270">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2271">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2271">VM</span></span>

* <span data-ttu-id="7a6b8-2272">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2272">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7a6b8-2273">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2273">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7a6b8-2274">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2274">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7a6b8-2275">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2275">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7a6b8-2276">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2276">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7a6b8-2277">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2277">October 24, 2017</span></span>

<span data-ttu-id="7a6b8-2278">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2278">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2279">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2279">Core</span></span>

* <span data-ttu-id="7a6b8-2280">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2280">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-2281">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2281">ACR</span></span>

* <span data-ttu-id="7a6b8-2282">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2282">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7a6b8-2283">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2283">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7a6b8-2284">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2284">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2285">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2285">ACS</span></span>

* <span data-ttu-id="7a6b8-2286">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2286">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7a6b8-2287">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2287">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2288">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2288">Appservice</span></span>

* <span data-ttu-id="7a6b8-2289">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2289">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7a6b8-2290">구성 요소</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2290">Component</span></span>

* <span data-ttu-id="7a6b8-2291">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2291">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2292">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2292">Monitor</span></span>

* <span data-ttu-id="7a6b8-2293">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2293">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2294">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2294">Resource</span></span>

* <span data-ttu-id="7a6b8-2295">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2295">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7a6b8-2296">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2296">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2297">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2297">VM</span></span>

* <span data-ttu-id="7a6b8-2298">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2298">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7a6b8-2299">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2299">October 9, 2017</span></span>

<span data-ttu-id="7a6b8-2300">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2300">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2301">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2301">Core</span></span>

* <span data-ttu-id="7a6b8-2302">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2302">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2303">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2303">Appservice</span></span>

* <span data-ttu-id="7a6b8-2304">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2304">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-2305">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2305">Batch</span></span>

* <span data-ttu-id="7a6b8-2306">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2306">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7a6b8-2307">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2307">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7a6b8-2308">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2308">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7a6b8-2309">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2309">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7a6b8-2310">Batchai</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2310">Batchai</span></span>

* <span data-ttu-id="7a6b8-2311">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2311">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-2312">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2312">Keyvault</span></span>

* <span data-ttu-id="7a6b8-2313">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2313">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7a6b8-2314">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2314">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7a6b8-2315">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2315">Network</span></span>

* <span data-ttu-id="7a6b8-2316">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2316">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7a6b8-2317">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2317">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2318">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2318">Resource</span></span>

* <span data-ttu-id="7a6b8-2319">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2319">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7a6b8-2320">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2320">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7a6b8-2321">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2321">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7a6b8-2322">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2322">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2323">Sql</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2323">Sql</span></span>

* <span data-ttu-id="7a6b8-2324">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2324">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7a6b8-2325">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2325">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7a6b8-2326">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2326">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2327">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2327">Storage</span></span>

* <span data-ttu-id="7a6b8-2328">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2328">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2329">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2329">Vm</span></span>

* <span data-ttu-id="7a6b8-2330">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2330">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7a6b8-2331">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2331">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7a6b8-2332">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2332">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7a6b8-2333">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2333">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7a6b8-2334">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2334">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7a6b8-2335">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2335">September 22, 2017</span></span>

<span data-ttu-id="7a6b8-2336">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2336">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2337">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2337">Resource</span></span>

* <span data-ttu-id="7a6b8-2338">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2338">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7a6b8-2339">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2339">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7a6b8-2340">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2340">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7a6b8-2341">[주요 변경 사항] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2341">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2342">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2342">Network</span></span>

* <span data-ttu-id="7a6b8-2343">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2343">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7a6b8-2344">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2344">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7a6b8-2345">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2345">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7a6b8-2346">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2346">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7a6b8-2347">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2347">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2348">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2348">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2349">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2349">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2350">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2350">Storage</span></span>

* <span data-ttu-id="7a6b8-2351">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2351">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7a6b8-2352">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2352">Eventgrid</span></span>

* <span data-ttu-id="7a6b8-2353">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2353">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2354">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2354">SQL</span></span>

* <span data-ttu-id="7a6b8-2355">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2355">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7a6b8-2356">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2356">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7a6b8-2357">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2357">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-2358">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2358">Keyvault</span></span>

* <span data-ttu-id="7a6b8-2359">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2359">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2360">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2360">VM</span></span>

* <span data-ttu-id="7a6b8-2361">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2361">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7a6b8-2362">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2362">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7a6b8-2363">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2363">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7a6b8-2364">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2364">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7a6b8-2365">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2365">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7a6b8-2366">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2366">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2367">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2367">ACS</span></span>

* <span data-ttu-id="7a6b8-2368">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2368">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2369">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2369">Appservice</span></span>

* <span data-ttu-id="7a6b8-2370">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2370">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7a6b8-2371">Backup</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2371">Backup</span></span>

* <span data-ttu-id="7a6b8-2372">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2372">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7a6b8-2373">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2373">September 11, 2017</span></span>

<span data-ttu-id="7a6b8-2374">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2374">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7a6b8-2375">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2375">Core</span></span>

* <span data-ttu-id="7a6b8-2376">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2376">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7a6b8-2377">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2377">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2378">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2378">Acs</span></span>

* <span data-ttu-id="7a6b8-2379">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2379">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7a6b8-2380">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2380">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2381">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2381">Appservice</span></span>

* <span data-ttu-id="7a6b8-2382">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2382">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-2383">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2383">CDN</span></span>

* <span data-ttu-id="7a6b8-2384">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2384">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="7a6b8-2385">내선 번호</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2385">Extension</span></span>

* <span data-ttu-id="7a6b8-2386">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2386">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-2387">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2387">Keyvault</span></span>

* <span data-ttu-id="7a6b8-2388">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2388">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2389">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2389">Network</span></span>

* <span data-ttu-id="7a6b8-2390">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2390">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7a6b8-2391">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2391">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7a6b8-2392">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2392">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7a6b8-2393">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2393">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7a6b8-2394">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2394">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2395">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2395">Resource</span></span>

* <span data-ttu-id="7a6b8-2396">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2396">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7a6b8-2397">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2397">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7a6b8-2398">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2398">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7a6b8-2399">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2399">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2400">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2400">SQL</span></span>

* <span data-ttu-id="7a6b8-2401">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2401">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2402">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2402">VM</span></span>

* <span data-ttu-id="7a6b8-2403">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2403">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7a6b8-2404">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2404">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7a6b8-2405">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2405">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7a6b8-2406">수정됨: `[vm|vmss] create` 스토리지 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2406">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7a6b8-2407">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2407">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7a6b8-2408">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2408">August 31, 2017</span></span>

<span data-ttu-id="7a6b8-2409">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2409">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-2410">Keyvault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2410">Keyvault</span></span>

* <span data-ttu-id="7a6b8-2411">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2411">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7a6b8-2412">Sf</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2412">Sf</span></span>

* <span data-ttu-id="7a6b8-2413">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2413">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2414">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2414">Storage</span></span>

* <span data-ttu-id="7a6b8-2415">스토리지 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2415">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7a6b8-2416">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2416">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7a6b8-2417">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2417">August 28, 2017</span></span>

<span data-ttu-id="7a6b8-2418">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2418">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7a6b8-2419">CLI</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2419">CLI</span></span>

* <span data-ttu-id="7a6b8-2420">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2420">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2421">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2421">ACS</span></span>

* <span data-ttu-id="7a6b8-2422">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2422">Corrected preview regions</span></span>
* <span data-ttu-id="7a6b8-2423">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2423">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="7a6b8-2424">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2424">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2425">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2425">Appservice</span></span>

* <span data-ttu-id="7a6b8-2426">[주요 변경 사항] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2426">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7a6b8-2427">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2427">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7a6b8-2428">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2428">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7a6b8-2429">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2429">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7a6b8-2430">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2430">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-2431">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2431">IoT</span></span>

* <span data-ttu-id="7a6b8-2432">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2432">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2433">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2433">Network</span></span>

* <span data-ttu-id="7a6b8-2434">[주요 변경 사항] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2434">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7a6b8-2435">[주요 변경 사항] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2435">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2436">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2436">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7a6b8-2437">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2437">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7a6b8-2438">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2438">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2439">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2439">Profile</span></span>

* <span data-ttu-id="7a6b8-2440">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2440">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7a6b8-2441">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2441">Service Fabric</span></span>

* <span data-ttu-id="7a6b8-2442">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2442">Preview release</span></span>
* <span data-ttu-id="7a6b8-2443">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2443">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7a6b8-2444">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2444">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7a6b8-2445">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2445">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2446">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2446">Storage</span></span>

* <span data-ttu-id="7a6b8-2447">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2447">Enabled setting blob tier</span></span>
* <span data-ttu-id="7a6b8-2448">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2448">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7a6b8-2449">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2449">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7a6b8-2450">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2450">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7a6b8-2451">[주요 변경 사항] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2451">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7a6b8-2452">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2452">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2453">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2453">VM</span></span>

* <span data-ttu-id="7a6b8-2454">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2454">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7a6b8-2455">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2455">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7a6b8-2456">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2456">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7a6b8-2457">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2457">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7a6b8-2458">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2458">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7a6b8-2459">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2459">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7a6b8-2460">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2460">August 15, 2017</span></span>

<span data-ttu-id="7a6b8-2461">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2461">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2462">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2462">ACS</span></span>

* <span data-ttu-id="7a6b8-2463">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2463">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2464">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2464">Appservice</span></span>

* <span data-ttu-id="7a6b8-2465">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2465">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7a6b8-2466">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2466">Event Grid</span></span>

* <span data-ttu-id="7a6b8-2467">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2467">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7a6b8-2468">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2468">August 11, 2017</span></span>

<span data-ttu-id="7a6b8-2469">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2469">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2470">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2470">ACS</span></span>

* <span data-ttu-id="7a6b8-2471">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2471">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2472">Batch</span></span>

* <span data-ttu-id="7a6b8-2473">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2473">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7a6b8-2474">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2474">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7a6b8-2475">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2475">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7a6b8-2476">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2476">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7a6b8-2477">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2477">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7a6b8-2478">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2478">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7a6b8-2479">구성 요소</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2479">Component</span></span>

* <span data-ttu-id="7a6b8-2480">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2480">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7a6b8-2481">컨테이너</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2481">Container</span></span>

* <span data-ttu-id="7a6b8-2482">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2482">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7a6b8-2483">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2483">Data Lake Store</span></span>

* <span data-ttu-id="7a6b8-2484">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2484">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7a6b8-2485">Event Grid</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2485">Event Grid</span></span>

* <span data-ttu-id="7a6b8-2486">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2486">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2487">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2487">Network</span></span>

* <span data-ttu-id="7a6b8-2488">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2488">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7a6b8-2489">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2489">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7a6b8-2490">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2490">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7a6b8-2491">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2491">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2492">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2492">Profile</span></span>

* <span data-ttu-id="7a6b8-2493">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2493">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2494">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2494">Storage</span></span>

* <span data-ttu-id="7a6b8-2495">시스템에 할당된 ID를 통한 스토리지 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2495">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2496">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2496">VM</span></span>

* <span data-ttu-id="7a6b8-2497">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2497">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7a6b8-2498">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2498">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7a6b8-2499">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2499">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7a6b8-2500">데이터 디스크 연결 시 스토리지 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2500">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7a6b8-2501">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 스토리지 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2501">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7a6b8-2502">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2502">July 28, 2017</span></span>

<span data-ttu-id="7a6b8-2503">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2503">Version 2.0.12</span></span>

* <span data-ttu-id="7a6b8-2504">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2504">Added container commands</span></span>
* <span data-ttu-id="7a6b8-2505">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2505">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7a6b8-2506">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2506">Core</span></span>

* <span data-ttu-id="7a6b8-2507">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2507">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7a6b8-2508">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2508">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7a6b8-2509">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2509">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7a6b8-2510">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2510">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7a6b8-2511">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2511">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7a6b8-2512">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2512">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7a6b8-2513">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2513">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7a6b8-2514">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2514">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7a6b8-2515">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2515">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7a6b8-2516">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2516">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7a6b8-2517">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2517">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7a6b8-2518">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2518">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7a6b8-2519">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2519">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7a6b8-2520">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2520">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7a6b8-2521">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2521">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7a6b8-2522">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2522">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7a6b8-2523">ACR</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2523">ACR</span></span>

* <span data-ttu-id="7a6b8-2524">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2524">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7a6b8-2525">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2525">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7a6b8-2526">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2526">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7a6b8-2527">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2527">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7a6b8-2528">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2528">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7a6b8-2529">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2529">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2530">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2530">ACS</span></span>

* <span data-ttu-id="7a6b8-2531">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2531">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2532">App Service</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2532">Appservice</span></span>

* <span data-ttu-id="7a6b8-2533">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2533">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7a6b8-2534">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2534">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7a6b8-2535">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2535">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7a6b8-2536">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2536">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7a6b8-2537">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2537">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7a6b8-2538">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2538">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7a6b8-2539">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2539">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7a6b8-2540">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2540">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7a6b8-2541">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2541">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7a6b8-2542">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2542">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7a6b8-2543">Batch</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2543">Batch</span></span>

* <span data-ttu-id="7a6b8-2544">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2544">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7a6b8-2545">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2545">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7a6b8-2546">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2546">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7a6b8-2547">CDN</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2547">CDN</span></span>

* <span data-ttu-id="7a6b8-2548">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2548">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="7a6b8-2549">클라우드</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2549">Cloud</span></span>

* <span data-ttu-id="7a6b8-2550">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2550">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7a6b8-2551">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2551">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7a6b8-2552">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2552">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7a6b8-2553">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2553">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7a6b8-2554">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2554">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-2555">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2555">CosmosDB</span></span>

* <span data-ttu-id="7a6b8-2556">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2556">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7a6b8-2557">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2557">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7a6b8-2558">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2558">Data Lake Analytics</span></span>

* <span data-ttu-id="7a6b8-2559">`dla account compute-policy` 제목 아래에 컴퓨팅 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2559">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7a6b8-2560">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2560">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7a6b8-2561">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2561">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7a6b8-2562">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2562">Data Lake Store</span></span>

* <span data-ttu-id="7a6b8-2563">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2563">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7a6b8-2564">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2564">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7a6b8-2565">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2565">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7a6b8-2566">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2566">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7a6b8-2567">대화형</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2567">Interactive</span></span>

* <span data-ttu-id="7a6b8-2568">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2568">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7a6b8-2569">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2569">Increased test coverage</span></span>
* <span data-ttu-id="7a6b8-2570">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2570">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7a6b8-2571">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2571">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7a6b8-2572">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2572">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7a6b8-2573">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2573">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7a6b8-2574">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2574">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7a6b8-2575">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2575">Added `--progress` flag</span></span>
* <span data-ttu-id="7a6b8-2576">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2576">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7a6b8-2577">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2577">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7a6b8-2578">IoT</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2578">IoT</span></span>

* <span data-ttu-id="7a6b8-2579">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2579">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7a6b8-2580">(#3934)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2580">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7a6b8-2581">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2581">Key vault</span></span>

* <span data-ttu-id="7a6b8-2582">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2582">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7a6b8-2583">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2583">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7a6b8-2584">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2584">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7a6b8-2585">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2585">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7a6b8-2586">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2586">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7a6b8-2587">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2587">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7a6b8-2588">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2588">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7a6b8-2589">(#3307)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2589">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7a6b8-2590">랩</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2590">Lab</span></span>

* <span data-ttu-id="7a6b8-2591">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2591">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7a6b8-2592">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2592">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2593">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2593">Monitor</span></span>

* <span data-ttu-id="7a6b8-2594">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2594">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7a6b8-2595">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2595">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7a6b8-2596">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2596">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7a6b8-2597">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2597">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7a6b8-2598">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2598">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7a6b8-2599">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2599">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7a6b8-2600">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2600">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7a6b8-2601">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2601">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7a6b8-2602">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2602">`location` no longer required</span></span>
  * <span data-ttu-id="7a6b8-2603">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2603">Add name and ID support for target</span></span>
  * <span data-ttu-id="7a6b8-2604">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2604">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7a6b8-2605">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2605">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7a6b8-2606">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2606">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7a6b8-2607">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2607">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7a6b8-2608">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2608">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7a6b8-2609">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2609">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2610">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2610">Network</span></span>

* <span data-ttu-id="7a6b8-2611">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2611">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7a6b8-2612">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2612">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7a6b8-2613">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2613">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7a6b8-2614">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2614">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7a6b8-2615">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2615">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7a6b8-2616">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2616">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7a6b8-2617">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2617">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7a6b8-2618">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2618">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7a6b8-2619">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2619">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7a6b8-2620">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2620">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7a6b8-2621">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2621">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7a6b8-2622">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2622">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7a6b8-2623">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2623">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7a6b8-2624">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2624">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7a6b8-2625">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2625">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7a6b8-2626">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2626">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7a6b8-2627">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2627">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7a6b8-2628">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2628">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7a6b8-2629">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2629">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7a6b8-2630">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2630">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7a6b8-2631">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2631">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7a6b8-2632">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2632">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7a6b8-2633">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2633">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7a6b8-2634">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2634">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7a6b8-2635">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2635">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7a6b8-2636">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2636">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7a6b8-2637">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2637">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2638">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2638">Profile</span></span>

* <span data-ttu-id="7a6b8-2639">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2639">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7a6b8-2640">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2640">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7a6b8-2641">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2641">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7a6b8-2642">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2642">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7a6b8-2643">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2643">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7a6b8-2644">RDBMS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2644">RDBMS</span></span>

* <span data-ttu-id="7a6b8-2645">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2645">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7a6b8-2646">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2646">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7a6b8-2647">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2647">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7a6b8-2648">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2648">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2649">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2649">Resource</span></span>

* <span data-ttu-id="7a6b8-2650">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2650">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7a6b8-2651">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2651">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7a6b8-2652">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2652">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7a6b8-2653">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2653">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7a6b8-2654">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2654">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7a6b8-2655">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2655">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7a6b8-2656">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2656">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7a6b8-2657">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2657">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-2658">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2658">Role</span></span>

* <span data-ttu-id="7a6b8-2659">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2659">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7a6b8-2660">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2660">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7a6b8-2661">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2661">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7a6b8-2662">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2662">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7a6b8-2663">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2663">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7a6b8-2664">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2664">Service Fabric</span></span>
* <span data-ttu-id="7a6b8-2665">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2665">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7a6b8-2666">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2666">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7a6b8-2667">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2667">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2668">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2668">SQL</span></span>

* <span data-ttu-id="7a6b8-2669">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2669">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7a6b8-2670">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2670">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7a6b8-2671">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2671">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2672">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2672">Storage</span></span>

* <span data-ttu-id="7a6b8-2673">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2673">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7a6b8-2674">HTTPS 전용 스토리지 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2674">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7a6b8-2675">스토리지 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2675">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7a6b8-2676">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2676">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7a6b8-2677">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2677">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7a6b8-2678">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2678">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2679">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2679">VM</span></span>

* <span data-ttu-id="7a6b8-2680">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2680">Support configuring nsg</span></span>
* <span data-ttu-id="7a6b8-2681">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2681">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7a6b8-2682">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2682">Support managed service identities</span></span>
* <span data-ttu-id="7a6b8-2683">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2683">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="7a6b8-2684">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2684">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7a6b8-2685">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2685">May 10, 2017</span></span>

<span data-ttu-id="7a6b8-2686">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2686">Version 2.0.6</span></span>

* <span data-ttu-id="7a6b8-2687">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2687">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7a6b8-2688">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2688">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7a6b8-2689">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2689">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="7a6b8-2690">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2690">Include Cognitive Services module</span></span>
* <span data-ttu-id="7a6b8-2691">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2691">Include Service Fabric module</span></span>
* <span data-ttu-id="7a6b8-2692">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2692">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="7a6b8-2693">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2693">Add support for CDN commands</span></span>
* <span data-ttu-id="7a6b8-2694">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2694">Remove Container module</span></span>
* <span data-ttu-id="7a6b8-2695">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2695">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7a6b8-2696">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2696">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7a6b8-2697">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2697">Core</span></span>

* <span data-ttu-id="7a6b8-2698">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2698">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7a6b8-2699">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2699">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7a6b8-2700">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2700">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7a6b8-2701">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2701">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7a6b8-2702">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2702">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7a6b8-2703">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2703">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7a6b8-2704">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2704">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7a6b8-2705">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2705">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7a6b8-2706">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2706">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7a6b8-2707">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2707">core: Improved performance</span></span>
* <span data-ttu-id="7a6b8-2708">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2708">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7a6b8-2709">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2709">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2710">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2710">ACS</span></span>

* <span data-ttu-id="7a6b8-2711">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2711">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7a6b8-2712">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2712">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7a6b8-2713">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2713">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7a6b8-2714">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2714">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2715">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2715">AppService</span></span>

* <span data-ttu-id="7a6b8-2716">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2716">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7a6b8-2717">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2717">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7a6b8-2718">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2718">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7a6b8-2719">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2719">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7a6b8-2720">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2720">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7a6b8-2721">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2721">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7a6b8-2722">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2722">support slot swap with preview</span></span>
* <span data-ttu-id="7a6b8-2723">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2723">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7a6b8-2724">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2724">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7a6b8-2725">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2725">CosmosDB</span></span>

* <span data-ttu-id="7a6b8-2726">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2726">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="7a6b8-2727">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2727">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7a6b8-2728">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2728">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7a6b8-2729">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2729">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7a6b8-2730">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2730">Data Lake Analytics</span></span>

* <span data-ttu-id="7a6b8-2731">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2731">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="7a6b8-2732">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2732">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7a6b8-2733">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2733">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7a6b8-2734">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2734">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7a6b8-2735">테이블</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2735">Table</span></span>
  * <span data-ttu-id="7a6b8-2736">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2736">Table valued function</span></span>
  * <span data-ttu-id="7a6b8-2737">보기</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2737">View</span></span>
  * <span data-ttu-id="7a6b8-2738">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2738">Table Statistics.</span></span> <span data-ttu-id="7a6b8-2739">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2739">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7a6b8-2740">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2740">Data Lake Store</span></span>

* <span data-ttu-id="7a6b8-2741">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2741">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="7a6b8-2742">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2742">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7a6b8-2743">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2743">missed help for access show.</span></span> <span data-ttu-id="7a6b8-2744">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2744">adding it.</span></span> <span data-ttu-id="7a6b8-2745">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2745">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7a6b8-2746">찾기</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2746">Find</span></span>

* <span data-ttu-id="7a6b8-2747">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2747">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7a6b8-2748">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2748">KeyVault</span></span>

* <span data-ttu-id="7a6b8-2749">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2749">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7a6b8-2750">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2750">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="7a6b8-2751">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2751">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7a6b8-2752">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2752">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="7a6b8-2753">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2753">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7a6b8-2754">랩</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2754">Lab</span></span>

* <span data-ttu-id="7a6b8-2755">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2755">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="7a6b8-2756">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2756">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="7a6b8-2757">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2757">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="7a6b8-2758">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2758">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="7a6b8-2759">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2759">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="7a6b8-2760">모니터</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2760">Monitor</span></span>

* <span data-ttu-id="7a6b8-2761">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2761">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7a6b8-2762">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2762">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7a6b8-2763">네트워크</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2763">Network</span></span>

* <span data-ttu-id="7a6b8-2764">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2764">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="7a6b8-2765">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2765">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="7a6b8-2766">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2766">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="7a6b8-2767">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2767">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="7a6b8-2768">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2768">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="7a6b8-2769">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2769">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="7a6b8-2770">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2770">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="7a6b8-2771">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2771">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="7a6b8-2772">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2772">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="7a6b8-2773">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2773">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7a6b8-2774">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2774">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="7a6b8-2775">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2775">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7a6b8-2776">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2776">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="7a6b8-2777">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2777">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="7a6b8-2778">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2778">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="7a6b8-2779">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2779">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="7a6b8-2780">프로필</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2780">Profile</span></span>

* <span data-ttu-id="7a6b8-2781">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2781">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7a6b8-2782">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2782">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7a6b8-2783">Redis</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2783">Redis</span></span>

* <span data-ttu-id="7a6b8-2784">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2784">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7a6b8-2785">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2785">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="7a6b8-2786">리소스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2786">Resource</span></span>

* <span data-ttu-id="7a6b8-2787">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2787">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7a6b8-2788">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2788">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7a6b8-2789">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2789">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7a6b8-2790">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2790">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7a6b8-2791">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2791">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7a6b8-2792">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2792">Add docs for az lock update.</span></span> <span data-ttu-id="7a6b8-2793">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2793">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7a6b8-2794">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2794">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7a6b8-2795">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2795">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7a6b8-2796">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2796">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7a6b8-2797">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2797">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7a6b8-2798">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2798">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7a6b8-2799">역할</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2799">Role</span></span>

* <span data-ttu-id="7a6b8-2800">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2800">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7a6b8-2801">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2801">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7a6b8-2802">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2802">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7a6b8-2803">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2803">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7a6b8-2804">SQL</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2804">SQL</span></span>

* <span data-ttu-id="7a6b8-2805">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2805">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="7a6b8-2806">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2806">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7a6b8-2807">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2807">Storage</span></span>

* <span data-ttu-id="7a6b8-2808">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2808">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="7a6b8-2809">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2809">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7a6b8-2810">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2810">Add support for large block blob upload</span></span>
* <span data-ttu-id="7a6b8-2811">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2811">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2812">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2812">VM</span></span>

* <span data-ttu-id="7a6b8-2813">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2813">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7a6b8-2814">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2814">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7a6b8-2815">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2815">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7a6b8-2816">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2816">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7a6b8-2817">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2817">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7a6b8-2818">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2818">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7a6b8-2819">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2819">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7a6b8-2820">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2820">April 3, 2017</span></span>

<span data-ttu-id="7a6b8-2821">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2821">Version 2.0.2</span></span>

<span data-ttu-id="7a6b8-2822">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2822">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="7a6b8-2823">코어</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2823">Core</span></span>

* <span data-ttu-id="7a6b8-2824">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2824">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="7a6b8-2825">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2825">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7a6b8-2826">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2826">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7a6b8-2827">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2827">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7a6b8-2828">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2828">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7a6b8-2829">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2829">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7a6b8-2830">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2830">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7a6b8-2831">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2831">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7a6b8-2832">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2832">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7a6b8-2833">ACS</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2833">ACS</span></span>

* <span data-ttu-id="7a6b8-2834">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2834">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7a6b8-2835">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2835">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7a6b8-2836">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2836">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7a6b8-2837">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2837">Add support for windows clusters.</span></span> <span data-ttu-id="7a6b8-2838">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2838">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7a6b8-2839">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2839">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7a6b8-2840">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2840">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7a6b8-2841">AppService</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2841">AppService</span></span>

* <span data-ttu-id="7a6b8-2842">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2842">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7a6b8-2843">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2843">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7a6b8-2844">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2844">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7a6b8-2845">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2845">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7a6b8-2846">DataLake</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2846">DataLake</span></span>

* <span data-ttu-id="7a6b8-2847">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2847">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="7a6b8-2848">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2848">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7a6b8-2849">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2849">DocuemntDB</span></span>

* <span data-ttu-id="7a6b8-2850">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2850">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7a6b8-2851">VM</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2851">VM</span></span>

* <span data-ttu-id="7a6b8-2852">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2852">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7a6b8-2853">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2853">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7a6b8-2854">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2854">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7a6b8-2855">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2855">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7a6b8-2856">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2856">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7a6b8-2857">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2857">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="7a6b8-2858">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2858">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7a6b8-2859">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2859">February 27, 2017</span></span>

<span data-ttu-id="7a6b8-2860">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2860">Version 2.0.0</span></span>

<span data-ttu-id="7a6b8-2861">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2861">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="7a6b8-2862">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2862">Container Service (acs)</span></span>
- <span data-ttu-id="7a6b8-2863">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2863">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7a6b8-2864">네트워킹</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2864">Networking</span></span>
- <span data-ttu-id="7a6b8-2865">스토리지</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2865">Storage</span></span>

<span data-ttu-id="7a6b8-2866">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2866">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="7a6b8-2867">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2867">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="7a6b8-2868">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2868">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="7a6b8-2869">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2869">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="7a6b8-2870">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2870">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="7a6b8-2871">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2871">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7a6b8-2872">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2872">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7a6b8-2873">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2873">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="7a6b8-2874">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="7a6b8-2874">Provide feedback from the command line with the `az feedback` command</span></span>


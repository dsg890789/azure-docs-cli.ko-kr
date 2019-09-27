---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/05/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1f829ba3d9ecdb158e96512bde5bcf1565cc205c
ms.sourcegitcommit: 5b9b4446c08b94256ced7f63c145b493ba8b50df
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/24/2019
ms.locfileid: "71217420"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="a72aa-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="a72aa-103">Azure CLI release notes</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="a72aa-104">2019년 9월 24일</span><span class="sxs-lookup"><span data-stu-id="a72aa-104">September 24, 2019</span></span>

<span data-ttu-id="a72aa-105">버전 2.0.74</span><span class="sxs-lookup"><span data-stu-id="a72aa-105">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-106">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-106">ACR</span></span>

* <span data-ttu-id="a72aa-107">`acr config retention update`에 필수 `--type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-107">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="a72aa-108">[주요 변경 사항] `--name -n` 매개 변수가 `acr config` 명령 그룹에 대한 `--registry -r `로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-108">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="a72aa-109">AKS</span><span class="sxs-lookup"><span data-stu-id="a72aa-109">AKS</span></span>

* <span data-ttu-id="a72aa-110">`aks create` 명령에 `--load-balancer-sku` 매개 변수가 추가되어 SLB로 AKS 클러스터를 만들 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-110">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="a72aa-111">`aks [create|update]` 명령에 `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` 및 `--load-balancer-outbound-ip-prefixes` 매개 변수가 추가되어 SLB로 AKS 클러스터의 부하 분산 장치 프로필을 업데이트할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-111">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="a72aa-112">`aks create` 명령에 `--vm-set-type` 매개 변수가 추가되어 AKS 클러스터의 vm 유형을 지정할 수 있게 되었습니다(vmas 또는 vmss).</span><span class="sxs-lookup"><span data-stu-id="a72aa-112">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="a72aa-113">ARM</span><span class="sxs-lookup"><span data-stu-id="a72aa-113">ARM</span></span>

* <span data-ttu-id="a72aa-114">json 템플릿에서 여러 줄과 주석을 지원할 수 있도록 `group deployment create` 명령에 `--handle-extended-json-format` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-114">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="a72aa-115">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="a72aa-115">Compute</span></span>

* <span data-ttu-id="a72aa-116">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss [create|update]` 명령에 `--terminate-notification-time` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-116">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="a72aa-117">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss update` 명령에 `--enable-terminate-notification` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-117">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="a72aa-118">`[vm|vmss] create` 명령에 `--priority,` `--eviction-policy,` `--max-billing` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-118">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="a72aa-119">디스크 업로드의 정확한 크기를 지정할 수 있도록 `disk create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-119">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="a72aa-120">관리 디스크의 증분 스냅샷에 대한 지원이 `snapshot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-120">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a72aa-121">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a72aa-121">Cosmos DB</span></span>

* <span data-ttu-id="a72aa-122">키, 읽기 전용 키 또는 연결 문자열을 표시하도록 `cosmosdb keys list` 명령에 `--type <key-type>` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-122">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="a72aa-123">`cosmosdb keys regenerate` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-123">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="a72aa-124">[사용 되지 않음] `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` 및 `cosmosdb list-read-only-keys` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-124">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a72aa-125">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a72aa-125">EventGrid</span></span>

* <span data-ttu-id="a72aa-126">오른쪽 매개 변수를 참조하도록 엔드포인트 도움말 텍스트가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-126">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="a72aa-127">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a72aa-127">Key Vault</span></span>

* <span data-ttu-id="a72aa-128">테넌트(`login -t`)로 로그인하면 `keyvault create`가 실패할 수 있는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-128">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-129">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-129">Monitor</span></span>

* <span data-ttu-id="a72aa-130">`--condition` 인수에서 `:` 문자가 허용되지 않아 `monitor metrics alert create` 할 수 없는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-130">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="a72aa-131">정책</span><span class="sxs-lookup"><span data-stu-id="a72aa-131">Policy</span></span>

* <span data-ttu-id="a72aa-132">정책 API 버전 2019-06-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-132">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="a72aa-133">`policy assignment create` 명령에 `--enforcement-mode` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-133">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-134">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-134">Storage</span></span>

* <span data-ttu-id="a72aa-135">`az storage copy` 명령에 `--blob-type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-135">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="a72aa-136">2019년 9월 10일</span><span class="sxs-lookup"><span data-stu-id="a72aa-136">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-137">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-137">ACR</span></span>

* <span data-ttu-id="a72aa-138">보존 정책을 구성하는 `acr config retention` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-138">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="a72aa-139">AKS</span><span class="sxs-lookup"><span data-stu-id="a72aa-139">AKS</span></span>

* <span data-ttu-id="a72aa-140">다음 명령을 통해 ACR 통합 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-140">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="a72aa-141">AKS 클러스터에 ACR을 연결하는 `--attach-acr` 매개 변수가 `aks [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-141">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="a72aa-142">AKS 클러스터에서 ACR을 분리하는 `--detach-acr` 매개 변수가 `aks update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-142">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="a72aa-143">ARM</span><span class="sxs-lookup"><span data-stu-id="a72aa-143">ARM</span></span>

* <span data-ttu-id="a72aa-144">2019-05-10 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-144">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-145">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-145">Batch</span></span>

* <span data-ttu-id="a72aa-146">`batch pool create`에 대한 `--json-file`에 새 JSON 구성 설정이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-146">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="a72aa-147">파일 시스템을 탑재하기 위한 `MountConfigurations`가 추가됨(자세한 내용은 https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="a72aa-147">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="a72aa-148">`NetworkConfiguration`에 풀의 공용 IP에 대한 선택적 속성 `publicIPs`가 추가됨(자세한 내용은 https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="a72aa-148">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="a72aa-149">공유 이미지 갤러리에 대한 지원이 `--image`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-149">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="a72aa-150">[주요 변경 사항] `batch pool create`의 기본값 `--start-task-wait-for-success`가 `true`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-150">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="a72aa-151">[주요 변경 사항] `AutoUserSpecification`의 `Scope` 기본값이 항상 풀이 되도록 변경됨(Windows 노드에서는 `Task`, Linux 노드에서는 `Pool`이었음)</span><span class="sxs-lookup"><span data-stu-id="a72aa-151">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="a72aa-152">이 인수는 `--json-file`을 사용하여 JSON 구성에서만 설정 가능</span><span class="sxs-lookup"><span data-stu-id="a72aa-152">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-153">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-153">HDInsight</span></span>

* <span data-ttu-id="a72aa-154">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-154">GA release</span></span>
* <span data-ttu-id="a72aa-155">[주요 변경 사항] `az hdinsight resize`의 `--workernode-count/-c` 매개 변수가 필수 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-155">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="a72aa-156">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a72aa-156">Key Vault</span></span>

* <span data-ttu-id="a72aa-157">네트워크 규칙에서 서브넷을 삭제할 수 없는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-157">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="a72aa-158">중복 서브넷 및 IP 주소를 네트워크 규칙에 추가할 수 있는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-158">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-159">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-159">Network</span></span>

* <span data-ttu-id="a72aa-160">트래픽 분석 간격 값을 설정하는 `--interval` 매개 변수가 `network watcher flow-log`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-160">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="a72aa-161">게이트웨이 ID를 관리하는 `network application-gateway identity`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-161">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="a72aa-162">Key Vault ID 설정 지원이 `network application-gateway ssl-cert`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-162">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="a72aa-163">`network express-route peering peer-connection [show|list]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-163">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="a72aa-164">정책</span><span class="sxs-lookup"><span data-stu-id="a72aa-164">Policy</span></span>

* <span data-ttu-id="a72aa-165">2019-01-01 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-165">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="a72aa-166">2019년 8월 27일</span><span class="sxs-lookup"><span data-stu-id="a72aa-166">August 27, 2019</span></span>

<span data-ttu-id="a72aa-167">버전 2.0.72</span><span class="sxs-lookup"><span data-stu-id="a72aa-167">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-168">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-168">ACR</span></span>

* <span data-ttu-id="a72aa-169">[주요 변경 사항] `classic` SKU 지원이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-169">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="a72aa-170">API Management</span><span class="sxs-lookup"><span data-stu-id="a72aa-170">API Management</span></span>

* <span data-ttu-id="a72aa-171">[미리 보기] `apim` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-171">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-172">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-172">AppService</span></span>

* <span data-ttu-id="a72aa-173">슬롯 지정 시의 `webapp webjob continuous start` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-173">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="a72aa-174">`env` 폴더를 검색하고 배포에 사용된 파일에서 제거하도록 `webapp up`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-174">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-175">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a72aa-175">Keyvault</span></span>

* <span data-ttu-id="a72aa-176">`--expires` 인수를 무시한 `keyvault secret set`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-176">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-177">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-177">Network</span></span>

* <span data-ttu-id="a72aa-178">`--private-ip-address-version` 인수에 IPv6 주소 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-178">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="a72aa-179">프라이빗 엔드포인트를 관리하기 위한 새 `network private-endpoint [create|update|list-types]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-179">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="a72aa-180">`network private-link-service` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-180">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="a72aa-181">`--private-endpoint-network-policies` 및 `--private-link-service-network-policies` 인수를 `network vnet subnet update`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-181">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="a72aa-182">RBAC</span><span class="sxs-lookup"><span data-stu-id="a72aa-182">RBAC</span></span>

* <span data-ttu-id="a72aa-183">홈페이지가 업데이트되지 않는 `ad app update --homepage` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-183">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a72aa-184">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-184">ServiceFabric</span></span>

* <span data-ttu-id="a72aa-185">대/소문자가 혼합된 Key Vault 이름 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-185">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="a72aa-186">Key Vault에서 인증서를 사용할 때 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-186">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="a72aa-187">PFX 인증서 파일의 사용 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-187">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="a72aa-188">Key Vault 리소스 그룹이 지정되지 않은 `sf cluster certificate add` 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-188">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="a72aa-189">`sf cluster set`가 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-189">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="a72aa-190">SignalR</span><span class="sxs-lookup"><span data-stu-id="a72aa-190">SignalR</span></span>

* <span data-ttu-id="a72aa-191">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="a72aa-191">Added new commands:</span></span>
  * <span data-ttu-id="a72aa-192">`signalr cors`: SignalR CORS 관리</span><span class="sxs-lookup"><span data-stu-id="a72aa-192">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="a72aa-193">`signalr restart`: SignalR Service 다시 시작</span><span class="sxs-lookup"><span data-stu-id="a72aa-193">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="a72aa-194">`signalr update`: SignalR Service 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-194">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="a72aa-195">`--service-mode` 인수를 `signalr create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-195">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-196">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-196">Storage</span></span>

* <span data-ttu-id="a72aa-197">`storage account revoke-delegation-keys` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-197">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="a72aa-198">2019년 8월 13일</span><span class="sxs-lookup"><span data-stu-id="a72aa-198">August 13, 2019</span></span>

<span data-ttu-id="a72aa-199">버전 2.0.71</span><span class="sxs-lookup"><span data-stu-id="a72aa-199">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-200">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-200">AppService</span></span>

* <span data-ttu-id="a72aa-201">슬롯에 대해 `webapp webjob continuous` 명령이 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-201">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-202">BotService</span><span class="sxs-lookup"><span data-stu-id="a72aa-202">BotService</span></span>

* <span data-ttu-id="a72aa-203">[주요 변경 사항] v3 SDK 봇 만들기에 대한 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-203">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="a72aa-204">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a72aa-204">CognitiveServices</span></span>

* <span data-ttu-id="a72aa-205">`cognitiveservices account network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-205">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a72aa-206">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a72aa-206">Cosmos DB</span></span>

* <span data-ttu-id="a72aa-207">여러 쓰기 위치 업데이트 시의 경고가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-207">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="a72aa-208">CosmosDB SQL, MongoDB, Cassandra, Gremlin 및 Table 리소스 및 리소스 처리량에 대한 CRUD 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-208">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-209">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-209">HDInsight</span></span>

<span data-ttu-id="a72aa-210">이 릴리스에는 호환성이 손상되는 변경이 많이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-210">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="a72aa-211">[주요 변경 사항] `hdinsight create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-211">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="a72aa-212">이름이 `--storage-default-container`에서 `--storage-container`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-212">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="a72aa-213">이름이 `--storage-default-filesystem`에서 `--storage-filesystem`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-213">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="a72aa-214">[주요 변경 사항] `application create`의 `--name` 인수에서 클러스터 이름 대신 애플리케이션 이름을 나타내도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-214">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="a72aa-215">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 `application create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-215">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="a72aa-216">[주요 변경 사항] `application create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-216">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="a72aa-217">이름이 `--application-type`에서 `--type`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-217">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="a72aa-218">이름이 `--marketplace-identifier`에서 `--marketplace-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-218">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="a72aa-219">이름이 `--https-endpoint-access-mode`에서 `--access-mode`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-219">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="a72aa-220">이름이 `--https-endpoint-destination-port`에서 `--destination-port`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-220">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="a72aa-221">[주요 변경 사항] `application create`에 대한 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-221">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="a72aa-222">[호환성이 손상되는 변경] `hdinsight resize`에 대한 이름이 `--target-instance-count`에서 `--workernode-count`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-222">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="a72aa-223">[주요 변경 사항] `hdinsight script-action` 그룹의 모든 명령에서 `--name` 매개 변수를 스크립트 작업 이름으로 사용하도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-223">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="a72aa-224">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 모든 `hdinsight script-action` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-224">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="a72aa-225">[주요 변경 사항] 모든 `hdinsight script-action` 명령에 대한 이름이 `--script-execution-id`에서 `--execution-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-225">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="a72aa-226">[주요 변경 사항] `hdinsight script-action show`에서 `hdinsight script-action show-execution-details`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-226">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="a72aa-227">[호환성이 손상되는 변경] `hdinsight script-action execute --roles`의 매개 변수에서 쉼표로 구분하는 대신 공백으로 구분하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-227">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="a72aa-228">[주요 변경 사항] `hdinsight script-action list`의 `--persisted` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-228">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="a72aa-229">`hdinsight create --cluster-configurations` 매개 변수에서 로컬 JSON 파일 또는 JSON 문자열에 대한 경로를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-229">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="a72aa-230">명령 `hdinsight script-action list-execution-history` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-230">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="a72aa-231">`hdinsight monitor enable --workspace`에서 Log Analytics 작업 영역 ID 또는 작업 영역 이름을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-231">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="a72aa-232">작업 영역 ID가 매개 변수로 제공되는 경우 필요한 `hdinsight monitor enable --primary-key` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-232">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="a72aa-233">도움말 메시지에 대한 추가 예제 및 업데이트된 설명이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-233">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-234">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-234">Interactive</span></span>

* <span data-ttu-id="a72aa-235">로드 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-235">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="a72aa-236">kubernetes</span><span class="sxs-lookup"><span data-stu-id="a72aa-236">Kubernetes</span></span>

* <span data-ttu-id="a72aa-237">대시보드 컨테이너 포트에서 `https`를 사용하는 경우 `https`를 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-237">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-238">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-238">Network</span></span>

* <span data-ttu-id="a72aa-239">`--yes` 인수가 `network dns record-set cname delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-239">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-240">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-240">Profile</span></span>

* <span data-ttu-id="a72aa-241">리소스 액세스 토큰을 가져오기 위해 `--resource-type` 인수가 `account get-access-token`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-241">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="a72aa-242">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-242">ServiceFabric</span></span>

* <span data-ttu-id="a72aa-243">sf 클러스터를 만드는 데 지원되는 모든 os 버전이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-243">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="a72aa-244">기본 인증서 유효성 검사 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-244">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-245">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-245">Storage</span></span>

* <span data-ttu-id="a72aa-246">명령 `storage copy` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-246">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="a72aa-247">2019년 7월 30일</span><span class="sxs-lookup"><span data-stu-id="a72aa-247">July 30, 2019</span></span>

<span data-ttu-id="a72aa-248">버전 2.0.70</span><span class="sxs-lookup"><span data-stu-id="a72aa-248">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-249">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-249">ACR</span></span>

* <span data-ttu-id="a72aa-250">#9952 문제(`acr pack build` 명령의 회귀)가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-250">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="a72aa-251">`acr pack build`의 기본 작성기 이미지 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-251">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-252">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-252">Appservice</span></span>

* <span data-ttu-id="a72aa-253">리소스를 찾을 수 없는 경우 메시지를 표시 하도록 `webapp config ssl`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-253">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="a72aa-254">`functionapp create`에서 `Standard_RAGRS` 스토리지 계정 유형을 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-254">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="a72aa-255">이전 버전의 python을 사용하여 실행할 경우 `webapp up`이(가) 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-255">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-256">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-256">Network</span></span>

* <span data-ttu-id="a72aa-257">`network nic ip-config add`에서 잘못된 매개 변수 `--ids` 제거됨(#9861 수정)</span><span class="sxs-lookup"><span data-stu-id="a72aa-257">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="a72aa-258">#9604 수정.</span><span class="sxs-lookup"><span data-stu-id="a72aa-258">Fixes #9604.</span></span> <span data-ttu-id="a72aa-259">사용자가 신뢰할 수 있는 루트 인증서를 연결할 수 있도록 `network application-gateway http-settings [create|update]`에 `--root-certs` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-259">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="a72aa-260">`network dns record-set ns create`(#9965)에 대해 인수 `--subscription`을 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-260">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="a72aa-261">RBAC</span><span class="sxs-lookup"><span data-stu-id="a72aa-261">RBAC</span></span>

* <span data-ttu-id="a72aa-262">`user update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-262">Added `user update` command</span></span>
* <span data-ttu-id="a72aa-263">[사용 되지 않음] 사용자 관련 명령 중 `--upn-or-object-id`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-263">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="a72aa-264">대체 인수 `--id` 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-264">Use replacement argument `--id`</span></span>
* <span data-ttu-id="a72aa-265">사용자 관련 명령에 `--id` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-265">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-266">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-266">SQL</span></span>

* <span data-ttu-id="a72aa-267">관리형 인스턴스 키 및 TDE 보호기에 대한 관리 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-267">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-268">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-268">Storage</span></span>

* <span data-ttu-id="a72aa-269">`storage remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-269">Added `storage remove` command</span></span>
* <span data-ttu-id="a72aa-270">`storage blob update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-270">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-271">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-271">VM</span></span>

* <span data-ttu-id="a72aa-272">새로운 API 버전을 사용하여 영역 세부 정보를 출력하도록 `list-skus`를 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-272">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="a72aa-273">`vmss create`에 대한 `--single-placement-group`의 기본값을 `false`로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-273">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="a72aa-274">`[snapshot|disk] create`에 대한 ZRS 스토리지 SKU를 선택하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-274">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="a72aa-275">전용 호스트를 지원하는 새로운 명령 그룹 `vm host`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-275">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="a72aa-276">VM 전용 호스트를 설정하기 위해 `vm create`에 매개 변수 `--host` 및 `--host-group` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-276">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="a72aa-277">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="a72aa-277">July 16, 2019</span></span>

<span data-ttu-id="a72aa-278">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="a72aa-278">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-279">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-279">Appservice</span></span>

* <span data-ttu-id="a72aa-280">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-280">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="a72aa-281">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-281">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="a72aa-282">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-282">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-283">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-283">Core</span></span>

* <span data-ttu-id="a72aa-284">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-284">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-285">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-285">Batch</span></span>

* <span data-ttu-id="a72aa-286">[주요 변경 사항] `batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="a72aa-286">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="a72aa-287">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-287">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="a72aa-288">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-288">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="a72aa-289">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-289">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a72aa-290">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a72aa-290">Eventhubs</span></span>

* <span data-ttu-id="a72aa-291">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-291">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-292">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-292">RDBMS</span></span>

* <span data-ttu-id="a72aa-293">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-293">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="a72aa-294">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-294">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="a72aa-295">릴레이</span><span class="sxs-lookup"><span data-stu-id="a72aa-295">Relay</span></span>

* <span data-ttu-id="a72aa-296">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-296">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="a72aa-297">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-297">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="a72aa-298">Servicebus</span><span class="sxs-lookup"><span data-stu-id="a72aa-298">Servicebus</span></span>

* <span data-ttu-id="a72aa-299">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-299">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-300">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-300">Storage</span></span>

* <span data-ttu-id="a72aa-301">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-301">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="a72aa-302">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-302">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="a72aa-303">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="a72aa-303">July 2, 2019</span></span>

<span data-ttu-id="a72aa-304">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="a72aa-304">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-305">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-305">Core</span></span>

* <span data-ttu-id="a72aa-306">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-306">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="a72aa-307">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-307">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="a72aa-308">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-308">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-309">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-309">ACR</span></span>

* <span data-ttu-id="a72aa-310">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-310">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-311">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-311">Appservice</span></span>

* <span data-ttu-id="a72aa-312">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-312">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="a72aa-313">[주요 변경 사항] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-313">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="a72aa-314">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-314">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="a72aa-315">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-315">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a72aa-316">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a72aa-316">Cosmos DB</span></span>

* <span data-ttu-id="a72aa-317">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-317">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="a72aa-318">DLS</span><span class="sxs-lookup"><span data-stu-id="a72aa-318">DLS</span></span>

* <span data-ttu-id="a72aa-319">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="a72aa-319">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="a72aa-320">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="a72aa-320">Feedback</span></span>

* <span data-ttu-id="a72aa-321">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-321">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-322">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-322">HDInsight</span></span>

* <span data-ttu-id="a72aa-323">[주요 변경 사항] `oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-323">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="a72aa-324">[주요 변경 사항] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-324">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="a72aa-325">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-325">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="a72aa-326">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-326">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="a72aa-327">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-327">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="a72aa-328">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-328">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="a72aa-329">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-329">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="a72aa-330">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-330">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="a72aa-331">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-331">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="a72aa-332">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="a72aa-332">Managed Services</span></span>

* <span data-ttu-id="a72aa-333">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="a72aa-333">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-334">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-334">Profile</span></span>
* <span data-ttu-id="a72aa-335">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-335">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="a72aa-336">RBAC</span><span class="sxs-lookup"><span data-stu-id="a72aa-336">RBAC</span></span>

* <span data-ttu-id="a72aa-337">[주요 변경 사항] `create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-337">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="a72aa-338">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-338">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="a72aa-339">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-339">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="a72aa-340">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-340">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-341">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-341">RDBMS</span></span>

* <span data-ttu-id="a72aa-342">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-342">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-343">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-343">SQL</span></span>

* <span data-ttu-id="a72aa-344">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-344">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-345">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-345">Storage</span></span>

* <span data-ttu-id="a72aa-346">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="a72aa-346">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="a72aa-347">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="a72aa-347">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="a72aa-348">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-348">VM</span></span>

* <span data-ttu-id="a72aa-349">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-349">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="a72aa-350">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-350">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="a72aa-351">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-351">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="a72aa-352">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-352">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="a72aa-353">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="a72aa-353">June 18, 2019</span></span>

<span data-ttu-id="a72aa-354">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="a72aa-354">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-355">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-355">Core</span></span>

<span data-ttu-id="a72aa-356">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-356">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="a72aa-357">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-357">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="a72aa-358">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-358">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="a72aa-359">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-359">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="a72aa-360">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-360">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="a72aa-361">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-361">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="a72aa-362">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-362">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-363">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-363">ACR</span></span>
* <span data-ttu-id="a72aa-364">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-364">Added 'acr check-health' command</span></span>
* <span data-ttu-id="a72aa-365">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="a72aa-365">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-366">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-366">ACS</span></span>
* <span data-ttu-id="a72aa-367">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="a72aa-367">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-368">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-368">AMS</span></span>
* <span data-ttu-id="a72aa-369">[주요 변경 사항] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-369">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-370">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-370">AppService</span></span>
* <span data-ttu-id="a72aa-371">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-371">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="a72aa-372">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-372">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="a72aa-373">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-373">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="a72aa-374">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-374">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="a72aa-375">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-375">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="a72aa-376">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-376">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-377">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-377">Batch</span></span>
* <span data-ttu-id="a72aa-378">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-378">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-379">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a72aa-379">BatchAI</span></span>
* <span data-ttu-id="a72aa-380">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-380">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-381">BotService</span><span class="sxs-lookup"><span data-stu-id="a72aa-381">BotService</span></span>
* <span data-ttu-id="a72aa-382">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-382">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-383">CosmosDB</span></span>
* <span data-ttu-id="a72aa-384">[사용 되지 않음] `cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-384">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="a72aa-385">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="a72aa-385">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="a72aa-386">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-386">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="a72aa-387">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-387">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a72aa-388">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a72aa-388">EventGrid</span></span>
* <span data-ttu-id="a72aa-389">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-389">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="a72aa-390">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-390">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="a72aa-391">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-391">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="a72aa-392">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-392">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="a72aa-393">[주요 변경 사항] `eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-393">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-394">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-394">HDInsight</span></span>
* <span data-ttu-id="a72aa-395">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-395">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-396">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-396">IoT</span></span>
* <span data-ttu-id="a72aa-397">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-397">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="a72aa-398">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-398">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-399">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-399">Network</span></span>
* <span data-ttu-id="a72aa-400">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-400">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="a72aa-401">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-401">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="a72aa-402">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-402">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="a72aa-403">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-403">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-404">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-404">Resource</span></span>
* <span data-ttu-id="a72aa-405">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-405">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="a72aa-406">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-406">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="a72aa-407">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a72aa-407">ServiceBus</span></span>
* <span data-ttu-id="a72aa-408">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-408">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-409">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-409">SQL</span></span>
* <span data-ttu-id="a72aa-410">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-410">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="a72aa-411">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-411">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="a72aa-412">SQLVm</span><span class="sxs-lookup"><span data-stu-id="a72aa-412">SQLVm</span></span>
* <span data-ttu-id="a72aa-413">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-413">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="a72aa-414">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-414">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-415">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-415">Storage</span></span>
* <span data-ttu-id="a72aa-416">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-416">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="a72aa-417">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-417">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-418">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-418">VM</span></span>
* <span data-ttu-id="a72aa-419">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-419">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="a72aa-420">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="a72aa-420">June 4, 2019</span></span>

<span data-ttu-id="a72aa-421">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="a72aa-421">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-422">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-422">Core</span></span>
* <span data-ttu-id="a72aa-423">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-423">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-424">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-424">ACR</span></span>
* <span data-ttu-id="a72aa-425">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-425">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-426">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-426">ACS</span></span>
* <span data-ttu-id="a72aa-427">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-427">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="a72aa-428">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-428">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-429">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-429">Batch</span></span>
* <span data-ttu-id="a72aa-430">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-430">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-431">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-431">IoT</span></span>
* <span data-ttu-id="a72aa-432">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-432">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-433">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-433">Network</span></span>
* <span data-ttu-id="a72aa-434">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-434">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="a72aa-435">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-435">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="a72aa-436">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-436">Resource</span></span>
* <span data-ttu-id="a72aa-437">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-437">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-438">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-438">Role</span></span>
* <span data-ttu-id="a72aa-439">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-439">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="a72aa-440">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="a72aa-440">Compute</span></span>
* <span data-ttu-id="a72aa-441">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-441">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="a72aa-442">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="a72aa-442">May 21, 2019</span></span>

<span data-ttu-id="a72aa-443">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="a72aa-443">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-444">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-444">Core</span></span>
* <span data-ttu-id="a72aa-445">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-445">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="a72aa-446">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-446">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="a72aa-447">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-447">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-448">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-448">ACR</span></span>
* <span data-ttu-id="a72aa-449">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-449">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-450">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-450">ACS</span></span>
* <span data-ttu-id="a72aa-451">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-451">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-452">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-452">AppService</span></span>
* <span data-ttu-id="a72aa-453">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-453">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="a72aa-454">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-454">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="a72aa-455">[주요 변경 사항] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-455">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="a72aa-456">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-456">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="a72aa-457">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-457">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="a72aa-458">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-458">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="a72aa-459">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-459">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-460">BotService</span><span class="sxs-lookup"><span data-stu-id="a72aa-460">BotService</span></span>
* <span data-ttu-id="a72aa-461">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-461">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="a72aa-462">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-462">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-463">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-463">Consumption</span></span>
* <span data-ttu-id="a72aa-464">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-464">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-465">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-465">IoT</span></span>
* <span data-ttu-id="a72aa-466">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-466">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-467">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-467">Network</span></span>
* [주요 변경 사항]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="a72aa-469">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-469">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="a72aa-470">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-470">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-471">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-471">RDBMS</span></span>
* <span data-ttu-id="a72aa-472">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-472">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="a72aa-473">RBAC</span><span class="sxs-lookup"><span data-stu-id="a72aa-473">RBAC</span></span>
* <span data-ttu-id="a72aa-474">`role assignment`에 관리 그룹 범위가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-474">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-475">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-475">Storage</span></span>
* <span data-ttu-id="a72aa-476">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-476">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="a72aa-477">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="a72aa-477">Compute</span></span>
* <span data-ttu-id="a72aa-478">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-478">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="a72aa-479">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-479">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="a72aa-480">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-480">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="a72aa-481">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-481">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="a72aa-482">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="a72aa-482">May 6, 2019</span></span>

<span data-ttu-id="a72aa-483">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="a72aa-483">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-484">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-484">ACS</span></span>
* <span data-ttu-id="a72aa-485">[주요 변경 사항] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-485">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="a72aa-486">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-486">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="a72aa-487">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-487">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="a72aa-488">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-488">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-489">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-489">Appservice</span></span>
* <span data-ttu-id="a72aa-490">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-490">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="a72aa-491">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-491">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="a72aa-492">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-492">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="a72aa-493">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-493">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="a72aa-494">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-494">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="a72aa-495">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-495">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="a72aa-496">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-496">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="a72aa-497">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-497">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="a72aa-498">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-498">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="a72aa-499">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-499">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-500">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-500">Batch</span></span>
* <span data-ttu-id="a72aa-501">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-501">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-502">Botservice</span><span class="sxs-lookup"><span data-stu-id="a72aa-502">Botservice</span></span>
* <span data-ttu-id="a72aa-503">[주요 변경 사항] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="a72aa-503">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="a72aa-504">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-504">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="a72aa-505">[주요 변경 사항] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-505">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="a72aa-506">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="a72aa-506">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="a72aa-507">[주요 변경 사항] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-507">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="a72aa-508">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="a72aa-508">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="a72aa-509">[주요 변경 사항] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-509">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="a72aa-510">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-510">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="a72aa-511">[주요 변경 사항] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-511">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="a72aa-512">[주요 변경 사항] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-512">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="a72aa-513">[주요 변경 사항] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-513">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="a72aa-514">[주요 변경 사항] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-514">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="a72aa-515">[주요 변경 사항] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-515">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="a72aa-516">[주요 변경 사항] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-516">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="a72aa-517">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="a72aa-517">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="a72aa-518">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-518">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="a72aa-519">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-519">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="a72aa-520">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-520">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="a72aa-521">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-521">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="a72aa-522">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-522">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="a72aa-523">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-523">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="a72aa-524">구성</span><span class="sxs-lookup"><span data-stu-id="a72aa-524">Configure</span></span>
* <span data-ttu-id="a72aa-525">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-525">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a72aa-526">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a72aa-526">Eventhubs</span></span>
* <span data-ttu-id="a72aa-527">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-527">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="a72aa-528">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-528">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-529">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-529">Network</span></span>
* <span data-ttu-id="a72aa-530">[주요 변경 사항] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="a72aa-530">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="a72aa-531">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a72aa-531">Policy Insights</span></span>
* <span data-ttu-id="a72aa-532">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-532">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-533">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-533">Role</span></span>
* <span data-ttu-id="a72aa-534">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-534">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="a72aa-535">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a72aa-535">Service Bus</span></span>
* <span data-ttu-id="a72aa-536">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-536">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="a72aa-537">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-537">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="a72aa-538">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-538">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-539">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-539">SQL</span></span>
* <span data-ttu-id="a72aa-540">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-540">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-541">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-541">VM</span></span>
* <span data-ttu-id="a72aa-542">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-542">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="a72aa-543">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-543">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="a72aa-544">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-544">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="a72aa-545">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-545">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="a72aa-546">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-546">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="a72aa-547">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-547">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="a72aa-548">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="a72aa-548">April 23, 2019</span></span>

<span data-ttu-id="a72aa-549">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="a72aa-549">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-550">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-550">ACS</span></span>
* <span data-ttu-id="a72aa-551">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-551">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="a72aa-552">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-552">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-553">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-553">AMS</span></span>
* <span data-ttu-id="a72aa-554">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-554">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-555">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-555">AppService</span></span>
* <span data-ttu-id="a72aa-556">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-556">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="a72aa-557">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-557">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="a72aa-558">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-558">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="a72aa-559">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-559">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="a72aa-560">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-560">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="a72aa-561">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-561">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="a72aa-562">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-562">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="a72aa-563">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-563">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="a72aa-564">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-564">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="a72aa-565">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="a72aa-565">Deployment Manager</span></span>
* <span data-ttu-id="a72aa-566">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="a72aa-566">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="a72aa-567">랩</span><span class="sxs-lookup"><span data-stu-id="a72aa-567">Lab</span></span>
* <span data-ttu-id="a72aa-568">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-568">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-569">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-569">Network</span></span>
* <span data-ttu-id="a72aa-570">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-570">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-571">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-571">Resource</span></span>
* <span data-ttu-id="a72aa-572">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="a72aa-572">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="a72aa-573">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="a72aa-573">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="a72aa-574">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-574">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="a72aa-575">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-575">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-576">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-576">SQL</span></span>
* <span data-ttu-id="a72aa-577">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-577">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="a72aa-578">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-578">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="a72aa-579">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-579">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="a72aa-580">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-580">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-581">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-581">Storage</span></span>
* <span data-ttu-id="a72aa-582">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-582">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-583">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-583">VM</span></span>
* <span data-ttu-id="a72aa-584">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-584">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="a72aa-585">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-585">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="a72aa-586">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-586">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="a72aa-587">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="a72aa-587">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-588">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-588">Core</span></span>
* <span data-ttu-id="a72aa-589">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-589">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-590">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-590">ACR</span></span>
* <span data-ttu-id="a72aa-591">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-591">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-592">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-592">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="a72aa-595">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-595">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="a72aa-596">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-596">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-597">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-597">AppService</span></span>
* <span data-ttu-id="a72aa-598">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-598">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="a72aa-599">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-599">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="a72aa-600">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="a72aa-600">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="a72aa-601">[주요 변경 사항] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="a72aa-601">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="a72aa-602">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-602">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="a72aa-603">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-603">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="a72aa-604">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-604">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-605">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-605">CDN</span></span>
* <span data-ttu-id="a72aa-606">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-606">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="a72aa-607">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="a72aa-607">Feedback</span></span>
* <span data-ttu-id="a72aa-608">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-608">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="a72aa-609">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-609">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="a72aa-610">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-610">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-611">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-611">Monitor</span></span>
* <span data-ttu-id="a72aa-612">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-612">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="a72aa-613">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-613">Network</span></span>
* <span data-ttu-id="a72aa-614">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-614">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="a72aa-615">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-615">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="a72aa-616">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-616">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="a72aa-617">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-617">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="a72aa-618">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="a72aa-618">PrivateDNS</span></span>
* <span data-ttu-id="a72aa-619">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-619">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-620">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-620">Resource</span></span>
* <span data-ttu-id="a72aa-621">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-621">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-622">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-622">Role</span></span>
* <span data-ttu-id="a72aa-623">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-623">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="a72aa-624">[주요 변경 사항] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-624">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-625">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-625">SQL</span></span>
* <span data-ttu-id="a72aa-626">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-626">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-627">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-627">Storage</span></span>
* <span data-ttu-id="a72aa-628">[주요 변경 사항] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-628">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="a72aa-629">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-629">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="a72aa-630">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-630">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="a72aa-631">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-631">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="a72aa-632">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="a72aa-632">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="a72aa-633">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-633">Core</span></span>
* <span data-ttu-id="a72aa-634">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-634">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="a72aa-635">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-635">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="a72aa-636">클라우드</span><span class="sxs-lookup"><span data-stu-id="a72aa-636">Cloud</span></span>
* <span data-ttu-id="a72aa-637">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-637">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-638">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-638">ACR</span></span>
* <span data-ttu-id="a72aa-639">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-639">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="a72aa-640">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-640">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="a72aa-641">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-641">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="a72aa-642">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-642">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-643">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-643">AppService</span></span>
* <span data-ttu-id="a72aa-644">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-644">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="a72aa-645">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-645">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="a72aa-646">BOT Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-646">BOT Service</span></span>
* <span data-ttu-id="a72aa-647">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-647">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="a72aa-648">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-648">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="a72aa-649">[주요 변경 사항] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-649">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="a72aa-650">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-650">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-651">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-651">CDN</span></span>
* <span data-ttu-id="a72aa-652">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-652">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [주요 변경 사항]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="a72aa-654">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-654">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a72aa-655">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-655">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-656">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a72aa-656">Cosmosdb</span></span>
* <span data-ttu-id="a72aa-657">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-657">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="a72aa-658">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-658">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-659">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-659">Interactive</span></span>
* <span data-ttu-id="a72aa-660">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-660">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-661">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-661">Monitor</span></span>
* <span data-ttu-id="a72aa-662">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-662">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-663">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-663">Network</span></span>
* <span data-ttu-id="a72aa-664">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-664">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-665">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-665">Profile</span></span>
* <span data-ttu-id="a72aa-666">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-666">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="a72aa-667">Postgres</span><span class="sxs-lookup"><span data-stu-id="a72aa-667">Postgres</span></span> 
* <span data-ttu-id="a72aa-668">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-668">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="a72aa-669">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-669">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-670">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-670">Resource</span></span>
* <span data-ttu-id="a72aa-671">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-671">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="a72aa-672">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-672">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="a72aa-673">그래프</span><span class="sxs-lookup"><span data-stu-id="a72aa-673">Graph</span></span>
* <span data-ttu-id="a72aa-674">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-674">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="a72aa-675">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-675">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="a72aa-676">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-676">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="a72aa-677">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-677">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="a72aa-678">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-678">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-679">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-679">storage</span></span>
* <span data-ttu-id="a72aa-680">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-680">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="a72aa-681">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-681">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="a72aa-682">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-682">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="a72aa-683">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-683">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-684">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-684">VM</span></span>
* <span data-ttu-id="a72aa-685">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-685">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="a72aa-686">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="a72aa-686">March 12, 2019</span></span>

<span data-ttu-id="a72aa-687">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="a72aa-687">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-688">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-688">Core</span></span>

* <span data-ttu-id="a72aa-689">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-689">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-690">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-690">ACR</span></span>

* <span data-ttu-id="a72aa-691">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-691">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-692">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-692">ACS</span></span>

* <span data-ttu-id="a72aa-693">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-693">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="a72aa-694">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-694">AppService</span></span>

* <span data-ttu-id="a72aa-695">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-695">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="a72aa-696">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="a72aa-696">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="a72aa-697">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-697">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="a72aa-698">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-698">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-699">Botservice</span><span class="sxs-lookup"><span data-stu-id="a72aa-699">Botservice</span></span>

* <span data-ttu-id="a72aa-700">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-700">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a72aa-701">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-701">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a72aa-702">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-702">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="a72aa-703">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-703">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-704">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-704">Container</span></span>

* <span data-ttu-id="a72aa-705">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-705">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="a72aa-706">EventHub</span><span class="sxs-lookup"><span data-stu-id="a72aa-706">EventHub</span></span>

* <span data-ttu-id="a72aa-707">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-707">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="a72aa-708">찾기</span><span class="sxs-lookup"><span data-stu-id="a72aa-708">Find</span></span>

* <span data-ttu-id="a72aa-709">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-709">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-710">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-710">HDInsight</span></span>

* <span data-ttu-id="a72aa-711">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-711">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-712">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-712">Network</span></span>

* <span data-ttu-id="a72aa-713">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-713">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-714">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a72aa-714">Rdbms</span></span>

* <span data-ttu-id="a72aa-715">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-715">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-716">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-716">Role</span></span>

* <span data-ttu-id="a72aa-717">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-717">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="a72aa-718">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-718">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a72aa-719">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-719">Service Fabric</span></span>

* <span data-ttu-id="a72aa-720">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-720">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="a72aa-721">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="a72aa-721">February 26, 2019</span></span>

<span data-ttu-id="a72aa-722">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="a72aa-722">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-723">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-723">Core</span></span>

* <span data-ttu-id="a72aa-724">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-724">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-725">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-725">ACR</span></span>

* <span data-ttu-id="a72aa-726">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-726">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="a72aa-727">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-727">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-728">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-728">ACS</span></span>

* <span data-ttu-id="a72aa-729">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-729">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-730">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-730">AppService</span></span>

* <span data-ttu-id="a72aa-731">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-731">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-732">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-732">Batch</span></span>
* <span data-ttu-id="a72aa-733">[주요 변경 사항] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-733">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="a72aa-734">[주요 변경 사항] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-734">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="a72aa-735">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-735">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="a72aa-736">[주요 변경 사항] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-736">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="a72aa-737">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-737">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="a72aa-738">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-738">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-739">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-739">CosmosDB</span></span>

* <span data-ttu-id="a72aa-740">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-740">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="a72aa-741">Kusto</span><span class="sxs-lookup"><span data-stu-id="a72aa-741">Kusto</span></span>

* <span data-ttu-id="a72aa-742">[주요 변경 사항] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-742">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-743">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-743">Network</span></span>

* <span data-ttu-id="a72aa-744">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-744">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="a72aa-745">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-745">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="a72aa-746">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-746">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="a72aa-747">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="a72aa-747">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="a72aa-748">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-748">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="a72aa-749">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-749">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="a72aa-750">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-750">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-751">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-751">Resource</span></span>

* <span data-ttu-id="a72aa-752">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-752">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="a72aa-753">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-753">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="a72aa-754">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-754">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="a72aa-755">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-755">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="a72aa-756">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-756">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-757">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-757">Role</span></span>

* <span data-ttu-id="a72aa-758">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-758">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-759">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-759">VM</span></span>

* <span data-ttu-id="a72aa-760">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-760">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="a72aa-761">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="a72aa-761">February 12, 2019</span></span>

<span data-ttu-id="a72aa-762">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="a72aa-762">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-763">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-763">Core</span></span>

* <span data-ttu-id="a72aa-764">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-764">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="a72aa-765">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-765">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-766">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-766">ACR</span></span>
* <span data-ttu-id="a72aa-767">[주요 변경 사항] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-767">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="a72aa-768">[주요 변경 사항] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-768">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-769">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-769">ACS</span></span>
* <span data-ttu-id="a72aa-770">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-770">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="a72aa-771">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-771">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="a72aa-772">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-772">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-773">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-773">AMS</span></span>
* <span data-ttu-id="a72aa-774">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-774">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="a72aa-775">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-775">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-776">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-776">Appservice</span></span>
* <span data-ttu-id="a72aa-777">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-777">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="a72aa-778">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-778">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="a72aa-779">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-779">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="a72aa-780">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-780">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="a72aa-781">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-781">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-782">Botservice</span><span class="sxs-lookup"><span data-stu-id="a72aa-782">Botservice</span></span>
* <span data-ttu-id="a72aa-783">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-783">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="a72aa-784">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-784">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="a72aa-785">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-785">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="a72aa-786">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-786">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="a72aa-787">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-787">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="a72aa-788">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-788">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="a72aa-789">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-789">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="a72aa-790">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-790">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="a72aa-791">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-791">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="a72aa-792">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-792">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="a72aa-793">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a72aa-793">Key Vault</span></span>
* <span data-ttu-id="a72aa-794">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-794">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-795">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-795">Monitor</span></span>
* <span data-ttu-id="a72aa-796">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-796">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-797">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-797">Network</span></span>
* <span data-ttu-id="a72aa-798">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-798">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="a72aa-799">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-799">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="a72aa-800">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-800">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="a72aa-801">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-801">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a72aa-802">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a72aa-802">Policy Insights</span></span>
* <span data-ttu-id="a72aa-803">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-803">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-804">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-804">RDBMS</span></span>
* <span data-ttu-id="a72aa-805">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-805">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="a72aa-806">Redis</span><span class="sxs-lookup"><span data-stu-id="a72aa-806">Redis</span></span>
* <span data-ttu-id="a72aa-807">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-807">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="a72aa-808">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-808">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="a72aa-809">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-809">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="a72aa-810">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-810">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="a72aa-811">[주요 변경 사항] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-811">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="a72aa-812">[주요 변경 사항] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-812">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="a72aa-813">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-813">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-814">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-814">Role</span></span>
* <span data-ttu-id="a72aa-815">[주요 변경 사항] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-815">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="a72aa-816">SQL VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-816">SQL VM</span></span>
* <span data-ttu-id="a72aa-817">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-817">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-818">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-818">VM</span></span>
* <span data-ttu-id="a72aa-819">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-819">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="a72aa-820">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-820">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="a72aa-821">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-821">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="a72aa-822">[주요 변경 사항] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-822">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="a72aa-823">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="a72aa-823">January 31, 2019</span></span>

<span data-ttu-id="a72aa-824">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="a72aa-824">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-825">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-825">Core</span></span>

* <span data-ttu-id="a72aa-826">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-826">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="a72aa-827">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="a72aa-827">January 28, 2019</span></span>

<span data-ttu-id="a72aa-828">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="a72aa-828">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-829">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-829">ACR</span></span>
* <span data-ttu-id="a72aa-830">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-830">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-831">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-831">ACS</span></span>
* <span data-ttu-id="a72aa-832">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-832">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a72aa-833">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-833">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="a72aa-834">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-834">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-835">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-835">AMS</span></span>
* <span data-ttu-id="a72aa-836">[주요 변경 사항] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-836">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="a72aa-837">[주요 변경 사항] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-837">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-838">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-838">Appservice</span></span>
* <span data-ttu-id="a72aa-839">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-839">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="a72aa-840">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-840">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="a72aa-841">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-841">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-842">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-842">Container</span></span>
* <span data-ttu-id="a72aa-843">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-843">Added `container start` command</span></span>
* <span data-ttu-id="a72aa-844">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-844">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a72aa-845">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a72aa-845">EventGrid</span></span>
* <span data-ttu-id="a72aa-846">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-846">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="a72aa-847">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-847">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="a72aa-848">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-848">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="a72aa-849">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-849">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="a72aa-850">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-850">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-851">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-851">HDInsight</span></span>
* <span data-ttu-id="a72aa-852">[주요 변경 사항] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-852">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="a72aa-853">[주요 변경 사항] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-853">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="a72aa-854">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-854">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="a72aa-855">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-855">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="a72aa-856">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-856">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="a72aa-857">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-857">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-858">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-858">IoT</span></span>
* <span data-ttu-id="a72aa-859">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-859">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="a72aa-860">Kusto</span><span class="sxs-lookup"><span data-stu-id="a72aa-860">Kusto</span></span>
* <span data-ttu-id="a72aa-861">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-861">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-862">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-862">Monitor</span></span>
* <span data-ttu-id="a72aa-863">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-863">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-864">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-864">Profile</span></span>
* <span data-ttu-id="a72aa-865">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-865">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-866">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-866">Network</span></span>
* <span data-ttu-id="a72aa-867">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-867">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="a72aa-868">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-868">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-869">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-869">Resource</span></span>
* <span data-ttu-id="a72aa-870">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-870">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="a72aa-871">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-871">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="a72aa-872">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="a72aa-872">SQL Virtual Machine</span></span>
* <span data-ttu-id="a72aa-873">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-873">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-874">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-874">Storage</span></span>
* <span data-ttu-id="a72aa-875">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-875">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="a72aa-876">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-876">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-877">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-877">VM</span></span>
* <span data-ttu-id="a72aa-878">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-878">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="a72aa-879">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-879">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="a72aa-880">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="a72aa-880">January 15, 2019</span></span>

<span data-ttu-id="a72aa-881">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="a72aa-881">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-882">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-882">ACR</span></span>
* <span data-ttu-id="a72aa-883">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-883">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="a72aa-884">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-884">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="a72aa-885">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="a72aa-885">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="a72aa-886">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-886">ACS</span></span>
* <span data-ttu-id="a72aa-887">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-887">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-888">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-888">Appservice</span></span>
* <span data-ttu-id="a72aa-889">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-889">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="a72aa-890">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-890">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="a72aa-891">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-891">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="a72aa-892">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-892">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-893">Botservice</span><span class="sxs-lookup"><span data-stu-id="a72aa-893">Botservice</span></span>
* <span data-ttu-id="a72aa-894">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-894">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="a72aa-895">구성</span><span class="sxs-lookup"><span data-stu-id="a72aa-895">Configure</span></span>
* <span data-ttu-id="a72aa-896">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-896">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-897">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-897">CosmosDB</span></span>
* <span data-ttu-id="a72aa-898">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-898">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-899">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-899">HDInsight</span></span>
* <span data-ttu-id="a72aa-900">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-900">Added commands for managing applications</span></span>
* <span data-ttu-id="a72aa-901">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-901">Added commands for managing script actions</span></span>
* <span data-ttu-id="a72aa-902">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-902">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="a72aa-903">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-903">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="a72aa-904">[주요 변경 사항] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-904">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-905">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-905">Network</span></span>
* <span data-ttu-id="a72aa-906">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-906">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="a72aa-907">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-907">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="a72aa-908">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-908">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="a72aa-909">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-909">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-910">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-910">Role</span></span>
* <span data-ttu-id="a72aa-911">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-911">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="a72aa-912">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-912">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="a72aa-913">보안</span><span class="sxs-lookup"><span data-stu-id="a72aa-913">Security</span></span>
* <span data-ttu-id="a72aa-914">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-914">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-915">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-915">Storage</span></span>
* <span data-ttu-id="a72aa-916">[주요 변경 사항] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-916">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="a72aa-917">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-917">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="a72aa-918">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-918">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="a72aa-919">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-919">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="a72aa-920">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-920">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-921">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-921">VM</span></span>
* <span data-ttu-id="a72aa-922">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-922">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="a72aa-923">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-923">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a72aa-924">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-924">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="a72aa-925">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-925">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="a72aa-926">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-926">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="a72aa-927">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-927">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="a72aa-928">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="a72aa-928">December 20, 2018</span></span>

<span data-ttu-id="a72aa-929">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="a72aa-929">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="a72aa-930">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-930">Appservice</span></span>
* <span data-ttu-id="a72aa-931">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-931">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="a72aa-932">웹앱 스냅샷 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-932">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="a72aa-933">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-933">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a72aa-934">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="a72aa-934">IoTCentral</span></span>
* <span data-ttu-id="a72aa-935">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-935">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-936">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-936">Role</span></span>
* <span data-ttu-id="a72aa-937">[주요 변경 사항] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-937">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-938">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-938">SQL</span></span>
* <span data-ttu-id="a72aa-939">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-939">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-940">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-940">VM</span></span>
* <span data-ttu-id="a72aa-941">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-941">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="a72aa-942">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="a72aa-942">December 18, 2018</span></span>

<span data-ttu-id="a72aa-943">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="a72aa-943">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="a72aa-944">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-944">ACR</span></span>
* <span data-ttu-id="a72aa-945">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-945">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="a72aa-946">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="a72aa-946">Condensed the table layout for task list</span></span>
* <span data-ttu-id="a72aa-947">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-947">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-948">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-948">ACS</span></span>
* <span data-ttu-id="a72aa-949">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-949">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a72aa-950">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="a72aa-950">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="a72aa-951">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-951">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="a72aa-952">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-952">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="a72aa-953">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-953">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="a72aa-954">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="a72aa-954">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-955">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-955">Appservice</span></span>
* <span data-ttu-id="a72aa-956">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-956">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="a72aa-957">Botservice</span><span class="sxs-lookup"><span data-stu-id="a72aa-957">Botservice</span></span>
* <span data-ttu-id="a72aa-958">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-958">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="a72aa-959">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="a72aa-959">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="a72aa-960">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="a72aa-960">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="a72aa-961">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="a72aa-961">Reduced Kudu network calls</span></span>
* <span data-ttu-id="a72aa-962">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-962">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-963">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-963">Consumption</span></span>
* <span data-ttu-id="a72aa-964">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-964">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-965">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-965">CosmosDB</span></span>
* <span data-ttu-id="a72aa-966">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-966">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="a72aa-967">지도</span><span class="sxs-lookup"><span data-stu-id="a72aa-967">Maps</span></span>
* <span data-ttu-id="a72aa-968">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-968">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-969">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-969">Network</span></span>
* <span data-ttu-id="a72aa-970">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-970">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="a72aa-971">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="a72aa-971">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-972">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-972">Resource</span></span>
* <span data-ttu-id="a72aa-973">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-973">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="a72aa-974">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-974">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-975">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-975">Storage</span></span>
*  <span data-ttu-id="a72aa-976">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-976">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-977">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-977">VM</span></span>
* <span data-ttu-id="a72aa-978">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-978">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="a72aa-979">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="a72aa-979">December 4, 2018</span></span>

<span data-ttu-id="a72aa-980">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="a72aa-980">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="a72aa-981">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-981">Core</span></span>
* <span data-ttu-id="a72aa-982">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-982">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="a72aa-983">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-983">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-984">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-984">Appservice</span></span>
* <span data-ttu-id="a72aa-985">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-985">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="a72aa-986">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-986">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-987">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-987">Network</span></span>
* <span data-ttu-id="a72aa-988">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-988">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-989">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-989">Role</span></span>
* <span data-ttu-id="a72aa-990">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-990">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="a72aa-991">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-991">VM</span></span>
* <span data-ttu-id="a72aa-992">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-992">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="a72aa-993">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-993">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="a72aa-994">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-994">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="a72aa-995">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-995">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="a72aa-996">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="a72aa-996">November 20, 2018</span></span>

<span data-ttu-id="a72aa-997">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="a72aa-997">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="a72aa-998">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-998">Core</span></span>
* <span data-ttu-id="a72aa-999">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-999">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1000">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1000">ACR</span></span>
* <span data-ttu-id="a72aa-1001">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1001">Added context token to task step</span></span>
* <span data-ttu-id="a72aa-1002">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1002">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="a72aa-1003">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-1003">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1004">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1004">Appservice</span></span>
* <span data-ttu-id="a72aa-1005">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1005">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="a72aa-1006">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1006">Updated the default `node_version`.</span></span> <span data-ttu-id="a72aa-1007">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1007">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="a72aa-1008">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1008">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="a72aa-1009">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1009">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a72aa-1010">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a72aa-1010">IotCentral</span></span>
* <span data-ttu-id="a72aa-1011">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1011">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-1012">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a72aa-1012">KeyVault</span></span>
* <span data-ttu-id="a72aa-1013">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1013">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1014">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1014">Network</span></span>
* <span data-ttu-id="a72aa-1015">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1015">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="a72aa-1016">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1016">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="a72aa-1017">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1017">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="a72aa-1018">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="a72aa-1018">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1019">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a72aa-1019">Rdbms</span></span>
* <span data-ttu-id="a72aa-1020">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1020">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="a72aa-1021">Rbac</span><span class="sxs-lookup"><span data-stu-id="a72aa-1021">Rbac</span></span>
* <span data-ttu-id="a72aa-1022">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1022">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="a72aa-1023">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1023">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="a72aa-1024">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1024">Storage</span></span>
* <span data-ttu-id="a72aa-1025">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1025">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="a72aa-1026">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1026">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="a72aa-1027">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1027">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="a72aa-1028">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1028">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1029">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1029">VM</span></span>
* <span data-ttu-id="a72aa-1030">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1030">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="a72aa-1031">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1031">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="a72aa-1032">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1032">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="a72aa-1033">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1033">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="a72aa-1034">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1034">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="a72aa-1035">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1035">Added `snapshot wait` command</span></span>
* <span data-ttu-id="a72aa-1036">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1036">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="a72aa-1037">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1037">November 6, 2018</span></span>

<span data-ttu-id="a72aa-1038">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="a72aa-1038">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1039">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1039">Core</span></span>
* <span data-ttu-id="a72aa-1040">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1040">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1041">ACR</span></span>
* <span data-ttu-id="a72aa-1042">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1042">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="a72aa-1043">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1043">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1044">ACS</span></span>
* <span data-ttu-id="a72aa-1045">[주요 변경 사항] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1045">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="a72aa-1046">Advisor</span><span class="sxs-lookup"><span data-stu-id="a72aa-1046">Advisor</span></span>
* <span data-ttu-id="a72aa-1047">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1047">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-1048">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1048">AMS</span></span>
* <span data-ttu-id="a72aa-1049">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1049">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="a72aa-1050">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1050">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="a72aa-1051">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1051">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="a72aa-1052">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1052">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="a72aa-1053">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1053">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="a72aa-1054">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1054">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="a72aa-1055">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1055">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="a72aa-1056">[주요 변경 사항] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1056">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="a72aa-1057">[주요 변경 사항] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1057">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="a72aa-1058">[주요 변경 사항] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1058">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="a72aa-1059">[주요 변경 사항] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1059">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="a72aa-1060">[주요 변경 사항] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1060">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="a72aa-1061">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="a72aa-1061">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="a72aa-1062">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-1062">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="a72aa-1063">[주요 변경 사항] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1063">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="a72aa-1064">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1064">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="a72aa-1065">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1065">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1066">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1066">AppService</span></span>
* <span data-ttu-id="a72aa-1067">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1067">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="a72aa-1068">구성</span><span class="sxs-lookup"><span data-stu-id="a72aa-1068">Configure</span></span>
* <span data-ttu-id="a72aa-1069">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1069">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1070">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1070">Container</span></span>
* <span data-ttu-id="a72aa-1071">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1071">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="a72aa-1072">EventHub</span><span class="sxs-lookup"><span data-stu-id="a72aa-1072">EventHub</span></span>
* <span data-ttu-id="a72aa-1073">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1073">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1074">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1074">Interactive</span></span>
* <span data-ttu-id="a72aa-1075">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1075">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1076">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1076">Monitor</span></span>
* <span data-ttu-id="a72aa-1077">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1077">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1078">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1078">Network</span></span>
* <span data-ttu-id="a72aa-1079">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1079">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="a72aa-1080">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1080">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="a72aa-1081">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1081">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="a72aa-1082">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-1082">Profile</span></span>
* <span data-ttu-id="a72aa-1083">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1083">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1084">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1084">RDBMS</span></span>
* <span data-ttu-id="a72aa-1085">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1085">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1086">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1086">Resource</span></span>
* <span data-ttu-id="a72aa-1087">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1087">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1088">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1088">Role</span></span>
* <span data-ttu-id="a72aa-1089">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1089">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="a72aa-1090">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1090">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="a72aa-1091">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1091">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1092">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1092">Storage</span></span>
* <span data-ttu-id="a72aa-1093">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1093">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1094">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1094">VM</span></span>
* <span data-ttu-id="a72aa-1095">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1095">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="a72aa-1096">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1096">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="a72aa-1097">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1097">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="a72aa-1098">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1098">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="a72aa-1099">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="a72aa-1099">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="a72aa-1100">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1100">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="a72aa-1101">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1101">October 23, 2018</span></span>

<span data-ttu-id="a72aa-1102">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="a72aa-1102">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1103">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1103">Core</span></span>
* <span data-ttu-id="a72aa-1104">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1104">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="a72aa-1105">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1105">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1106">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1106">ACR</span></span>
* <span data-ttu-id="a72aa-1107">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1107">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-1108">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-1108">CDN</span></span>
* <span data-ttu-id="a72aa-1109">[주요 변경 사항] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1109">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a72aa-1110">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1110">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1111">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1111">Container</span></span>
* <span data-ttu-id="a72aa-1112">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1112">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="a72aa-1113">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1113">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="a72aa-1114">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1114">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="a72aa-1115">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1115">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="a72aa-1116">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1116">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="a72aa-1117">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1117">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="a72aa-1118">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1118">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-1119">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-1119">CosmosDB</span></span>
* <span data-ttu-id="a72aa-1120">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1120">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1121">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1121">Interactive</span></span>
* <span data-ttu-id="a72aa-1122">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1122">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="a72aa-1123">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a72aa-1123">IoT Central</span></span>
* <span data-ttu-id="a72aa-1124">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1124">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="a72aa-1125">[주요 변경 사항] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1125">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1126">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1126">Monitor</span></span>
* <span data-ttu-id="a72aa-1127">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1127">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="a72aa-1128">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1128">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="a72aa-1129">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1129">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a72aa-1130">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1130">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="a72aa-1131">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1131">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="a72aa-1132">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1132">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="a72aa-1133">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1133">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="a72aa-1134">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1134">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a72aa-1135">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1135">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="a72aa-1136">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1136">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1137">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1137">Network</span></span>
* <span data-ttu-id="a72aa-1138">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1138">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="a72aa-1139">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1139">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="a72aa-1140">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a72aa-1140">ServiceBus</span></span>
* <span data-ttu-id="a72aa-1141">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1141">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1142">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1142">SQL</span></span>
* <span data-ttu-id="a72aa-1143">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1143">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1144">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1144">Storage</span></span>
* <span data-ttu-id="a72aa-1145">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1145">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="a72aa-1146">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1146">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1147">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1147">VM</span></span>
* <span data-ttu-id="a72aa-1148">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1148">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="a72aa-1149">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1149">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="a72aa-1150">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1150">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="a72aa-1151">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1151">October 16, 2018</span></span>

<span data-ttu-id="a72aa-1152">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="a72aa-1152">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1153">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1153">VM</span></span>
* <span data-ttu-id="a72aa-1154">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1154">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="a72aa-1155">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1155">October 9, 2018</span></span>

<span data-ttu-id="a72aa-1156">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="a72aa-1156">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1157">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1157">Core</span></span>
* <span data-ttu-id="a72aa-1158">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-1158">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1159">ACR</span></span>
* <span data-ttu-id="a72aa-1160">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1160">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1161">ACS</span></span>
* <span data-ttu-id="a72aa-1162">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="a72aa-1162">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="a72aa-1163">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1163">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="a72aa-1164">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1164">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="a72aa-1165">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-1165">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1166">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1166">Container</span></span>
* <span data-ttu-id="a72aa-1167">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1167">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="a72aa-1168">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1168">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="a72aa-1169">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="a72aa-1169">Event Hub</span></span>
* <span data-ttu-id="a72aa-1170">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1170">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="a72aa-1171">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1171">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="a72aa-1172">확장</span><span class="sxs-lookup"><span data-stu-id="a72aa-1172">Extensions</span></span>
* <span data-ttu-id="a72aa-1173">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1173">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a72aa-1174">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a72aa-1174">HDInsight</span></span>
* <span data-ttu-id="a72aa-1175">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1175">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-1176">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1176">IoT</span></span>
* <span data-ttu-id="a72aa-1177">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1177">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-1178">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a72aa-1178">KeyVault</span></span>
* <span data-ttu-id="a72aa-1179">최신 API 프로필에 keyvault 스토리지 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1179">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1180">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1180">Network</span></span>
* <span data-ttu-id="a72aa-1181">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1181">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="a72aa-1182">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="a72aa-1182">See #6052</span></span>
* <span data-ttu-id="a72aa-1183">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1183">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="a72aa-1184">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1184">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="a72aa-1185">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1185">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="a72aa-1186">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1186">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="a72aa-1187">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1187">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="a72aa-1188">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1188">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1189">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1189">Role</span></span>
* <span data-ttu-id="a72aa-1190">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1190">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="a72aa-1191">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1191">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="a72aa-1192">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1192">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="a72aa-1193">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1193">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="a72aa-1194">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a72aa-1194">Service Bus</span></span>
* <span data-ttu-id="a72aa-1195">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1195">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1196">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1196">VM</span></span>
* <span data-ttu-id="a72aa-1197">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1197">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="a72aa-1198">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1198">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="a72aa-1199">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1199">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="a72aa-1200">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1200">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="a72aa-1201">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1201">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="a72aa-1202">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1202">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="a72aa-1203">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1203">September 21, 2018</span></span>

<span data-ttu-id="a72aa-1204">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="a72aa-1204">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1205">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1205">ACR</span></span>
* <span data-ttu-id="a72aa-1206">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1206">Added ACR Task commands</span></span>
* <span data-ttu-id="a72aa-1207">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1207">Added quick run command</span></span>
* <span data-ttu-id="a72aa-1208">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1208">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="a72aa-1209">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1209">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="a72aa-1210">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1210">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="a72aa-1211">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1211">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1212">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1212">ACS</span></span>
* <span data-ttu-id="a72aa-1213">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1213">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="a72aa-1214">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1214">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1215">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1215">AppService</span></span>

* <span data-ttu-id="a72aa-1216">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1216">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="a72aa-1217">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1217">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="a72aa-1218">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1218">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="a72aa-1219">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1219">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-1220">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-1220">Batch</span></span>
* <span data-ttu-id="a72aa-1221">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1221">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="a72aa-1222">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1222">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="a72aa-1223">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1223">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="a72aa-1224">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1224">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a72aa-1225">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1225">Batch AI</span></span> 
* <span data-ttu-id="a72aa-1226">`batchai cluster create` 명령에서 자동 스토리지 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1226">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a72aa-1227">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a72aa-1227">Cognitive Services</span></span>
* <span data-ttu-id="a72aa-1228">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1228">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="a72aa-1229">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1229">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="a72aa-1230">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1230">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="a72aa-1231">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1231">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="a72aa-1232">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1232">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="a72aa-1233">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1233">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1234">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1234">Container</span></span>
* <span data-ttu-id="a72aa-1235">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1235">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="a72aa-1236">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1236">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="a72aa-1237">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1237">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="a72aa-1238">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1238">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="a72aa-1239">Datalake</span><span class="sxs-lookup"><span data-stu-id="a72aa-1239">Datalake</span></span>
* <span data-ttu-id="a72aa-1240">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1240">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="a72aa-1241">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="a72aa-1241">Interactive Shell</span></span>
* <span data-ttu-id="a72aa-1242">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1242">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="a72aa-1243">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1243">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-1244">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1244">IoT</span></span>
* <span data-ttu-id="a72aa-1245">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1245">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="a72aa-1246">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a72aa-1246">Key Vault</span></span>
* <span data-ttu-id="a72aa-1247">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1247">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1248">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1248">Network</span></span>
* <span data-ttu-id="a72aa-1249">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1249">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="a72aa-1250">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1250">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="a72aa-1251">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1251">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="a72aa-1252">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1252">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="a72aa-1253">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1253">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="a72aa-1254">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1254">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="a72aa-1255">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1255">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="a72aa-1256">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1256">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="a72aa-1257">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1257">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="a72aa-1258">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1258">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="a72aa-1259">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1259">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="a72aa-1260">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1260">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="a72aa-1261">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1261">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="a72aa-1262">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1262">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="a72aa-1263">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1263">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="a72aa-1264">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1264">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="a72aa-1265">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1265">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="a72aa-1266">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1266">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1267">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1267">RDBMS</span></span>
* <span data-ttu-id="a72aa-1268">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1268">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="a72aa-1269">예약</span><span class="sxs-lookup"><span data-stu-id="a72aa-1269">Reservation</span></span>
* <span data-ttu-id="a72aa-1270">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1270">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="a72aa-1271">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1271">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="a72aa-1272">앱 관리</span><span class="sxs-lookup"><span data-stu-id="a72aa-1272">Manage App</span></span>
* <span data-ttu-id="a72aa-1273">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1273">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="a72aa-1274">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1274">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1275">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1275">Role</span></span>
* <span data-ttu-id="a72aa-1276">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1276">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="a72aa-1277">SignalR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1277">SignalR</span></span>
* <span data-ttu-id="a72aa-1278">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1278">First release</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1279">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1279">Storage</span></span>
* <span data-ttu-id="a72aa-1280">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1280">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="a72aa-1281">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1281">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1282">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1282">VM</span></span>
* <span data-ttu-id="a72aa-1283">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="a72aa-1283">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="a72aa-1284">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1284">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="a72aa-1285">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1285">August 28, 2018</span></span>

<span data-ttu-id="a72aa-1286">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a72aa-1286">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1287">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1287">Core</span></span>

* <span data-ttu-id="a72aa-1288">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1288">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a72aa-1289">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1289">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1290">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1290">ACR</span></span>

* <span data-ttu-id="a72aa-1291">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1291">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a72aa-1292">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1292">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1293">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1293">ACS</span></span>

* <span data-ttu-id="a72aa-1294">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1294">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a72aa-1295">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1295">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1296">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1296">AppService</span></span>

* <span data-ttu-id="a72aa-1297">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1297">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a72aa-1298">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1298">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a72aa-1299">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1299">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a72aa-1300">Backup</span><span class="sxs-lookup"><span data-stu-id="a72aa-1300">Backup</span></span>

* <span data-ttu-id="a72aa-1301">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1301">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a72aa-1302">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1302">Bot Service</span></span>

* <span data-ttu-id="a72aa-1303">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1303">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a72aa-1304">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a72aa-1304">Cognitive Services</span></span>

* <span data-ttu-id="a72aa-1305">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1305">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-1306">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1306">IoT</span></span>

* <span data-ttu-id="a72aa-1307">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1307">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1308">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1308">Monitor</span></span>

* <span data-ttu-id="a72aa-1309">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1309">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a72aa-1310">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="a72aa-1310">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1311">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1311">Network</span></span>

* <span data-ttu-id="a72aa-1312">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1312">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1313">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1313">Resource</span></span>

* <span data-ttu-id="a72aa-1314">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1314">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1315">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1315">Storage</span></span>

* <span data-ttu-id="a72aa-1316">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1316">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1317">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1317">VM</span></span>

* <span data-ttu-id="a72aa-1318">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1318">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a72aa-1319">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1319">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="a72aa-1320">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1320">Auguest 14, 2018</span></span>

<span data-ttu-id="a72aa-1321">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a72aa-1321">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1322">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1322">Core</span></span>

* <span data-ttu-id="a72aa-1323">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1323">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a72aa-1324">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="a72aa-1324">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a72aa-1325">원격 분석</span><span class="sxs-lookup"><span data-stu-id="a72aa-1325">Telemetry</span></span>

* <span data-ttu-id="a72aa-1326">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="a72aa-1326">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1327">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1327">ACR</span></span>

* <span data-ttu-id="a72aa-1328">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1328">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a72aa-1329">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1329">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1330">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1330">ACS</span></span>

* <span data-ttu-id="a72aa-1331">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1331">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a72aa-1332">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1332">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a72aa-1333">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1333">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a72aa-1334">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1334">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a72aa-1335">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1335">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a72aa-1336">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1336">AppService</span></span>

* <span data-ttu-id="a72aa-1337">외부 리소스 그룹에 스토리지 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1337">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a72aa-1338">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1338">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-1339">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1339">BatchAI</span></span>

* <span data-ttu-id="a72aa-1340">자동 스토리지 계정 만들기가 &quot;리소스 *그룹*&quot;을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1340">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a72aa-1341">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1341">Container</span></span>

* <span data-ttu-id="a72aa-1342">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1342">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a72aa-1343">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1343">IoT</span></span>

* <span data-ttu-id="a72aa-1344">[주요 변경 사항] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="a72aa-1344">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a72aa-1345">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1345">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a72aa-1346">Iot Central</span><span class="sxs-lookup"><span data-stu-id="a72aa-1346">Iot Central</span></span>

* <span data-ttu-id="a72aa-1347">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1347">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-1348">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a72aa-1348">KeyVault</span></span>


* <span data-ttu-id="a72aa-1349">스토리지 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1349">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a72aa-1350">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1350">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a72aa-1351">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1351">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a72aa-1352">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1352">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a72aa-1353">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1353">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a72aa-1354">릴레이</span><span class="sxs-lookup"><span data-stu-id="a72aa-1354">Relay</span></span>

* <span data-ttu-id="a72aa-1355">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1355">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1356">Sql</span><span class="sxs-lookup"><span data-stu-id="a72aa-1356">Sql</span></span>

* <span data-ttu-id="a72aa-1357">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1357">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1358">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1358">Storage</span></span>

* <span data-ttu-id="a72aa-1359">[주요 변경 사항] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1359">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a72aa-1360">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1360">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a72aa-1361">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1361">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a72aa-1362">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1362">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a72aa-1363">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1363">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1364">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1364">VM</span></span>

* <span data-ttu-id="a72aa-1365">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1365">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a72aa-1366">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1366">July 31, 2018</span></span>

<span data-ttu-id="a72aa-1367">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a72aa-1367">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1368">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1368">ACR</span></span>

* <span data-ttu-id="a72aa-1369">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1369">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a72aa-1370">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1370">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1371">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1371">ACS</span></span>

* <span data-ttu-id="a72aa-1372">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1372">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-1373">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-1373">Batch</span></span>

* <span data-ttu-id="a72aa-1374">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1374">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1375">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1375">Container</span></span>

* <span data-ttu-id="a72aa-1376">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1376">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1377">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1377">Network</span></span>

* <span data-ttu-id="a72aa-1378">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1378">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a72aa-1379">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1379">Resource</span></span>

* <span data-ttu-id="a72aa-1380">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1380">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a72aa-1381">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1381">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1382">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1382">Role</span></span>

* <span data-ttu-id="a72aa-1383">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1383">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a72aa-1384">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1384">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a72aa-1385">검색</span><span class="sxs-lookup"><span data-stu-id="a72aa-1385">Search</span></span>

* <span data-ttu-id="a72aa-1386">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1386">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a72aa-1387">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a72aa-1387">Service Bus</span></span>

* <span data-ttu-id="a72aa-1388">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1388">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a72aa-1389">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1389">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="a72aa-1390">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="a72aa-1390">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="a72aa-1391">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="a72aa-1391">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1392">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1392">Storage</span></span>

* <span data-ttu-id="a72aa-1393">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1393">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a72aa-1394">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="a72aa-1394">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1395">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1395">VM</span></span>

* <span data-ttu-id="a72aa-1396">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1396">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a72aa-1397">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1397">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="a72aa-1398">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1398">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a72aa-1399">[주요 변경 사항] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1399">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a72aa-1400">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1400">July 18, 2018</span></span>

<span data-ttu-id="a72aa-1401">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a72aa-1401">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1402">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1402">Core</span></span>

* <span data-ttu-id="a72aa-1403">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1403">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a72aa-1404">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1404">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a72aa-1405">[주요 변경 사항] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1405">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1406">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1406">ACR</span></span>

* <span data-ttu-id="a72aa-1407">[주요 변경 사항] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1407">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a72aa-1408">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1408">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a72aa-1409">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1409">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a72aa-1410">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1410">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1411">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1411">ACS</span></span>

* <span data-ttu-id="a72aa-1412">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1412">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1413">AppService</span></span>

* <span data-ttu-id="a72aa-1414">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1414">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-1415">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-1415">Batch</span></span>

* <span data-ttu-id="a72aa-1416">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1416">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a72aa-1417">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1417">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a72aa-1418">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1418">Batch AI</span></span>

* <span data-ttu-id="a72aa-1419">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1419">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1420">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1420">Container</span></span>

* <span data-ttu-id="a72aa-1421">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1421">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a72aa-1422">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1422">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1423">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1423">Network</span></span>

* <span data-ttu-id="a72aa-1424">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1424">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="a72aa-1425">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1425">Added `network nic wait`</span></span>
* <span data-ttu-id="a72aa-1426">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1426">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="a72aa-1427">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1427">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="a72aa-1428">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1428">Resource</span></span>

* <span data-ttu-id="a72aa-1429">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1429">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="a72aa-1430">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1430">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="a72aa-1431">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1431">Added `deployment wait` command</span></span>
* <span data-ttu-id="a72aa-1432">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1432">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1433">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1433">SQL</span></span>

* <span data-ttu-id="a72aa-1434">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1434">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a72aa-1435">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1435">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="a72aa-1436">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1436">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1437">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1437">Storage</span></span>

* <span data-ttu-id="a72aa-1438">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1438">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1439">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1439">VM</span></span>

* <span data-ttu-id="a72aa-1440">[주요 변경 사항] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1440">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a72aa-1441">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1441">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="a72aa-1442">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1442">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a72aa-1443">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1443">July 3, 2018</span></span>

<span data-ttu-id="a72aa-1444">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a72aa-1444">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a72aa-1445">AKS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1445">AKS</span></span>

* <span data-ttu-id="a72aa-1446">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1446">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a72aa-1447">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1447">July 3, 2018</span></span>

<span data-ttu-id="a72aa-1448">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a72aa-1448">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1449">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1449">Core</span></span>

* <span data-ttu-id="a72aa-1450">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1450">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1451">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1451">ACR</span></span>

* <span data-ttu-id="a72aa-1452">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1452">Added polling build status</span></span>
* <span data-ttu-id="a72aa-1453">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1453">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a72aa-1454">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1454">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1455">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1455">ACS</span></span>

* <span data-ttu-id="a72aa-1456">[주요 변경 사항]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1456">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a72aa-1457">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1457">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a72aa-1458">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1458">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a72aa-1459">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1459">Added `--listen-port` support</span></span>
* <span data-ttu-id="a72aa-1460">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1460">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a72aa-1461">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1461">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a72aa-1462">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1462">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1463">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1463">AppService</span></span>

* <span data-ttu-id="a72aa-1464">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1464">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="a72aa-1465">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1465">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a72aa-1466">Backup</span><span class="sxs-lookup"><span data-stu-id="a72aa-1466">Backup</span></span>

* <span data-ttu-id="a72aa-1467">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1467">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-1468">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1468">BatchAI</span></span>

* <span data-ttu-id="a72aa-1469">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1469">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a72aa-1470">클라우드</span><span class="sxs-lookup"><span data-stu-id="a72aa-1470">Cloud</span></span>

* <span data-ttu-id="a72aa-1471">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1471">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1472">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1472">Container</span></span>

* <span data-ttu-id="a72aa-1473">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1473">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a72aa-1474">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1474">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="a72aa-1475">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1475">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1476">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1476">Extension</span></span>

* <span data-ttu-id="a72aa-1477">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1477">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1478">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1478">Network</span></span>

* <span data-ttu-id="a72aa-1479">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="a72aa-1479">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1480">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a72aa-1480">Rdbms</span></span>

* <span data-ttu-id="a72aa-1481">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1481">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1482">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1482">Resource</span></span>

* <span data-ttu-id="a72aa-1483">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1483">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1484">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1484">VM</span></span>

* <span data-ttu-id="a72aa-1485">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1485">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a72aa-1486">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1486">June 25, 2018</span></span>

<span data-ttu-id="a72aa-1487">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a72aa-1487">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a72aa-1488">CLI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1488">CLI</span></span>

* <span data-ttu-id="a72aa-1489">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1489">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a72aa-1490">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1490">June 19, 2018</span></span>

<span data-ttu-id="a72aa-1491">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a72aa-1491">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1492">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1492">Core</span></span>

* <span data-ttu-id="a72aa-1493">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1493">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1494">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1494">ACR</span></span>

* <span data-ttu-id="a72aa-1495">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1495">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a72aa-1496">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1496">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1497">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1497">ACS</span></span>

* <span data-ttu-id="a72aa-1498">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1498">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a72aa-1499">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1499">Added `--update` support</span></span>
* <span data-ttu-id="a72aa-1500">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1500">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="a72aa-1501">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="a72aa-1501">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a72aa-1502">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1502">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a72aa-1503">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1503">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="a72aa-1504">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1504">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="a72aa-1505">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1505">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1506">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1506">AppService</span></span>

* <span data-ttu-id="a72aa-1507">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1507">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a72aa-1508">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1508">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-1509">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-1509">Batch</span></span>

* <span data-ttu-id="a72aa-1510">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1510">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a72aa-1511">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1511">Batch AI</span></span>

* <span data-ttu-id="a72aa-1512">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1512">Added support for workspaces.</span></span> <span data-ttu-id="a72aa-1513">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1513">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a72aa-1514">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1514">Added support for experiments.</span></span> <span data-ttu-id="a72aa-1515">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1515">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a72aa-1516">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1516">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a72aa-1517">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1517">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a72aa-1518">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1518">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a72aa-1519">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1519">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a72aa-1520">[주요 변경 사항] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-1520">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a72aa-1521">[주요 변경 사항] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-1521">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a72aa-1522">[주요 변경 사항] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1522">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a72aa-1523">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="a72aa-1523">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a72aa-1524">[주요 변경 사항] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1524">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a72aa-1525">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="a72aa-1525">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a72aa-1526">[주요 변경 사항] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1526">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a72aa-1527">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1527">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a72aa-1528">[주요 변경 사항] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1528">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a72aa-1529">[주요 변경 사항] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1529">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="a72aa-1530">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="a72aa-1530">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="a72aa-1531">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="a72aa-1531">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a72aa-1532">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="a72aa-1532">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a72aa-1533">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="a72aa-1533">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a72aa-1534">지도</span><span class="sxs-lookup"><span data-stu-id="a72aa-1534">Maps</span></span>

* <span data-ttu-id="a72aa-1535">[주요 변경 사항] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1535">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1536">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1536">Network</span></span>

* <span data-ttu-id="a72aa-1537">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1537">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a72aa-1538">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1538">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a72aa-1539">#6502</span><span class="sxs-lookup"><span data-stu-id="a72aa-1539">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a72aa-1540">예약</span><span class="sxs-lookup"><span data-stu-id="a72aa-1540">Reservations</span></span>

* <span data-ttu-id="a72aa-1541">[주요 변경 사항] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1541">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="a72aa-1542">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1542">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="a72aa-1543">[주요 변경 사항] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1543">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="a72aa-1544">[주요 변경 사항] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1544">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="a72aa-1545">[주요 변경 사항] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1545">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="a72aa-1546">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1546">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1547">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1547">Role</span></span>

* <span data-ttu-id="a72aa-1548">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="a72aa-1548">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1549">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1549">SQL</span></span>

* <span data-ttu-id="a72aa-1550">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1550">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1551">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1551">Storage</span></span>

* <span data-ttu-id="a72aa-1552">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1552">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1553">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1553">VM</span></span>

* <span data-ttu-id="a72aa-1554">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-1554">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="a72aa-1555">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1555">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="a72aa-1556">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1556">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a72aa-1557">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1557">June 13, 2018</span></span>

<span data-ttu-id="a72aa-1558">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a72aa-1558">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1559">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1559">Core</span></span>

* <span data-ttu-id="a72aa-1560">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="a72aa-1560">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a72aa-1561">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1561">June 13, 2018</span></span>

<span data-ttu-id="a72aa-1562">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a72aa-1562">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a72aa-1563">AKS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1563">AKS</span></span>

* <span data-ttu-id="a72aa-1564">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1564">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a72aa-1565">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="a72aa-1565">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a72aa-1566">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1566">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a72aa-1567">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1567">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a72aa-1568">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1568">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1569">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1569">AppService</span></span>

* <span data-ttu-id="a72aa-1570">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1570">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a72aa-1571">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1571">June 5, 2018</span></span>

<span data-ttu-id="a72aa-1572">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a72aa-1572">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1573">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1573">Interactive</span></span>

* <span data-ttu-id="a72aa-1574">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1574">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a72aa-1575">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1575">June 5, 2018</span></span>

<span data-ttu-id="a72aa-1576">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a72aa-1576">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1577">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1577">Core</span></span>

* <span data-ttu-id="a72aa-1578">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1578">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a72aa-1579">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1579">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1580">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1580">ACR</span></span>

* <span data-ttu-id="a72aa-1581">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1581">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a72aa-1582">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1582">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a72aa-1583">AKS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1583">AKS</span></span>

* <span data-ttu-id="a72aa-1584">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1584">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-1585">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-1585">Batch</span></span>

* <span data-ttu-id="a72aa-1586">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a72aa-1586">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-1587">IOT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1587">IOT</span></span>

* <span data-ttu-id="a72aa-1588">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1588">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1589">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1589">Network</span></span>

* <span data-ttu-id="a72aa-1590">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="a72aa-1590">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a72aa-1591">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a72aa-1591">Policy Insights</span></span>

* <span data-ttu-id="a72aa-1592">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1592">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a72aa-1593">ARM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1593">ARM</span></span>

* <span data-ttu-id="a72aa-1594">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1594">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1595">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1595">SQL</span></span>

* <span data-ttu-id="a72aa-1596">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1596">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a72aa-1597">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1597">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a72aa-1598">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1598">Storage</span></span>

* <span data-ttu-id="a72aa-1599">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1599">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1600">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1600">VM</span></span>

* <span data-ttu-id="a72aa-1601">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1601">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a72aa-1602">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1602">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a72aa-1603">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1603">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a72aa-1604">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1604">May 22, 2018</span></span>

<span data-ttu-id="a72aa-1605">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a72aa-1605">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1606">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1606">Core</span></span>

* <span data-ttu-id="a72aa-1607">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1607">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1608">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1608">ACS</span></span>

* <span data-ttu-id="a72aa-1609">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1609">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a72aa-1610">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1610">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1611">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-1611">AppService</span></span>

* <span data-ttu-id="a72aa-1612">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1612">Improved generic update commands</span></span>
* <span data-ttu-id="a72aa-1613">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1613">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1614">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1614">Container</span></span>

* <span data-ttu-id="a72aa-1615">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1615">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a72aa-1616">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1616">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1617">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1617">Extension</span></span>

* <span data-ttu-id="a72aa-1618">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1618">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1619">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1619">Interactive</span></span>

* <span data-ttu-id="a72aa-1620">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1620">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a72aa-1621">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1621">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-1622">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a72aa-1622">KeyVault</span></span>

* <span data-ttu-id="a72aa-1623">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1623">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1624">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1624">Network</span></span>

* <span data-ttu-id="a72aa-1625">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1625">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a72aa-1626">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1626">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1627">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1627">SQL</span></span>

* <span data-ttu-id="a72aa-1628">[주요 변경 사항] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="a72aa-1628">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a72aa-1629">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="a72aa-1629">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a72aa-1630">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1630">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a72aa-1631">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1631">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a72aa-1632">[주요 변경 사항] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1632">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a72aa-1633">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1633">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a72aa-1634">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1634">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a72aa-1635">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1635">`edition`.</span></span> <span data-ttu-id="a72aa-1636">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1636">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a72aa-1637">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1637">`elasticPoolName`.</span></span> <span data-ttu-id="a72aa-1638">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1638">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a72aa-1639">[주요 변경 사항] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1639">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a72aa-1640">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1640">`edition`.</span></span> <span data-ttu-id="a72aa-1641">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1641">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a72aa-1642">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1642">`dtu`.</span></span> <span data-ttu-id="a72aa-1643">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1643">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a72aa-1644">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1644">`databaseDtuMin`.</span></span> <span data-ttu-id="a72aa-1645">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1645">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a72aa-1646">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1646">`databaseDtuMax`.</span></span> <span data-ttu-id="a72aa-1647">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1647">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a72aa-1648">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1648">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a72aa-1649">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1649">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1650">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1650">Storage</span></span>

* <span data-ttu-id="a72aa-1651">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1651">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a72aa-1652">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1652">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1653">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1653">VM</span></span>

* <span data-ttu-id="a72aa-1654">[주요 변경 사항] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1654">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a72aa-1655">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1655">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a72aa-1656">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1656">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a72aa-1657">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1657">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a72aa-1658">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1658">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a72aa-1659">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1659">May 7, 2018</span></span>

<span data-ttu-id="a72aa-1660">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a72aa-1660">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1661">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1661">Core</span></span>

* <span data-ttu-id="a72aa-1662">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1662">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a72aa-1663">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1663">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a72aa-1664">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1664">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a72aa-1665">#5591</span><span class="sxs-lookup"><span data-stu-id="a72aa-1665">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a72aa-1666">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1666">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a72aa-1667">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-1667">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a72aa-1668">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1668">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a72aa-1669">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1669">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a72aa-1670">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1670">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1671">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1671">ACR</span></span>

* <span data-ttu-id="a72aa-1672">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1672">Added ACR Build commands</span></span>
* <span data-ttu-id="a72aa-1673">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1673">Improved resource not found error messages</span></span>
* <span data-ttu-id="a72aa-1674">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1674">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a72aa-1675">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1675">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a72aa-1676">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1676">Improved repository commands error messages</span></span>
* <span data-ttu-id="a72aa-1677">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1677">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1678">ACS</span></span>

* <span data-ttu-id="a72aa-1679">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1679">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a72aa-1680">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1680">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a72aa-1681">AMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1681">AMS</span></span>

* <span data-ttu-id="a72aa-1682">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="a72aa-1682">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1683">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1683">Appservice</span></span>

* <span data-ttu-id="a72aa-1684">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1684">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a72aa-1685">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1685">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a72aa-1686">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1686">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a72aa-1687">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1687">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a72aa-1688">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1688">Batch AI</span></span>

* <span data-ttu-id="a72aa-1689">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1689">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a72aa-1690">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a72aa-1690">Cognitive Services</span></span>

* <span data-ttu-id="a72aa-1691">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1691">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-1692">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-1692">Consumption</span></span>

* <span data-ttu-id="a72aa-1693">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1693">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1694">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1694">Container</span></span>

* <span data-ttu-id="a72aa-1695">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1695">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a72aa-1696">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a72aa-1696">Cosmos DB</span></span>

* <span data-ttu-id="a72aa-1697">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a72aa-1697">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a72aa-1698">DMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1698">DMS</span></span>

* <span data-ttu-id="a72aa-1699">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1699">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1700">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1700">Extension</span></span>

* <span data-ttu-id="a72aa-1701">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1701">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1702">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1702">Interactive</span></span>

* <span data-ttu-id="a72aa-1703">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1703">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a72aa-1704">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="a72aa-1704">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a72aa-1705">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1705">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a72aa-1706">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1706">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a72aa-1707">랩</span><span class="sxs-lookup"><span data-stu-id="a72aa-1707">Lab</span></span>

* <span data-ttu-id="a72aa-1708">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1708">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1709">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1709">Network</span></span>

* <span data-ttu-id="a72aa-1710">[주요 변경 사항] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1710">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a72aa-1711">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-1711">Profile</span></span>

* <span data-ttu-id="a72aa-1712">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1712">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a72aa-1713">[주요 변경 사항] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1713">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a72aa-1714">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1714">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a72aa-1715">Redis</span><span class="sxs-lookup"><span data-stu-id="a72aa-1715">Redis</span></span>

* <span data-ttu-id="a72aa-1716">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1716">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a72aa-1717">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1717">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a72aa-1718">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1718">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a72aa-1719">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1719">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a72aa-1720">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1720">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1721">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1721">Role</span></span>

* <span data-ttu-id="a72aa-1722">[주요 변경 사항] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1722">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1723">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1723">Storage</span></span>

* <span data-ttu-id="a72aa-1724">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1724">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a72aa-1725">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="a72aa-1725">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a72aa-1726">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="a72aa-1726">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a72aa-1727">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1727">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a72aa-1728">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1728">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1729">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1729">VM</span></span>

* <span data-ttu-id="a72aa-1730">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1730">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a72aa-1731">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1731">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a72aa-1732">[주요 변경 사항] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1732">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a72aa-1733">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1733">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a72aa-1734">[주요 변경 사항] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1734">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a72aa-1735">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1735">Added write accelerator support</span></span>
* <span data-ttu-id="a72aa-1736">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1736">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a72aa-1737">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1737">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a72aa-1738">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1738">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a72aa-1739">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1739">April 10, 2018</span></span>

<span data-ttu-id="a72aa-1740">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a72aa-1740">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1741">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1741">ACR</span></span>

* <span data-ttu-id="a72aa-1742">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="a72aa-1742">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1743">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1743">ACS</span></span>

* <span data-ttu-id="a72aa-1744">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1744">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1745">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1745">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a72aa-1747">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1747">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-1748">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a72aa-1748">BatchAI</span></span>

* <span data-ttu-id="a72aa-1749">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1749">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="a72aa-1750">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="a72aa-1750">Job level mounting</span></span>
  - <span data-ttu-id="a72aa-1751">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="a72aa-1751">Environment variables with secret values</span></span>
  - <span data-ttu-id="a72aa-1752">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1752">Performance counters settings</span></span>
  - <span data-ttu-id="a72aa-1753">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="a72aa-1753">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="a72aa-1754">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-1754">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="a72aa-1755">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="a72aa-1755">Usage and limits reporting</span></span>
  - <span data-ttu-id="a72aa-1756">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1756">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="a72aa-1757">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-1757">Support for custom images</span></span>
  - <span data-ttu-id="a72aa-1758">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1758">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a72aa-1759">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1759">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a72aa-1760">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1760">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a72aa-1761">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1761">National clouds are supported</span></span>
* <span data-ttu-id="a72aa-1762">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1762">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a72aa-1763">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1763">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a72aa-1764">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1764">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a72aa-1765">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1765">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a72aa-1766">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="a72aa-1766">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a72aa-1767">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="a72aa-1767">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a72aa-1768">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1768">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a72aa-1769">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1769">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a72aa-1770">이 옵션을 사용하면 보다 쉽게 스토리지 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1770">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a72aa-1771">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1771">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a72aa-1772">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1772">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a72aa-1773">[주요 변경 사항] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1773">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a72aa-1774">[주요 변경 사항] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1774">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a72aa-1775">결제</span><span class="sxs-lookup"><span data-stu-id="a72aa-1775">Billing</span></span>

* <span data-ttu-id="a72aa-1776">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1776">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-1777">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-1777">Consumption</span></span>

* <span data-ttu-id="a72aa-1778">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1778">Added `marketplace` commands</span></span>
* <span data-ttu-id="a72aa-1779">[주요 변경 사항] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1779">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a72aa-1780">[주요 변경 사항] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1780">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a72aa-1781">[주요 변경 사항] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1781">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a72aa-1782">[주요 변경 사항] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1782">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a72aa-1783">[주요 변경 사항] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1783">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1784">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1784">Container</span></span>

* <span data-ttu-id="a72aa-1785">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1785">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a72aa-1786">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="a72aa-1786">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1787">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1787">Extension</span></span>

* <span data-ttu-id="a72aa-1788">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1788">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1789">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1789">Interactive</span></span>

* <span data-ttu-id="a72aa-1790">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1790">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a72aa-1791">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1791">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a72aa-1792">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1792">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1793">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1793">Network</span></span>

* <span data-ttu-id="a72aa-1794">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1794">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a72aa-1795">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1795">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a72aa-1796">#4910</span><span class="sxs-lookup"><span data-stu-id="a72aa-1796">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a72aa-1797">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1797">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a72aa-1798">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1798">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a72aa-1799">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1799">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a72aa-1800">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1800">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a72aa-1801">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1801">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-1802">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-1802">Profile</span></span>

* <span data-ttu-id="a72aa-1803">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1803">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a72aa-1804">[주요 변경 사항] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1804">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1805">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1805">RDBMS</span></span>

* <span data-ttu-id="a72aa-1806">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1806">Added `georestore` command</span></span>
* <span data-ttu-id="a72aa-1807">`create` 명령에서 스토리지 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1807">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1808">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1808">Resource</span></span>

* <span data-ttu-id="a72aa-1809">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1809">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a72aa-1810">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1810">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1811">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1811">SQL</span></span>

* <span data-ttu-id="a72aa-1812">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1812">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1813">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1813">Storage</span></span>

* <span data-ttu-id="a72aa-1814">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1814">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1815">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1815">VM</span></span>

* <span data-ttu-id="a72aa-1816">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1816">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a72aa-1817">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1817">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a72aa-1819">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1819">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a72aa-1820">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1820">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a72aa-1821">#5718</span><span class="sxs-lookup"><span data-stu-id="a72aa-1821">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a72aa-1822">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1822">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a72aa-1823">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1823">March 27, 2018</span></span>

<span data-ttu-id="a72aa-1824">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a72aa-1824">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1825">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1825">Core</span></span>

* <span data-ttu-id="a72aa-1826">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="a72aa-1826">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1827">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1827">ACS</span></span>

* <span data-ttu-id="a72aa-1828">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1828">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1829">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1829">Appservice</span></span>

* <span data-ttu-id="a72aa-1830">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1830">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a72aa-1831">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1831">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a72aa-1832">Backup</span><span class="sxs-lookup"><span data-stu-id="a72aa-1832">Backup</span></span>

* <span data-ttu-id="a72aa-1833">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1833">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a72aa-1834">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1834">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a72aa-1835">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1835">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a72aa-1836">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1836">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1837">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1837">Container</span></span>

* <span data-ttu-id="a72aa-1838">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1838">Added `container exec` command.</span></span> <span data-ttu-id="a72aa-1839">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-1839">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a72aa-1840">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-1840">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1841">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1841">Extension</span></span>

* <span data-ttu-id="a72aa-1842">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1842">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a72aa-1843">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1843">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a72aa-1844">[주요 변경 사항] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1844">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1845">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1845">Interactive</span></span>

* <span data-ttu-id="a72aa-1846">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="a72aa-1846">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a72aa-1847">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1847">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a72aa-1848">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1848">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a72aa-1849">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1849">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a72aa-1850">랩</span><span class="sxs-lookup"><span data-stu-id="a72aa-1850">Lab</span></span>

* <span data-ttu-id="a72aa-1851">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1851">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1852">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1852">Monitor</span></span>

* <span data-ttu-id="a72aa-1853">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1853">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a72aa-1854">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1854">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a72aa-1855">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1855">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1856">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1856">Network</span></span>

* <span data-ttu-id="a72aa-1857">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1857">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-1858">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-1858">Profile</span></span>

* <span data-ttu-id="a72aa-1859">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1859">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1860">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1860">RDBMS</span></span>

* <span data-ttu-id="a72aa-1861">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1861">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1862">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1862">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a72aa-1864">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1864">Role</span></span>

* <span data-ttu-id="a72aa-1865">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1865">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a72aa-1866">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1866">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a72aa-1867">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1867">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a72aa-1868">[주요 변경 사항] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1868">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a72aa-1869">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1869">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1870">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1870">Storage</span></span>

* <span data-ttu-id="a72aa-1871">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1871">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a72aa-1872">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="a72aa-1872">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1873">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1873">VM</span></span>

* <span data-ttu-id="a72aa-1874">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1874">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a72aa-1875">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1875">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a72aa-1876">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1876">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a72aa-1877">[주요 변경 사항] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1877">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a72aa-1878">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1878">March 13, 2018</span></span>

<span data-ttu-id="a72aa-1879">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a72aa-1879">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-1880">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-1880">ACR</span></span>

* <span data-ttu-id="a72aa-1881">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1881">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a72aa-1882">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1882">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a72aa-1883">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1883">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1884">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1884">ACS</span></span>

* <span data-ttu-id="a72aa-1885">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1885">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a72aa-1886">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1886">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a72aa-1887">Advisor</span><span class="sxs-lookup"><span data-stu-id="a72aa-1887">Advisor</span></span>

* <span data-ttu-id="a72aa-1888">[주요 변경 사항] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1888">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a72aa-1889">[주요 변경 사항] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1889">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a72aa-1890">[주요 변경 사항] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1890">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="a72aa-1891">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1891">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a72aa-1892">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1892">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1893">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1893">Appservice</span></span>

* <span data-ttu-id="a72aa-1894">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1894">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a72aa-1895">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1895">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a72aa-1896">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="a72aa-1896">Eventhubs</span></span>

* <span data-ttu-id="a72aa-1897">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1897">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1898">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1898">Extension</span></span>

* <span data-ttu-id="a72aa-1899">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1899">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1900">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1900">Interactive</span></span>

* <span data-ttu-id="a72aa-1901">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1901">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a72aa-1902">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="a72aa-1902">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a72aa-1903">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1903">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a72aa-1904">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1904">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1905">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1905">Monitor</span></span>

* <span data-ttu-id="a72aa-1906">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1906">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a72aa-1907">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1907">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a72aa-1908">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1908">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a72aa-1909">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1909">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1910">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1910">Network</span></span>

* <span data-ttu-id="a72aa-1911">[주요 변경 사항] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1911">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a72aa-1912">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="a72aa-1912">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a72aa-1913">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1913">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a72aa-1914">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1914">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-1915">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-1915">Profile</span></span>

* <span data-ttu-id="a72aa-1916">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1916">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a72aa-1917">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1917">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-1918">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1918">RDBMS</span></span>

* <span data-ttu-id="a72aa-1919">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1919">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a72aa-1920">Service Bus</span><span class="sxs-lookup"><span data-stu-id="a72aa-1920">Service Bus</span></span>

* <span data-ttu-id="a72aa-1921">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1921">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1922">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1922">Storage</span></span>

* <span data-ttu-id="a72aa-1923">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-1923">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a72aa-1924">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1924">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1925">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1925">VM</span></span>

* <span data-ttu-id="a72aa-1926">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1926">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a72aa-1927">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-1927">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a72aa-1928">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1928">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a72aa-1929">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1929">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a72aa-1930">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1930">February 27, 2018</span></span>

<span data-ttu-id="a72aa-1931">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a72aa-1931">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1932">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1932">Core</span></span>

* <span data-ttu-id="a72aa-1933">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="a72aa-1933">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a72aa-1934">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1934">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a72aa-1935">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1935">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1936">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1936">ACS</span></span>

* <span data-ttu-id="a72aa-1937">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1937">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a72aa-1938">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="a72aa-1938">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a72aa-1939">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1939">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a72aa-1940">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-1940">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1941">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1941">Appservice</span></span>

* <span data-ttu-id="a72aa-1942">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a72aa-1942">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a72aa-1943">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1943">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a72aa-1944">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a72aa-1944">Cognitive Services</span></span>

* <span data-ttu-id="a72aa-1945">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1945">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-1946">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-1946">Consumption</span></span>

* <span data-ttu-id="a72aa-1947">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1947">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a72aa-1948">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1948">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1949">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1949">Container</span></span>

* <span data-ttu-id="a72aa-1950">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1950">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-1951">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-1951">Network</span></span>

* <span data-ttu-id="a72aa-1952">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1952">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-1953">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-1953">Resource</span></span>

* <span data-ttu-id="a72aa-1954">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1954">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-1955">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-1955">Role</span></span>

* <span data-ttu-id="a72aa-1956">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1956">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-1957">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-1957">SQL</span></span>

* <span data-ttu-id="a72aa-1958">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1958">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-1959">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-1959">Storage</span></span>

* <span data-ttu-id="a72aa-1960">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1960">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-1961">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-1961">VM</span></span>

* <span data-ttu-id="a72aa-1962">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1962">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a72aa-1963">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="a72aa-1963">February 13, 2018</span></span>

<span data-ttu-id="a72aa-1964">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a72aa-1964">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-1965">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-1965">Core</span></span>

* <span data-ttu-id="a72aa-1966">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1966">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-1967">ACS</span></span>

* <span data-ttu-id="a72aa-1968">[주요 변경 사항] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1968">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a72aa-1969">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1969">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a72aa-1970">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1970">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a72aa-1971">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="a72aa-1971">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a72aa-1972">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1972">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a72aa-1973">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-1973">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a72aa-1974">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-1974">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a72aa-1975">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1975">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-1976">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-1976">Appservice</span></span>

* <span data-ttu-id="a72aa-1977">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1977">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a72aa-1978">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1978">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-1979">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-1979">CDN</span></span>

* <span data-ttu-id="a72aa-1980">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1980">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-1981">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-1981">Container</span></span>

* <span data-ttu-id="a72aa-1982">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1982">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a72aa-1983">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1983">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-1984">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-1984">CosmosDB</span></span>

* <span data-ttu-id="a72aa-1985">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1985">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-1986">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-1986">Extension</span></span>

* <span data-ttu-id="a72aa-1987">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1987">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a72aa-1988">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1988">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a72aa-1989">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="a72aa-1989">Feedback</span></span>

* <span data-ttu-id="a72aa-1990">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1990">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-1991">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-1991">Interactive</span></span>

* <span data-ttu-id="a72aa-1992">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1992">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a72aa-1993">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-1993">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-1994">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-1994">IoT</span></span>

* <span data-ttu-id="a72aa-1995">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1995">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a72aa-1996">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-1996">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a72aa-1997">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-1997">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a72aa-1998">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-1998">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-1999">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-1999">Monitor</span></span>

* <span data-ttu-id="a72aa-2000">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2000">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2001">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2001">Network</span></span>

* <span data-ttu-id="a72aa-2002">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2002">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a72aa-2003">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2003">Profile</span></span>

* <span data-ttu-id="a72aa-2004">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2004">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2005">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2005">Resource</span></span>

* <span data-ttu-id="a72aa-2006">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2006">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-2007">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-2007">Role</span></span>

* <span data-ttu-id="a72aa-2008">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2008">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2009">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2009">SQL</span></span>

* <span data-ttu-id="a72aa-2010">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2010">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a72aa-2011">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2011">Added `sql db rename`</span></span>
* <span data-ttu-id="a72aa-2012">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2012">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2013">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2013">Storage</span></span>

* <span data-ttu-id="a72aa-2014">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2014">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2015">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2015">VM</span></span>

* <span data-ttu-id="a72aa-2016">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2016">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a72aa-2017">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2017">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a72aa-2018">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2018">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a72aa-2019">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2019">January 31, 2018</span></span>

<span data-ttu-id="a72aa-2020">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a72aa-2020">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-2021">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2021">Core</span></span>

* <span data-ttu-id="a72aa-2022">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2022">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a72aa-2023">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-2023">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a72aa-2024">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2024">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a72aa-2025">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="a72aa-2025">Use `--verbose` to see</span></span>
* <span data-ttu-id="a72aa-2026">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2026">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2027">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2027">ACS</span></span>

* <span data-ttu-id="a72aa-2028">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2028">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a72aa-2029">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="a72aa-2029">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2030">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2030">Appservice</span></span>

* <span data-ttu-id="a72aa-2031">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2031">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a72aa-2032">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-2032">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-2033">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-2033">CDN</span></span>

* <span data-ttu-id="a72aa-2034">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2034">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-2035">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-2035">CosmosDB</span></span>

* <span data-ttu-id="a72aa-2036">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2036">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-2037">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-2037">Interactive</span></span>

* <span data-ttu-id="a72aa-2038">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2038">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2039">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2039">Network</span></span>

* <span data-ttu-id="a72aa-2040">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2040">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a72aa-2041">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2041">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a72aa-2042">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2042">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a72aa-2043">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2043">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a72aa-2044">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2044">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a72aa-2045">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="a72aa-2045">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a72aa-2046">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2046">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a72aa-2047">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2047">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a72aa-2048">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2048">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="a72aa-2049">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2049">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2050">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2050">Profile</span></span>

* <span data-ttu-id="a72aa-2051">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2051">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2052">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2052">Resource</span></span>

* <span data-ttu-id="a72aa-2053">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2053">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2054">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2054">Storage</span></span>

* <span data-ttu-id="a72aa-2055">스토리지 V1 계정을 스토리지 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2055">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a72aa-2056">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2056">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a72aa-2057">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2057">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="a72aa-2058">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2058">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a72aa-2059">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2059">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2060">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2060">VM</span></span>

* <span data-ttu-id="a72aa-2061">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2061">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a72aa-2062">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2062">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a72aa-2063">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2063">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a72aa-2064">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2064">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a72aa-2065">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2065">January 17, 2018</span></span>

<span data-ttu-id="a72aa-2066">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a72aa-2066">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-2067">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-2067">ACR</span></span>

* <span data-ttu-id="a72aa-2068">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2068">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a72aa-2069">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2069">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2070">ACS</span></span>

* <span data-ttu-id="a72aa-2071">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2071">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a72aa-2072">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2072">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2073">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2073">Appservice</span></span>

* <span data-ttu-id="a72aa-2074">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2074">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a72aa-2075">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2075">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a72aa-2076">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2076">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a72aa-2077">Backup</span><span class="sxs-lookup"><span data-stu-id="a72aa-2077">Backup</span></span>

* <span data-ttu-id="a72aa-2078">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2078">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a72aa-2079">`backup restore restore-disks`에 스토리지 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2079">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a72aa-2080">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2080">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a72aa-2081">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2081">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a72aa-2082">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2082">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-2083">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-2083">Batch</span></span>

* <span data-ttu-id="a72aa-2084">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2084">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a72aa-2085">클라우드</span><span class="sxs-lookup"><span data-stu-id="a72aa-2085">Cloud</span></span>

* <span data-ttu-id="a72aa-2086">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2086">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-2087">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-2087">Consumption</span></span>

* <span data-ttu-id="a72aa-2088">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2088">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a72aa-2089">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a72aa-2089">Event Grid</span></span>

* <span data-ttu-id="a72aa-2090">[주요 변경 사항] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2090">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a72aa-2091">[주요 변경 사항] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2091">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a72aa-2092">[주요 변경 사항] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2092">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a72aa-2093">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2093">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a72aa-2094">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2094">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a72aa-2095">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2095">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a72aa-2096">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2096">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a72aa-2097">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2097">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-2098">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-2098">Interactive</span></span>

* <span data-ttu-id="a72aa-2099">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2099">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a72aa-2100">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2100">Fixed errors on startup</span></span>
* <span data-ttu-id="a72aa-2101">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2101">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-2102">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-2102">IoT</span></span>

* <span data-ttu-id="a72aa-2103">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2103">Added support for device provisioning service</span></span>
* <span data-ttu-id="a72aa-2104">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2104">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a72aa-2105">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2105">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2106">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2106">Monitor</span></span>

* <span data-ttu-id="a72aa-2107">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2107">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a72aa-2108">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-2108">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a72aa-2109">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2109">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2110">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2110">Network</span></span>

* <span data-ttu-id="a72aa-2111">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2111">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a72aa-2112">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2112">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2113">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2113">Profile</span></span>

* <span data-ttu-id="a72aa-2114">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2114">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-2115">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-2115">Role</span></span>

* <span data-ttu-id="a72aa-2116">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2116">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a72aa-2117">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-2117">Service Fabric</span></span>

* <span data-ttu-id="a72aa-2118">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2118">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a72aa-2119">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2119">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2120">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2120">VM</span></span>

* <span data-ttu-id="a72aa-2121">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2121">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a72aa-2122">[주요 변경 사항] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2122">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a72aa-2123">[주요 변경 사항] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2123">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a72aa-2124">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2124">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a72aa-2125">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2125">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a72aa-2126">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2126">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a72aa-2127">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2127">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a72aa-2128">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2128">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a72aa-2129">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2129">December 19, 2017</span></span>

<span data-ttu-id="a72aa-2130">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a72aa-2130">Version 2.0.23</span></span>

* <span data-ttu-id="a72aa-2131">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2131">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-2132">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-2132">Container</span></span>

* <span data-ttu-id="a72aa-2133">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2133">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2134">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2134">Network</span></span>

* <span data-ttu-id="a72aa-2135">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2135">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a72aa-2136">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2136">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2137">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2137">Storage</span></span>

* <span data-ttu-id="a72aa-2138">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2138">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2139">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2139">VM</span></span>

* <span data-ttu-id="a72aa-2140">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2140">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a72aa-2141">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2141">December 5, 2017</span></span>

<span data-ttu-id="a72aa-2142">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a72aa-2142">Version 2.0.22</span></span>

* <span data-ttu-id="a72aa-2143">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2143">Removed `az component` commands.</span></span> <span data-ttu-id="a72aa-2144">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2144">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-2145">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2145">Core</span></span>
* <span data-ttu-id="a72aa-2146">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2146">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a72aa-2147">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2147">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2148">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2148">ACS</span></span>

* <span data-ttu-id="a72aa-2149">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2149">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a72aa-2150">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2150">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a72aa-2151">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2151">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a72aa-2152">Advisor</span><span class="sxs-lookup"><span data-stu-id="a72aa-2152">Advisor</span></span>

* <span data-ttu-id="a72aa-2153">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2153">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2154">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2154">Appservice</span></span>

* <span data-ttu-id="a72aa-2155">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2155">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a72aa-2156">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2156">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a72aa-2157">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2157">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a72aa-2158">Consumption</span><span class="sxs-lookup"><span data-stu-id="a72aa-2158">Consumption</span></span>

* <span data-ttu-id="a72aa-2159">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2159">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-2160">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-2160">Container</span></span>

* <span data-ttu-id="a72aa-2161">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2161">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2162">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2162">Monitor</span></span>

* <span data-ttu-id="a72aa-2163">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2163">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2164">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2164">Resource</span></span>

* <span data-ttu-id="a72aa-2165">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2165">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-2166">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-2166">Role</span></span>

* <span data-ttu-id="a72aa-2167">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2167">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a72aa-2168">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2168">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a72aa-2169">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2169">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2170">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2170">SQL</span></span>

* <span data-ttu-id="a72aa-2171">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2171">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a72aa-2172">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2172">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2173">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2173">VM</span></span>

* <span data-ttu-id="a72aa-2174">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2174">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a72aa-2175">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2175">November 14, 2017</span></span>

<span data-ttu-id="a72aa-2176">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a72aa-2176">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-2177">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-2177">ACR</span></span>

* <span data-ttu-id="a72aa-2178">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2178">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a72aa-2179">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2179">ACS</span></span>

* <span data-ttu-id="a72aa-2180">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2180">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a72aa-2181">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="a72aa-2181">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a72aa-2182">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2182">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a72aa-2183">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2183">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a72aa-2184">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2184">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2185">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2185">Appservice</span></span>

* <span data-ttu-id="a72aa-2186">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2186">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a72aa-2187">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2187">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a72aa-2188">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2188">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a72aa-2189">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2189">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a72aa-2190">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2190">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a72aa-2191">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2191">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-2192">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-2192">Batch</span></span>

* <span data-ttu-id="a72aa-2193">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2193">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-2194">Batchai</span><span class="sxs-lookup"><span data-stu-id="a72aa-2194">Batchai</span></span>

* <span data-ttu-id="a72aa-2195">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2195">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a72aa-2196">스토리지 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2196">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a72aa-2197">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2197">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a72aa-2198">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2198">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a72aa-2199">클라우드</span><span class="sxs-lookup"><span data-stu-id="a72aa-2199">Cloud</span></span>

* <span data-ttu-id="a72aa-2200">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2200">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-2201">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-2201">Container</span></span>

* <span data-ttu-id="a72aa-2202">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2202">Added support to open multiple ports</span></span>
* <span data-ttu-id="a72aa-2203">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2203">Added container group restart policy</span></span>
* <span data-ttu-id="a72aa-2204">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2204">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a72aa-2205">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="a72aa-2205">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a72aa-2206">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a72aa-2206">Data Lake Analytics</span></span>

* <span data-ttu-id="a72aa-2207">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2207">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a72aa-2208">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a72aa-2208">Data Lake Store</span></span>

* <span data-ttu-id="a72aa-2209">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2209">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-2210">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-2210">Extension</span></span>

* <span data-ttu-id="a72aa-2211">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2211">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a72aa-2212">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2212">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-2213">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-2213">IoT</span></span>

* <span data-ttu-id="a72aa-2214">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2214">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2215">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2215">Monitor</span></span>

* <span data-ttu-id="a72aa-2216">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2216">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2217">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2217">Network</span></span>

* <span data-ttu-id="a72aa-2218">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2218">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a72aa-2219">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2219">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a72aa-2220">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2220">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a72aa-2221">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2221">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a72aa-2222">예약</span><span class="sxs-lookup"><span data-stu-id="a72aa-2222">Reservations</span></span>

* <span data-ttu-id="a72aa-2223">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2223">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2224">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2224">Resource</span></span>

* <span data-ttu-id="a72aa-2225">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2225">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2226">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2226">SQL</span></span>

* <span data-ttu-id="a72aa-2227">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2227">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2228">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2228">Storage</span></span>

* <span data-ttu-id="a72aa-2229">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2229">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a72aa-2230">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2230">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a72aa-2231">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2231">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a72aa-2232">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="a72aa-2232">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a72aa-2233">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2233">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a72aa-2234">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2234">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a72aa-2235">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2235">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2236">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2236">VM</span></span>

* <span data-ttu-id="a72aa-2237">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2237">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a72aa-2238">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2238">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a72aa-2239">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2239">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a72aa-2240">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2240">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a72aa-2241">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2241">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a72aa-2242">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2242">October 24, 2017</span></span>

<span data-ttu-id="a72aa-2243">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a72aa-2243">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-2244">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2244">Core</span></span>

* <span data-ttu-id="a72aa-2245">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2245">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-2246">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-2246">ACR</span></span>

* <span data-ttu-id="a72aa-2247">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2247">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a72aa-2248">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2248">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a72aa-2249">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2249">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2250">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2250">ACS</span></span>

* <span data-ttu-id="a72aa-2251">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2251">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a72aa-2252">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2252">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2253">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2253">Appservice</span></span>

* <span data-ttu-id="a72aa-2254">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2254">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a72aa-2255">구성 요소</span><span class="sxs-lookup"><span data-stu-id="a72aa-2255">Component</span></span>

* <span data-ttu-id="a72aa-2256">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2256">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2257">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2257">Monitor</span></span>

* <span data-ttu-id="a72aa-2258">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2258">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2259">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2259">Resource</span></span>

* <span data-ttu-id="a72aa-2260">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2260">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a72aa-2261">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2261">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2262">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2262">VM</span></span>

* <span data-ttu-id="a72aa-2263">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2263">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a72aa-2264">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2264">October 9, 2017</span></span>

<span data-ttu-id="a72aa-2265">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a72aa-2265">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-2266">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2266">Core</span></span>

* <span data-ttu-id="a72aa-2267">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2267">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2268">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2268">Appservice</span></span>

* <span data-ttu-id="a72aa-2269">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2269">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-2270">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-2270">Batch</span></span>

* <span data-ttu-id="a72aa-2271">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2271">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a72aa-2272">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2272">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a72aa-2273">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2273">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a72aa-2274">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2274">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a72aa-2275">Batchai</span><span class="sxs-lookup"><span data-stu-id="a72aa-2275">Batchai</span></span>

* <span data-ttu-id="a72aa-2276">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2276">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-2277">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a72aa-2277">Keyvault</span></span>

* <span data-ttu-id="a72aa-2278">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2278">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a72aa-2279">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2279">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a72aa-2280">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2280">Network</span></span>

* <span data-ttu-id="a72aa-2281">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2281">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a72aa-2282">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2282">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2283">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2283">Resource</span></span>

* <span data-ttu-id="a72aa-2284">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2284">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a72aa-2285">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2285">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a72aa-2286">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2286">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a72aa-2287">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2287">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2288">Sql</span><span class="sxs-lookup"><span data-stu-id="a72aa-2288">Sql</span></span>

* <span data-ttu-id="a72aa-2289">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2289">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a72aa-2290">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2290">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a72aa-2291">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2291">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2292">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2292">Storage</span></span>

* <span data-ttu-id="a72aa-2293">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2293">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2294">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2294">Vm</span></span>

* <span data-ttu-id="a72aa-2295">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2295">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a72aa-2296">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2296">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a72aa-2297">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2297">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a72aa-2298">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2298">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a72aa-2299">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2299">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a72aa-2300">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2300">September 22, 2017</span></span>

<span data-ttu-id="a72aa-2301">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a72aa-2301">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2302">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2302">Resource</span></span>

* <span data-ttu-id="a72aa-2303">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2303">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a72aa-2304">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2304">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a72aa-2305">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2305">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a72aa-2306">[주요 변경 사항] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2306">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2307">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2307">Network</span></span>

* <span data-ttu-id="a72aa-2308">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2308">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a72aa-2309">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2309">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a72aa-2310">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2310">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a72aa-2311">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2311">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a72aa-2312">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2312">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a72aa-2313">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2313">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a72aa-2314">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2314">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2315">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2315">Storage</span></span>

* <span data-ttu-id="a72aa-2316">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2316">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a72aa-2317">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a72aa-2317">Eventgrid</span></span>

* <span data-ttu-id="a72aa-2318">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="a72aa-2318">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2319">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2319">SQL</span></span>

* <span data-ttu-id="a72aa-2320">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2320">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a72aa-2321">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2321">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a72aa-2322">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2322">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-2323">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a72aa-2323">Keyvault</span></span>

* <span data-ttu-id="a72aa-2324">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2324">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2325">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2325">VM</span></span>

* <span data-ttu-id="a72aa-2326">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2326">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a72aa-2327">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a72aa-2327">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a72aa-2328">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2328">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a72aa-2329">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2329">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a72aa-2330">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2330">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a72aa-2331">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2331">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2332">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2332">ACS</span></span>

* <span data-ttu-id="a72aa-2333">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2333">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2334">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2334">Appservice</span></span>

* <span data-ttu-id="a72aa-2335">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2335">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a72aa-2336">Backup</span><span class="sxs-lookup"><span data-stu-id="a72aa-2336">Backup</span></span>

* <span data-ttu-id="a72aa-2337">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2337">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a72aa-2338">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2338">September 11, 2017</span></span>

<span data-ttu-id="a72aa-2339">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a72aa-2339">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a72aa-2340">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2340">Core</span></span>

* <span data-ttu-id="a72aa-2341">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2341">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a72aa-2342">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2342">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2343">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2343">Acs</span></span>

* <span data-ttu-id="a72aa-2344">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2344">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a72aa-2345">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2345">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2346">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2346">Appservice</span></span>

* <span data-ttu-id="a72aa-2347">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2347">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-2348">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-2348">CDN</span></span>

* <span data-ttu-id="a72aa-2349">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2349">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a72aa-2350">내선 번호</span><span class="sxs-lookup"><span data-stu-id="a72aa-2350">Extension</span></span>

* <span data-ttu-id="a72aa-2351">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2351">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-2352">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a72aa-2352">Keyvault</span></span>

* <span data-ttu-id="a72aa-2353">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2353">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2354">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2354">Network</span></span>

* <span data-ttu-id="a72aa-2355">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2355">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a72aa-2356">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2356">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a72aa-2357">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2357">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a72aa-2358">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2358">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a72aa-2359">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2359">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2360">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2360">Resource</span></span>

* <span data-ttu-id="a72aa-2361">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2361">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a72aa-2362">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2362">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a72aa-2363">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2363">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a72aa-2364">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="a72aa-2364">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2365">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2365">SQL</span></span>

* <span data-ttu-id="a72aa-2366">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2366">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2367">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2367">VM</span></span>

* <span data-ttu-id="a72aa-2368">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2368">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a72aa-2369">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2369">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a72aa-2370">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2370">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a72aa-2371">수정됨: `[vm|vmss] create` 스토리지 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2371">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a72aa-2372">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2372">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a72aa-2373">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2373">August 31, 2017</span></span>

<span data-ttu-id="a72aa-2374">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a72aa-2374">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-2375">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a72aa-2375">Keyvault</span></span>

* <span data-ttu-id="a72aa-2376">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2376">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a72aa-2377">Sf</span><span class="sxs-lookup"><span data-stu-id="a72aa-2377">Sf</span></span>

* <span data-ttu-id="a72aa-2378">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2378">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2379">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2379">Storage</span></span>

* <span data-ttu-id="a72aa-2380">스토리지 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2380">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a72aa-2381">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2381">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a72aa-2382">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2382">August 28, 2017</span></span>

<span data-ttu-id="a72aa-2383">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a72aa-2383">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a72aa-2384">CLI</span><span class="sxs-lookup"><span data-stu-id="a72aa-2384">CLI</span></span>

* <span data-ttu-id="a72aa-2385">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2385">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2386">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2386">ACS</span></span>

* <span data-ttu-id="a72aa-2387">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2387">Corrected preview regions</span></span>
* <span data-ttu-id="a72aa-2388">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2388">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a72aa-2389">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2389">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2390">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2390">Appservice</span></span>

* <span data-ttu-id="a72aa-2391">[주요 변경 사항] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2391">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a72aa-2392">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2392">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a72aa-2393">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2393">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a72aa-2394">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2394">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a72aa-2395">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2395">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-2396">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-2396">IoT</span></span>

* <span data-ttu-id="a72aa-2397">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2397">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2398">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2398">Network</span></span>

* <span data-ttu-id="a72aa-2399">[주요 변경 사항] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2399">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a72aa-2400">[주요 변경 사항] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2400">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a72aa-2401">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2401">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a72aa-2402">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2402">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a72aa-2403">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2403">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2404">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2404">Profile</span></span>

* <span data-ttu-id="a72aa-2405">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2405">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a72aa-2406">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-2406">Service Fabric</span></span>

* <span data-ttu-id="a72aa-2407">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2407">Preview release</span></span>
* <span data-ttu-id="a72aa-2408">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2408">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a72aa-2409">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2409">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a72aa-2410">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2410">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2411">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2411">Storage</span></span>

* <span data-ttu-id="a72aa-2412">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2412">Enabled setting blob tier</span></span>
* <span data-ttu-id="a72aa-2413">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2413">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a72aa-2414">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2414">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a72aa-2415">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2415">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a72aa-2416">[주요 변경 사항] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2416">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a72aa-2417">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2417">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2418">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2418">VM</span></span>

* <span data-ttu-id="a72aa-2419">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2419">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a72aa-2420">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2420">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a72aa-2421">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2421">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a72aa-2422">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2422">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a72aa-2423">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2423">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a72aa-2424">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2424">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a72aa-2425">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2425">August 15, 2017</span></span>

<span data-ttu-id="a72aa-2426">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a72aa-2426">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2427">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2427">ACS</span></span>

* <span data-ttu-id="a72aa-2428">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2428">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2429">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2429">Appservice</span></span>

* <span data-ttu-id="a72aa-2430">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2430">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a72aa-2431">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a72aa-2431">Event Grid</span></span>

* <span data-ttu-id="a72aa-2432">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2432">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a72aa-2433">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2433">August 11, 2017</span></span>

<span data-ttu-id="a72aa-2434">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a72aa-2434">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2435">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2435">ACS</span></span>

* <span data-ttu-id="a72aa-2436">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2436">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-2437">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-2437">Batch</span></span>

* <span data-ttu-id="a72aa-2438">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2438">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a72aa-2439">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2439">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a72aa-2440">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2440">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a72aa-2441">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2441">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a72aa-2442">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2442">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a72aa-2443">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2443">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a72aa-2444">구성 요소</span><span class="sxs-lookup"><span data-stu-id="a72aa-2444">Component</span></span>

* <span data-ttu-id="a72aa-2445">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2445">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a72aa-2446">컨테이너</span><span class="sxs-lookup"><span data-stu-id="a72aa-2446">Container</span></span>

* <span data-ttu-id="a72aa-2447">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2447">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a72aa-2448">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a72aa-2448">Data Lake Store</span></span>

* <span data-ttu-id="a72aa-2449">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2449">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a72aa-2450">Event Grid</span><span class="sxs-lookup"><span data-stu-id="a72aa-2450">Event Grid</span></span>

* <span data-ttu-id="a72aa-2451">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2451">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2452">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2452">Network</span></span>

* <span data-ttu-id="a72aa-2453">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2453">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a72aa-2454">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2454">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a72aa-2455">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2455">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a72aa-2456">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2456">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2457">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2457">Profile</span></span>

* <span data-ttu-id="a72aa-2458">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2458">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2459">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2459">Storage</span></span>

* <span data-ttu-id="a72aa-2460">시스템에 할당된 ID를 통한 스토리지 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2460">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2461">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2461">VM</span></span>

* <span data-ttu-id="a72aa-2462">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2462">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a72aa-2463">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2463">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a72aa-2464">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2464">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a72aa-2465">데이터 디스크 연결 시 스토리지 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2465">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a72aa-2466">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 스토리지 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2466">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a72aa-2467">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2467">July 28, 2017</span></span>

<span data-ttu-id="a72aa-2468">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a72aa-2468">Version 2.0.12</span></span>

* <span data-ttu-id="a72aa-2469">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2469">Added container commands</span></span>
* <span data-ttu-id="a72aa-2470">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2470">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a72aa-2471">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2471">Core</span></span>

* <span data-ttu-id="a72aa-2472">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2472">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a72aa-2473">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2473">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a72aa-2474">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2474">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a72aa-2475">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2475">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a72aa-2476">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="a72aa-2476">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a72aa-2477">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2477">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a72aa-2478">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2478">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a72aa-2479">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2479">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a72aa-2480">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2480">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a72aa-2481">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2481">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a72aa-2482">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="a72aa-2482">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a72aa-2483">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2483">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a72aa-2484">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2484">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a72aa-2485">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2485">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a72aa-2486">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2486">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a72aa-2487">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2487">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a72aa-2488">ACR</span><span class="sxs-lookup"><span data-stu-id="a72aa-2488">ACR</span></span>

* <span data-ttu-id="a72aa-2489">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2489">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a72aa-2490">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2490">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a72aa-2491">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2491">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a72aa-2492">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2492">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a72aa-2493">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2493">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a72aa-2494">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2494">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2495">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2495">ACS</span></span>

* <span data-ttu-id="a72aa-2496">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2496">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2497">App Service</span><span class="sxs-lookup"><span data-stu-id="a72aa-2497">Appservice</span></span>

* <span data-ttu-id="a72aa-2498">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2498">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a72aa-2499">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2499">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a72aa-2500">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2500">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a72aa-2501">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2501">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a72aa-2502">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2502">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a72aa-2503">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2503">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a72aa-2504">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2504">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a72aa-2505">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2505">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a72aa-2506">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2506">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a72aa-2507">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2507">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a72aa-2508">Batch</span><span class="sxs-lookup"><span data-stu-id="a72aa-2508">Batch</span></span>

* <span data-ttu-id="a72aa-2509">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2509">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a72aa-2510">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2510">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a72aa-2511">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2511">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a72aa-2512">CDN</span><span class="sxs-lookup"><span data-stu-id="a72aa-2512">CDN</span></span>

* <span data-ttu-id="a72aa-2513">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2513">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a72aa-2514">클라우드</span><span class="sxs-lookup"><span data-stu-id="a72aa-2514">Cloud</span></span>

* <span data-ttu-id="a72aa-2515">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2515">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a72aa-2516">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2516">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a72aa-2517">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2517">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a72aa-2518">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2518">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a72aa-2519">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2519">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-2520">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-2520">CosmosDB</span></span>

* <span data-ttu-id="a72aa-2521">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2521">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a72aa-2522">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2522">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a72aa-2523">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a72aa-2523">Data Lake Analytics</span></span>

* <span data-ttu-id="a72aa-2524">`dla account compute-policy` 제목 아래에 컴퓨팅 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2524">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a72aa-2525">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2525">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a72aa-2526">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2526">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a72aa-2527">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a72aa-2527">Data Lake Store</span></span>

* <span data-ttu-id="a72aa-2528">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2528">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a72aa-2529">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2529">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a72aa-2530">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2530">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a72aa-2531">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="a72aa-2531">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a72aa-2532">대화형</span><span class="sxs-lookup"><span data-stu-id="a72aa-2532">Interactive</span></span>

* <span data-ttu-id="a72aa-2533">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2533">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a72aa-2534">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2534">Increased test coverage</span></span>
* <span data-ttu-id="a72aa-2535">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2535">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a72aa-2536">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2536">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a72aa-2537">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2537">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a72aa-2538">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2538">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a72aa-2539">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2539">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a72aa-2540">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2540">Added `--progress` flag</span></span>
* <span data-ttu-id="a72aa-2541">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2541">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a72aa-2542">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2542">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a72aa-2543">IoT</span><span class="sxs-lookup"><span data-stu-id="a72aa-2543">IoT</span></span>

* <span data-ttu-id="a72aa-2544">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2544">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a72aa-2545">(#3934)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2545">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a72aa-2546">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2546">Key vault</span></span>

* <span data-ttu-id="a72aa-2547">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="a72aa-2547">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a72aa-2548">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2548">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a72aa-2549">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2549">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a72aa-2550">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2550">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a72aa-2551">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2551">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a72aa-2552">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2552">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a72aa-2553">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2553">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a72aa-2554">(#3307)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2554">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a72aa-2555">랩</span><span class="sxs-lookup"><span data-stu-id="a72aa-2555">Lab</span></span>

* <span data-ttu-id="a72aa-2556">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2556">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a72aa-2557">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2557">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2558">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2558">Monitor</span></span>

* <span data-ttu-id="a72aa-2559">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2559">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a72aa-2560">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2560">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a72aa-2561">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2561">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a72aa-2562">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2562">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a72aa-2563">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2563">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a72aa-2564">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="a72aa-2564">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a72aa-2565">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2565">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a72aa-2566">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2566">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a72aa-2567">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2567">`location` no longer required</span></span>
  * <span data-ttu-id="a72aa-2568">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2568">Add name and ID support for target</span></span>
  * <span data-ttu-id="a72aa-2569">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2569">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a72aa-2570">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2570">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a72aa-2571">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2571">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a72aa-2572">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2572">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a72aa-2573">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2573">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a72aa-2574">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2574">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2575">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2575">Network</span></span>

* <span data-ttu-id="a72aa-2576">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2576">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a72aa-2577">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2577">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a72aa-2578">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2578">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a72aa-2579">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2579">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a72aa-2580">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2580">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a72aa-2581">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2581">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a72aa-2582">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2582">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a72aa-2583">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2583">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a72aa-2584">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2584">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a72aa-2585">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2585">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a72aa-2586">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2586">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a72aa-2587">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2587">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a72aa-2588">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2588">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a72aa-2589">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a72aa-2589">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a72aa-2590">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2590">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a72aa-2591">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2591">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a72aa-2592">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2592">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a72aa-2593">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2593">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a72aa-2594">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2594">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a72aa-2595">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2595">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a72aa-2596">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2596">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a72aa-2597">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2597">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a72aa-2598">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2598">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a72aa-2599">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2599">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a72aa-2600">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2600">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a72aa-2601">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2601">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a72aa-2602">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2602">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2603">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2603">Profile</span></span>

* <span data-ttu-id="a72aa-2604">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2604">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a72aa-2605">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2605">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a72aa-2606">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2606">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a72aa-2607">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2607">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a72aa-2608">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2608">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a72aa-2609">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2609">RDBMS</span></span>

* <span data-ttu-id="a72aa-2610">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2610">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a72aa-2611">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2611">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a72aa-2612">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2612">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a72aa-2613">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2613">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2614">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2614">Resource</span></span>

* <span data-ttu-id="a72aa-2615">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2615">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a72aa-2616">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2616">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a72aa-2617">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2617">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a72aa-2618">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2618">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a72aa-2619">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2619">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a72aa-2620">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2620">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a72aa-2621">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2621">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a72aa-2622">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2622">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-2623">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-2623">Role</span></span>

* <span data-ttu-id="a72aa-2624">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2624">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a72aa-2625">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2625">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a72aa-2626">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2626">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a72aa-2627">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2627">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a72aa-2628">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2628">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a72aa-2629">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a72aa-2629">Service Fabric</span></span>
* <span data-ttu-id="a72aa-2630">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="a72aa-2630">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a72aa-2631">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2631">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a72aa-2632">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2632">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2633">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2633">SQL</span></span>

* <span data-ttu-id="a72aa-2634">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2634">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a72aa-2635">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2635">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a72aa-2636">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2636">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2637">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2637">Storage</span></span>

* <span data-ttu-id="a72aa-2638">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2638">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a72aa-2639">HTTPS 전용 스토리지 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2639">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a72aa-2640">스토리지 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2640">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a72aa-2641">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2641">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a72aa-2642">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2642">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a72aa-2643">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2643">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2644">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2644">VM</span></span>

* <span data-ttu-id="a72aa-2645">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2645">Support configuring nsg</span></span>
* <span data-ttu-id="a72aa-2646">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2646">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a72aa-2647">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2647">Support managed service identities</span></span>
* <span data-ttu-id="a72aa-2648">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2648">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a72aa-2649">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2649">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a72aa-2650">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2650">May 10, 2017</span></span>

<span data-ttu-id="a72aa-2651">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a72aa-2651">Version 2.0.6</span></span>

* <span data-ttu-id="a72aa-2652">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="a72aa-2652">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a72aa-2653">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2653">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a72aa-2654">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2654">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a72aa-2655">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2655">Include Cognitive Services module</span></span>
* <span data-ttu-id="a72aa-2656">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2656">Include Service Fabric module</span></span>
* <span data-ttu-id="a72aa-2657">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="a72aa-2657">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a72aa-2658">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2658">Add support for CDN commands</span></span>
* <span data-ttu-id="a72aa-2659">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-2659">Remove Container module</span></span>
* <span data-ttu-id="a72aa-2660">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2660">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a72aa-2661">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2661">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a72aa-2662">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2662">Core</span></span>

* <span data-ttu-id="a72aa-2663">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="a72aa-2663">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a72aa-2664">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2664">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a72aa-2665">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2665">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a72aa-2666">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2666">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a72aa-2667">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2667">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a72aa-2668">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2668">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a72aa-2669">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2669">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a72aa-2670">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2670">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a72aa-2671">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2671">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a72aa-2672">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="a72aa-2672">core: Improved performance</span></span>
* <span data-ttu-id="a72aa-2673">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2673">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a72aa-2674">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2674">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2675">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2675">ACS</span></span>

* <span data-ttu-id="a72aa-2676">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2676">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a72aa-2677">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="a72aa-2677">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a72aa-2678">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="a72aa-2678">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a72aa-2679">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2679">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-2680">AppService</span></span>

* <span data-ttu-id="a72aa-2681">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2681">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a72aa-2682">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2682">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a72aa-2683">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2683">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a72aa-2684">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="a72aa-2684">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a72aa-2685">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="a72aa-2685">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a72aa-2686">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2686">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a72aa-2687">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2687">support slot swap with preview</span></span>
* <span data-ttu-id="a72aa-2688">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2688">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a72aa-2689">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2689">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a72aa-2690">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-2690">CosmosDB</span></span>

* <span data-ttu-id="a72aa-2691">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="a72aa-2691">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a72aa-2692">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2692">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a72aa-2693">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2693">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a72aa-2694">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2694">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a72aa-2695">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a72aa-2695">Data Lake Analytics</span></span>

* <span data-ttu-id="a72aa-2696">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2696">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a72aa-2697">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2697">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a72aa-2698">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2698">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a72aa-2699">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="a72aa-2699">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a72aa-2700">테이블</span><span class="sxs-lookup"><span data-stu-id="a72aa-2700">Table</span></span>
  * <span data-ttu-id="a72aa-2701">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="a72aa-2701">Table valued function</span></span>
  * <span data-ttu-id="a72aa-2702">보기</span><span class="sxs-lookup"><span data-stu-id="a72aa-2702">View</span></span>
  * <span data-ttu-id="a72aa-2703">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2703">Table Statistics.</span></span> <span data-ttu-id="a72aa-2704">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2704">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a72aa-2705">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a72aa-2705">Data Lake Store</span></span>

* <span data-ttu-id="a72aa-2706">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="a72aa-2706">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a72aa-2707">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2707">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a72aa-2708">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2708">missed help for access show.</span></span> <span data-ttu-id="a72aa-2709">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2709">adding it.</span></span> <span data-ttu-id="a72aa-2710">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2710">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a72aa-2711">찾기</span><span class="sxs-lookup"><span data-stu-id="a72aa-2711">Find</span></span>

* <span data-ttu-id="a72aa-2712">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="a72aa-2712">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a72aa-2713">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a72aa-2713">KeyVault</span></span>

* <span data-ttu-id="a72aa-2714">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2714">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a72aa-2715">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="a72aa-2715">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a72aa-2716">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2716">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a72aa-2717">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2717">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a72aa-2718">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2718">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a72aa-2719">랩</span><span class="sxs-lookup"><span data-stu-id="a72aa-2719">Lab</span></span>

* <span data-ttu-id="a72aa-2720">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2720">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a72aa-2721">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2721">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a72aa-2722">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="a72aa-2722">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a72aa-2723">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="a72aa-2723">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a72aa-2724">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2724">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a72aa-2725">모니터</span><span class="sxs-lookup"><span data-stu-id="a72aa-2725">Monitor</span></span>

* <span data-ttu-id="a72aa-2726">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2726">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a72aa-2727">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2727">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a72aa-2728">네트워크</span><span class="sxs-lookup"><span data-stu-id="a72aa-2728">Network</span></span>

* <span data-ttu-id="a72aa-2729">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2729">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a72aa-2730">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2730">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a72aa-2731">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2731">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a72aa-2732">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2732">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a72aa-2733">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2733">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a72aa-2734">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2734">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a72aa-2735">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2735">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a72aa-2736">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2736">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a72aa-2737">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2737">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a72aa-2738">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2738">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a72aa-2739">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="a72aa-2739">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a72aa-2740">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2740">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a72aa-2741">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2741">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a72aa-2742">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2742">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a72aa-2743">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2743">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a72aa-2744">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2744">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a72aa-2745">프로필</span><span class="sxs-lookup"><span data-stu-id="a72aa-2745">Profile</span></span>

* <span data-ttu-id="a72aa-2746">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2746">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a72aa-2747">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2747">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a72aa-2748">Redis</span><span class="sxs-lookup"><span data-stu-id="a72aa-2748">Redis</span></span>

* <span data-ttu-id="a72aa-2749">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2749">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a72aa-2750">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="a72aa-2750">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a72aa-2751">리소스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2751">Resource</span></span>

* <span data-ttu-id="a72aa-2752">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2752">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a72aa-2753">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2753">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a72aa-2754">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2754">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a72aa-2755">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2755">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a72aa-2756">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2756">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a72aa-2757">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2757">Add docs for az lock update.</span></span> <span data-ttu-id="a72aa-2758">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2758">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a72aa-2759">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2759">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a72aa-2760">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2760">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a72aa-2761">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2761">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a72aa-2762">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2762">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a72aa-2763">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2763">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a72aa-2764">역할</span><span class="sxs-lookup"><span data-stu-id="a72aa-2764">Role</span></span>

* <span data-ttu-id="a72aa-2765">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2765">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a72aa-2766">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2766">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a72aa-2767">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2767">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a72aa-2768">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="a72aa-2768">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a72aa-2769">SQL</span><span class="sxs-lookup"><span data-stu-id="a72aa-2769">SQL</span></span>

* <span data-ttu-id="a72aa-2770">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="a72aa-2770">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a72aa-2771">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2771">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a72aa-2772">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2772">Storage</span></span>

* <span data-ttu-id="a72aa-2773">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="a72aa-2773">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a72aa-2774">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2774">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a72aa-2775">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2775">Add support for large block blob upload</span></span>
* <span data-ttu-id="a72aa-2776">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="a72aa-2776">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2777">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2777">VM</span></span>

* <span data-ttu-id="a72aa-2778">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="a72aa-2778">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a72aa-2779">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2779">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a72aa-2780">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a72aa-2780">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a72aa-2781">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a72aa-2781">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a72aa-2782">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2782">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a72aa-2783">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="a72aa-2783">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a72aa-2784">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2784">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a72aa-2785">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2785">April 3, 2017</span></span>

<span data-ttu-id="a72aa-2786">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a72aa-2786">Version 2.0.2</span></span>

<span data-ttu-id="a72aa-2787">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2787">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a72aa-2788">코어</span><span class="sxs-lookup"><span data-stu-id="a72aa-2788">Core</span></span>

* <span data-ttu-id="a72aa-2789">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="a72aa-2789">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a72aa-2790">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2790">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a72aa-2791">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2791">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a72aa-2792">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2792">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a72aa-2793">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2793">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a72aa-2794">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2794">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a72aa-2795">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2795">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a72aa-2796">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2796">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a72aa-2797">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="a72aa-2797">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a72aa-2798">ACS</span><span class="sxs-lookup"><span data-stu-id="a72aa-2798">ACS</span></span>

* <span data-ttu-id="a72aa-2799">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2799">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a72aa-2800">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2800">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a72aa-2801">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2801">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a72aa-2802">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2802">Add support for windows clusters.</span></span> <span data-ttu-id="a72aa-2803">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2803">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a72aa-2804">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2804">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a72aa-2805">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2805">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a72aa-2806">AppService</span><span class="sxs-lookup"><span data-stu-id="a72aa-2806">AppService</span></span>

* <span data-ttu-id="a72aa-2807">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2807">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a72aa-2808">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2808">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a72aa-2809">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2809">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a72aa-2810">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2810">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a72aa-2811">DataLake</span><span class="sxs-lookup"><span data-stu-id="a72aa-2811">DataLake</span></span>

* <span data-ttu-id="a72aa-2812">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2812">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a72aa-2813">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="a72aa-2813">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a72aa-2814">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="a72aa-2814">DocuemntDB</span></span>

* <span data-ttu-id="a72aa-2815">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2815">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a72aa-2816">VM</span><span class="sxs-lookup"><span data-stu-id="a72aa-2816">VM</span></span>

* <span data-ttu-id="a72aa-2817">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2817">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a72aa-2818">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2818">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a72aa-2819">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2819">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a72aa-2820">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2820">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a72aa-2821">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2821">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a72aa-2822">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2822">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="a72aa-2823">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a72aa-2823">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a72aa-2824">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="a72aa-2824">February 27, 2017</span></span>

<span data-ttu-id="a72aa-2825">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a72aa-2825">Version 2.0.0</span></span>

<span data-ttu-id="a72aa-2826">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2826">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a72aa-2827">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2827">Container Service (acs)</span></span>
- <span data-ttu-id="a72aa-2828">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="a72aa-2828">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a72aa-2829">네트워킹</span><span class="sxs-lookup"><span data-stu-id="a72aa-2829">Networking</span></span>
- <span data-ttu-id="a72aa-2830">스토리지</span><span class="sxs-lookup"><span data-stu-id="a72aa-2830">Storage</span></span>

<span data-ttu-id="a72aa-2831">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2831">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a72aa-2832">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2832">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a72aa-2833">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2833">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a72aa-2834">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2834">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a72aa-2835">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2835">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a72aa-2836">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a72aa-2836">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a72aa-2837">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="a72aa-2837">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a72aa-2838">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="a72aa-2838">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a72aa-2839">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="a72aa-2839">Provide feedback from the command line with the `az feedback` command</span></span>


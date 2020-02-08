---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/04/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: eafd18344ac4c1c0124ff53864a45510070b6fe7
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013287"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="460d8-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="460d8-103">Azure CLI release notes</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="460d8-104">2020년 2월 4일</span><span class="sxs-lookup"><span data-stu-id="460d8-104">February 04, 2020</span></span>

<span data-ttu-id="460d8-105">버전 2.0.81</span><span class="sxs-lookup"><span data-stu-id="460d8-105">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-106">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-106">ACS</span></span>

* <span data-ttu-id="460d8-107">표준 부하 분산 장치에서 아웃바운드 할당된 포트 및 유휴 시간 제한을 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-107">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="460d8-108">API 버전 2019-11-01 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-108">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-109">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-109">ACR</span></span>

* <span data-ttu-id="460d8-110">[호환성이 손상되는 변경]  `az acr delete` 메시지가 표시됨</span><span class="sxs-lookup"><span data-stu-id="460d8-110">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="460d8-111">[호환성이 손상되는 변경] 'az acr task delete' 메시지가 표시됨</span><span class="sxs-lookup"><span data-stu-id="460d8-111">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="460d8-112">taskrun 관리를 위한 새 명령 그룹 'az acr taskrun show/list/delete' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-112">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-113">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-113">AKS</span></span>

* <span data-ttu-id="460d8-114">각 클러스터는 격리를 향상하기 위한 별도의 서비스 주체 보유</span><span class="sxs-lookup"><span data-stu-id="460d8-114">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="460d8-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="460d8-115">AppConfig</span></span>

* <span data-ttu-id="460d8-116">appservice에서 키 자격 증명 모음 참조 가져오기/내보내기 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-116">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="460d8-117">appconfig에서 appconfig로 모든 레이블 가져오기/내보내기 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-117">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="460d8-118">키 및 기능 이름을 가져오기 전에 유효성 검사</span><span class="sxs-lookup"><span data-stu-id="460d8-118">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="460d8-119">구성 저장소에 대한 sku 수정 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-119">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="460d8-120">관리 ID에 대한 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-120">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-121">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-121">AppService</span></span>

* <span data-ttu-id="460d8-122">Azure Stack: 2019-03-01-hybrid 프로필 아래에 명령 표시</span><span class="sxs-lookup"><span data-stu-id="460d8-122">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="460d8-123">functionapp: Linux에서 Java 함수 앱을 만드는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-123">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-124">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-124">ARM</span></span>

* <span data-ttu-id="460d8-125">이슈 #10246 해결: 전달된 `--ids` 매개 변수가 리소스 그룹 ID인 경우 `az resource tag`가 충돌</span><span class="sxs-lookup"><span data-stu-id="460d8-125">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="460d8-126">이슈 #11658 해결: `az group export` 명령은 `--query` 및 `--output` 매개 변수를 지원하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-126">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="460d8-127">이슈 #10279 해결: 확인이 실패하면 `az group deployment validate`의 종료 코드는 0</span><span class="sxs-lookup"><span data-stu-id="460d8-127">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="460d8-128">이슈 #9916 해결: `az resource list` 명령의 태그와 기타 필터 조건 간의 충돌 오류 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-128">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="460d8-129">`az group create` 명령의 managedBy 정보를 추가할 수 있도록 새 매개 변수 `--managed-by` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-129">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="460d8-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="460d8-130">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="460d8-131">Azure Red Hat OpensShift 클러스터에서 Log Analytics 모니터링을 관리할 `monitor` 하위 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-131">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-132">BotService</span><span class="sxs-lookup"><span data-stu-id="460d8-132">BotService</span></span>

* <span data-ttu-id="460d8-133">이슈 #11697 해결: `az bot create`는 멱등원(idempotent)이 아님</span><span class="sxs-lookup"><span data-stu-id="460d8-133">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="460d8-134">라이브 모드에서만 실행되도록 이름-수정 테스트 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-134">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-135">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-135">CDN</span></span>

* <span data-ttu-id="460d8-136">rulesEngine 기능에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-136">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="460d8-137">규칙을 관리하는 새 명령 그룹 'cdn endpoint rule' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-137">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="460d8-138">api 버전 2019-04-15를 사용하도록 azure-mgmt-cdn 버전을 4.0.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-138">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="460d8-139">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="460d8-139">Deployment Manager</span></span>

* <span data-ttu-id="460d8-140">모든 리소스에 대한 나열 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-140">Add list operation for all resources.</span></span>
* <span data-ttu-id="460d8-141">새 단계 유형에 대한 단계 리소스를 향상합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-141">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="460d8-142">0\.2.0 버전을 사용하도록 azure-mgmt-deploymentmanager 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-142">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-143">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-143">IoT</span></span>

* <span data-ttu-id="460d8-144">'IoT hub Job' 명령을 사용 중단합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-144">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="460d8-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="460d8-145">IoT Central</span></span>

* <span data-ttu-id="460d8-146">새 sku 이름 ST0, ST1, ST2를 사용하여 앱 만들기/업데이트를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-146">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-147">Key Vault</span></span>

* <span data-ttu-id="460d8-148">키를 다운로드하는 새 명령 `az keyvault key download`를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-148">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="460d8-149">기타</span><span class="sxs-lookup"><span data-stu-id="460d8-149">Misc</span></span>

* <span data-ttu-id="460d8-150">#6371 해결: Bash에서 파일 이름 및 환경 변수 완료 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-150">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="460d8-151">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-151">Network</span></span>

* <span data-ttu-id="460d8-152">#2092 해결: az network dns record-set add/remove: 레코드 세트를 찾을 수 없을 때 표시할 경고를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-152">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="460d8-153">나중에 이 자동 생성을 확인하는 추가 인수를 지원할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-153">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="460d8-154">정책</span><span class="sxs-lookup"><span data-stu-id="460d8-154">Policy</span></span>

* <span data-ttu-id="460d8-155">다양한 정책 메타데이터 리소스를 검색하는 새 명령 `az policy metadata` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-155">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="460d8-156">`az policy remediation create`: `--resource-discovery-mode` 매개 변수를 사용하여 재구성하기 전에 규정 준수를 다시 평가해야 하는지 여부를 지정</span><span class="sxs-lookup"><span data-stu-id="460d8-156">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-157">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-157">Profile</span></span>

* <span data-ttu-id="460d8-158">`az account get-access-token`: 구독을 지정할 필요 없이 테넌트의 토큰을 직접 획득할 수 있도록 `--tenant` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-158">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-159">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-159">RBAC</span></span>

* <span data-ttu-id="460d8-160">[호환성이 손상되는 변경] #11883 해결: `az role assignment create`: 빈 범위에서 오류 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="460d8-160">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="460d8-161">보안</span><span class="sxs-lookup"><span data-stu-id="460d8-161">Security</span></span>

* <span data-ttu-id="460d8-162">스토리지 계정의 고급 위협 방지 설정을 살펴보고 관리할 수 있는 새 명령 `az atp show` 및 `az atp update`를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-162">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-163">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-163">SQL</span></span>

* <span data-ttu-id="460d8-164">`sql dw create`: `--zone-redundant` 및 `--read-replica-count` 매개 변수를 사용 중단합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-164">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="460d8-165">이러한 매개 변수는 DataWarehouse에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-165">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="460d8-166">[호환성이 손상되는 변경] `az sql db create`: "az sql db create --sample-name"에 허용되는 값으로 설명된 "WideWorldImportersStd" 및 "WideWorldImportersFull"을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-166">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="460d8-167">이러한 샘플 데이터베이스는 항상 만들기가 실패하는 원인이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-167">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="460d8-168">SQL 데이터베이스의 민감도 분류를 관리하는 새 명령 `sql db classification show/list/update/delete` 및 `sql db classification recommendation list/enable/disable`을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-168">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="460d8-169">`az sql db audit-policy`: 빈 감사 작업 및 그룹에 대한 픽스</span><span class="sxs-lookup"><span data-stu-id="460d8-169">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-170">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-170">Storage</span></span>

* <span data-ttu-id="460d8-171">Azure 파일 공유 관리 작업에 Microsoft.Storage 리소스 공급자를 사용하도록 새 명령 그룹 `az storage share-rm`을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-171">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="460d8-172">이슈 #11415: `az storage blob update`에 대한 권한 오류 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-172">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="460d8-173">Azcopy 10.3.3을 통합하고 Win32를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-173">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="460d8-174">`az storage copy`: `--include-path`, `--include-pattern`, `--exclude-path` 및 `--exclude-pattern` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-174">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="460d8-175">`az storage remove`: `--inlcude` 및 `--exclude` 매개 변수를 `--include-path`, `--include-pattern`, `--exclude-path` 및 `--exclude-pattern` 매개 변수로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-175">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="460d8-176">`az storage sync`: `--include-pattern`, `--exclude-path` 및 `--exclude-pattern` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-176">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="460d8-177">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="460d8-177">ServiceFabric</span></span>

* <span data-ttu-id="460d8-178">애플리케이션 및 서비스를 관리하는 새 명령이 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-178">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="460d8-179">2020년 1월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-179">January 13, 2020</span></span>

<span data-ttu-id="460d8-180">버전 2.0.80</span><span class="sxs-lookup"><span data-stu-id="460d8-180">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-181">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-181">Compute</span></span>

* <span data-ttu-id="460d8-182">디스크 업데이트: --disk-encryption-set 및 --encryption-type 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-182">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="460d8-183">스냅샷 만들기/업데이트: --disk-encryption-set 및 --encryption-type 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-183">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-184">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-184">Storage</span></span>

* <span data-ttu-id="460d8-185">azure-mgmt-storage 버전을 7.1.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="460d8-185">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="460d8-186">`az storage account create`: 테이블 및 큐 암호화 서비스를 지원하기 위해 `--encryption-key-type-for-table` 및 `--encryption-key-type-for-queue` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-186">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="460d8-187">2020년 1월 7일</span><span class="sxs-lookup"><span data-stu-id="460d8-187">January 07, 2020</span></span>

<span data-ttu-id="460d8-188">버전 2.0.79</span><span class="sxs-lookup"><span data-stu-id="460d8-188">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-189">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-189">ACR</span></span>

* <span data-ttu-id="460d8-190">[호환성이 손상되는 변경] 'acr build', 'acr task create/update', 'acr run' 및 'acr pack'에서 '--os' 매개 변수 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-190">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="460d8-191">대신 '--platform'을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="460d8-191">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="460d8-192">AppConfig</span><span class="sxs-lookup"><span data-stu-id="460d8-192">AppConfig</span></span>

* <span data-ttu-id="460d8-193">기능 플래그 가져오기/내보내기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-193">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="460d8-194">keyvault 참조를 만들려면 새 명령 'az appconfig kv set-keyvault' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-194">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="460d8-195">기능 플래그를 파일로 내보낼 때 다양한 명명 규칙 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-195">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-196">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-196">AppService</span></span>

* <span data-ttu-id="460d8-197">이슈 #7154 해결: 작은따옴표 대신 백틱을 사용하도록 명령 <>에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-197">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="460d8-198">이슈 #11287 해결: webapp up: up을 사용하여 만든 앱은 기본적으로 'SSL 사용'으로 설정되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-198">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="460d8-199">이슈 #11592 해결: html 정적 사이트에 대한 az webapp up 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-199">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-200">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-200">ARM</span></span>

* <span data-ttu-id="460d8-201">`az resource tag` 해결: Recovery Services 자격 증명 모음 태그를 업데이트할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-201">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-202">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-202">Backup</span></span>

* <span data-ttu-id="460d8-203">IaasVM 워크로드의 일시 삭제 기능을 지원하기 위해 새 명령 'backup protection undelete' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-203">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="460d8-204">backup-properties 명령을 설정하기 위해 새 매개 변수 '--soft-delete-feature-state' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-204">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="460d8-205">IaasVM 워크로드에 대한 디스크 제외 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-205">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-206">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-206">Compute</span></span>

* <span data-ttu-id="460d8-207">Azure Stack 프로필에서 `vm create` 오류 해결.</span><span class="sxs-lookup"><span data-stu-id="460d8-207">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="460d8-208">vm monitor metrics tail/list-definitions: vm에 쿼리 메트릭 및 목록 정의 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-208">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="460d8-209">az vm의 새로운 다시 적용 명령 작업 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-209">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-210">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-210">HDInsight</span></span>

* <span data-ttu-id="460d8-211">Kafka Rest 프록시로 Kafka 클러스터 생성 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-211">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="460d8-212">azure-mgmt-hdinsight를 1.3.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="460d8-212">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="460d8-213">기타</span><span class="sxs-lookup"><span data-stu-id="460d8-213">Misc.</span></span>

* <span data-ttu-id="460d8-214">기본적으로 JSON 형식 또는 --output으로 구성된 형식으로 Azure CLI 모듈 및 확장 버전을 표시하기 위해 미리 보기 명령 `az version show` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-214">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="460d8-215">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="460d8-215">Event Hubs</span></span>

* <span data-ttu-id="460d8-216">[호환성이 손상되는 변경] 'az eventhubs eventhub update' 및 'az eventhubs eventhub create' 명령에서 'ReceiveDisabled' 상태 옵션 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-216">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="460d8-217">이 옵션은 이벤트 허브 항목에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-217">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="460d8-218">Service Bus</span><span class="sxs-lookup"><span data-stu-id="460d8-218">Service Bus</span></span>

* <span data-ttu-id="460d8-219">[호환성이 손상되는 변경] 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' 및 'az servicebus queue update' 명령에서 'ReceiveDisabled' 상태 옵션 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-219">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="460d8-220">이 옵션은 Service Bus 항목 및 큐에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-220">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-221">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-221">RBAC</span></span>

* <span data-ttu-id="460d8-222">#11712 해결: 애플리케이션 또는 서비스 주체가 없을 때 `az ad app/sp show`가 종료 코드 3을 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-222">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-223">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-223">Storage</span></span>

* <span data-ttu-id="460d8-224">`az storage account create`: --enable-hierarchical-namespace 매개 변수에 대한 미리 보기 플래그 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-224">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="460d8-225">api 버전 2019-06-01을 사용하도록 azure-mgmt-storage 버전이 7.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-225">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="460d8-226">스토리지 계정 blob-service-properties에 대한 보존 정책 삭제 관리를 지원하도록 새 매개 변수 `--enable-delete-retention` 및 `--delete-retention-days` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-226">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="460d8-227">2019년 12월 17일</span><span class="sxs-lookup"><span data-stu-id="460d8-227">December 17, 2019</span></span>

<span data-ttu-id="460d8-228">2.0.78</span><span class="sxs-lookup"><span data-stu-id="460d8-228">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-229">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-229">ACR</span></span>

* <span data-ttu-id="460d8-230">acr task run에 로컬 컨텍스트 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-230">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-231">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-231">ACS</span></span>

* <span data-ttu-id="460d8-232">[호환성이 손상되는 변경]az openshift create: `--workspace-resource-id`에서 `--workspace-id`로 이름이 변경됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-232">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-233">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-233">AMS</span></span>

* <span data-ttu-id="460d8-234">리소스를 찾을 수 없을 때 3을 반환하도록 show 명령 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-234">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="460d8-235">AppConfig</span><span class="sxs-lookup"><span data-stu-id="460d8-235">AppConfig</span></span>

* <span data-ttu-id="460d8-236">요청 url에 api-version을 추가할 때 버그 해결.</span><span class="sxs-lookup"><span data-stu-id="460d8-236">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="460d8-237">기존 해결책은 페이지 매김과 함께 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-237">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="460d8-238">백 엔드 서비스에서 세계화를 위한 유니코드를 지원함에 따라 영어 이외의 언어를 표시하는 지원 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-238">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-239">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-239">AppService</span></span>

* <span data-ttu-id="460d8-240">이슈 #11217 해결: webapp: az webapp config ssl upload가 슬롯 매개 변수를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-240">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="460d8-241">이슈 #10965 해결: 오류: 이름을 비워 둘 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-241">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="460d8-242">ip_address 및 subnet으로 제거 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-242">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="460d8-243">Key Vault `az webapp config ssl import`에서 인증서 가져오기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-243">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-244">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-244">ARM</span></span>

* <span data-ttu-id="460d8-245">6\.0.0을 사용하도록 azure-mgmt-resource 패키지가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-245">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="460d8-246">새 매개 변수 `--aux-subs`를 추가하여 `az group deployment create` 명령에 대한 교차 테넌트 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-246">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="460d8-247">정책 세트 정의에 대한 메타데이터 정보 추가를 지원하기 위해 새 매개 변수 `--metadata` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-247">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-248">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-248">Backup</span></span>

* <span data-ttu-id="460d8-249">SQL 및 SAP Hana 워크로드에 대한 Backup 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-249">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-250">BotService</span><span class="sxs-lookup"><span data-stu-id="460d8-250">BotService</span></span>

* <span data-ttu-id="460d8-251">[호환성이 손상되는 변경] 미리 보기 명령 'az bot create'에서 '--version' 플래그 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-251">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="460d8-252">v4 SDK 봇만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-252">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="460d8-253">'az bot create'에 대한 이름 가용성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-253">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="460d8-254">'az bot update'를 통해 봇의 아이콘 URL 업데이트에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-254">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="460d8-255">'az bot directline update'를 통해 Direct Line 채널을 업데이트하는 기능에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-255">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="460d8-256">'az bot directline create'에 '--enable-enhanced-auth' 플래그 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-256">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="460d8-257">'az bot authsetting' 명령 그룹은 미리 보기 상태가 아니라 GA입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-257">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="460d8-258">'az bot'의 'create', 'prepare-deploy', 'show', 'delete', 'update' 명령은 미리 보기 상태가 아니라 GA입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-258">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="460d8-259">'--proj-file-path' 값을 소문자로 변경(예: "Test.csproj"를 "test.csproj"로)하는 'az bot prepare-deploy' 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-259">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-260">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-260">Compute</span></span>

* <span data-ttu-id="460d8-261">vmss create/update: VMSS를 축소할 때 어떤 가상 머신을 제거할지 결정하는 --scale-in-policy 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-261">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="460d8-262">vm/vmss update: --priority 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-262">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="460d8-263">vm/vmss update: --max-price 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-263">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="460d8-264">disk-encryption-set 명령 그룹(create, show, update, delete, list) 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-264">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="460d8-265">disk create: --encryption-type 및 --disk-encryption-set 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-265">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="460d8-266">vm/vmss create: --os-disk-encryption-set 및 --data-disk-encryption-sets 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-266">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="460d8-267">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-267">Core</span></span>

* <span data-ttu-id="460d8-268">Python 3.4에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-268">Removed support for Python 3.4</span></span>
* <span data-ttu-id="460d8-269">여러 명령에 HaTS 설문 조사 연결</span><span class="sxs-lookup"><span data-stu-id="460d8-269">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="460d8-270">DLS</span><span class="sxs-lookup"><span data-stu-id="460d8-270">DLS</span></span>

* <span data-ttu-id="460d8-271">ADLS sdk 버전이 업데이트되었습니다(0.0.48).</span><span class="sxs-lookup"><span data-stu-id="460d8-271">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="460d8-272">설치</span><span class="sxs-lookup"><span data-stu-id="460d8-272">Install</span></span>

* <span data-ttu-id="460d8-273">설치 스크립트 지원(python 3.8)</span><span class="sxs-lookup"><span data-stu-id="460d8-273">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-274">IOT</span><span class="sxs-lookup"><span data-stu-id="460d8-274">IOT</span></span>

* <span data-ttu-id="460d8-275">[호환성이 손상되는 변경] manual-failover에서 --failover-region 매개 변수 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-275">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="460d8-276">이제 할당된, 지리적으로 연결된 보조 지역으로 장애 조치(failover)됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-276">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-277">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-277">Key Vault</span></span>

* <span data-ttu-id="460d8-278">#8095 해결: `az keyvault storage remove`: 도움말 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-278">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="460d8-279">#8921 해결: `az keyvault key/secret/certificate list/list-deleted/list-versions`: 매개 변수 `--maxresults`의 유효성 검사 버그 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-279">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="460d8-280">#10512 해결: `az keyvault set-policy`: `--object-id`, `--spn` 또는 `--upn`이 지정된 경우 오류 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-280">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="460d8-281">#10846 해결: `az keyvault secret show-deleted`: `--id`가 지정된 경우 `--name/-n`이 필요 없습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-281">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="460d8-282">#11084 해결: `az keyvault secret download`: 매개 변수 `--encoding`의 도움말 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-282">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-283">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-283">Network</span></span>

* <span data-ttu-id="460d8-284">az network application-gateway probe: 생성 및 업데이트 시 백엔드 서버를 검색할 포트를 지정하는 --port 옵션에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-284">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="460d8-285">az network application-gateway url-path-map create/update: `--waf-policy`에 대한 버그 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-285">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="460d8-286">az network application-gateway: `--rewrite-rule-set` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-286">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="460d8-287">az network list-service-aliases: 서비스 엔드포인트 정책에 사용할 수 있는 지원 목록 서비스 별칭 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-287">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="460d8-288">az network dns zone import: 레코드 이름에 .@ 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-288">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="460d8-289">패키징</span><span class="sxs-lookup"><span data-stu-id="460d8-289">Packaging</span></span>

* <span data-ttu-id="460d8-290">pip 설치를 위한 백 에지 빌드 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-290">Added back edge builds for pip install</span></span>
* <span data-ttu-id="460d8-291">Ubuntu eoan 패키지 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-291">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="460d8-292">정책</span><span class="sxs-lookup"><span data-stu-id="460d8-292">Policy</span></span>

* <span data-ttu-id="460d8-293">정책 API 버전 2019-09-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-293">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="460d8-294">az policy set-definition: 정책 세트 정의 내에서 `--definition-groups` 매개 변수를 사용한 그룹화 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-294">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="460d8-295">Redis</span><span class="sxs-lookup"><span data-stu-id="460d8-295">Redis</span></span>

* <span data-ttu-id="460d8-296">`az redis create` 명령에 `--replicas-per-master` 미리 보기 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-296">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="460d8-297">azure-mgmt-redis가 6.0.0에서 7.0.0rc1로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-297">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="460d8-298">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="460d8-298">ServiceFabric</span></span>

* <span data-ttu-id="460d8-299">#10963을 포함한 노드 유형 추가 논리 이슈 해결: 내구성 수준이 Gold인 새 노드 유형을 추가할 때마다 CLI 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-299">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="460d8-300">생성 템플릿에서 ServiceFabricNodeVmExt 버전이 1.1로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-300">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-301">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-301">SQL</span></span>

* <span data-ttu-id="460d8-302">읽기 확장 관리를 지원하도록 sql db create 및 update 명령에 "--read-scale" 및 "--read-replicas" 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-302">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-303">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-303">Storage</span></span>

* <span data-ttu-id="460d8-304">스토리지 계정 만들기 및 업데이트 명령의 GA 릴리스 대용량 파일 공유 속성</span><span class="sxs-lookup"><span data-stu-id="460d8-304">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="460d8-305">GA 릴리스 사용자 위임 SAS 토큰 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-305">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="460d8-306">스토리지 계정의 blob service 속성을 관리하기 위해 새 명령 `az storage account blob-service-properties show` 및 `az storage account blob-service-properties update --enable-change-feed` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-306">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="460d8-307">[예정된 호환성이 손상되는 변경] `az storage copy`: `*` 문자는 더 이상 URL에서 와일드카드로 지원되지 않지만 `*` 와일드카드 지원과 함께 새 매개 변수 --include-pattern 및 --exclude-pattern이 추가될 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-307">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="460d8-308">이슈 #11043 해결: `az storage remove` 명령에서 전체 컨테이너/공유를 제거하는 지원 기능 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-308">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="460d8-309">2019년 11월 26일</span><span class="sxs-lookup"><span data-stu-id="460d8-309">November 26, 2019</span></span>

<span data-ttu-id="460d8-310">버전 2.0.77</span><span class="sxs-lookup"><span data-stu-id="460d8-310">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-311">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-311">ACR</span></span>

* <span data-ttu-id="460d8-312">acr task create/update의 `--branch` 매개 변수가 더 이상 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-312">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="460d8-313">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="460d8-313">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="460d8-314">`--workspace-resource-id` 플래그가 추가되어 모니터링으로 Azure Red Hat Openshift 클러스터 생성 가능</span><span class="sxs-lookup"><span data-stu-id="460d8-314">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="460d8-315">모니터링으로 Azure Red Hat OpenShift 클러스터를 만드는 `monitor_profile`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-315">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-316">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-316">AKS</span></span>

* <span data-ttu-id="460d8-317">"az aks rotate-certs"를 사용한 지원 클러스터 인증서 순환 작업이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-317">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="460d8-318">AppConfig</span><span class="sxs-lookup"><span data-stu-id="460d8-318">AppConfig</span></span>

* <span data-ttu-id="460d8-319">":"을 `as az appconfig kv import` 구분 기호로 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-319">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="460d8-320">Null 레이블을 포함하여 여러 레이블이 있는 키 값을 나열하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-320">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="460d8-321">관리 평면 sdk, azure-mgmt-appconfiguration이 버전 0.3.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-321">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="460d8-322">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-322">AppService</span></span>

* <span data-ttu-id="460d8-323">#11100 문제가 해결됨: 서비스 계획을 만들 때 az webapp up의 AttributeError</span><span class="sxs-lookup"><span data-stu-id="460d8-323">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="460d8-324">az webapp up: 지원되는 언어를 위해 사이트를 만들거나 배포하도록 적용하면 기본값이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-324">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="460d8-325">App Service Environment에 대한 지원 추가t: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="460d8-325">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-326">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-326">Backup</span></span>

* <span data-ttu-id="460d8-327">az backup policy list-associated-items 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-327">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="460d8-328">선택적 BackupManagementType 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-328">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-329">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-329">Compute</span></span>

* <span data-ttu-id="460d8-330">컴퓨팅, 디스크, 스냅샷의 API 버전이 2019-07-01로 업그레이드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-330">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="460d8-331">vmss create: --orchestration-mode 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-331">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="460d8-332">sig image-definition create: --os-state가 추가되어 이 이미지로 생성된 가상 머신이 'Generalized'인지 아니면 'Specialized'인지 지정 가능</span><span class="sxs-lookup"><span data-stu-id="460d8-332">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="460d8-333">sig image-definition create: --hyper-v-generation이 추가되어 하이퍼바이저 세대 지정 가능</span><span class="sxs-lookup"><span data-stu-id="460d8-333">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="460d8-334">sig image-version create: 지원 --os-snapshot 및 --data-snapshots 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-334">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="460d8-335">image create: --data-disk-caching이 추가되어 데이터 디스크의 캐싱 설정을 지정할 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-335">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="460d8-336">Python Compute SDK를 10.0.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="460d8-336">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="460d8-337">vm/vmss create: 'Priority' 열거형 속성에 'Spot' 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-337">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="460d8-338">[호환성이 손상되는 변경] Swagger 및 Powershell cmdlet과 일치하도록 VM 및 VMSS에 대한 '--max-billing' 매개 변수의 이름이 '--max-price'로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-338">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="460d8-339">vm monitor log show: 연결된 로그 분석 작업 영역을 통한 로그 쿼리에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-339">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-340">IOT</span><span class="sxs-lookup"><span data-stu-id="460d8-340">IOT</span></span>

* <span data-ttu-id="460d8-341">#2531 수정됨: 허브 업데이트에 대한 편의 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-341">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="460d8-342">#8323 수정됨: 스토리지 사용자 지정 엔드포인트를 만드는 누락된 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-342">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="460d8-343">재발 버그 수정: 기본 스토리지 엔드포인트를 재정의하는 변경 사항을 되돌렸습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-343">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-344">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-344">Key Vault</span></span>

* <span data-ttu-id="460d8-345">#11121 수정됨: `az keyvault certificate list`를 사용하는 경우 `--include-pending`을 전달할 때 이제 `true` 또는 `false` 값이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-345">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="460d8-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="460d8-346">NetAppFiles</span></span>

* <span data-ttu-id="460d8-347">azure-mgmt-netapp이 0.7.0으로 업그레이드되고, 여기에는 향후 복제 작업과 연결된 몇 가지 추가 볼륨 속성이 포함됨</span><span class="sxs-lookup"><span data-stu-id="460d8-347">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="460d8-348">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-348">Network</span></span>

* <span data-ttu-id="460d8-349">application-gateway waf-config: 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-349">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="460d8-350">application-gateway waf-policy: 관리형 규칙 집합과 제외 규칙을 관리하는 하위 그룹 managed-rules가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-350">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="460d8-351">application-gateway waf-policy: waf-policy의 글로벌 구성을 관리하는 하위 그룹 policy-setting이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-351">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="460d8-352">[호환성이 손상되는 변경] application-gateway waf-policy: 하위 그룹 규칙의 이름이 custom-rule로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-352">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="460d8-353">application-gateway http-listener: 생성 시 --firewall-policy가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-353">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="460d8-354">application-gateway url-path-map 규칙: 생성 시 --firewall-policy가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-354">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="460d8-355">패키징</span><span class="sxs-lookup"><span data-stu-id="460d8-355">Packaging</span></span>

* <span data-ttu-id="460d8-356">az wrapper가 Python으로 다시 작성됨</span><span class="sxs-lookup"><span data-stu-id="460d8-356">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="460d8-357">Python 3.8에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-357">Added support for Python 3.8</span></span>
* <span data-ttu-id="460d8-358">RPM 패키지의 경우 Python 3으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-358">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-359">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-359">Profile</span></span>

* <span data-ttu-id="460d8-360">Microsoft 계정으로 `az login -u {} -p {}` 실행 시 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-360">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="460d8-361">자체 서명된 루트 인증서로 프록시 뒤에서 `az login` 실행 시 `SSLError`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-361">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="460d8-362">#10578 수정됨: Windows 또는 WSL에서 동시에 둘 이상의 인스턴스가 시작되면 `az login`이 중단됨</span><span class="sxs-lookup"><span data-stu-id="460d8-362">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="460d8-363">#11059 수정됨: 테넌트에 구독이 있는 경우`az login --allow-no-subscriptions`가 실패함</span><span class="sxs-lookup"><span data-stu-id="460d8-363">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="460d8-364">#11238 수정됨: 구독 이름을 바꾼 후 MSI로 로그인하면 동일한 구독이 두 번 나타남</span><span class="sxs-lookup"><span data-stu-id="460d8-364">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-365">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-365">RBAC</span></span>

* <span data-ttu-id="460d8-366">#10996 수정됨: `--password`가 지정되지 않은 경우 `az ad user update`의 `--force-change-password-next-login`에 대한 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-366">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="460d8-367">Redis</span><span class="sxs-lookup"><span data-stu-id="460d8-367">Redis</span></span>

* <span data-ttu-id="460d8-368">#2902 수정됨: 기본 SKU 캐시를 업데이트하는 동안 메모리 구성을 설정하지 마십시오</span><span class="sxs-lookup"><span data-stu-id="460d8-368">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="460d8-369">예약</span><span class="sxs-lookup"><span data-stu-id="460d8-369">Reservations</span></span>

* <span data-ttu-id="460d8-370">SDK 버전을 0.6.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="460d8-370">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="460d8-371">Get-Gatalogs를 호출한 후 billingplan 세부 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-371">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="460d8-372">예약 가격을 계산하는 새 명령 `az reservations reservation-order calculate`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-372">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="460d8-373">새 예약을 구입하는 `az reservations reservation-order purchase`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-373">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="460d8-374">Rest</span><span class="sxs-lookup"><span data-stu-id="460d8-374">Rest</span></span>
* <span data-ttu-id="460d8-375">`az rest`가 GA로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-375">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-376">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-376">SQL</span></span>

* <span data-ttu-id="460d8-377">azure-mgmt-sql이 버전 0.15.0으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="460d8-377">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-378">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-378">Storage</span></span>

* <span data-ttu-id="460d8-379">storage account create: Blob service에서 파일 시스템 의미 체계를 지원하는 --enable-hierarchical-namespace가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-379">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="460d8-380">오류 메시지에서 관련되지 않은 예외가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-380">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="460d8-381">잘못된 오류 메시지 "이 작업을 수행하는 데 필요한 권한이 없습니다." 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-381">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="460d8-382">네트워크 규칙 또는 AuthenticationFailed로 차단된 경우</span><span class="sxs-lookup"><span data-stu-id="460d8-382">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="460d8-383">2019년 11월 4일</span><span class="sxs-lookup"><span data-stu-id="460d8-383">November 4, 2019</span></span>

<span data-ttu-id="460d8-384">버전 2.0.76</span><span class="sxs-lookup"><span data-stu-id="460d8-384">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-385">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-385">ACR</span></span>

* <span data-ttu-id="460d8-386">`az acr pack build` 명령에 `--pack-image-tag` 미리 보기 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-386">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="460d8-387">레지스트리 생성에 대한 감사를 가능하게 하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-387">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="460d8-388">리포지토리 범위 RBAC에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-388">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-389">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-389">AKS</span></span>

* <span data-ttu-id="460d8-390">노드 풀에 대한 클러스터 자동 크기 조정기를 사용할 수 있도록 `--enable-cluster-autoscaler`, `--min-count` 및 `--max-count`를 `az aks create` 명령에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-390">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="460d8-391">위의 플래그뿐만 아니라 클러스터 자동 크기 조정기를 업데이트할 수 있도록 `--update-cluster-autoscaler` 및 `--disable-cluster-autoscaler`도 `az aks update` 명령에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-391">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="460d8-392">AppConfig</span><span class="sxs-lookup"><span data-stu-id="460d8-392">AppConfig</span></span>

* <span data-ttu-id="460d8-393">App Configuration에 저장된 기능 플래그를 관리하는 appconfig 기능 명령 그룹을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-393">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="460d8-394">appconfig kv export to file 명령에 대한 사소한 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-394">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="460d8-395">내보내는 동안 대상 파일 콘텐츠 읽기를 중지합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-395">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-396">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-396">AppService</span></span>

* <span data-ttu-id="460d8-397">`az appservice plan create`: appservice plan create에서 'persitescaling'을 설정하는 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-397">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="460d8-398">webapp config ssl bind 작업이 리소스에서 기존 태그를 제거하는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-398">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="460d8-399">함수 앱을 배포하는 동안 원격 빌드 작업을 지원하기 위해 `az functionapp deployment source config-zip`에 대해 `--build-remote` 플래그를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-399">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="460d8-400">Windows의 경우 함수 앱의 기본 노드 버전을 ~10으로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-400">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="460d8-401">`az functionapp create`에 `--runtime-version` 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-401">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-402">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-402">ARM</span></span>

* <span data-ttu-id="460d8-403">`az deployment/group deployment validate`: 배포 시 json 템플릿에서 여러 줄과 주석을 지원하기 위해 `--handle-extended-json-format` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-403">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="460d8-404">azure-mgmt-resource가 2019-07-01로 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-404">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-405">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-405">Backup</span></span>

* <span data-ttu-id="460d8-406">AzureFiles 백업 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-406">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-407">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-407">Compute</span></span>

* <span data-ttu-id="460d8-408">`az vm create`: 가속화된 네트워킹 및 기존 NIC를 함께 지정하는 경우 경고를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-408">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="460d8-409">`az vm create`: 가상 머신을 할당해야 하는 기존 가상 머신 확장 집합을 지정하는 `--vmss`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-409">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="460d8-410">`az vm/vmss create`: 제한된 네트워크 환경에서 액세스할 수 있도록 이미지 별칭 파일의 로컬 복사본을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-410">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="460d8-411">`az vmss create`: 확장 집합에서 가상 머신을 관리하는 방법을 지정하는 `--orchestration-mode`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-411">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="460d8-412">`az vm/vmss update`: Ultra SSD 설정 업데이트를 허용하는 `--ultra-ssd-enabled`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-412">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="460d8-413">[호환성이 손상되는 변경] `az vm extension set`: 사용자가 `--ids`를 사용하여 VM에서 확장을 설정할 수 없는 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-413">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="460d8-414">Azure Marketplace 이미지 용어를 관리하는 `az vm image terms accept/cancel/show` 명령을 새로 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-414">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="460d8-415">VMAccessForLinux가 버전 1.5로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-415">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-416">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-416">CosmosDB</span></span>

* <span data-ttu-id="460d8-417">[호환성이 손상되는 변경] `az sql container create`: `--partition-key-path`가 필수 매개 변수로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-417">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="460d8-418">[호환성이 손상되는 변경] `az gremlin graph create`: `--partition-key-path`가 필수 매개 변수로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-418">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="460d8-419">`az sql container create`: `--unique-key-policy` 및 `--conflict-resolution-policy`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-419">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="460d8-420">`az sql container create/update`: `--idx` 기본 스키마가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-420">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="460d8-421">`gremlin graph create`: `--conflict-resolution-policy`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-421">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="460d8-422">`gremlin graph create/update`: `--idx` 기본 스키마가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-422">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="460d8-423">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-423">Fixed typo in help message</span></span>
* <span data-ttu-id="460d8-424">데이터베이스: 사용 중단 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-424">database: Added deprecation infomation</span></span>
* <span data-ttu-id="460d8-425">컬렉션: 사용 중단 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-425">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-426">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-426">IoT</span></span>

* <span data-ttu-id="460d8-427">새 라우팅 원본 유형이 추가됨: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="460d8-427">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="460d8-428">`az iot hub create`에서 누락된 기능이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-428">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-429">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-429">Key Vault</span></span>

* <span data-ttu-id="460d8-430">인증서 파일이 없을 때 발생하는 예기치 않은 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-430">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="460d8-431">`az keyvault recover/purge`가 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-431">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="460d8-432">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="460d8-432">NetAppFiles</span></span>

* <span data-ttu-id="460d8-433">API 버전 2019-07-01을 사용 하도록 azure-mgmt-netapp을 0.6.0으로 업그레이드했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-433">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="460d8-434">이 새로운 API 버전에는 다음이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-434">This new API version includes:</span></span>

    - <span data-ttu-id="460d8-435">볼륨 만들기 `--protocol-types`에서 이제는 "NFSv4"가 아닌 "NFSv4.1"이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-435">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="460d8-436">볼륨 내보내기 정책 속성의 이름은 이제 'nfsv4'가 아닌 'nfsv41'입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-436">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="460d8-437">볼륨 `--creation-token`의 이름이 `--file-path`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-437">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="460d8-438">스냅샷 생성 날짜가 이제 'created'라는 이름으로만 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-438">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="460d8-439">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-439">Network</span></span>

* <span data-ttu-id="460d8-440">`az network private-dns link vnet create/update`: 교차 테넌트 가상 네트워킹 연결을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-440">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="460d8-441">[호환성이 손상되는 변경] `az network vnet subnet list`: `--resource-group` 및 `--vnet-name`이 이제 필수 항목으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-441">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="460d8-442">`az network public-ip prefix create`: 생성 시 IP 주소 버전(IPv4, IPv6)을 지정하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-442">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="460d8-443">azure-mgmt-network를 7.0.0으로 향상시키고 api-version을 2019-09-01로 증가함</span><span class="sxs-lookup"><span data-stu-id="460d8-443">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="460d8-444">`az network vrouter`: 새 서비스 가상 라우터 및 가상 라우터 피어링에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-444">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="460d8-445">`az network express-route gateway connection`: `--internet-security`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-445">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-446">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-446">Profile</span></span>

* <span data-ttu-id="460d8-447">`az account get-access-token --resource-type ms-graph`가 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-447">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="460d8-448">`az login`에서 경고 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-448">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-449">RBAC</span></span>

* <span data-ttu-id="460d8-450">`az ad app update --id {} --display-name {}`이 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-450">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="460d8-451">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="460d8-451">ServiceFabric</span></span>

* <span data-ttu-id="460d8-452">`az sf cluster create`: service fabric linux 및 windows template.json compute vmss를 표준에서 관리 디스크로 수정하여 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-452">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-453">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-453">SQL</span></span>

* <span data-ttu-id="460d8-454">새 SQL Database 제품에 대한 CRUD 작업을 지원하기 위해 `--compute-model`, `--auto-pause-delay` 및 `--min-capacity` 매개 변수를 추가했습니다. 서버리스 컴퓨팅 모델.</span><span class="sxs-lookup"><span data-stu-id="460d8-454">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-455">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-455">Storage</span></span>

* <span data-ttu-id="460d8-456">`az storage account create/update`: --enable-files-adds 매개 변수 및 Azure Active Directory 속성 인수 그룹이 추가되어 Azure Files Active Directory 도메인 서비스 인증을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-456">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="460d8-457">스토리지 계정의 Kerberos 키 나열 또는 다시 생성을 지원하도록 `az storage account keys list/renew`를 확장했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-457">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="460d8-458">2019년 10월 15일</span><span class="sxs-lookup"><span data-stu-id="460d8-458">October 15, 2019</span></span>

<span data-ttu-id="460d8-459">버전 2.0.75</span><span class="sxs-lookup"><span data-stu-id="460d8-459">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-460">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-460">AKS</span></span>

* <span data-ttu-id="460d8-461">Kubernetes 버전에서 지원되는 경우 `--load-balancer-sku` 기본값이 `standard`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-461">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="460d8-462">Kubernetes 버전에서 지원되는 경우 `--vm-set-type` 기본값이 `virtualmachinescalesets`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-462">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-463">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-463">AMS</span></span>

* <span data-ttu-id="460d8-464">[호환성이 손상되는 변경]`job start`의 이름이 `job create`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-464">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="460d8-465">[호환성이 손상되는 변경] UTF8 대신 32자 16진수 문자열을 사용하도록 `content-key-policy create`의 `--ask` 매개 변수가 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-465">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-466">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-466">AppService</span></span>

* <span data-ttu-id="460d8-467">`webapp config access-restriction show|set|add|remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-467">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="460d8-468">`webapp up`에 더 나은 오류 처리 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-468">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="460d8-469">`Isolated` SKU에 대한 지원이 `appservice plan update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-469">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-470">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-470">ARM</span></span>

* <span data-ttu-id="460d8-471">json 템플릿에서 여러 줄과 주석을 지원하기 위해 `--handle-extended-json-format` 매개 변수가 `deployment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-471">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-472">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-472">Compute</span></span>

* <span data-ttu-id="460d8-473">`--enable-agent` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-473">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="460d8-474">영역 사용 시 표준 공용 IP SKU를 자동으로 사용하도록 `vm create`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-474">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="460d8-475">VM에 대해 유효한 컴퓨터 이름을 자동으로 만들도록 `vm create`이 변경됨(제공되지 않은 경우)</span><span class="sxs-lookup"><span data-stu-id="460d8-475">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="460d8-476">VMSS에서 가상 머신의 사용자 지정 컴퓨터 이름 접두사를 지원하기 위해 `vmss create`에 `--computer-name-prefix` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-476">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="460d8-477">로그 분석 작업 영역을 자동으로 사용하도록 `vm create`에 `--workspace` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-477">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="460d8-478">갤러리 API 버전이 2019-07-01로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-478">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="460d8-479">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-479">Core</span></span>

* <span data-ttu-id="460d8-480">일반 업데이트 명령에 `--set` 매개 변수에 대한 구문 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-480">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-481">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-481">IoT</span></span>

* <span data-ttu-id="460d8-482">`iot hub show`에서 "리소스를 찾을 수 없음" 오류가 잘못 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-482">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-483">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-483">Monitor</span></span>

* <span data-ttu-id="460d8-484">CRUD에 대한 지원이 `monitor log-analytics workspace`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-484">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-485">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-485">Network</span></span>

* <span data-ttu-id="460d8-486">교차 테넌트 가상 연결에 대한 지원이 `network private-dns link vnet [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-486">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="460d8-487">[호환성이 손상되는 변경]`--resource-group` 및 `--vnet-name` 매개 변수가 필수 매개 변수가 되도록 `network vnet subnet list`가 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-487">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-488">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-488">SQL</span></span>

* <span data-ttu-id="460d8-489">관리형 인스턴스에서 AAD 관리자 설정을 지원하는 명령이 `sql mi ad-admin`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-489">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-490">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-490">Storage</span></span>

* <span data-ttu-id="460d8-491">서비스에서 서비스로 복사하는 동안 액세스 계층을 유지하기 위해 `storage copy`에 `--preserve-s2s-access-tier` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-491">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="460d8-492">스토리지 계정에 대한 대용량 파일 공유를 지원하기 위해 `storage account [create|update]`에 `--enable-large-file-share` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-492">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="460d8-493">2019년 9월 24일</span><span class="sxs-lookup"><span data-stu-id="460d8-493">September 24, 2019</span></span>

<span data-ttu-id="460d8-494">버전 2.0.74</span><span class="sxs-lookup"><span data-stu-id="460d8-494">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-495">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-495">ACR</span></span>

* <span data-ttu-id="460d8-496">`acr config retention update`에 필수 `--type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-496">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="460d8-497">[호환성이 손상되는 변경] `--name -n` 매개 변수가 `acr config` 명령 그룹에 대한 `--registry -r `로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-497">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-498">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-498">AKS</span></span>

* <span data-ttu-id="460d8-499">`aks create` 명령에 `--load-balancer-sku` 매개 변수가 추가되어 SLB로 AKS 클러스터를 만들 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-499">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="460d8-500">`aks [create|update]` 명령에 `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` 및 `--load-balancer-outbound-ip-prefixes` 매개 변수가 추가되어 SLB로 AKS 클러스터의 부하 분산 장치 프로필을 업데이트할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-500">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="460d8-501">`aks create` 명령에 `--vm-set-type` 매개 변수가 추가되어 AKS 클러스터의 vm 유형을 지정할 수 있게 되었습니다(vmas 또는 vmss).</span><span class="sxs-lookup"><span data-stu-id="460d8-501">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-502">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-502">ARM</span></span>

* <span data-ttu-id="460d8-503">json 템플릿에서 여러 줄과 주석을 지원할 수 있도록 `group deployment create` 명령에 `--handle-extended-json-format` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-503">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-504">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-504">Compute</span></span>

* <span data-ttu-id="460d8-505">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss [create|update]` 명령에 `--terminate-notification-time` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-505">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="460d8-506">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss update` 명령에 `--enable-terminate-notification` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-506">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="460d8-507">`[vm|vmss] create` 명령에 `--priority,` `--eviction-policy,` `--max-billing` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-507">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="460d8-508">디스크 업로드의 정확한 크기를 지정할 수 있도록 `disk create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-508">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="460d8-509">관리 디스크의 증분 스냅샷에 대한 지원이 `snapshot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-509">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="460d8-510">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="460d8-510">Cosmos DB</span></span>

* <span data-ttu-id="460d8-511">키, 읽기 전용 키 또는 연결 문자열을 표시하도록 `cosmosdb keys list` 명령에 `--type <key-type>` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-511">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="460d8-512">`cosmosdb keys regenerate` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-512">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="460d8-513">[사용 되지 않음]`cosmosdb list-connection-strings`, `cosmosdb regenerate-key` 및 `cosmosdb list-read-only-keys` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-513">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="460d8-514">EventGrid</span><span class="sxs-lookup"><span data-stu-id="460d8-514">EventGrid</span></span>

* <span data-ttu-id="460d8-515">오른쪽 매개 변수를 참조하도록 엔드포인트 도움말 텍스트가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-515">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-516">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-516">Key Vault</span></span>

* <span data-ttu-id="460d8-517">테넌트(`login -t`)로 로그인하면 `keyvault create`가 실패할 수 있는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-517">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-518">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-518">Monitor</span></span>

* <span data-ttu-id="460d8-519">`--condition` 인수에서 `:` 문자가 허용되지 않아 `monitor metrics alert create` 할 수 없는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-519">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="460d8-520">정책</span><span class="sxs-lookup"><span data-stu-id="460d8-520">Policy</span></span>

* <span data-ttu-id="460d8-521">정책 API 버전 2019-06-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-521">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="460d8-522">`policy assignment create` 명령에 `--enforcement-mode` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-522">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-523">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-523">Storage</span></span>

* <span data-ttu-id="460d8-524">`az storage copy` 명령에 `--blob-type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-524">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="460d8-525">2019년 9월 10일</span><span class="sxs-lookup"><span data-stu-id="460d8-525">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-526">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-526">ACR</span></span>

* <span data-ttu-id="460d8-527">보존 정책을 구성하는 `acr config retention` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-527">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-528">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-528">AKS</span></span>

* <span data-ttu-id="460d8-529">다음 명령을 통해 ACR 통합 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-529">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="460d8-530">AKS 클러스터에 ACR을 연결하는 `--attach-acr` 매개 변수가 `aks [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-530">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="460d8-531">AKS 클러스터에서 ACR을 분리하는 `--detach-acr` 매개 변수가 `aks update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-531">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-532">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-532">ARM</span></span>

* <span data-ttu-id="460d8-533">2019-05-10 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-533">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-534">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-534">Batch</span></span>

* <span data-ttu-id="460d8-535">`batch pool create`에 대한 `--json-file`에 새 JSON 구성 설정이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-535">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="460d8-536">파일 시스템을 탑재하기 위한 `MountConfigurations`가 추가됨(자세한 내용은 https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="460d8-536">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="460d8-537">`NetworkConfiguration`에 풀의 공용 IP에 대한 선택적 속성 `publicIPs`가 추가됨(자세한 내용은 https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="460d8-537">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="460d8-538">공유 이미지 갤러리에 대한 지원이 `--image`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-538">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="460d8-539">[호환성이 손상되는 변경]`batch pool create`의 기본값 `--start-task-wait-for-success`가 `true`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-539">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="460d8-540">[호환성이 손상되는 변경]`AutoUserSpecification`의 `Scope` 기본값이 항상 풀이 되도록 변경됨(Windows 노드에서는 `Task`, Linux 노드에서는 `Pool`이었음)</span><span class="sxs-lookup"><span data-stu-id="460d8-540">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="460d8-541">이 인수는 `--json-file`을 사용하여 JSON 구성에서만 설정 가능</span><span class="sxs-lookup"><span data-stu-id="460d8-541">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-542">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-542">HDInsight</span></span>

* <span data-ttu-id="460d8-543">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-543">GA release</span></span>
* <span data-ttu-id="460d8-544">[호환성이 손상되는 변경]`az hdinsight resize`의 `--workernode-count/-c` 매개 변수가 필수 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-544">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-545">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-545">Key Vault</span></span>

* <span data-ttu-id="460d8-546">네트워크 규칙에서 서브넷을 삭제할 수 없는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-546">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="460d8-547">중복 서브넷 및 IP 주소를 네트워크 규칙에 추가할 수 있는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-547">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="460d8-548">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-548">Network</span></span>

* <span data-ttu-id="460d8-549">트래픽 분석 간격 값을 설정하는 `--interval` 매개 변수가 `network watcher flow-log`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-549">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="460d8-550">게이트웨이 ID를 관리하는 `network application-gateway identity`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-550">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="460d8-551">Key Vault ID 설정 지원이 `network application-gateway ssl-cert`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-551">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="460d8-552">`network express-route peering peer-connection [show|list]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-552">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="460d8-553">정책</span><span class="sxs-lookup"><span data-stu-id="460d8-553">Policy</span></span>

* <span data-ttu-id="460d8-554">2019-01-01 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-554">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="460d8-555">2019년 8월 27일</span><span class="sxs-lookup"><span data-stu-id="460d8-555">August 27, 2019</span></span>

<span data-ttu-id="460d8-556">버전 2.0.72</span><span class="sxs-lookup"><span data-stu-id="460d8-556">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-557">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-557">ACR</span></span>

* <span data-ttu-id="460d8-558">[호환성이 손상되는 변경]`classic` SKU 지원이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-558">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="460d8-559">API Management</span><span class="sxs-lookup"><span data-stu-id="460d8-559">API Management</span></span>

* <span data-ttu-id="460d8-560">[미리 보기] `apim` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-560">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-561">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-561">AppService</span></span>

* <span data-ttu-id="460d8-562">슬롯 지정 시의 `webapp webjob continuous start` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-562">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="460d8-563">`env` 폴더를 검색하고 배포에 사용된 파일에서 제거하도록 `webapp up`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-563">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-564">Keyvault</span><span class="sxs-lookup"><span data-stu-id="460d8-564">Keyvault</span></span>

* <span data-ttu-id="460d8-565">`--expires` 인수를 무시한 `keyvault secret set`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-565">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="460d8-566">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-566">Network</span></span>

* <span data-ttu-id="460d8-567">`--private-ip-address-version` 인수에 IPv6 주소 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-567">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="460d8-568">프라이빗 엔드포인트를 관리하기 위한 새 `network private-endpoint [create|update|list-types]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-568">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="460d8-569">`network private-link-service` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-569">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="460d8-570">`--private-endpoint-network-policies` 및 `--private-link-service-network-policies` 인수를 `network vnet subnet update`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-570">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-571">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-571">RBAC</span></span>

* <span data-ttu-id="460d8-572">홈페이지가 업데이트되지 않는 `ad app update --homepage` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-572">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="460d8-573">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="460d8-573">ServiceFabric</span></span>

* <span data-ttu-id="460d8-574">대/소문자가 혼합된 Key Vault 이름 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-574">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="460d8-575">Key Vault에서 인증서를 사용할 때 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-575">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="460d8-576">PFX 인증서 파일의 사용 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-576">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="460d8-577">Key Vault 리소스 그룹이 지정되지 않은 `sf cluster certificate add` 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-577">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="460d8-578">`sf cluster set`가 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-578">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="460d8-579">SignalR</span><span class="sxs-lookup"><span data-stu-id="460d8-579">SignalR</span></span>

* <span data-ttu-id="460d8-580">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="460d8-580">Added new commands:</span></span>
  * <span data-ttu-id="460d8-581">`signalr cors`: SignalR CORS 관리</span><span class="sxs-lookup"><span data-stu-id="460d8-581">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="460d8-582">`signalr restart`: SignalR Service 다시 시작</span><span class="sxs-lookup"><span data-stu-id="460d8-582">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="460d8-583">`signalr update`: SignalR Service 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-583">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="460d8-584">`--service-mode` 인수를 `signalr create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-584">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-585">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-585">Storage</span></span>

* <span data-ttu-id="460d8-586">`storage account revoke-delegation-keys` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-586">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="460d8-587">2019년 8월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-587">August 13, 2019</span></span>

<span data-ttu-id="460d8-588">버전 2.0.71</span><span class="sxs-lookup"><span data-stu-id="460d8-588">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-589">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-589">AppService</span></span>

* <span data-ttu-id="460d8-590">슬롯에 대해 `webapp webjob continuous` 명령이 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-590">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-591">BotService</span><span class="sxs-lookup"><span data-stu-id="460d8-591">BotService</span></span>

* <span data-ttu-id="460d8-592">[호환성이 손상되는 변경] v3 SDK 봇 만들기에 대한 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-592">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="460d8-593">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="460d8-593">CognitiveServices</span></span>

* <span data-ttu-id="460d8-594">`cognitiveservices account network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-594">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="460d8-595">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="460d8-595">Cosmos DB</span></span>

* <span data-ttu-id="460d8-596">여러 쓰기 위치 업데이트 시의 경고가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-596">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="460d8-597">CosmosDB SQL, MongoDB, Cassandra, Gremlin 및 Table 리소스 및 리소스 처리량에 대한 CRUD 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-597">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-598">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-598">HDInsight</span></span>

<span data-ttu-id="460d8-599">이 릴리스에는 호환성이 손상되는 변경이 많이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-599">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="460d8-600">[호환성이 손상되는 변경]`hdinsight create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-600">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="460d8-601">`--storage-default-container`에서 `--storage-container`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-601">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="460d8-602">`--storage-default-filesystem`에서 `--storage-filesystem`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-602">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="460d8-603">[호환성이 손상되는 변경]`application create`의 `--name` 인수에서 클러스터 이름 대신 애플리케이션 이름을 나타내도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-603">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="460d8-604">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 `application create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-604">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="460d8-605">[호환성이 손상되는 변경]`application create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-605">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="460d8-606">`--application-type`에서 `--type`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-606">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="460d8-607">`--marketplace-identifier`에서 `--marketplace-id`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-607">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="460d8-608">`--https-endpoint-access-mode`에서 `--access-mode`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-608">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="460d8-609">이름이 `--https-endpoint-destination-port`에서 `--destination-port`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-609">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="460d8-610">[호환성이 손상되는 변경]`application create`에 대한 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-610">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="460d8-611">[호환성이 손상되는 변경] `hdinsight resize`에 대한 이름이 `--target-instance-count`에서 `--workernode-count`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-611">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="460d8-612">[호환성이 손상되는 변경]`hdinsight script-action` 그룹의 모든 명령에서 `--name` 매개 변수를 스크립트 작업 이름으로 사용하도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-612">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="460d8-613">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 모든 `hdinsight script-action` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-613">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="460d8-614">[호환성이 손상되는 변경] 모든 `hdinsight script-action` 명령에 대한 이름이 `--script-execution-id`에서 `--execution-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-614">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="460d8-615">[호환성이 손상되는 변경]`hdinsight script-action show`에서 `hdinsight script-action show-execution-details`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-615">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="460d8-616">[호환성이 손상되는 변경] `hdinsight script-action execute --roles`의 매개 변수에서 쉼표로 구분하는 대신 공백으로 구분하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-616">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="460d8-617">[호환성이 손상되는 변경]`hdinsight script-action list`의 `--persisted` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-617">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="460d8-618">`hdinsight create --cluster-configurations` 매개 변수에서 로컬 JSON 파일 또는 JSON 문자열에 대한 경로를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-618">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="460d8-619">명령 `hdinsight script-action list-execution-history` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-619">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="460d8-620">`hdinsight monitor enable --workspace`에서 Log Analytics 작업 영역 ID 또는 작업 영역 이름을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-620">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="460d8-621">작업 영역 ID가 매개 변수로 제공되는 경우 필요한 `hdinsight monitor enable --primary-key` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-621">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="460d8-622">도움말 메시지에 대한 추가 예제 및 업데이트된 설명이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-622">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-623">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-623">Interactive</span></span>

* <span data-ttu-id="460d8-624">로드 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-624">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="460d8-625">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="460d8-625">Kubernetes</span></span>

* <span data-ttu-id="460d8-626">대시보드 컨테이너 포트에서 `https`를 사용하는 경우 `https`를 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-626">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-627">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-627">Network</span></span>

* <span data-ttu-id="460d8-628">`--yes` 인수가 `network dns record-set cname delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-628">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-629">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-629">Profile</span></span>

* <span data-ttu-id="460d8-630">리소스 액세스 토큰을 가져오기 위해 `--resource-type` 인수가 `account get-access-token`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-630">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="460d8-631">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="460d8-631">ServiceFabric</span></span>

* <span data-ttu-id="460d8-632">sf 클러스터를 만드는 데 지원되는 모든 os 버전이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-632">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="460d8-633">기본 인증서 유효성 검사 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-633">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-634">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-634">Storage</span></span>

* <span data-ttu-id="460d8-635">명령 `storage copy` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-635">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="460d8-636">2019년 7월 30일</span><span class="sxs-lookup"><span data-stu-id="460d8-636">July 30, 2019</span></span>

<span data-ttu-id="460d8-637">버전 2.0.70</span><span class="sxs-lookup"><span data-stu-id="460d8-637">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-638">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-638">ACR</span></span>

* <span data-ttu-id="460d8-639">#9952 문제(`acr pack build` 명령의 회귀)가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-639">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="460d8-640">`acr pack build`의 기본 작성기 이미지 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-640">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-641">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-641">Appservice</span></span>

* <span data-ttu-id="460d8-642">리소스를 찾을 수 없는 경우 메시지를 표시 하도록 `webapp config ssl`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-642">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="460d8-643">`functionapp create`에서 `Standard_RAGRS` 스토리지 계정 유형을 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-643">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="460d8-644">이전 버전의 python을 사용하여 실행할 경우 `webapp up`이(가) 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-644">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="460d8-645">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-645">Network</span></span>

* <span data-ttu-id="460d8-646">`network nic ip-config add`에서 잘못된 매개 변수 `--ids` 제거됨(#9861 수정)</span><span class="sxs-lookup"><span data-stu-id="460d8-646">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="460d8-647">#9604 수정.</span><span class="sxs-lookup"><span data-stu-id="460d8-647">Fixes #9604.</span></span> <span data-ttu-id="460d8-648">사용자가 신뢰할 수 있는 루트 인증서를 연결할 수 있도록 `network application-gateway http-settings [create|update]`에 `--root-certs` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-648">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="460d8-649">`network dns record-set ns create`(#9965)에 대해 인수 `--subscription`을 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-649">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-650">RBAC</span></span>

* <span data-ttu-id="460d8-651">`user update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-651">Added `user update` command</span></span>
* <span data-ttu-id="460d8-652">[사용 되지 않음] 사용자 관련 명령 중 `--upn-or-object-id`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-652">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="460d8-653">대체 인수 `--id` 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-653">Use replacement argument `--id`</span></span>
* <span data-ttu-id="460d8-654">사용자 관련 명령에 `--id` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-654">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-655">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-655">SQL</span></span>

* <span data-ttu-id="460d8-656">관리형 인스턴스 키 및 TDE 보호기에 대한 관리 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-656">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-657">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-657">Storage</span></span>

* <span data-ttu-id="460d8-658">`storage remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-658">Added `storage remove` command</span></span>
* <span data-ttu-id="460d8-659">`storage blob update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-659">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-660">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-660">VM</span></span>

* <span data-ttu-id="460d8-661">새로운 API 버전을 사용하여 영역 세부 정보를 출력하도록 `list-skus`를 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-661">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="460d8-662">`vmss create`에 대한 `--single-placement-group`의 기본값을 `false`로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-662">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="460d8-663">`[snapshot|disk] create`에 대한 ZRS 스토리지 SKU를 선택하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-663">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="460d8-664">전용 호스트를 지원하는 새로운 명령 그룹 `vm host`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-664">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="460d8-665">VM 전용 호스트를 설정하기 위해 `vm create`에 매개 변수 `--host` 및 `--host-group` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-665">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="460d8-666">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="460d8-666">July 16, 2019</span></span>

<span data-ttu-id="460d8-667">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="460d8-667">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-668">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-668">Appservice</span></span>

* <span data-ttu-id="460d8-669">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-669">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="460d8-670">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-670">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="460d8-671">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-671">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="460d8-672">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-672">Core</span></span>

* <span data-ttu-id="460d8-673">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-673">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-674">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-674">Batch</span></span>

* <span data-ttu-id="460d8-675">[호환성이 손상되는 변경]`batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="460d8-675">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="460d8-676">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-676">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="460d8-677">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-677">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="460d8-678">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-678">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="460d8-679">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="460d8-679">Eventhubs</span></span>

* <span data-ttu-id="460d8-680">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-680">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-681">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-681">RDBMS</span></span>

* <span data-ttu-id="460d8-682">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-682">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="460d8-683">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-683">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="460d8-684">릴레이</span><span class="sxs-lookup"><span data-stu-id="460d8-684">Relay</span></span>

* <span data-ttu-id="460d8-685">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-685">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="460d8-686">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-686">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="460d8-687">Servicebus</span><span class="sxs-lookup"><span data-stu-id="460d8-687">Servicebus</span></span>

* <span data-ttu-id="460d8-688">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-688">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-689">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-689">Storage</span></span>

* <span data-ttu-id="460d8-690">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-690">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="460d8-691">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-691">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="460d8-692">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="460d8-692">July 2, 2019</span></span>

<span data-ttu-id="460d8-693">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="460d8-693">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="460d8-694">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-694">Core</span></span>

* <span data-ttu-id="460d8-695">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-695">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="460d8-696">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-696">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="460d8-697">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-697">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-698">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-698">ACR</span></span>

* <span data-ttu-id="460d8-699">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-699">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-700">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-700">Appservice</span></span>

* <span data-ttu-id="460d8-701">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-701">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="460d8-702">[호환성이 손상되는 변경] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-702">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="460d8-703">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-703">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="460d8-704">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-704">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="460d8-705">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="460d8-705">Cosmos DB</span></span>

* <span data-ttu-id="460d8-706">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-706">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="460d8-707">DLS</span><span class="sxs-lookup"><span data-stu-id="460d8-707">DLS</span></span>

* <span data-ttu-id="460d8-708">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="460d8-708">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="460d8-709">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="460d8-709">Feedback</span></span>

* <span data-ttu-id="460d8-710">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-710">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-711">HDInsight</span></span>

* <span data-ttu-id="460d8-712">[호환성이 손상되는 변경]`oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-712">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="460d8-713">[호환성이 손상되는 변경] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-713">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="460d8-714">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-714">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="460d8-715">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-715">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="460d8-716">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-716">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="460d8-717">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-717">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="460d8-718">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-718">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="460d8-719">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-719">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="460d8-720">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-720">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="460d8-721">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="460d8-721">Managed Services</span></span>

* <span data-ttu-id="460d8-722">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="460d8-722">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-723">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-723">Profile</span></span>
* <span data-ttu-id="460d8-724">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-724">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-725">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-725">RBAC</span></span>

* <span data-ttu-id="460d8-726">[호환성이 손상되는 변경]`create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-726">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="460d8-727">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-727">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="460d8-728">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-728">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="460d8-729">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-729">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-730">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-730">RDBMS</span></span>

* <span data-ttu-id="460d8-731">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-731">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-732">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-732">SQL</span></span>

* <span data-ttu-id="460d8-733">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="460d8-733">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-734">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-734">Storage</span></span>

* <span data-ttu-id="460d8-735">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="460d8-735">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="460d8-736">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="460d8-736">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="460d8-737">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-737">VM</span></span>

* <span data-ttu-id="460d8-738">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-738">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="460d8-739">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-739">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="460d8-740">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-740">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="460d8-741">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-741">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="460d8-742">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="460d8-742">June 18, 2019</span></span>

<span data-ttu-id="460d8-743">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="460d8-743">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="460d8-744">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-744">Core</span></span>

<span data-ttu-id="460d8-745">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-745">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="460d8-746">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-746">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="460d8-747">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-747">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="460d8-748">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-748">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="460d8-749">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-749">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="460d8-750">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-750">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="460d8-751">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-751">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-752">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-752">ACR</span></span>
* <span data-ttu-id="460d8-753">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-753">Added 'acr check-health' command</span></span>
* <span data-ttu-id="460d8-754">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-754">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-755">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-755">ACS</span></span>
* <span data-ttu-id="460d8-756">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="460d8-756">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-757">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-757">AMS</span></span>
* <span data-ttu-id="460d8-758">[호환성이 손상되는 변경] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-758">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-759">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-759">AppService</span></span>
* <span data-ttu-id="460d8-760">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-760">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="460d8-761">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-761">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="460d8-762">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-762">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="460d8-763">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-763">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="460d8-764">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-764">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="460d8-765">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-765">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-766">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-766">Batch</span></span>
* <span data-ttu-id="460d8-767">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-767">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-768">BatchAI</span><span class="sxs-lookup"><span data-stu-id="460d8-768">BatchAI</span></span>
* <span data-ttu-id="460d8-769">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="460d8-769">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-770">BotService</span><span class="sxs-lookup"><span data-stu-id="460d8-770">BotService</span></span>
* <span data-ttu-id="460d8-771">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-771">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-772">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-772">CosmosDB</span></span>
* <span data-ttu-id="460d8-773">[사용 되지 않음]`cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-773">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="460d8-774">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="460d8-774">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="460d8-775">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-775">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="460d8-776">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-776">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="460d8-777">EventGrid</span><span class="sxs-lookup"><span data-stu-id="460d8-777">EventGrid</span></span>
* <span data-ttu-id="460d8-778">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-778">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="460d8-779">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-779">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="460d8-780">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-780">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="460d8-781">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-781">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="460d8-782">[호환성이 손상되는 변경]`eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-782">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-783">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-783">HDInsight</span></span>
* <span data-ttu-id="460d8-784">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-784">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-785">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-785">IoT</span></span>
* <span data-ttu-id="460d8-786">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-786">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="460d8-787">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-787">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="460d8-788">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-788">Network</span></span>
* <span data-ttu-id="460d8-789">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-789">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="460d8-790">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-790">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="460d8-791">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-791">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="460d8-792">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-792">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-793">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-793">Resource</span></span>
* <span data-ttu-id="460d8-794">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-794">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="460d8-795">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-795">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="460d8-796">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="460d8-796">ServiceBus</span></span>
* <span data-ttu-id="460d8-797">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-797">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-798">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-798">SQL</span></span>
* <span data-ttu-id="460d8-799">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-799">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="460d8-800">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-800">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="460d8-801">SQLVm</span><span class="sxs-lookup"><span data-stu-id="460d8-801">SQLVm</span></span>
* <span data-ttu-id="460d8-802">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-802">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="460d8-803">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-803">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-804">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-804">Storage</span></span>
* <span data-ttu-id="460d8-805">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-805">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="460d8-806">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-806">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-807">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-807">VM</span></span>
* <span data-ttu-id="460d8-808">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-808">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="460d8-809">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="460d8-809">June 4, 2019</span></span>

<span data-ttu-id="460d8-810">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="460d8-810">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="460d8-811">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-811">Core</span></span>
* <span data-ttu-id="460d8-812">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-812">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-813">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-813">ACR</span></span>
* <span data-ttu-id="460d8-814">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-814">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-815">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-815">ACS</span></span>
* <span data-ttu-id="460d8-816">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-816">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="460d8-817">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="460d8-817">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-818">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-818">Batch</span></span>
* <span data-ttu-id="460d8-819">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-819">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-820">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-820">IoT</span></span>
* <span data-ttu-id="460d8-821">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-821">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="460d8-822">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-822">Network</span></span>
* <span data-ttu-id="460d8-823">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-823">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="460d8-824">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-824">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="460d8-825">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-825">Resource</span></span>
* <span data-ttu-id="460d8-826">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-826">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="460d8-827">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-827">Role</span></span>
* <span data-ttu-id="460d8-828">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-828">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-829">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-829">Compute</span></span>
* <span data-ttu-id="460d8-830">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-830">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="460d8-831">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="460d8-831">May 21, 2019</span></span>

<span data-ttu-id="460d8-832">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="460d8-832">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="460d8-833">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-833">Core</span></span>
* <span data-ttu-id="460d8-834">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-834">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="460d8-835">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-835">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="460d8-836">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-836">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-837">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-837">ACR</span></span>
* <span data-ttu-id="460d8-838">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-838">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-839">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-839">ACS</span></span>
* <span data-ttu-id="460d8-840">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-840">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-841">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-841">AppService</span></span>
* <span data-ttu-id="460d8-842">[사용 되지 않음]`functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-842">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="460d8-843">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-843">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="460d8-844">[호환성이 손상되는 변경]`functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-844">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="460d8-845">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-845">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="460d8-846">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-846">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="460d8-847">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-847">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="460d8-848">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-848">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-849">BotService</span><span class="sxs-lookup"><span data-stu-id="460d8-849">BotService</span></span>
* <span data-ttu-id="460d8-850">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-850">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="460d8-851">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-851">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-852">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-852">Consumption</span></span>
* <span data-ttu-id="460d8-853">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-853">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-854">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-854">IoT</span></span>
* <span data-ttu-id="460d8-855">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-855">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="460d8-856">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-856">Network</span></span>
* [호환성이 손상되는 변경]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="460d8-858">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-858">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="460d8-859">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-859">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-860">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-860">RDBMS</span></span>
* <span data-ttu-id="460d8-861">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-861">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-862">RBAC</span><span class="sxs-lookup"><span data-stu-id="460d8-862">RBAC</span></span>
* <span data-ttu-id="460d8-863">`role assignment`에 관리 그룹 범위 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-863">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-864">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-864">Storage</span></span>
* <span data-ttu-id="460d8-865">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-865">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="460d8-866">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="460d8-866">Compute</span></span>
* <span data-ttu-id="460d8-867">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-867">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="460d8-868">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-868">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="460d8-869">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="460d8-869">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="460d8-870">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-870">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="460d8-871">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="460d8-871">May 6, 2019</span></span>

<span data-ttu-id="460d8-872">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="460d8-872">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-873">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-873">ACS</span></span>
* <span data-ttu-id="460d8-874">[호환성이 손상되는 변경]`openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-874">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="460d8-875">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-875">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="460d8-876">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-876">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="460d8-877">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-877">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-878">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-878">Appservice</span></span>
* <span data-ttu-id="460d8-879">[사용 되지 않음]`functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-879">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="460d8-880">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-880">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="460d8-881">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-881">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="460d8-882">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-882">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="460d8-883">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-883">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="460d8-884">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-884">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="460d8-885">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-885">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="460d8-886">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-886">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="460d8-887">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-887">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="460d8-888">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-888">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-889">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-889">Batch</span></span>
* <span data-ttu-id="460d8-890">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-890">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-891">Botservice</span><span class="sxs-lookup"><span data-stu-id="460d8-891">Botservice</span></span>
* <span data-ttu-id="460d8-892">[호환성이 손상되는 변경]`bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="460d8-892">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="460d8-893">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-893">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="460d8-894">[호환성이 손상되는 변경]`--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-894">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="460d8-895">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="460d8-895">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="460d8-896">[호환성이 손상되는 변경]`--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-896">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="460d8-897">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="460d8-897">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="460d8-898">[호환성이 손상되는 변경]`bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-898">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="460d8-899">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-899">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="460d8-900">[호환성이 손상되는 변경]`bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-900">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="460d8-901">[호환성이 손상되는 변경]`bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-901">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="460d8-902">[호환성이 손상되는 변경]`bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-902">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="460d8-903">[호환성이 손상되는 변경]`--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-903">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="460d8-904">[호환성이 손상되는 변경]`Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-904">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="460d8-905">[호환성이 손상되는 변경]`bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-905">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="460d8-906">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="460d8-906">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="460d8-907">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-907">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="460d8-908">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-908">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="460d8-909">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-909">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="460d8-910">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-910">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="460d8-911">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-911">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="460d8-912">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-912">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="460d8-913">구성</span><span class="sxs-lookup"><span data-stu-id="460d8-913">Configure</span></span>
* <span data-ttu-id="460d8-914">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-914">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="460d8-915">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="460d8-915">Eventhubs</span></span>
* <span data-ttu-id="460d8-916">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-916">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="460d8-917">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-917">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-918">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-918">Network</span></span>
* <span data-ttu-id="460d8-919">[호환성이 손상되는 변경]`vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="460d8-919">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="460d8-920">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="460d8-920">Policy Insights</span></span>
* <span data-ttu-id="460d8-921">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-921">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="460d8-922">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-922">Role</span></span>
* <span data-ttu-id="460d8-923">[사용 되지 않음]`create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-923">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="460d8-924">Service Bus</span><span class="sxs-lookup"><span data-stu-id="460d8-924">Service Bus</span></span>
* <span data-ttu-id="460d8-925">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-925">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="460d8-926">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-926">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="460d8-927">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-927">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-928">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-928">SQL</span></span>
* <span data-ttu-id="460d8-929">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-929">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-930">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-930">VM</span></span>
* <span data-ttu-id="460d8-931">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-931">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="460d8-932">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-932">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="460d8-933">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-933">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="460d8-934">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-934">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="460d8-935">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-935">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="460d8-936">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-936">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="460d8-937">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="460d8-937">April 23, 2019</span></span>

<span data-ttu-id="460d8-938">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="460d8-938">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-939">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-939">ACS</span></span>
* <span data-ttu-id="460d8-940">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-940">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="460d8-941">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-941">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-942">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-942">AMS</span></span>
* <span data-ttu-id="460d8-943">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-943">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-944">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-944">AppService</span></span>
* <span data-ttu-id="460d8-945">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-945">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="460d8-946">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-946">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="460d8-947">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-947">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="460d8-948">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-948">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="460d8-949">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-949">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="460d8-950">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-950">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="460d8-951">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-951">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="460d8-952">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-952">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="460d8-953">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-953">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="460d8-954">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="460d8-954">Deployment Manager</span></span>
* <span data-ttu-id="460d8-955">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="460d8-955">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="460d8-956">랩</span><span class="sxs-lookup"><span data-stu-id="460d8-956">Lab</span></span>
* <span data-ttu-id="460d8-957">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-957">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="460d8-958">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-958">Network</span></span>
* <span data-ttu-id="460d8-959">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-959">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-960">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-960">Resource</span></span>
* <span data-ttu-id="460d8-961">[사용 되지 않음]`resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="460d8-961">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="460d8-962">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="460d8-962">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="460d8-963">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-963">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="460d8-964">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-964">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-965">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-965">SQL</span></span>
* <span data-ttu-id="460d8-966">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-966">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="460d8-967">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-967">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="460d8-968">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-968">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="460d8-969">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-969">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-970">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-970">Storage</span></span>
* <span data-ttu-id="460d8-971">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-971">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-972">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-972">VM</span></span>
* <span data-ttu-id="460d8-973">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-973">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="460d8-974">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-974">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="460d8-975">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-975">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="460d8-976">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="460d8-976">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="460d8-977">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-977">Core</span></span>
* <span data-ttu-id="460d8-978">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-978">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-979">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-979">ACR</span></span>
* <span data-ttu-id="460d8-980">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-980">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-981">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-981">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="460d8-984">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-984">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="460d8-985">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-985">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-986">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-986">AppService</span></span>
* <span data-ttu-id="460d8-987">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-987">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="460d8-988">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-988">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="460d8-989">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-989">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="460d8-990">[호환성이 손상되는 변경]`devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="460d8-990">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="460d8-991">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-991">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="460d8-992">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-992">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="460d8-993">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-993">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-994">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-994">CDN</span></span>
* <span data-ttu-id="460d8-995">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-995">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="460d8-996">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="460d8-996">Feedback</span></span>
* <span data-ttu-id="460d8-997">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-997">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="460d8-998">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-998">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="460d8-999">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-999">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1000">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1000">Monitor</span></span>
* <span data-ttu-id="460d8-1001">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1001">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="460d8-1002">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1002">Network</span></span>
* <span data-ttu-id="460d8-1003">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1003">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="460d8-1004">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1004">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="460d8-1005">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1005">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="460d8-1006">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1006">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="460d8-1007">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="460d8-1007">PrivateDNS</span></span>
* <span data-ttu-id="460d8-1008">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1008">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1009">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1009">Resource</span></span>
* <span data-ttu-id="460d8-1010">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1010">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1011">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1011">Role</span></span>
* <span data-ttu-id="460d8-1012">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1012">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="460d8-1013">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1013">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1014">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1014">SQL</span></span>
* <span data-ttu-id="460d8-1015">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1015">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1016">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1016">Storage</span></span>
* <span data-ttu-id="460d8-1017">[호환성이 손상되는 변경]`storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1017">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="460d8-1018">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1018">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="460d8-1019">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1019">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="460d8-1020">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1020">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="460d8-1021">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="460d8-1021">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="460d8-1022">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1022">Core</span></span>
* <span data-ttu-id="460d8-1023">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1023">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="460d8-1024">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1024">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="460d8-1025">클라우드</span><span class="sxs-lookup"><span data-stu-id="460d8-1025">Cloud</span></span>
* <span data-ttu-id="460d8-1026">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1026">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1027">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1027">ACR</span></span>
* <span data-ttu-id="460d8-1028">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1028">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="460d8-1029">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1029">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="460d8-1030">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1030">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="460d8-1031">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1031">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1032">AppService</span></span>
* <span data-ttu-id="460d8-1033">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1033">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="460d8-1034">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1034">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="460d8-1035">BOT Service</span><span class="sxs-lookup"><span data-stu-id="460d8-1035">BOT Service</span></span>
* <span data-ttu-id="460d8-1036">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1036">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="460d8-1037">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1037">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="460d8-1038">[호환성이 손상되는 변경]`bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1038">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="460d8-1039">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1039">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-1040">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-1040">CDN</span></span>
* <span data-ttu-id="460d8-1041">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1041">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="460d8-1043">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1043">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="460d8-1044">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1044">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-1045">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="460d8-1045">Cosmosdb</span></span>
* <span data-ttu-id="460d8-1046">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1046">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="460d8-1047">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1047">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-1048">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-1048">Interactive</span></span>
* <span data-ttu-id="460d8-1049">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1049">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1050">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1050">Monitor</span></span>
* <span data-ttu-id="460d8-1051">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1051">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1052">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1052">Network</span></span>
* <span data-ttu-id="460d8-1053">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1053">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-1054">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-1054">Profile</span></span>
* <span data-ttu-id="460d8-1055">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1055">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="460d8-1056">Postgres</span><span class="sxs-lookup"><span data-stu-id="460d8-1056">Postgres</span></span> 
* <span data-ttu-id="460d8-1057">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1057">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="460d8-1058">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1058">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1059">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1059">Resource</span></span>
* <span data-ttu-id="460d8-1060">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1060">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="460d8-1061">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1061">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="460d8-1062">그래프</span><span class="sxs-lookup"><span data-stu-id="460d8-1062">Graph</span></span>
* <span data-ttu-id="460d8-1063">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1063">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="460d8-1064">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1064">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="460d8-1065">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1065">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="460d8-1066">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1066">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="460d8-1067">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1067">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1068">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1068">storage</span></span>
* <span data-ttu-id="460d8-1069">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1069">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="460d8-1070">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1070">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="460d8-1071">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1071">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="460d8-1072">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1072">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1073">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1073">VM</span></span>
* <span data-ttu-id="460d8-1074">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1074">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="460d8-1075">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="460d8-1075">March 12, 2019</span></span>

<span data-ttu-id="460d8-1076">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="460d8-1076">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1077">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1077">Core</span></span>

* <span data-ttu-id="460d8-1078">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1078">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1079">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1079">ACR</span></span>

* <span data-ttu-id="460d8-1080">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1080">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1081">ACS</span></span>

* <span data-ttu-id="460d8-1082">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1082">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="460d8-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1083">AppService</span></span>

* <span data-ttu-id="460d8-1084">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1084">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="460d8-1085">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="460d8-1085">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="460d8-1086">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1086">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="460d8-1087">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1087">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-1088">Botservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1088">Botservice</span></span>

* <span data-ttu-id="460d8-1089">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1089">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="460d8-1090">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1090">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="460d8-1091">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1091">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="460d8-1092">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1092">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1093">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1093">Container</span></span>

* <span data-ttu-id="460d8-1094">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1094">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="460d8-1095">EventHub</span><span class="sxs-lookup"><span data-stu-id="460d8-1095">EventHub</span></span>

* <span data-ttu-id="460d8-1096">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1096">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="460d8-1097">찾기</span><span class="sxs-lookup"><span data-stu-id="460d8-1097">Find</span></span>

* <span data-ttu-id="460d8-1098">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1098">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-1099">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-1099">HDInsight</span></span>

* <span data-ttu-id="460d8-1100">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1100">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1101">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1101">Network</span></span>

* <span data-ttu-id="460d8-1102">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1102">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="460d8-1103">Rdbms</span></span>

* <span data-ttu-id="460d8-1104">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1104">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1105">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1105">Role</span></span>

* <span data-ttu-id="460d8-1106">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1106">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="460d8-1107">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1107">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="460d8-1108">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="460d8-1108">Service Fabric</span></span>

* <span data-ttu-id="460d8-1109">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1109">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="460d8-1110">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="460d8-1110">February 26, 2019</span></span>

<span data-ttu-id="460d8-1111">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="460d8-1111">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1112">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1112">Core</span></span>

* <span data-ttu-id="460d8-1113">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1113">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1114">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1114">ACR</span></span>

* <span data-ttu-id="460d8-1115">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1115">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="460d8-1116">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1116">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1117">ACS</span></span>

* <span data-ttu-id="460d8-1118">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1118">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1119">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1119">AppService</span></span>

* <span data-ttu-id="460d8-1120">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1120">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1121">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1121">Batch</span></span>
* <span data-ttu-id="460d8-1122">[호환성이 손상되는 변경]`batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1122">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="460d8-1123">[호환성이 손상되는 변경]`Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1123">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="460d8-1124">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1124">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="460d8-1125">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1125">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="460d8-1126">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1126">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="460d8-1127">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1127">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-1128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-1128">CosmosDB</span></span>

* <span data-ttu-id="460d8-1129">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1129">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="460d8-1130">Kusto</span><span class="sxs-lookup"><span data-stu-id="460d8-1130">Kusto</span></span>

* <span data-ttu-id="460d8-1131">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1131">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1132">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1132">Network</span></span>

* <span data-ttu-id="460d8-1133">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1133">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="460d8-1134">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1134">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="460d8-1135">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1135">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="460d8-1136">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="460d8-1136">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="460d8-1137">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1137">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="460d8-1138">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1138">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="460d8-1139">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1139">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1140">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1140">Resource</span></span>

* <span data-ttu-id="460d8-1141">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1141">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="460d8-1142">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1142">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="460d8-1143">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1143">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="460d8-1144">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1144">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="460d8-1145">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1145">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1146">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1146">Role</span></span>

* <span data-ttu-id="460d8-1147">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1147">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1148">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1148">VM</span></span>

* <span data-ttu-id="460d8-1149">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1149">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="460d8-1150">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="460d8-1150">February 12, 2019</span></span>

<span data-ttu-id="460d8-1151">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="460d8-1151">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1152">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1152">Core</span></span>

* <span data-ttu-id="460d8-1153">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1153">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="460d8-1154">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1154">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1155">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1155">ACR</span></span>
* <span data-ttu-id="460d8-1156">[호환성이 손상되는 변경]`acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1156">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="460d8-1157">[호환성이 손상되는 변경]`acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1157">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1158">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1158">ACS</span></span>
* <span data-ttu-id="460d8-1159">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1159">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="460d8-1160">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1160">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="460d8-1161">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1161">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-1162">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1162">AMS</span></span>
* <span data-ttu-id="460d8-1163">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1163">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="460d8-1164">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1164">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1165">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1165">Appservice</span></span>
* <span data-ttu-id="460d8-1166">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1166">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="460d8-1167">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1167">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="460d8-1168">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1168">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="460d8-1169">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1169">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="460d8-1170">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1170">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-1171">Botservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1171">Botservice</span></span>
* <span data-ttu-id="460d8-1172">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1172">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="460d8-1173">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1173">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="460d8-1174">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1174">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="460d8-1175">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1175">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="460d8-1176">[사용 되지 않음]`--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1176">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="460d8-1177">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1177">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="460d8-1178">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1178">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="460d8-1179">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1179">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="460d8-1180">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1180">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="460d8-1181">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1181">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-1182">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-1182">Key Vault</span></span>
* <span data-ttu-id="460d8-1183">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1183">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1184">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1184">Monitor</span></span>
* <span data-ttu-id="460d8-1185">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1185">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1186">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1186">Network</span></span>
* <span data-ttu-id="460d8-1187">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1187">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="460d8-1188">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1188">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="460d8-1189">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1189">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="460d8-1190">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1190">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="460d8-1191">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="460d8-1191">Policy Insights</span></span>
* <span data-ttu-id="460d8-1192">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1192">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1193">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1193">RDBMS</span></span>
* <span data-ttu-id="460d8-1194">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1194">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="460d8-1195">Redis</span><span class="sxs-lookup"><span data-stu-id="460d8-1195">Redis</span></span>
* <span data-ttu-id="460d8-1196">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1196">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="460d8-1197">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1197">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="460d8-1198">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1198">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="460d8-1199">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1199">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="460d8-1200">[호환성이 손상되는 변경]`redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1200">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="460d8-1201">[호환성이 손상되는 변경]`redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1201">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="460d8-1202">[사용 되지 않음]`redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1202">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1203">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1203">Role</span></span>
* <span data-ttu-id="460d8-1204">[호환성이 손상되는 변경]`vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1204">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="460d8-1205">SQL VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1205">SQL VM</span></span>
* <span data-ttu-id="460d8-1206">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1206">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1207">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1207">VM</span></span>
* <span data-ttu-id="460d8-1208">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1208">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="460d8-1209">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1209">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="460d8-1210">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1210">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="460d8-1211">[호환성이 손상되는 변경]`az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1211">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="460d8-1212">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="460d8-1212">January 31, 2019</span></span>

<span data-ttu-id="460d8-1213">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="460d8-1213">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1214">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1214">Core</span></span>

* <span data-ttu-id="460d8-1215">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1215">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="460d8-1216">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="460d8-1216">January 28, 2019</span></span>

<span data-ttu-id="460d8-1217">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="460d8-1217">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1218">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1218">ACR</span></span>
* <span data-ttu-id="460d8-1219">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1219">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1220">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1220">ACS</span></span>
* <span data-ttu-id="460d8-1221">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1221">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="460d8-1222">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1222">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="460d8-1223">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1223">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-1224">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1224">AMS</span></span>
* <span data-ttu-id="460d8-1225">[호환성이 손상되는 변경]`ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1225">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="460d8-1226">[호환성이 손상되는 변경]`ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1226">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1227">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1227">Appservice</span></span>
* <span data-ttu-id="460d8-1228">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1228">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="460d8-1229">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1229">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="460d8-1230">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1230">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1231">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1231">Container</span></span>
* <span data-ttu-id="460d8-1232">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1232">Added `container start` command</span></span>
* <span data-ttu-id="460d8-1233">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1233">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="460d8-1234">EventGrid</span><span class="sxs-lookup"><span data-stu-id="460d8-1234">EventGrid</span></span>
* <span data-ttu-id="460d8-1235">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1235">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="460d8-1236">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1236">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="460d8-1237">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1237">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="460d8-1238">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1238">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="460d8-1239">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1239">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-1240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-1240">HDInsight</span></span>
* <span data-ttu-id="460d8-1241">[호환성이 손상되는 변경]`hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1241">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="460d8-1242">[호환성이 손상되는 변경]`hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1242">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="460d8-1243">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1243">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="460d8-1244">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1244">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="460d8-1245">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1245">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="460d8-1246">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1246">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-1247">IoT</span></span>
* <span data-ttu-id="460d8-1248">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1248">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="460d8-1249">Kusto</span><span class="sxs-lookup"><span data-stu-id="460d8-1249">Kusto</span></span>
* <span data-ttu-id="460d8-1250">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1250">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1251">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1251">Monitor</span></span>
* <span data-ttu-id="460d8-1252">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1252">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-1253">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-1253">Profile</span></span>
* <span data-ttu-id="460d8-1254">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1254">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1255">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1255">Network</span></span>
* <span data-ttu-id="460d8-1256">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1256">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="460d8-1257">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1257">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1258">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1258">Resource</span></span>
* <span data-ttu-id="460d8-1259">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1259">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="460d8-1260">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1260">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="460d8-1261">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="460d8-1261">SQL Virtual Machine</span></span>
* <span data-ttu-id="460d8-1262">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1262">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1263">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1263">Storage</span></span>
* <span data-ttu-id="460d8-1264">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1264">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="460d8-1265">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1265">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1266">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1266">VM</span></span>
* <span data-ttu-id="460d8-1267">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1267">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="460d8-1268">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1268">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="460d8-1269">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="460d8-1269">January 15, 2019</span></span>

<span data-ttu-id="460d8-1270">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="460d8-1270">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1271">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1271">ACR</span></span>
* <span data-ttu-id="460d8-1272">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1272">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="460d8-1273">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1273">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="460d8-1274">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="460d8-1274">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="460d8-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1275">ACS</span></span>
* <span data-ttu-id="460d8-1276">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1276">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1277">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1277">Appservice</span></span>
* <span data-ttu-id="460d8-1278">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1278">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="460d8-1279">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1279">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="460d8-1280">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1280">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="460d8-1281">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1281">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-1282">Botservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1282">Botservice</span></span>
* <span data-ttu-id="460d8-1283">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1283">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="460d8-1284">구성</span><span class="sxs-lookup"><span data-stu-id="460d8-1284">Configure</span></span>
* <span data-ttu-id="460d8-1285">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1285">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-1286">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-1286">CosmosDB</span></span>
* <span data-ttu-id="460d8-1287">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1287">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-1288">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-1288">HDInsight</span></span>
* <span data-ttu-id="460d8-1289">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1289">Added commands for managing applications</span></span>
* <span data-ttu-id="460d8-1290">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1290">Added commands for managing script actions</span></span>
* <span data-ttu-id="460d8-1291">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1291">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="460d8-1292">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1292">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="460d8-1293">[호환성이 손상되는 변경]`hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1293">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1294">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1294">Network</span></span>
* <span data-ttu-id="460d8-1295">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1295">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="460d8-1296">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1296">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="460d8-1297">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1297">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="460d8-1298">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1298">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1299">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1299">Role</span></span>
* <span data-ttu-id="460d8-1300">[사용 되지 않음]`create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1300">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="460d8-1301">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1301">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="460d8-1302">보안</span><span class="sxs-lookup"><span data-stu-id="460d8-1302">Security</span></span>
* <span data-ttu-id="460d8-1303">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1303">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1304">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1304">Storage</span></span>
* <span data-ttu-id="460d8-1305">[호환성이 손상되는 변경]`storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1305">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="460d8-1306">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1306">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="460d8-1307">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1307">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="460d8-1308">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1308">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="460d8-1309">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1309">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1310">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1310">VM</span></span>
* <span data-ttu-id="460d8-1311">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1311">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="460d8-1312">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1312">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="460d8-1313">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1313">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="460d8-1314">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1314">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="460d8-1315">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1315">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="460d8-1316">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1316">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="460d8-1317">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="460d8-1317">December 20, 2018</span></span>

<span data-ttu-id="460d8-1318">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="460d8-1318">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="460d8-1319">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1319">Appservice</span></span>
* <span data-ttu-id="460d8-1320">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1320">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="460d8-1321">웹앱 스냅샷 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1321">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="460d8-1322">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1322">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="460d8-1323">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="460d8-1323">IoTCentral</span></span>
* <span data-ttu-id="460d8-1324">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1324">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1325">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1325">Role</span></span>
* <span data-ttu-id="460d8-1326">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-1326">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1327">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1327">SQL</span></span>
* <span data-ttu-id="460d8-1328">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1328">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1329">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1329">VM</span></span>
* <span data-ttu-id="460d8-1330">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1330">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="460d8-1331">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="460d8-1331">December 18, 2018</span></span>

<span data-ttu-id="460d8-1332">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="460d8-1332">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="460d8-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1333">ACR</span></span>
* <span data-ttu-id="460d8-1334">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1334">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="460d8-1335">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="460d8-1335">Condensed the table layout for task list</span></span>
* <span data-ttu-id="460d8-1336">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1336">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1337">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1337">ACS</span></span>
* <span data-ttu-id="460d8-1338">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1338">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="460d8-1339">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="460d8-1339">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="460d8-1340">[사용 되지 않음]`az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1340">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="460d8-1341">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1341">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="460d8-1342">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1342">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="460d8-1343">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="460d8-1343">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1344">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1344">Appservice</span></span>
* <span data-ttu-id="460d8-1345">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1345">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="460d8-1346">Botservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1346">Botservice</span></span>
* <span data-ttu-id="460d8-1347">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1347">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="460d8-1348">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="460d8-1348">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="460d8-1349">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="460d8-1349">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="460d8-1350">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="460d8-1350">Reduced Kudu network calls</span></span>
* <span data-ttu-id="460d8-1351">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1351">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-1352">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-1352">Consumption</span></span>
* <span data-ttu-id="460d8-1353">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1353">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-1354">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-1354">CosmosDB</span></span>
* <span data-ttu-id="460d8-1355">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1355">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="460d8-1356">지도</span><span class="sxs-lookup"><span data-stu-id="460d8-1356">Maps</span></span>
* <span data-ttu-id="460d8-1357">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1357">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1358">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1358">Network</span></span>
* <span data-ttu-id="460d8-1359">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1359">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="460d8-1360">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="460d8-1360">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1361">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1361">Resource</span></span>
* <span data-ttu-id="460d8-1362">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1362">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="460d8-1363">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1363">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1364">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1364">Storage</span></span>
*  <span data-ttu-id="460d8-1365">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1365">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1366">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1366">VM</span></span>
* <span data-ttu-id="460d8-1367">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1367">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="460d8-1368">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="460d8-1368">December 4, 2018</span></span>

<span data-ttu-id="460d8-1369">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="460d8-1369">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="460d8-1370">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1370">Core</span></span>
* <span data-ttu-id="460d8-1371">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1371">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="460d8-1372">tsv 출력을 사용한 명령에서 파이핑된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1372">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1373">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1373">Appservice</span></span>
* <span data-ttu-id="460d8-1374">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1374">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="460d8-1375">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1375">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1376">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1376">Network</span></span>
* <span data-ttu-id="460d8-1377">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1377">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1378">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1378">Role</span></span>
* <span data-ttu-id="460d8-1379">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1379">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="460d8-1380">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1380">VM</span></span>
* <span data-ttu-id="460d8-1381">[사용 되지 않음]`vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1381">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="460d8-1382">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1382">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="460d8-1383">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1383">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="460d8-1384">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1384">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="460d8-1385">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="460d8-1385">November 20, 2018</span></span>

<span data-ttu-id="460d8-1386">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="460d8-1386">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="460d8-1387">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1387">Core</span></span>
* <span data-ttu-id="460d8-1388">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1388">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1389">ACR</span></span>
* <span data-ttu-id="460d8-1390">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1390">Added context token to task step</span></span>
* <span data-ttu-id="460d8-1391">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1391">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="460d8-1392">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1392">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1393">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-1393">Appservice</span></span>
* <span data-ttu-id="460d8-1394">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1394">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="460d8-1395">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1395">Updated the default `node_version`.</span></span> <span data-ttu-id="460d8-1396">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1396">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="460d8-1397">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1397">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="460d8-1398">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1398">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="460d8-1399">IotCentral</span><span class="sxs-lookup"><span data-stu-id="460d8-1399">IotCentral</span></span>
* <span data-ttu-id="460d8-1400">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1400">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-1401">KeyVault</span><span class="sxs-lookup"><span data-stu-id="460d8-1401">KeyVault</span></span>
* <span data-ttu-id="460d8-1402">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1402">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1403">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1403">Network</span></span>
* <span data-ttu-id="460d8-1404">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1404">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="460d8-1405">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="460d8-1405">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="460d8-1406">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1406">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="460d8-1407">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="460d8-1407">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1408">Rdbms</span><span class="sxs-lookup"><span data-stu-id="460d8-1408">Rdbms</span></span>
* <span data-ttu-id="460d8-1409">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1409">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="460d8-1410">Rbac</span><span class="sxs-lookup"><span data-stu-id="460d8-1410">Rbac</span></span>
* <span data-ttu-id="460d8-1411">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1411">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="460d8-1412">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1412">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="460d8-1413">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1413">Storage</span></span>
* <span data-ttu-id="460d8-1414">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1414">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="460d8-1415">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1415">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="460d8-1416">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1416">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="460d8-1417">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1417">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1418">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1418">VM</span></span>
* <span data-ttu-id="460d8-1419">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1419">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="460d8-1420">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1420">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="460d8-1421">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1421">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="460d8-1422">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1422">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="460d8-1423">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1423">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="460d8-1424">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1424">Added `snapshot wait` command</span></span>
* <span data-ttu-id="460d8-1425">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1425">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="460d8-1426">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="460d8-1426">November 6, 2018</span></span>

<span data-ttu-id="460d8-1427">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="460d8-1427">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1428">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1428">Core</span></span>
* <span data-ttu-id="460d8-1429">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1429">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1430">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1430">ACR</span></span>
* <span data-ttu-id="460d8-1431">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1431">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="460d8-1432">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1432">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1433">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1433">ACS</span></span>
* <span data-ttu-id="460d8-1434">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1434">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="460d8-1435">Advisor</span><span class="sxs-lookup"><span data-stu-id="460d8-1435">Advisor</span></span>
* <span data-ttu-id="460d8-1436">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1436">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-1437">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1437">AMS</span></span>
* <span data-ttu-id="460d8-1438">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="460d8-1438">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="460d8-1439">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="460d8-1439">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="460d8-1440">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1440">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="460d8-1441">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-1441">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="460d8-1442">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1442">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="460d8-1443">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1443">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="460d8-1444">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1444">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="460d8-1445">[호환성이 손상되는 변경]`ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1445">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="460d8-1446">[호환성이 손상되는 변경]`ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1446">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="460d8-1447">[호환성이 손상되는 변경]`ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1447">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="460d8-1448">[호환성이 손상되는 변경]`ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1448">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="460d8-1449">[호환성이 손상되는 변경]`ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1449">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="460d8-1450">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="460d8-1450">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="460d8-1451">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="460d8-1451">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="460d8-1452">[호환성이 손상되는 변경]`ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1452">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="460d8-1453">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1453">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="460d8-1454">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1454">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1455">AppService</span></span>
* <span data-ttu-id="460d8-1456">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1456">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="460d8-1457">구성</span><span class="sxs-lookup"><span data-stu-id="460d8-1457">Configure</span></span>
* <span data-ttu-id="460d8-1458">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1458">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1459">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1459">Container</span></span>
* <span data-ttu-id="460d8-1460">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1460">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="460d8-1461">EventHub</span><span class="sxs-lookup"><span data-stu-id="460d8-1461">EventHub</span></span>
* <span data-ttu-id="460d8-1462">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1462">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-1463">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-1463">Interactive</span></span>
* <span data-ttu-id="460d8-1464">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1464">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1465">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1465">Monitor</span></span>
* <span data-ttu-id="460d8-1466">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1466">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1467">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1467">Network</span></span>
* <span data-ttu-id="460d8-1468">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1468">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="460d8-1469">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1469">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="460d8-1470">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1470">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="460d8-1471">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-1471">Profile</span></span>
* <span data-ttu-id="460d8-1472">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1472">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1473">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1473">RDBMS</span></span>
* <span data-ttu-id="460d8-1474">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1474">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1475">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1475">Resource</span></span>
* <span data-ttu-id="460d8-1476">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1476">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1477">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1477">Role</span></span>
* <span data-ttu-id="460d8-1478">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1478">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="460d8-1479">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-1479">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="460d8-1480">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1480">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1481">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1481">Storage</span></span>
* <span data-ttu-id="460d8-1482">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1482">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1483">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1483">VM</span></span>
* <span data-ttu-id="460d8-1484">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1484">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="460d8-1485">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1485">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="460d8-1486">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1486">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="460d8-1487">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1487">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="460d8-1488">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="460d8-1488">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="460d8-1489">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1489">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="460d8-1490">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="460d8-1490">October 23, 2018</span></span>

<span data-ttu-id="460d8-1491">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="460d8-1491">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1492">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1492">Core</span></span>
* <span data-ttu-id="460d8-1493">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1493">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="460d8-1494">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1494">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1495">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1495">ACR</span></span>
* <span data-ttu-id="460d8-1496">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1496">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-1497">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-1497">CDN</span></span>
* <span data-ttu-id="460d8-1498">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1498">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="460d8-1499">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1499">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1500">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1500">Container</span></span>
* <span data-ttu-id="460d8-1501">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1501">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="460d8-1502">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1502">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="460d8-1503">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1503">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="460d8-1504">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1504">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="460d8-1505">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1505">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="460d8-1506">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1506">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="460d8-1507">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1507">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-1508">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-1508">CosmosDB</span></span>
* <span data-ttu-id="460d8-1509">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1509">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-1510">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-1510">Interactive</span></span>
* <span data-ttu-id="460d8-1511">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1511">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="460d8-1512">IoT Central</span><span class="sxs-lookup"><span data-stu-id="460d8-1512">IoT Central</span></span>
* <span data-ttu-id="460d8-1513">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1513">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="460d8-1514">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1514">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1515">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1515">Monitor</span></span>
* <span data-ttu-id="460d8-1516">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="460d8-1516">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="460d8-1517">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1517">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="460d8-1518">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1518">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="460d8-1519">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1519">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="460d8-1520">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1520">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="460d8-1521">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1521">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="460d8-1522">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="460d8-1522">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="460d8-1523">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1523">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="460d8-1524">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1524">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="460d8-1525">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1525">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1526">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1526">Network</span></span>
* <span data-ttu-id="460d8-1527">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1527">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="460d8-1528">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1528">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="460d8-1529">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="460d8-1529">ServiceBus</span></span>
* <span data-ttu-id="460d8-1530">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1530">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1531">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1531">SQL</span></span>
* <span data-ttu-id="460d8-1532">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1532">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1533">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1533">Storage</span></span>
* <span data-ttu-id="460d8-1534">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1534">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="460d8-1535">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1535">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1536">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1536">VM</span></span>
* <span data-ttu-id="460d8-1537">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1537">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="460d8-1538">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1538">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="460d8-1539">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1539">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="460d8-1540">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="460d8-1540">October 16, 2018</span></span>

<span data-ttu-id="460d8-1541">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="460d8-1541">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1542">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1542">VM</span></span>
* <span data-ttu-id="460d8-1543">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1543">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="460d8-1544">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="460d8-1544">October 9, 2018</span></span>

<span data-ttu-id="460d8-1545">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="460d8-1545">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1546">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1546">Core</span></span>
* <span data-ttu-id="460d8-1547">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1547">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1548">ACR</span></span>
* <span data-ttu-id="460d8-1549">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1549">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1550">ACS</span></span>
* <span data-ttu-id="460d8-1551">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="460d8-1551">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="460d8-1552">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1552">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="460d8-1553">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1553">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="460d8-1554">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1554">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1555">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1555">Container</span></span>
* <span data-ttu-id="460d8-1556">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1556">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="460d8-1557">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1557">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="460d8-1558">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="460d8-1558">Event Hub</span></span>
* <span data-ttu-id="460d8-1559">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1559">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="460d8-1560">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1560">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="460d8-1561">확장</span><span class="sxs-lookup"><span data-stu-id="460d8-1561">Extensions</span></span>
* <span data-ttu-id="460d8-1562">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1562">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="460d8-1563">HDInsight</span><span class="sxs-lookup"><span data-stu-id="460d8-1563">HDInsight</span></span>
* <span data-ttu-id="460d8-1564">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1564">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-1565">IoT</span></span>
* <span data-ttu-id="460d8-1566">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1566">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-1567">KeyVault</span><span class="sxs-lookup"><span data-stu-id="460d8-1567">KeyVault</span></span>
* <span data-ttu-id="460d8-1568">최신 API 프로필에 keyvault 스토리지 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1568">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1569">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1569">Network</span></span>
* <span data-ttu-id="460d8-1570">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1570">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="460d8-1571">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="460d8-1571">See #6052</span></span>
* <span data-ttu-id="460d8-1572">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="460d8-1572">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="460d8-1573">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1573">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="460d8-1574">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1574">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="460d8-1575">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1575">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="460d8-1576">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1576">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="460d8-1577">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1577">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1578">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1578">Role</span></span>
* <span data-ttu-id="460d8-1579">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1579">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="460d8-1580">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1580">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="460d8-1581">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1581">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="460d8-1582">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1582">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="460d8-1583">Service Bus</span><span class="sxs-lookup"><span data-stu-id="460d8-1583">Service Bus</span></span>
* <span data-ttu-id="460d8-1584">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1585">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1585">VM</span></span>
* <span data-ttu-id="460d8-1586">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1586">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="460d8-1587">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1587">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="460d8-1588">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1588">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="460d8-1589">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1589">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="460d8-1590">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1590">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="460d8-1591">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1591">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="460d8-1592">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="460d8-1592">September 21, 2018</span></span>

<span data-ttu-id="460d8-1593">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="460d8-1593">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1594">ACR</span></span>
* <span data-ttu-id="460d8-1595">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1595">Added ACR Task commands</span></span>
* <span data-ttu-id="460d8-1596">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1596">Added quick run command</span></span>
* <span data-ttu-id="460d8-1597">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1597">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="460d8-1598">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1598">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="460d8-1599">관리되는 레지스트리의 멱등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1599">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="460d8-1600">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1600">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1601">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1601">ACS</span></span>
* <span data-ttu-id="460d8-1602">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1602">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="460d8-1603">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1603">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1604">AppService</span></span>

* <span data-ttu-id="460d8-1605">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1605">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="460d8-1606">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1606">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="460d8-1607">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1607">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="460d8-1608">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1608">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1609">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1609">Batch</span></span>
* <span data-ttu-id="460d8-1610">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1610">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="460d8-1611">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1611">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="460d8-1612">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1612">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="460d8-1613">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1613">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="460d8-1614">Batch AI</span><span class="sxs-lookup"><span data-stu-id="460d8-1614">Batch AI</span></span> 
* <span data-ttu-id="460d8-1615">`batchai cluster create` 명령에서 자동 스토리지 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1615">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="460d8-1616">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="460d8-1616">Cognitive Services</span></span>
* <span data-ttu-id="460d8-1617">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1617">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="460d8-1618">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1618">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="460d8-1619">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1619">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="460d8-1620">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1620">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="460d8-1621">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1621">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="460d8-1622">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1622">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1623">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1623">Container</span></span>
* <span data-ttu-id="460d8-1624">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1624">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="460d8-1625">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1625">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="460d8-1626">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1626">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="460d8-1627">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1627">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="460d8-1628">Datalake</span><span class="sxs-lookup"><span data-stu-id="460d8-1628">Datalake</span></span>
* <span data-ttu-id="460d8-1629">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1629">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="460d8-1630">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="460d8-1630">Interactive Shell</span></span>
* <span data-ttu-id="460d8-1631">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1631">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="460d8-1632">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1632">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-1633">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-1633">IoT</span></span>
* <span data-ttu-id="460d8-1634">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1634">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-1635">Key Vault</span><span class="sxs-lookup"><span data-stu-id="460d8-1635">Key Vault</span></span>
* <span data-ttu-id="460d8-1636">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1636">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1637">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1637">Network</span></span>
* <span data-ttu-id="460d8-1638">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1638">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="460d8-1639">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1639">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="460d8-1640">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1640">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="460d8-1641">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1641">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="460d8-1642">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1642">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="460d8-1643">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1643">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="460d8-1644">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-1644">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="460d8-1645">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1645">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="460d8-1646">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1646">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="460d8-1647">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1647">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="460d8-1648">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1648">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="460d8-1649">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1649">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="460d8-1650">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1650">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="460d8-1651">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-1651">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="460d8-1652">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1652">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="460d8-1653">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1653">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="460d8-1654">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1654">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="460d8-1655">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1655">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1656">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-1656">RDBMS</span></span>
* <span data-ttu-id="460d8-1657">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1657">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="460d8-1658">예약</span><span class="sxs-lookup"><span data-stu-id="460d8-1658">Reservation</span></span>
* <span data-ttu-id="460d8-1659">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1659">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="460d8-1660">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1660">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="460d8-1661">앱 관리</span><span class="sxs-lookup"><span data-stu-id="460d8-1661">Manage App</span></span>
* <span data-ttu-id="460d8-1662">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1662">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="460d8-1663">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1663">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1664">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1664">Role</span></span>
* <span data-ttu-id="460d8-1665">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1665">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="460d8-1666">SignalR</span><span class="sxs-lookup"><span data-stu-id="460d8-1666">SignalR</span></span>
* <span data-ttu-id="460d8-1667">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1667">First release</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1668">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1668">Storage</span></span>
* <span data-ttu-id="460d8-1669">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1669">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="460d8-1670">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1670">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1671">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1671">VM</span></span>
* <span data-ttu-id="460d8-1672">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="460d8-1672">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="460d8-1673">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1673">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="460d8-1674">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="460d8-1674">August 28, 2018</span></span>

<span data-ttu-id="460d8-1675">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="460d8-1675">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1676">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1676">Core</span></span>

* <span data-ttu-id="460d8-1677">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1677">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="460d8-1678">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1678">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1679">ACR</span></span>

* <span data-ttu-id="460d8-1680">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1680">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="460d8-1681">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1681">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1682">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1682">ACS</span></span>

* <span data-ttu-id="460d8-1683">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1683">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="460d8-1684">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1684">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1685">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1685">AppService</span></span>

* <span data-ttu-id="460d8-1686">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1686">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="460d8-1687">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1687">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="460d8-1688">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1688">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-1689">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-1689">Backup</span></span>

* <span data-ttu-id="460d8-1690">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1690">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="460d8-1691">Bot Service</span><span class="sxs-lookup"><span data-stu-id="460d8-1691">Bot Service</span></span>

* <span data-ttu-id="460d8-1692">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1692">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="460d8-1693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="460d8-1693">Cognitive Services</span></span>

* <span data-ttu-id="460d8-1694">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1694">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-1695">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-1695">IoT</span></span>

* <span data-ttu-id="460d8-1696">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1696">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-1697">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-1697">Monitor</span></span>

* <span data-ttu-id="460d8-1698">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1698">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="460d8-1699">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="460d8-1699">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1700">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1700">Network</span></span>

* <span data-ttu-id="460d8-1701">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1701">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1702">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1702">Resource</span></span>

* <span data-ttu-id="460d8-1703">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1703">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1704">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1704">Storage</span></span>

* <span data-ttu-id="460d8-1705">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1705">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1706">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1706">VM</span></span>

* <span data-ttu-id="460d8-1707">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1707">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="460d8-1708">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="460d8-1708">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="460d8-1709">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="460d8-1709">Auguest 14, 2018</span></span>

<span data-ttu-id="460d8-1710">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="460d8-1710">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1711">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1711">Core</span></span>

* <span data-ttu-id="460d8-1712">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1712">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="460d8-1713">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="460d8-1713">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="460d8-1714">원격 분석</span><span class="sxs-lookup"><span data-stu-id="460d8-1714">Telemetry</span></span>

* <span data-ttu-id="460d8-1715">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="460d8-1715">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1716">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1716">ACR</span></span>

* <span data-ttu-id="460d8-1717">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1717">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="460d8-1718">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1718">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1719">ACS</span></span>

* <span data-ttu-id="460d8-1720">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1720">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="460d8-1721">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1721">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="460d8-1722">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1722">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="460d8-1723">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1723">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="460d8-1724">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1724">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="460d8-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1725">AppService</span></span>

* <span data-ttu-id="460d8-1726">외부 리소스 그룹에 스토리지 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1726">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="460d8-1727">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1727">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-1728">BatchAI</span><span class="sxs-lookup"><span data-stu-id="460d8-1728">BatchAI</span></span>

* <span data-ttu-id="460d8-1729">자동 스토리지 계정 만들기가 &quot;리소스 *그룹*&quot;을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1729">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="460d8-1730">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1730">Container</span></span>

* <span data-ttu-id="460d8-1731">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1731">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="460d8-1732">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-1732">IoT</span></span>

* <span data-ttu-id="460d8-1733">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="460d8-1733">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="460d8-1734">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1734">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="460d8-1735">Iot Central</span><span class="sxs-lookup"><span data-stu-id="460d8-1735">Iot Central</span></span>

* <span data-ttu-id="460d8-1736">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1736">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-1737">KeyVault</span><span class="sxs-lookup"><span data-stu-id="460d8-1737">KeyVault</span></span>


* <span data-ttu-id="460d8-1738">스토리지 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1738">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="460d8-1739">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1739">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="460d8-1740">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1740">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="460d8-1741">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1741">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="460d8-1742">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1742">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="460d8-1743">릴레이</span><span class="sxs-lookup"><span data-stu-id="460d8-1743">Relay</span></span>

* <span data-ttu-id="460d8-1744">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1744">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1745">Sql</span><span class="sxs-lookup"><span data-stu-id="460d8-1745">Sql</span></span>

* <span data-ttu-id="460d8-1746">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1746">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1747">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1747">Storage</span></span>

* <span data-ttu-id="460d8-1748">[호환성이 손상되는 변경]`--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1748">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="460d8-1749">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1749">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="460d8-1750">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1750">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="460d8-1751">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="460d8-1751">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="460d8-1752">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1752">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1753">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1753">VM</span></span>

* <span data-ttu-id="460d8-1754">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1754">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="460d8-1755">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="460d8-1755">July 31, 2018</span></span>

<span data-ttu-id="460d8-1756">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="460d8-1756">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1757">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1757">ACR</span></span>

* <span data-ttu-id="460d8-1758">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1758">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="460d8-1759">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1759">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1760">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1760">ACS</span></span>

* <span data-ttu-id="460d8-1761">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1761">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1762">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1762">Batch</span></span>

* <span data-ttu-id="460d8-1763">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1763">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1764">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1764">Container</span></span>

* <span data-ttu-id="460d8-1765">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1765">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1766">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1766">Network</span></span>

* <span data-ttu-id="460d8-1767">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1767">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="460d8-1768">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1768">Resource</span></span>

* <span data-ttu-id="460d8-1769">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="460d8-1769">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="460d8-1770">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1770">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1771">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1771">Role</span></span>

* <span data-ttu-id="460d8-1772">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1772">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="460d8-1773">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1773">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="460d8-1774">검색</span><span class="sxs-lookup"><span data-stu-id="460d8-1774">Search</span></span>

* <span data-ttu-id="460d8-1775">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1775">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="460d8-1776">Service Bus</span><span class="sxs-lookup"><span data-stu-id="460d8-1776">Service Bus</span></span>

* <span data-ttu-id="460d8-1777">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1777">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="460d8-1778">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1778">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="460d8-1779">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="460d8-1779">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="460d8-1780">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="460d8-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1781">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1781">Storage</span></span>

* <span data-ttu-id="460d8-1782">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1782">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="460d8-1783">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="460d8-1783">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1784">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1784">VM</span></span>

* <span data-ttu-id="460d8-1785">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1785">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="460d8-1786">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1786">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="460d8-1787">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1787">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="460d8-1788">[호환성이 손상되는 변경]`[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1788">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="460d8-1789">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="460d8-1789">July 18, 2018</span></span>

<span data-ttu-id="460d8-1790">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="460d8-1790">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1791">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1791">Core</span></span>

* <span data-ttu-id="460d8-1792">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1792">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="460d8-1793">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1793">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="460d8-1794">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1794">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1795">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1795">ACR</span></span>

* <span data-ttu-id="460d8-1796">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1796">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="460d8-1797">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1797">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="460d8-1798">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1798">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="460d8-1799">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1799">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1800">ACS</span></span>

* <span data-ttu-id="460d8-1801">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1801">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1802">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1802">AppService</span></span>

* <span data-ttu-id="460d8-1803">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1803">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1804">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1804">Batch</span></span>

* <span data-ttu-id="460d8-1805">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1805">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="460d8-1806">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1806">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="460d8-1807">Batch AI</span><span class="sxs-lookup"><span data-stu-id="460d8-1807">Batch AI</span></span>

* <span data-ttu-id="460d8-1808">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1808">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1809">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1809">Container</span></span>

* <span data-ttu-id="460d8-1810">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1810">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="460d8-1811">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1811">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1812">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1812">Network</span></span>

* <span data-ttu-id="460d8-1813">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1813">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="460d8-1814">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1814">Added `network nic wait`</span></span>
* <span data-ttu-id="460d8-1815">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1815">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="460d8-1816">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1816">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="460d8-1817">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1817">Resource</span></span>

* <span data-ttu-id="460d8-1818">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1818">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="460d8-1819">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1819">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="460d8-1820">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1820">Added `deployment wait` command</span></span>
* <span data-ttu-id="460d8-1821">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1821">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1822">SQL</span></span>

* <span data-ttu-id="460d8-1823">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1823">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="460d8-1824">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-1824">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="460d8-1825">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="460d8-1825">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1826">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1826">Storage</span></span>

* <span data-ttu-id="460d8-1827">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1827">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1828">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1828">VM</span></span>

* <span data-ttu-id="460d8-1829">[호환성이 손상되는 변경]`vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1829">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="460d8-1830">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1830">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="460d8-1831">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1831">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="460d8-1832">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="460d8-1832">July 3, 2018</span></span>

<span data-ttu-id="460d8-1833">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="460d8-1833">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-1834">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-1834">AKS</span></span>

* <span data-ttu-id="460d8-1835">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1835">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="460d8-1836">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="460d8-1836">July 3, 2018</span></span>

<span data-ttu-id="460d8-1837">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="460d8-1837">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1838">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1838">Core</span></span>

* <span data-ttu-id="460d8-1839">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1839">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1840">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1840">ACR</span></span>

* <span data-ttu-id="460d8-1841">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1841">Added polling build status</span></span>
* <span data-ttu-id="460d8-1842">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1842">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="460d8-1843">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1843">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1844">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1844">ACS</span></span>

* <span data-ttu-id="460d8-1845">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1845">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="460d8-1846">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-1846">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="460d8-1847">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-1847">Updated options for `aks browse` command.</span></span> <span data-ttu-id="460d8-1848">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1848">Added `--listen-port` support</span></span>
* <span data-ttu-id="460d8-1849">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1849">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="460d8-1850">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-1850">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="460d8-1851">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1851">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1852">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1852">AppService</span></span>

* <span data-ttu-id="460d8-1853">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1853">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="460d8-1854">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1854">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-1855">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-1855">Backup</span></span>

* <span data-ttu-id="460d8-1856">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1856">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-1857">BatchAI</span><span class="sxs-lookup"><span data-stu-id="460d8-1857">BatchAI</span></span>

* <span data-ttu-id="460d8-1858">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1858">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="460d8-1859">클라우드</span><span class="sxs-lookup"><span data-stu-id="460d8-1859">Cloud</span></span>

* <span data-ttu-id="460d8-1860">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1860">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="460d8-1861">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-1861">Container</span></span>

* <span data-ttu-id="460d8-1862">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1862">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="460d8-1863">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1863">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="460d8-1864">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1864">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-1865">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-1865">Extension</span></span>

* <span data-ttu-id="460d8-1866">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1866">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1867">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1867">Network</span></span>

* <span data-ttu-id="460d8-1868">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="460d8-1868">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-1869">Rdbms</span><span class="sxs-lookup"><span data-stu-id="460d8-1869">Rdbms</span></span>

* <span data-ttu-id="460d8-1870">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1870">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-1871">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-1871">Resource</span></span>

* <span data-ttu-id="460d8-1872">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1872">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1873">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1873">VM</span></span>

* <span data-ttu-id="460d8-1874">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1874">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="460d8-1875">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="460d8-1875">June 25, 2018</span></span>

<span data-ttu-id="460d8-1876">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="460d8-1876">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="460d8-1877">CLI</span><span class="sxs-lookup"><span data-stu-id="460d8-1877">CLI</span></span>

* <span data-ttu-id="460d8-1878">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-1878">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="460d8-1879">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="460d8-1879">June 19, 2018</span></span>

<span data-ttu-id="460d8-1880">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="460d8-1880">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1881">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1881">Core</span></span>

* <span data-ttu-id="460d8-1882">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1882">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1883">ACR</span></span>

* <span data-ttu-id="460d8-1884">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1884">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="460d8-1885">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1885">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1886">ACS</span></span>

* <span data-ttu-id="460d8-1887">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-1887">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="460d8-1888">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1888">Added `--update` support</span></span>
* <span data-ttu-id="460d8-1889">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1889">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="460d8-1890">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="460d8-1890">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="460d8-1891">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1891">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="460d8-1892">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-1892">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="460d8-1893">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1893">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="460d8-1894">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1894">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1895">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1895">AppService</span></span>

* <span data-ttu-id="460d8-1896">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1896">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="460d8-1897">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1897">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1898">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1898">Batch</span></span>

* <span data-ttu-id="460d8-1899">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1899">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="460d8-1900">Batch AI</span><span class="sxs-lookup"><span data-stu-id="460d8-1900">Batch AI</span></span>

* <span data-ttu-id="460d8-1901">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="460d8-1901">Added support for workspaces.</span></span> <span data-ttu-id="460d8-1902">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1902">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="460d8-1903">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="460d8-1903">Added support for experiments.</span></span> <span data-ttu-id="460d8-1904">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1904">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="460d8-1905">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1905">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="460d8-1906">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-1906">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="460d8-1907">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1907">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="460d8-1908">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1908">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="460d8-1909">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="460d8-1909">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="460d8-1910">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="460d8-1910">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="460d8-1911">[호환성이 손상되는 변경]`cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-1911">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="460d8-1912">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="460d8-1912">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="460d8-1913">[호환성이 손상되는 변경]`job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-1913">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="460d8-1914">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="460d8-1914">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="460d8-1915">[호환성이 손상되는 변경]`location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="460d8-1915">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="460d8-1916">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-1916">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="460d8-1917">[호환성이 손상되는 변경]`job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1917">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="460d8-1918">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="460d8-1918">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="460d8-1919">[`--config`, `-c`]을 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="460d8-1919">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="460d8-1920">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="460d8-1920">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="460d8-1921">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="460d8-1921">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="460d8-1922">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="460d8-1922">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="460d8-1923">지도</span><span class="sxs-lookup"><span data-stu-id="460d8-1923">Maps</span></span>

* <span data-ttu-id="460d8-1924">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1924">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1925">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1925">Network</span></span>

* <span data-ttu-id="460d8-1926">`network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 `https` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1926">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="460d8-1927">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1927">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="460d8-1928">#6502</span><span class="sxs-lookup"><span data-stu-id="460d8-1928">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="460d8-1929">예약</span><span class="sxs-lookup"><span data-stu-id="460d8-1929">Reservations</span></span>

* <span data-ttu-id="460d8-1930">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1930">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="460d8-1931">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1931">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="460d8-1932">[호환성이 손상되는 변경]`ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1932">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="460d8-1933">[호환성이 손상되는 변경]`Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1933">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="460d8-1934">[호환성이 손상되는 변경]`Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-1934">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="460d8-1935">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1935">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="460d8-1936">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-1936">Role</span></span>

* <span data-ttu-id="460d8-1937">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-1937">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1938">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1938">SQL</span></span>

* <span data-ttu-id="460d8-1939">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-1939">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-1940">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1940">Storage</span></span>

* <span data-ttu-id="460d8-1941">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1941">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1942">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1942">VM</span></span>

* <span data-ttu-id="460d8-1943">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-1943">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="460d8-1944">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1944">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="460d8-1945">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1945">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="460d8-1946">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-1946">June 13, 2018</span></span>

<span data-ttu-id="460d8-1947">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="460d8-1947">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1948">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1948">Core</span></span>

* <span data-ttu-id="460d8-1949">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="460d8-1949">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="460d8-1950">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-1950">June 13, 2018</span></span>

<span data-ttu-id="460d8-1951">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="460d8-1951">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-1952">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-1952">AKS</span></span>

* <span data-ttu-id="460d8-1953">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1953">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="460d8-1954">인수를 `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="460d8-1954">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="460d8-1955">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1955">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="460d8-1956">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1956">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="460d8-1957">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1957">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-1958">AppService</span></span>

* <span data-ttu-id="460d8-1959">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1959">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="460d8-1960">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="460d8-1960">June 5, 2018</span></span>

<span data-ttu-id="460d8-1961">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="460d8-1961">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-1962">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-1962">Interactive</span></span>

* <span data-ttu-id="460d8-1963">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1963">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="460d8-1964">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="460d8-1964">June 5, 2018</span></span>

<span data-ttu-id="460d8-1965">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="460d8-1965">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1966">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1966">Core</span></span>

* <span data-ttu-id="460d8-1967">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1967">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="460d8-1968">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1968">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-1969">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-1969">ACR</span></span>

* <span data-ttu-id="460d8-1970">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1970">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="460d8-1971">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1971">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="460d8-1972">AKS</span><span class="sxs-lookup"><span data-stu-id="460d8-1972">AKS</span></span>

* <span data-ttu-id="460d8-1973">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-1973">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-1974">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-1974">Batch</span></span>

* <span data-ttu-id="460d8-1975">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="460d8-1975">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-1976">IOT</span><span class="sxs-lookup"><span data-stu-id="460d8-1976">IOT</span></span>

* <span data-ttu-id="460d8-1977">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1977">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="460d8-1978">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-1978">Network</span></span>

* <span data-ttu-id="460d8-1979">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="460d8-1979">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="460d8-1980">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="460d8-1980">Policy Insights</span></span>

* <span data-ttu-id="460d8-1981">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-1981">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="460d8-1982">ARM</span><span class="sxs-lookup"><span data-stu-id="460d8-1982">ARM</span></span>

* <span data-ttu-id="460d8-1983">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1983">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-1984">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-1984">SQL</span></span>

* <span data-ttu-id="460d8-1985">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="460d8-1985">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="460d8-1986">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1986">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="460d8-1987">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-1987">Storage</span></span>

* <span data-ttu-id="460d8-1988">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="460d8-1988">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-1989">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-1989">VM</span></span>

* <span data-ttu-id="460d8-1990">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-1990">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="460d8-1991">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1991">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="460d8-1992">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1992">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="460d8-1993">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="460d8-1993">May 22, 2018</span></span>

<span data-ttu-id="460d8-1994">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="460d8-1994">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="460d8-1995">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-1995">Core</span></span>

* <span data-ttu-id="460d8-1996">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-1996">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-1997">ACS</span></span>

* <span data-ttu-id="460d8-1998">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-1998">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="460d8-1999">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-1999">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-2000">AppService</span></span>

* <span data-ttu-id="460d8-2001">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2001">Improved generic update commands</span></span>
* <span data-ttu-id="460d8-2002">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2002">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2003">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2003">Container</span></span>

* <span data-ttu-id="460d8-2004">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2004">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="460d8-2005">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2005">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2006">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2006">Extension</span></span>

* <span data-ttu-id="460d8-2007">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2007">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2008">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2008">Interactive</span></span>

* <span data-ttu-id="460d8-2009">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2009">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="460d8-2010">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2010">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-2011">KeyVault</span><span class="sxs-lookup"><span data-stu-id="460d8-2011">KeyVault</span></span>

* <span data-ttu-id="460d8-2012">클라우드 셸 또는 id를 가진 VM에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="460d8-2012">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2013">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2013">Network</span></span>

* <span data-ttu-id="460d8-2014">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2014">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="460d8-2015">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2015">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2016">SQL</span></span>

* <span data-ttu-id="460d8-2017">[호환성이 손상되는 변경]`db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="460d8-2017">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="460d8-2018">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="460d8-2018">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="460d8-2019">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-2019">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="460d8-2020">`maxSizeBytes` 속성을 문자열 대신 정수 값으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2020">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="460d8-2021">[호환성이 손상되는 변경]`db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2021">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="460d8-2022">`requestedServiceObjectiveName`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2022">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="460d8-2023">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-2023">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="460d8-2024">`edition`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2024">`edition`.</span></span> <span data-ttu-id="460d8-2025">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-2025">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="460d8-2026">`elasticPoolName`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2026">`elasticPoolName`.</span></span> <span data-ttu-id="460d8-2027">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-2027">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="460d8-2028">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2028">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="460d8-2029">`edition`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2029">`edition`.</span></span> <span data-ttu-id="460d8-2030">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-2030">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="460d8-2031">`dtu`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2031">`dtu`.</span></span> <span data-ttu-id="460d8-2032">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-2032">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="460d8-2033">`databaseDtuMin`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2033">`databaseDtuMin`.</span></span> <span data-ttu-id="460d8-2034">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-2034">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="460d8-2035">`databaseDtuMax`입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2035">`databaseDtuMax`.</span></span> <span data-ttu-id="460d8-2036">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-2036">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="460d8-2037">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2037">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="460d8-2038">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2038">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2039">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2039">Storage</span></span>

* <span data-ttu-id="460d8-2040">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2040">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="460d8-2041">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2041">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2042">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2042">VM</span></span>

* <span data-ttu-id="460d8-2043">[호환성이 손상되는 변경]`vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="460d8-2043">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="460d8-2044">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-2044">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="460d8-2045">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2045">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="460d8-2046">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2046">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="460d8-2047">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2047">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="460d8-2048">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="460d8-2048">May 7, 2018</span></span>

<span data-ttu-id="460d8-2049">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="460d8-2049">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2050">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2050">Core</span></span>

* <span data-ttu-id="460d8-2051">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2051">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="460d8-2052">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2052">Added limited support for positional arguments</span></span>
* <span data-ttu-id="460d8-2053">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2053">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="460d8-2054">#5591</span><span class="sxs-lookup"><span data-stu-id="460d8-2054">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="460d8-2055">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2055">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="460d8-2056">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2056">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="460d8-2057">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2057">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="460d8-2058">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2058">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="460d8-2059">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2059">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2060">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2060">ACR</span></span>

* <span data-ttu-id="460d8-2061">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2061">Added ACR Build commands</span></span>
* <span data-ttu-id="460d8-2062">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2062">Improved resource not found error messages</span></span>
* <span data-ttu-id="460d8-2063">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2063">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="460d8-2064">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2064">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="460d8-2065">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2065">Improved repository commands error messages</span></span>
* <span data-ttu-id="460d8-2066">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-2066">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2067">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2067">ACS</span></span>

* <span data-ttu-id="460d8-2068">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2068">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="460d8-2069">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2069">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="460d8-2070">AMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2070">AMS</span></span>

* <span data-ttu-id="460d8-2071">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="460d8-2071">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2072">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2072">Appservice</span></span>

* <span data-ttu-id="460d8-2073">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2073">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="460d8-2074">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2074">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="460d8-2075">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2075">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="460d8-2076">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2076">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="460d8-2077">Batch AI</span><span class="sxs-lookup"><span data-stu-id="460d8-2077">Batch AI</span></span>

* <span data-ttu-id="460d8-2078">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2078">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="460d8-2079">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="460d8-2079">Cognitive Services</span></span>

* <span data-ttu-id="460d8-2080">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2080">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-2081">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-2081">Consumption</span></span>

* <span data-ttu-id="460d8-2082">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2082">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2083">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2083">Container</span></span>

* <span data-ttu-id="460d8-2084">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2084">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="460d8-2085">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="460d8-2085">Cosmos DB</span></span>

* <span data-ttu-id="460d8-2086">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="460d8-2086">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="460d8-2087">DMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2087">DMS</span></span>

* <span data-ttu-id="460d8-2088">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2088">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2089">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2089">Extension</span></span>

* <span data-ttu-id="460d8-2090">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2090">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2091">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2091">Interactive</span></span>

* <span data-ttu-id="460d8-2092">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2092">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="460d8-2093">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="460d8-2093">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="460d8-2094">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2094">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="460d8-2095">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2095">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="460d8-2096">랩</span><span class="sxs-lookup"><span data-stu-id="460d8-2096">Lab</span></span>

* <span data-ttu-id="460d8-2097">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2097">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2098">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2098">Network</span></span>

* <span data-ttu-id="460d8-2099">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2099">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="460d8-2100">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2100">Profile</span></span>

* <span data-ttu-id="460d8-2101">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2101">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="460d8-2102">[호환성이 손상되는 변경]`--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2102">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="460d8-2103">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2103">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="460d8-2104">Redis</span><span class="sxs-lookup"><span data-stu-id="460d8-2104">Redis</span></span>

* <span data-ttu-id="460d8-2105">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2105">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="460d8-2106">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2106">Deprecated `redis list-all`.</span></span> <span data-ttu-id="460d8-2107">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2107">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="460d8-2108">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2108">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="460d8-2109">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2109">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="460d8-2110">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2110">Role</span></span>

* <span data-ttu-id="460d8-2111">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2111">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2112">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2112">Storage</span></span>

* <span data-ttu-id="460d8-2113">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2113">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="460d8-2114">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-2114">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="460d8-2115">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="460d8-2115">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="460d8-2116">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2116">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="460d8-2117">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2117">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2118">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2118">VM</span></span>

* <span data-ttu-id="460d8-2119">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2119">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="460d8-2120">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2120">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="460d8-2121">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="460d8-2121">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="460d8-2122">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2122">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="460d8-2123">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2123">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="460d8-2124">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2124">Added write accelerator support</span></span>
* <span data-ttu-id="460d8-2125">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2125">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="460d8-2126">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2126">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="460d8-2127">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2127">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="460d8-2128">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="460d8-2128">April 10, 2018</span></span>

<span data-ttu-id="460d8-2129">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="460d8-2129">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2130">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2130">ACR</span></span>

* <span data-ttu-id="460d8-2131">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="460d8-2131">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2132">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2132">ACS</span></span>

* <span data-ttu-id="460d8-2133">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2133">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2134">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2134">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="460d8-2136">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2136">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-2137">BatchAI</span><span class="sxs-lookup"><span data-stu-id="460d8-2137">BatchAI</span></span>

* <span data-ttu-id="460d8-2138">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2138">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="460d8-2139">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="460d8-2139">Job level mounting</span></span>
  - <span data-ttu-id="460d8-2140">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="460d8-2140">Environment variables with secret values</span></span>
  - <span data-ttu-id="460d8-2141">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-2141">Performance counters settings</span></span>
  - <span data-ttu-id="460d8-2142">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="460d8-2142">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="460d8-2143">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2143">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="460d8-2144">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="460d8-2144">Usage and limits reporting</span></span>
  - <span data-ttu-id="460d8-2145">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2145">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="460d8-2146">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2146">Support for custom images</span></span>
  - <span data-ttu-id="460d8-2147">pyTorch 도구 키트 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2147">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="460d8-2148">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2148">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="460d8-2149">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2149">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="460d8-2150">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2150">National clouds are supported</span></span>
* <span data-ttu-id="460d8-2151">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2151">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="460d8-2152">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="460d8-2152">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="460d8-2153">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2153">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="460d8-2154">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2154">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="460d8-2155">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="460d8-2155">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="460d8-2156">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="460d8-2156">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="460d8-2157">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2157">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="460d8-2158">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2158">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="460d8-2159">이 옵션을 사용하면 보다 쉽게 스토리지 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2159">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="460d8-2160">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2160">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="460d8-2161">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2161">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="460d8-2162">[호환성이 손상되는 변경]`job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="460d8-2162">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="460d8-2163">[호환성이 손상되는 변경]`cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2163">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="460d8-2164">결제</span><span class="sxs-lookup"><span data-stu-id="460d8-2164">Billing</span></span>

* <span data-ttu-id="460d8-2165">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2165">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-2166">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-2166">Consumption</span></span>

* <span data-ttu-id="460d8-2167">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2167">Added `marketplace` commands</span></span>
* <span data-ttu-id="460d8-2168">[호환성이 손상되는 변경]`reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2168">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="460d8-2169">[호환성이 손상되는 변경]`reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2169">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="460d8-2170">[호환성이 손상되는 변경]`reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2170">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="460d8-2171">[호환성이 손상되는 변경]`reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2171">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="460d8-2172">[호환성이 손상되는 변경]`pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2172">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2173">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2173">Container</span></span>

* <span data-ttu-id="460d8-2174">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2174">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="460d8-2175">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="460d8-2175">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2176">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2176">Extension</span></span>

* <span data-ttu-id="460d8-2177">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2177">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2178">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2178">Interactive</span></span>

* <span data-ttu-id="460d8-2179">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2179">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="460d8-2180">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2180">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="460d8-2181">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2181">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2182">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2182">Network</span></span>

* <span data-ttu-id="460d8-2183">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2183">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="460d8-2184">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2184">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="460d8-2185">#4910</span><span class="sxs-lookup"><span data-stu-id="460d8-2185">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="460d8-2186">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2186">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="460d8-2187">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="460d8-2187">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="460d8-2188">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2188">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="460d8-2189">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2189">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="460d8-2190">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2190">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2191">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2191">Profile</span></span>

* <span data-ttu-id="460d8-2192">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2192">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="460d8-2193">[호환성이 손상되는 변경]`--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2193">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-2194">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2194">RDBMS</span></span>

* <span data-ttu-id="460d8-2195">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2195">Added `georestore` command</span></span>
* <span data-ttu-id="460d8-2196">`create` 명령에서 스토리지 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2196">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2197">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2197">Resource</span></span>

* <span data-ttu-id="460d8-2198">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2198">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="460d8-2199">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2199">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2200">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2200">SQL</span></span>

* <span data-ttu-id="460d8-2201">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2201">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2202">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2202">Storage</span></span>

* <span data-ttu-id="460d8-2203">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2203">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2204">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2204">VM</span></span>

* <span data-ttu-id="460d8-2205">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2205">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="460d8-2206">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2206">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="460d8-2208">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2208">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="460d8-2209">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2209">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="460d8-2210">#5718</span><span class="sxs-lookup"><span data-stu-id="460d8-2210">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="460d8-2211">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2211">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="460d8-2212">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="460d8-2212">March 27, 2018</span></span>

<span data-ttu-id="460d8-2213">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="460d8-2213">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2214">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2214">Core</span></span>

* <span data-ttu-id="460d8-2215">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="460d8-2215">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2216">ACS</span></span>

* <span data-ttu-id="460d8-2217">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2217">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2218">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2218">Appservice</span></span>

* <span data-ttu-id="460d8-2219">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2219">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="460d8-2220">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2220">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-2221">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-2221">Backup</span></span>

* <span data-ttu-id="460d8-2222">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2222">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="460d8-2223">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2223">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="460d8-2224">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2224">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="460d8-2225">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2225">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2226">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2226">Container</span></span>

* <span data-ttu-id="460d8-2227">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2227">Added `container exec` command.</span></span> <span data-ttu-id="460d8-2228">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2228">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="460d8-2229">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2229">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2230">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2230">Extension</span></span>

* <span data-ttu-id="460d8-2231">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2231">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="460d8-2232">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2232">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="460d8-2233">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2233">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2234">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2234">Interactive</span></span>

* <span data-ttu-id="460d8-2235">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="460d8-2235">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="460d8-2236">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2236">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="460d8-2237">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2237">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="460d8-2238">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2238">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="460d8-2239">랩</span><span class="sxs-lookup"><span data-stu-id="460d8-2239">Lab</span></span>

* <span data-ttu-id="460d8-2240">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2240">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2241">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2241">Monitor</span></span>

* <span data-ttu-id="460d8-2242">`metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 `--top`, `--orderby` 및 `--namespace`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2242">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="460d8-2243">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="460d8-2243">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="460d8-2244">`metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 `--namespace` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2244">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2245">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2245">Network</span></span>

* <span data-ttu-id="460d8-2246">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2246">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2247">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2247">Profile</span></span>

* <span data-ttu-id="460d8-2248">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2248">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-2249">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2249">RDBMS</span></span>

* <span data-ttu-id="460d8-2250">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2250">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2251">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2251">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="460d8-2253">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2253">Role</span></span>

* <span data-ttu-id="460d8-2254">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2254">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="460d8-2255">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2255">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="460d8-2256">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2256">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="460d8-2257">[호환성이 손상되는 변경]`az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2257">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="460d8-2258">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2258">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2259">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2259">Storage</span></span>

* <span data-ttu-id="460d8-2260">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2260">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="460d8-2261">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="460d8-2261">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2262">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2262">VM</span></span>

* <span data-ttu-id="460d8-2263">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2263">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="460d8-2264">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2264">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="460d8-2265">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2265">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="460d8-2266">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2266">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="460d8-2267">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-2267">March 13, 2018</span></span>

<span data-ttu-id="460d8-2268">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="460d8-2268">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2269">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2269">ACR</span></span>

* <span data-ttu-id="460d8-2270">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2270">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="460d8-2271">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2271">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="460d8-2272">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2272">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2273">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2273">ACS</span></span>

* <span data-ttu-id="460d8-2274">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2274">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="460d8-2275">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2275">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="460d8-2276">Advisor</span><span class="sxs-lookup"><span data-stu-id="460d8-2276">Advisor</span></span>

* <span data-ttu-id="460d8-2277">[호환성이 손상되는 변경]`advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2277">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="460d8-2278">[호환성이 손상되는 변경]`advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2278">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="460d8-2279">[호환성이 손상되는 변경]`advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2279">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="460d8-2280">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2280">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="460d8-2281">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2281">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2282">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2282">Appservice</span></span>

* <span data-ttu-id="460d8-2283">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2283">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="460d8-2284">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2284">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="460d8-2285">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="460d8-2285">Eventhubs</span></span>

* <span data-ttu-id="460d8-2286">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2286">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2287">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2287">Extension</span></span>

* <span data-ttu-id="460d8-2288">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2288">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2289">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2289">Interactive</span></span>

* <span data-ttu-id="460d8-2290">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="460d8-2290">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="460d8-2291">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="460d8-2291">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="460d8-2292">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2292">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="460d8-2293">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2293">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2294">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2294">Monitor</span></span>

* <span data-ttu-id="460d8-2295">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2295">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="460d8-2296">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2296">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="460d8-2297">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2297">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="460d8-2298">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2298">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2299">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2299">Network</span></span>

* <span data-ttu-id="460d8-2300">[호환성이 손상되는 변경]`route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2300">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="460d8-2301">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="460d8-2301">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="460d8-2302">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2302">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="460d8-2303">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2303">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2304">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2304">Profile</span></span>

* <span data-ttu-id="460d8-2305">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2305">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="460d8-2306">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2306">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-2307">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2307">RDBMS</span></span>

* <span data-ttu-id="460d8-2308">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2308">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="460d8-2309">Service Bus</span><span class="sxs-lookup"><span data-stu-id="460d8-2309">Service Bus</span></span>

* <span data-ttu-id="460d8-2310">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2310">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2311">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2311">Storage</span></span>

* <span data-ttu-id="460d8-2312">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2312">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="460d8-2313">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2313">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2314">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2314">VM</span></span>

* <span data-ttu-id="460d8-2315">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2315">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="460d8-2316">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2316">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="460d8-2317">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2317">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="460d8-2318">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2318">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="460d8-2319">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="460d8-2319">February 27, 2018</span></span>

<span data-ttu-id="460d8-2320">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="460d8-2320">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2321">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2321">Core</span></span>

* <span data-ttu-id="460d8-2322">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="460d8-2322">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="460d8-2323">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2323">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="460d8-2324">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2324">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2325">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2325">ACS</span></span>

* <span data-ttu-id="460d8-2326">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2326">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="460d8-2327">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="460d8-2327">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="460d8-2328">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2328">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="460d8-2329">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-2329">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2330">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2330">Appservice</span></span>

* <span data-ttu-id="460d8-2331">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="460d8-2331">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="460d8-2332">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2332">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="460d8-2333">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="460d8-2333">Cognitive Services</span></span>

* <span data-ttu-id="460d8-2334">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-2334">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-2335">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-2335">Consumption</span></span>

* <span data-ttu-id="460d8-2336">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2336">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="460d8-2337">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-2337">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2338">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2338">Container</span></span>

* <span data-ttu-id="460d8-2339">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2339">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2340">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2340">Network</span></span>

* <span data-ttu-id="460d8-2341">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2341">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2342">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2342">Resource</span></span>

* <span data-ttu-id="460d8-2343">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2343">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="460d8-2344">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2344">Role</span></span>

* <span data-ttu-id="460d8-2345">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2345">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2346">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2346">SQL</span></span>

* <span data-ttu-id="460d8-2347">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2347">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2348">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2348">Storage</span></span>

* <span data-ttu-id="460d8-2349">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="460d8-2349">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2350">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2350">VM</span></span>

* <span data-ttu-id="460d8-2351">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2351">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="460d8-2352">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="460d8-2352">February 13, 2018</span></span>

<span data-ttu-id="460d8-2353">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="460d8-2353">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2354">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2354">Core</span></span>

* <span data-ttu-id="460d8-2355">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2355">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2356">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2356">ACS</span></span>

* <span data-ttu-id="460d8-2357">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2357">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="460d8-2358">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2358">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="460d8-2359">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2359">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="460d8-2360">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="460d8-2360">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="460d8-2361">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2361">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="460d8-2362">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-2362">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="460d8-2363">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2363">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="460d8-2364">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2364">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2365">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2365">Appservice</span></span>

* <span data-ttu-id="460d8-2366">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2366">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="460d8-2367">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2367">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-2368">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-2368">CDN</span></span>

* <span data-ttu-id="460d8-2369">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2369">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2370">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2370">Container</span></span>

* <span data-ttu-id="460d8-2371">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2371">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="460d8-2372">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2372">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-2373">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-2373">CosmosDB</span></span>

* <span data-ttu-id="460d8-2374">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2374">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2375">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2375">Extension</span></span>

* <span data-ttu-id="460d8-2376">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2376">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="460d8-2377">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2377">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="460d8-2378">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="460d8-2378">Feedback</span></span>

* <span data-ttu-id="460d8-2379">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2379">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2380">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2380">Interactive</span></span>

* <span data-ttu-id="460d8-2381">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2381">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="460d8-2382">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2382">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-2383">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-2383">IoT</span></span>

* <span data-ttu-id="460d8-2384">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2384">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="460d8-2385">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2385">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="460d8-2386">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2386">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="460d8-2387">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2387">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2388">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2388">Monitor</span></span>

* <span data-ttu-id="460d8-2389">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2389">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2390">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2390">Network</span></span>

* <span data-ttu-id="460d8-2391">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2391">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="460d8-2392">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2392">Profile</span></span>

* <span data-ttu-id="460d8-2393">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2393">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2394">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2394">Resource</span></span>

* <span data-ttu-id="460d8-2395">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2395">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="460d8-2396">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2396">Role</span></span>

* <span data-ttu-id="460d8-2397">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2397">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2398">SQL</span></span>

* <span data-ttu-id="460d8-2399">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2399">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="460d8-2400">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2400">Added `sql db rename`</span></span>
* <span data-ttu-id="460d8-2401">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2401">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2402">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2402">Storage</span></span>

* <span data-ttu-id="460d8-2403">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2403">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2404">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2404">VM</span></span>

* <span data-ttu-id="460d8-2405">VM 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2405">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="460d8-2406">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2406">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="460d8-2407">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="460d8-2407">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="460d8-2408">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="460d8-2408">January 31, 2018</span></span>

<span data-ttu-id="460d8-2409">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="460d8-2409">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2410">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2410">Core</span></span>

* <span data-ttu-id="460d8-2411">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2411">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="460d8-2412">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-2412">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="460d8-2413">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2413">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="460d8-2414">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="460d8-2414">Use `--verbose` to see</span></span>
* <span data-ttu-id="460d8-2415">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2415">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2416">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2416">ACS</span></span>

* <span data-ttu-id="460d8-2417">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2417">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="460d8-2418">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-2418">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2419">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2419">Appservice</span></span>

* <span data-ttu-id="460d8-2420">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="460d8-2420">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="460d8-2421">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-2421">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-2422">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-2422">CDN</span></span>

* <span data-ttu-id="460d8-2423">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2423">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-2424">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-2424">CosmosDB</span></span>

* <span data-ttu-id="460d8-2425">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2425">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2426">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2426">Interactive</span></span>

* <span data-ttu-id="460d8-2427">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2427">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2428">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2428">Network</span></span>

* <span data-ttu-id="460d8-2429">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2429">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="460d8-2430">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2430">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="460d8-2431">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2431">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="460d8-2432">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2432">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="460d8-2433">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2433">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="460d8-2434">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="460d8-2434">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="460d8-2435">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2435">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="460d8-2436">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2436">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="460d8-2437">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2437">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="460d8-2438">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="460d8-2438">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2439">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2439">Profile</span></span>

* <span data-ttu-id="460d8-2440">ID가 있는 VM 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2440">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2441">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2441">Resource</span></span>

* <span data-ttu-id="460d8-2442">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2442">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2443">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2443">Storage</span></span>

* <span data-ttu-id="460d8-2444">스토리지 V1 계정을 스토리지 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2444">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="460d8-2445">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2445">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="460d8-2446">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2446">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="460d8-2447">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2447">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="460d8-2448">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2448">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2449">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2449">VM</span></span>

* <span data-ttu-id="460d8-2450">추가 비용이 있는 이미지에서 VM을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2450">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="460d8-2451">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2451">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="460d8-2452">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2452">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="460d8-2453">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2453">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="460d8-2454">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="460d8-2454">January 17, 2018</span></span>

<span data-ttu-id="460d8-2455">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="460d8-2455">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2456">ACR</span></span>

* <span data-ttu-id="460d8-2457">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2457">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="460d8-2458">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2458">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2459">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2459">ACS</span></span>

* <span data-ttu-id="460d8-2460">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2460">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="460d8-2461">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2461">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2462">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2462">Appservice</span></span>

* <span data-ttu-id="460d8-2463">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2463">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="460d8-2464">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2464">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="460d8-2465">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2465">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-2466">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-2466">Backup</span></span>

* <span data-ttu-id="460d8-2467">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2467">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="460d8-2468">`backup restore restore-disks`에 스토리지 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2468">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="460d8-2469">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2469">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="460d8-2470">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2470">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="460d8-2471">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2471">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-2472">Batch</span></span>

* <span data-ttu-id="460d8-2473">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2473">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="460d8-2474">클라우드</span><span class="sxs-lookup"><span data-stu-id="460d8-2474">Cloud</span></span>

* <span data-ttu-id="460d8-2475">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2475">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-2476">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-2476">Consumption</span></span>

* <span data-ttu-id="460d8-2477">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2477">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="460d8-2478">Event Grid</span><span class="sxs-lookup"><span data-stu-id="460d8-2478">Event Grid</span></span>

* <span data-ttu-id="460d8-2479">[호환성이 손상되는 변경]`az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2479">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="460d8-2480">[호환성이 손상되는 변경]`az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2480">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="460d8-2481">[호환성이 손상되는 변경]`eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2481">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="460d8-2482">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="460d8-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="460d8-2483">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2483">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="460d8-2484">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2484">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="460d8-2485">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2485">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="460d8-2486">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2486">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2487">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2487">Interactive</span></span>

* <span data-ttu-id="460d8-2488">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2488">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="460d8-2489">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2489">Fixed errors on startup</span></span>
* <span data-ttu-id="460d8-2490">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2490">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-2491">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-2491">IoT</span></span>

* <span data-ttu-id="460d8-2492">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2492">Added support for device provisioning service</span></span>
* <span data-ttu-id="460d8-2493">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2493">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="460d8-2494">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2494">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2495">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2495">Monitor</span></span>

* <span data-ttu-id="460d8-2496">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2496">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="460d8-2497">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="460d8-2497">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="460d8-2498">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2498">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2499">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2499">Network</span></span>

* <span data-ttu-id="460d8-2500">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2500">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="460d8-2501">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2501">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2502">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2502">Profile</span></span>

* <span data-ttu-id="460d8-2503">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2503">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="460d8-2504">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2504">Role</span></span>

* <span data-ttu-id="460d8-2505">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2505">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="460d8-2506">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="460d8-2506">Service Fabric</span></span>

* <span data-ttu-id="460d8-2507">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2507">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="460d8-2508">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2508">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2509">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2509">VM</span></span>

* <span data-ttu-id="460d8-2510">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2510">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="460d8-2511">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2511">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="460d8-2512">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2512">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="460d8-2513">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2513">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="460d8-2514">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2514">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="460d8-2515">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2515">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="460d8-2516">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2516">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="460d8-2517">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2517">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="460d8-2518">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="460d8-2518">December 19, 2017</span></span>

<span data-ttu-id="460d8-2519">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="460d8-2519">Version 2.0.23</span></span>

* <span data-ttu-id="460d8-2520">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2520">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2521">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2521">Container</span></span>

* <span data-ttu-id="460d8-2522">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2522">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2523">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2523">Network</span></span>

* <span data-ttu-id="460d8-2524">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2524">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="460d8-2525">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2525">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2526">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2526">Storage</span></span>

* <span data-ttu-id="460d8-2527">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2527">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2528">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2528">VM</span></span>

* <span data-ttu-id="460d8-2529">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2529">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="460d8-2530">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="460d8-2530">December 5, 2017</span></span>

<span data-ttu-id="460d8-2531">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="460d8-2531">Version 2.0.22</span></span>

* <span data-ttu-id="460d8-2532">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2532">Removed `az component` commands.</span></span> <span data-ttu-id="460d8-2533">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="460d8-2533">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2534">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2534">Core</span></span>
* <span data-ttu-id="460d8-2535">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2535">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="460d8-2536">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2536">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2537">ACS</span></span>

* <span data-ttu-id="460d8-2538">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2538">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="460d8-2539">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2539">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="460d8-2540">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2540">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="460d8-2541">Advisor</span><span class="sxs-lookup"><span data-stu-id="460d8-2541">Advisor</span></span>

* <span data-ttu-id="460d8-2542">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2542">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2543">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2543">Appservice</span></span>

* <span data-ttu-id="460d8-2544">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2544">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="460d8-2545">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2545">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="460d8-2546">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2546">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="460d8-2547">Consumption</span><span class="sxs-lookup"><span data-stu-id="460d8-2547">Consumption</span></span>

* <span data-ttu-id="460d8-2548">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2548">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2549">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2549">Container</span></span>

* <span data-ttu-id="460d8-2550">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2550">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2551">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2551">Monitor</span></span>

* <span data-ttu-id="460d8-2552">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2552">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2553">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2553">Resource</span></span>

* <span data-ttu-id="460d8-2554">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2554">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="460d8-2555">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-2555">Role</span></span>

* <span data-ttu-id="460d8-2556">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2556">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="460d8-2557">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2557">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="460d8-2558">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2558">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2559">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2559">SQL</span></span>

* <span data-ttu-id="460d8-2560">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2560">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="460d8-2561">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2561">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2562">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2562">VM</span></span>

* <span data-ttu-id="460d8-2563">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2563">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="460d8-2564">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="460d8-2564">November 14, 2017</span></span>

<span data-ttu-id="460d8-2565">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="460d8-2565">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2566">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2566">ACR</span></span>

* <span data-ttu-id="460d8-2567">복제 영역에서 webhook를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2567">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="460d8-2568">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2568">ACS</span></span>

* <span data-ttu-id="460d8-2569">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2569">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="460d8-2570">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="460d8-2570">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="460d8-2571">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2571">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="460d8-2572">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2572">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="460d8-2573">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2573">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2574">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2574">Appservice</span></span>

* <span data-ttu-id="460d8-2575">웹앱 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2575">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="460d8-2576">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2576">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="460d8-2577">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2577">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="460d8-2578">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2578">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="460d8-2579">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2579">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="460d8-2580">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="460d8-2580">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-2581">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-2581">Batch</span></span>

* <span data-ttu-id="460d8-2582">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2582">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-2583">Batchai</span><span class="sxs-lookup"><span data-stu-id="460d8-2583">Batchai</span></span>

* <span data-ttu-id="460d8-2584">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2584">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="460d8-2585">스토리지 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2585">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="460d8-2586">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2586">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="460d8-2587">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2587">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="460d8-2588">클라우드</span><span class="sxs-lookup"><span data-stu-id="460d8-2588">Cloud</span></span>

* <span data-ttu-id="460d8-2589">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2589">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2590">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2590">Container</span></span>

* <span data-ttu-id="460d8-2591">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2591">Added support to open multiple ports</span></span>
* <span data-ttu-id="460d8-2592">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2592">Added container group restart policy</span></span>
* <span data-ttu-id="460d8-2593">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2593">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="460d8-2594">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="460d8-2594">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="460d8-2595">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="460d8-2595">Data Lake Analytics</span></span>

* <span data-ttu-id="460d8-2596">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2596">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="460d8-2597">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="460d8-2597">Data Lake Store</span></span>

* <span data-ttu-id="460d8-2598">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2598">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2599">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2599">Extension</span></span>

* <span data-ttu-id="460d8-2600">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2600">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="460d8-2601">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2601">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-2602">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-2602">IoT</span></span>

* <span data-ttu-id="460d8-2603">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2603">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2604">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2604">Monitor</span></span>

* <span data-ttu-id="460d8-2605">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2605">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2606">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2606">Network</span></span>

* <span data-ttu-id="460d8-2607">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2607">Added support for CAA DNS records</span></span>
* <span data-ttu-id="460d8-2608">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2608">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="460d8-2609">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2609">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="460d8-2610">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2610">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="460d8-2611">예약</span><span class="sxs-lookup"><span data-stu-id="460d8-2611">Reservations</span></span>

* <span data-ttu-id="460d8-2612">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2612">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2613">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2613">Resource</span></span>

* <span data-ttu-id="460d8-2614">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2614">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2615">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2615">SQL</span></span>

* <span data-ttu-id="460d8-2616">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2616">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2617">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2617">Storage</span></span>

* <span data-ttu-id="460d8-2618">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2618">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="460d8-2619">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2619">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="460d8-2620">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2620">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="460d8-2621">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="460d8-2621">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="460d8-2622">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2622">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="460d8-2623">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2623">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="460d8-2624">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2624">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2625">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2625">VM</span></span>

* <span data-ttu-id="460d8-2626">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2626">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="460d8-2627">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2627">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="460d8-2628">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2628">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="460d8-2629">`vm format-secret`에서 `vm secret format`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2629">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="460d8-2630">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2630">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="460d8-2631">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="460d8-2631">October 24, 2017</span></span>

<span data-ttu-id="460d8-2632">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="460d8-2632">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2633">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2633">Core</span></span>

* <span data-ttu-id="460d8-2634">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="460d8-2634">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2635">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2635">ACR</span></span>

* <span data-ttu-id="460d8-2636">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="460d8-2636">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="460d8-2637">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2637">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="460d8-2638">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="460d8-2638">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2639">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2639">ACS</span></span>

* <span data-ttu-id="460d8-2640">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2640">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="460d8-2641">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2641">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2642">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2642">Appservice</span></span>

* <span data-ttu-id="460d8-2643">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2643">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="460d8-2644">구성 요소</span><span class="sxs-lookup"><span data-stu-id="460d8-2644">Component</span></span>

* <span data-ttu-id="460d8-2645">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2645">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2646">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2646">Monitor</span></span>

* <span data-ttu-id="460d8-2647">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2647">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2648">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2648">Resource</span></span>

* <span data-ttu-id="460d8-2649">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2649">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="460d8-2650">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-2650">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2651">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2651">VM</span></span>

* <span data-ttu-id="460d8-2652">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2652">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="460d8-2653">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="460d8-2653">October 9, 2017</span></span>

<span data-ttu-id="460d8-2654">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="460d8-2654">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2655">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2655">Core</span></span>

* <span data-ttu-id="460d8-2656">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2656">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2657">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2657">Appservice</span></span>

* <span data-ttu-id="460d8-2658">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2658">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-2659">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-2659">Batch</span></span>

* <span data-ttu-id="460d8-2660">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2660">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="460d8-2661">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2661">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="460d8-2662">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2662">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="460d8-2663">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2663">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="460d8-2664">Batchai</span><span class="sxs-lookup"><span data-stu-id="460d8-2664">Batchai</span></span>

* <span data-ttu-id="460d8-2665">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2665">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-2666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="460d8-2666">Keyvault</span></span>

* <span data-ttu-id="460d8-2667">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2667">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="460d8-2668">(#4448)</span><span class="sxs-lookup"><span data-stu-id="460d8-2668">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="460d8-2669">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2669">Network</span></span>

* <span data-ttu-id="460d8-2670">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2670">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="460d8-2671">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2671">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2672">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2672">Resource</span></span>

* <span data-ttu-id="460d8-2673">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2673">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="460d8-2674">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2674">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="460d8-2675">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2675">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="460d8-2676">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2676">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2677">Sql</span><span class="sxs-lookup"><span data-stu-id="460d8-2677">Sql</span></span>

* <span data-ttu-id="460d8-2678">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2678">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="460d8-2679">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2679">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="460d8-2680">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2680">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2681">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2681">Storage</span></span>

* <span data-ttu-id="460d8-2682">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2682">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2683">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2683">Vm</span></span>

* <span data-ttu-id="460d8-2684">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2684">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="460d8-2685">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2685">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="460d8-2686">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2686">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="460d8-2687">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2687">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="460d8-2688">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2688">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="460d8-2689">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="460d8-2689">September 22, 2017</span></span>

<span data-ttu-id="460d8-2690">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="460d8-2690">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2691">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2691">Resource</span></span>

* <span data-ttu-id="460d8-2692">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2692">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="460d8-2693">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2693">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="460d8-2694">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2694">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="460d8-2695">[호환성이 손상되는 변경]`managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2695">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2696">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2696">Network</span></span>

* <span data-ttu-id="460d8-2697">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2697">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="460d8-2698">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2698">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="460d8-2699">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2699">Added `asg` application security group commands</span></span>
* <span data-ttu-id="460d8-2700">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2700">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="460d8-2701">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2701">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="460d8-2702">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2702">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="460d8-2703">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2703">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2704">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2704">Storage</span></span>

* <span data-ttu-id="460d8-2705">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2705">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="460d8-2706">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="460d8-2706">Eventgrid</span></span>

* <span data-ttu-id="460d8-2707">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="460d8-2707">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2708">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2708">SQL</span></span>

* <span data-ttu-id="460d8-2709">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2709">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="460d8-2710">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2710">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="460d8-2711">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2711">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-2712">Keyvault</span><span class="sxs-lookup"><span data-stu-id="460d8-2712">Keyvault</span></span>

* <span data-ttu-id="460d8-2713">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2713">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2714">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2714">VM</span></span>

* <span data-ttu-id="460d8-2715">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2715">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="460d8-2716">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460d8-2716">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="460d8-2717">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2717">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="460d8-2718">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2718">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="460d8-2719">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2719">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="460d8-2720">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2720">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2721">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2721">ACS</span></span>

* <span data-ttu-id="460d8-2722">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2722">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2723">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2723">Appservice</span></span>

* <span data-ttu-id="460d8-2724">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2724">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="460d8-2725">Backup</span><span class="sxs-lookup"><span data-stu-id="460d8-2725">Backup</span></span>

* <span data-ttu-id="460d8-2726">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2726">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="460d8-2727">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="460d8-2727">September 11, 2017</span></span>

<span data-ttu-id="460d8-2728">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="460d8-2728">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="460d8-2729">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2729">Core</span></span>

* <span data-ttu-id="460d8-2730">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2730">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="460d8-2731">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2731">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2732">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2732">Acs</span></span>

* <span data-ttu-id="460d8-2733">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2733">Added `acs list-locations` command</span></span>
* <span data-ttu-id="460d8-2734">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="460d8-2734">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2735">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2735">Appservice</span></span>

* <span data-ttu-id="460d8-2736">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2736">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-2737">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-2737">CDN</span></span>

* <span data-ttu-id="460d8-2738">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2738">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="460d8-2739">내선 번호</span><span class="sxs-lookup"><span data-stu-id="460d8-2739">Extension</span></span>

* <span data-ttu-id="460d8-2740">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2740">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-2741">Keyvault</span><span class="sxs-lookup"><span data-stu-id="460d8-2741">Keyvault</span></span>

* <span data-ttu-id="460d8-2742">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2742">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2743">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2743">Network</span></span>

* <span data-ttu-id="460d8-2744">`vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2744">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="460d8-2745">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-2745">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="460d8-2746">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2746">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="460d8-2747">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2747">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="460d8-2748">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2748">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-2749">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-2749">Resource</span></span>

* <span data-ttu-id="460d8-2750">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2750">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="460d8-2751">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2751">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="460d8-2752">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-2752">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="460d8-2753">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="460d8-2753">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-2754">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-2754">SQL</span></span>

* <span data-ttu-id="460d8-2755">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2755">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2756">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2756">VM</span></span>

* <span data-ttu-id="460d8-2757">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2757">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="460d8-2758">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="460d8-2758">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="460d8-2759">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2759">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="460d8-2760">수정됨: `[vm|vmss] create` 스토리지 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2760">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="460d8-2761">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2761">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="460d8-2762">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="460d8-2762">August 31, 2017</span></span>

<span data-ttu-id="460d8-2763">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="460d8-2763">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-2764">Keyvault</span><span class="sxs-lookup"><span data-stu-id="460d8-2764">Keyvault</span></span>

* <span data-ttu-id="460d8-2765">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2765">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="460d8-2766">Sf</span><span class="sxs-lookup"><span data-stu-id="460d8-2766">Sf</span></span>

* <span data-ttu-id="460d8-2767">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2767">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2768">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2768">Storage</span></span>

* <span data-ttu-id="460d8-2769">스토리지 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2769">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="460d8-2770">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="460d8-2770">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="460d8-2771">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="460d8-2771">August 28, 2017</span></span>

<span data-ttu-id="460d8-2772">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="460d8-2772">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="460d8-2773">CLI</span><span class="sxs-lookup"><span data-stu-id="460d8-2773">CLI</span></span>

* <span data-ttu-id="460d8-2774">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2774">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2775">ACS</span></span>

* <span data-ttu-id="460d8-2776">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2776">Corrected preview regions</span></span>
* <span data-ttu-id="460d8-2777">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2777">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="460d8-2778">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2778">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2779">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2779">Appservice</span></span>

* <span data-ttu-id="460d8-2780">[호환성이 손상되는 변경]`az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2780">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="460d8-2781">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2781">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="460d8-2782">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2782">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="460d8-2783">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2783">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="460d8-2784">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="460d8-2784">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-2785">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-2785">IoT</span></span>

* <span data-ttu-id="460d8-2786">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2786">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2787">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2787">Network</span></span>

* <span data-ttu-id="460d8-2788">[호환성이 손상되는 변경]`vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2788">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="460d8-2789">[호환성이 손상되는 변경]`vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2789">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="460d8-2790">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2790">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="460d8-2791">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2791">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="460d8-2792">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2792">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2793">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2793">Profile</span></span>

* <span data-ttu-id="460d8-2794">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2794">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="460d8-2795">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="460d8-2795">Service Fabric</span></span>

* <span data-ttu-id="460d8-2796">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2796">Preview release</span></span>
* <span data-ttu-id="460d8-2797">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2797">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="460d8-2798">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2798">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="460d8-2799">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2799">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2800">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2800">Storage</span></span>

* <span data-ttu-id="460d8-2801">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2801">Enabled setting blob tier</span></span>
* <span data-ttu-id="460d8-2802">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2802">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="460d8-2803">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2803">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="460d8-2804">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2804">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="460d8-2805">[호환성이 손상되는 변경]`az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2805">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="460d8-2806">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2806">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2807">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2807">VM</span></span>

* <span data-ttu-id="460d8-2808">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2808">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="460d8-2809">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2809">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="460d8-2810">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2810">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="460d8-2811">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2811">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="460d8-2812">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2812">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="460d8-2813">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2813">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="460d8-2814">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="460d8-2814">August 15, 2017</span></span>

<span data-ttu-id="460d8-2815">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="460d8-2815">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2816">ACS</span></span>

* <span data-ttu-id="460d8-2817">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2817">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2818">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2818">Appservice</span></span>

* <span data-ttu-id="460d8-2819">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2819">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="460d8-2820">Event Grid</span><span class="sxs-lookup"><span data-stu-id="460d8-2820">Event Grid</span></span>

* <span data-ttu-id="460d8-2821">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2821">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="460d8-2822">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="460d8-2822">August 11, 2017</span></span>

<span data-ttu-id="460d8-2823">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="460d8-2823">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2824">ACS</span></span>

* <span data-ttu-id="460d8-2825">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2825">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-2826">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-2826">Batch</span></span>

* <span data-ttu-id="460d8-2827">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2827">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="460d8-2828">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2828">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="460d8-2829">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2829">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="460d8-2830">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2830">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="460d8-2831">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2831">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="460d8-2832">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2832">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="460d8-2833">구성 요소</span><span class="sxs-lookup"><span data-stu-id="460d8-2833">Component</span></span>

* <span data-ttu-id="460d8-2834">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2834">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="460d8-2835">컨테이너</span><span class="sxs-lookup"><span data-stu-id="460d8-2835">Container</span></span>

* <span data-ttu-id="460d8-2836">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2836">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="460d8-2837">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="460d8-2837">Data Lake Store</span></span>

* <span data-ttu-id="460d8-2838">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2838">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="460d8-2839">Event Grid</span><span class="sxs-lookup"><span data-stu-id="460d8-2839">Event Grid</span></span>

* <span data-ttu-id="460d8-2840">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-2840">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2841">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2841">Network</span></span>

* <span data-ttu-id="460d8-2842">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2842">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="460d8-2843">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2843">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="460d8-2844">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2844">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="460d8-2845">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2845">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2846">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2846">Profile</span></span>

* <span data-ttu-id="460d8-2847">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2847">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-2848">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-2848">Storage</span></span>

* <span data-ttu-id="460d8-2849">시스템에 할당된 ID를 통한 스토리지 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2849">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-2850">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-2850">VM</span></span>

* <span data-ttu-id="460d8-2851">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2851">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="460d8-2852">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2852">Exposed `list-skus` command</span></span>
* <span data-ttu-id="460d8-2853">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2853">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="460d8-2854">데이터 디스크 연결 시 스토리지 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2854">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="460d8-2855">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 스토리지 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2855">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="460d8-2856">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="460d8-2856">July 28, 2017</span></span>

<span data-ttu-id="460d8-2857">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="460d8-2857">Version 2.0.12</span></span>

* <span data-ttu-id="460d8-2858">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2858">Added container commands</span></span>
* <span data-ttu-id="460d8-2859">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2859">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="460d8-2860">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-2860">Core</span></span>

* <span data-ttu-id="460d8-2861">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2861">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="460d8-2862">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2862">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="460d8-2863">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-2863">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="460d8-2864">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="460d8-2864">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="460d8-2865">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="460d8-2865">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="460d8-2866">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="460d8-2866">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="460d8-2867">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="460d8-2867">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="460d8-2868">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="460d8-2868">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="460d8-2869">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="460d8-2869">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="460d8-2870">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-2870">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="460d8-2871">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="460d8-2871">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="460d8-2872">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="460d8-2872">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="460d8-2873">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2873">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="460d8-2874">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2874">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="460d8-2875">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2875">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="460d8-2876">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="460d8-2876">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="460d8-2877">ACR</span><span class="sxs-lookup"><span data-stu-id="460d8-2877">ACR</span></span>

* <span data-ttu-id="460d8-2878">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2878">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="460d8-2879">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2879">Support SKU update for managed registries</span></span>
* <span data-ttu-id="460d8-2880">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2880">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="460d8-2881">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 webhook가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2881">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="460d8-2882">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2882">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="460d8-2883">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2883">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-2884">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-2884">ACS</span></span>

* <span data-ttu-id="460d8-2885">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-2885">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-2886">Appservice</span><span class="sxs-lookup"><span data-stu-id="460d8-2886">Appservice</span></span>

* <span data-ttu-id="460d8-2887">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2887">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="460d8-2888">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2888">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="460d8-2889">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2889">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="460d8-2890">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="460d8-2890">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="460d8-2891">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="460d8-2891">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="460d8-2892">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="460d8-2892">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="460d8-2893">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="460d8-2893">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="460d8-2894">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="460d8-2894">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="460d8-2895">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2895">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="460d8-2896">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2896">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="460d8-2897">Batch</span><span class="sxs-lookup"><span data-stu-id="460d8-2897">Batch</span></span>

* <span data-ttu-id="460d8-2898">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2898">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="460d8-2899">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2899">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="460d8-2900">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2900">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="460d8-2901">CDN</span><span class="sxs-lookup"><span data-stu-id="460d8-2901">CDN</span></span>

* <span data-ttu-id="460d8-2902">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2902">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="460d8-2903">클라우드</span><span class="sxs-lookup"><span data-stu-id="460d8-2903">Cloud</span></span>

* <span data-ttu-id="460d8-2904">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2904">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="460d8-2905">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-2905">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="460d8-2906">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2906">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="460d8-2907">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2907">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="460d8-2908">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2908">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-2909">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-2909">CosmosDB</span></span>

* <span data-ttu-id="460d8-2910">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2910">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="460d8-2911">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2911">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="460d8-2912">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="460d8-2912">Data Lake Analytics</span></span>

* <span data-ttu-id="460d8-2913">`dla account compute-policy` 제목 아래에 컴퓨팅 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2913">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="460d8-2914">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2914">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="460d8-2915">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2915">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="460d8-2916">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="460d8-2916">Data Lake Store</span></span>

* <span data-ttu-id="460d8-2917">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2917">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="460d8-2918">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2918">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="460d8-2919">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2919">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="460d8-2920">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="460d8-2920">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="460d8-2921">대화형</span><span class="sxs-lookup"><span data-stu-id="460d8-2921">Interactive</span></span>

* <span data-ttu-id="460d8-2922">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2922">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="460d8-2923">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2923">Increased test coverage</span></span>
* <span data-ttu-id="460d8-2924">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2924">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="460d8-2925">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="460d8-2925">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="460d8-2926">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="460d8-2926">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="460d8-2927">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="460d8-2927">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="460d8-2928">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="460d8-2928">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="460d8-2929">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2929">Added `--progress` flag</span></span>
* <span data-ttu-id="460d8-2930">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2930">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="460d8-2931">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="460d8-2931">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="460d8-2932">IoT</span><span class="sxs-lookup"><span data-stu-id="460d8-2932">IoT</span></span>

* <span data-ttu-id="460d8-2933">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2933">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="460d8-2934">(#3934)</span><span class="sxs-lookup"><span data-stu-id="460d8-2934">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="460d8-2935">키 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="460d8-2935">Key vault</span></span>

* <span data-ttu-id="460d8-2936">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="460d8-2936">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="460d8-2937">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="460d8-2937">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="460d8-2938">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="460d8-2938">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="460d8-2939">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="460d8-2939">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="460d8-2940">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="460d8-2940">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="460d8-2941">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="460d8-2941">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="460d8-2942">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2942">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="460d8-2943">(#3307)</span><span class="sxs-lookup"><span data-stu-id="460d8-2943">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="460d8-2944">랩</span><span class="sxs-lookup"><span data-stu-id="460d8-2944">Lab</span></span>

* <span data-ttu-id="460d8-2945">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2945">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="460d8-2946">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2946">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-2947">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-2947">Monitor</span></span>

* <span data-ttu-id="460d8-2948">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="460d8-2948">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="460d8-2949">`monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2949">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="460d8-2950">`monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2950">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="460d8-2951">`monitor metric-defintions list`에서 `monitor metrics list-definitions`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2951">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="460d8-2952">`monitor alert-rules`에서 `monitor alert`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2952">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="460d8-2953">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="460d8-2953">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="460d8-2954">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2954">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="460d8-2955">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2955">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="460d8-2956">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2956">`location` no longer required</span></span>
  * <span data-ttu-id="460d8-2957">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2957">Add name and ID support for target</span></span>
  * <span data-ttu-id="460d8-2958">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2958">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="460d8-2959">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2959">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="460d8-2960">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2960">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="460d8-2961">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2961">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="460d8-2962">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2962">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="460d8-2963">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2963">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="460d8-2964">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-2964">Network</span></span>

* <span data-ttu-id="460d8-2965">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2965">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="460d8-2966">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2966">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="460d8-2967">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2967">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="460d8-2968">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2968">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="460d8-2969">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2969">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="460d8-2970">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2970">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="460d8-2971">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="460d8-2971">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="460d8-2972">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="460d8-2972">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="460d8-2973">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="460d8-2973">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="460d8-2974">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="460d8-2974">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="460d8-2975">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="460d8-2975">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="460d8-2976">`--no-wait`에 대한 지원이 `application-gateway url-path-map rule delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2976">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="460d8-2977">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="460d8-2977">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="460d8-2978">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="460d8-2978">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="460d8-2979">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2979">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="460d8-2980">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2980">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="460d8-2981">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-2981">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="460d8-2982">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2982">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="460d8-2983">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2983">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="460d8-2984">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2984">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="460d8-2985">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2985">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="460d8-2986">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-2986">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="460d8-2987">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2987">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="460d8-2988">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2988">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="460d8-2989">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2989">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="460d8-2990">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2990">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="460d8-2991">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2991">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-2992">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-2992">Profile</span></span>

* <span data-ttu-id="460d8-2993">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2993">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="460d8-2994">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2994">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="460d8-2995">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2995">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="460d8-2996">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2996">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="460d8-2997">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-2997">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="460d8-2998">RDBMS</span><span class="sxs-lookup"><span data-stu-id="460d8-2998">RDBMS</span></span>

* <span data-ttu-id="460d8-2999">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="460d8-2999">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="460d8-3000">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="460d8-3000">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="460d8-3001">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="460d8-3001">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="460d8-3002">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="460d8-3002">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-3003">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-3003">Resource</span></span>

* <span data-ttu-id="460d8-3004">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3004">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="460d8-3005">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3005">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="460d8-3006">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3006">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="460d8-3007">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3007">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="460d8-3008">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="460d8-3008">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="460d8-3009">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3009">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="460d8-3010">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="460d8-3010">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="460d8-3011">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3011">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="460d8-3012">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-3012">Role</span></span>

* <span data-ttu-id="460d8-3013">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3013">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="460d8-3014">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="460d8-3014">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="460d8-3015">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3015">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="460d8-3016">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3016">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="460d8-3017">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3017">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="460d8-3018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="460d8-3018">Service Fabric</span></span>
* <span data-ttu-id="460d8-3019">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="460d8-3019">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="460d8-3020">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="460d8-3020">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="460d8-3021">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="460d8-3021">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-3022">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-3022">SQL</span></span>

* <span data-ttu-id="460d8-3023">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3023">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="460d8-3024">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3024">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="460d8-3025">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3025">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-3026">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-3026">Storage</span></span>

* <span data-ttu-id="460d8-3027">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="460d8-3027">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="460d8-3028">HTTPS 전용 스토리지 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-3028">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="460d8-3029">스토리지 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="460d8-3029">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="460d8-3030">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3030">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="460d8-3031">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="460d8-3031">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="460d8-3032">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="460d8-3032">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-3033">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-3033">VM</span></span>

* <span data-ttu-id="460d8-3034">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3034">Support configuring nsg</span></span>
* <span data-ttu-id="460d8-3035">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3035">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="460d8-3036">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3036">Support managed service identities</span></span>
* <span data-ttu-id="460d8-3037">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3037">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="460d8-3038">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3038">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="460d8-3039">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="460d8-3039">May 10, 2017</span></span>

<span data-ttu-id="460d8-3040">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="460d8-3040">Version 2.0.6</span></span>

* <span data-ttu-id="460d8-3041">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="460d8-3041">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="460d8-3042">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3042">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="460d8-3043">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="460d8-3043">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="460d8-3044">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="460d8-3044">Include Cognitive Services module</span></span>
* <span data-ttu-id="460d8-3045">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="460d8-3045">Include Service Fabric module</span></span>
* <span data-ttu-id="460d8-3046">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="460d8-3046">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="460d8-3047">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3047">Add support for CDN commands</span></span>
* <span data-ttu-id="460d8-3048">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-3048">Remove Container module</span></span>
* <span data-ttu-id="460d8-3049">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="460d8-3049">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="460d8-3050">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="460d8-3050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="460d8-3051">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-3051">Core</span></span>

* <span data-ttu-id="460d8-3052">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="460d8-3052">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="460d8-3053">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="460d8-3053">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="460d8-3054">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="460d8-3054">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="460d8-3055">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="460d8-3055">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="460d8-3056">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="460d8-3056">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="460d8-3057">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="460d8-3057">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="460d8-3058">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="460d8-3058">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="460d8-3059">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="460d8-3059">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="460d8-3060">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="460d8-3060">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="460d8-3061">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="460d8-3061">core: Improved performance</span></span>
* <span data-ttu-id="460d8-3062">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-3062">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="460d8-3063">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="460d8-3063">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-3064">ACS</span></span>

* <span data-ttu-id="460d8-3065">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3065">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="460d8-3066">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-3066">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="460d8-3067">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-3067">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="460d8-3068">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="460d8-3068">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-3069">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-3069">AppService</span></span>

* <span data-ttu-id="460d8-3070">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="460d8-3070">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="460d8-3071">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3071">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="460d8-3072">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="460d8-3072">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="460d8-3073">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-3073">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="460d8-3074">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="460d8-3074">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="460d8-3075">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="460d8-3075">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="460d8-3076">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-3076">support slot swap with preview</span></span>
* <span data-ttu-id="460d8-3077">appservice 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="460d8-3077">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="460d8-3078">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="460d8-3078">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="460d8-3079">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="460d8-3079">CosmosDB</span></span>

* <span data-ttu-id="460d8-3080">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="460d8-3080">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="460d8-3081">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3081">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="460d8-3082">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3082">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="460d8-3083">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3083">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="460d8-3084">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="460d8-3084">Data Lake Analytics</span></span>

* <span data-ttu-id="460d8-3085">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3085">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="460d8-3086">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3086">Add support for new catalog item type: package.</span></span> <span data-ttu-id="460d8-3087">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="460d8-3087">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="460d8-3088">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="460d8-3088">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="460d8-3089">테이블</span><span class="sxs-lookup"><span data-stu-id="460d8-3089">Table</span></span>
  * <span data-ttu-id="460d8-3090">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="460d8-3090">Table valued function</span></span>
  * <span data-ttu-id="460d8-3091">보기</span><span class="sxs-lookup"><span data-stu-id="460d8-3091">View</span></span>
  * <span data-ttu-id="460d8-3092">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="460d8-3092">Table Statistics.</span></span> <span data-ttu-id="460d8-3093">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="460d8-3093">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="460d8-3094">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="460d8-3094">Data Lake Store</span></span>

* <span data-ttu-id="460d8-3095">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="460d8-3095">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="460d8-3096">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="460d8-3096">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="460d8-3097">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="460d8-3097">missed help for access show.</span></span> <span data-ttu-id="460d8-3098">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3098">adding it.</span></span> <span data-ttu-id="460d8-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="460d8-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="460d8-3100">찾기</span><span class="sxs-lookup"><span data-stu-id="460d8-3100">Find</span></span>

* <span data-ttu-id="460d8-3101">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="460d8-3101">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="460d8-3102">KeyVault</span><span class="sxs-lookup"><span data-stu-id="460d8-3102">KeyVault</span></span>

* <span data-ttu-id="460d8-3103">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3103">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="460d8-3104">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="460d8-3104">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="460d8-3105">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3105">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="460d8-3106">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3106">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="460d8-3107">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="460d8-3107">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="460d8-3108">랩</span><span class="sxs-lookup"><span data-stu-id="460d8-3108">Lab</span></span>

* <span data-ttu-id="460d8-3109">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3109">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="460d8-3110">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3110">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="460d8-3111">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="460d8-3111">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="460d8-3112">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="460d8-3112">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="460d8-3113">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3113">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="460d8-3114">모니터</span><span class="sxs-lookup"><span data-stu-id="460d8-3114">Monitor</span></span>

* <span data-ttu-id="460d8-3115">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="460d8-3115">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="460d8-3116">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="460d8-3116">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="460d8-3117">네트워크</span><span class="sxs-lookup"><span data-stu-id="460d8-3117">Network</span></span>

* <span data-ttu-id="460d8-3118">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3118">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="460d8-3119">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3119">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="460d8-3120">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3120">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="460d8-3121">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3121">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="460d8-3122">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3122">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="460d8-3123">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3123">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="460d8-3124">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3124">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="460d8-3125">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3125">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="460d8-3126">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3126">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="460d8-3127">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3127">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="460d8-3128">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="460d8-3128">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="460d8-3129">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3129">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="460d8-3130">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3130">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="460d8-3131">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3131">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="460d8-3132">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="460d8-3132">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="460d8-3133">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3133">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="460d8-3134">프로필</span><span class="sxs-lookup"><span data-stu-id="460d8-3134">Profile</span></span>

* <span data-ttu-id="460d8-3135">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="460d8-3135">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="460d8-3136">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="460d8-3136">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="460d8-3137">Redis</span><span class="sxs-lookup"><span data-stu-id="460d8-3137">Redis</span></span>

* <span data-ttu-id="460d8-3138">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3138">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="460d8-3139">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="460d8-3139">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="460d8-3140">리소스</span><span class="sxs-lookup"><span data-stu-id="460d8-3140">Resource</span></span>

* <span data-ttu-id="460d8-3141">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="460d8-3141">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="460d8-3142">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="460d8-3142">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="460d8-3143">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="460d8-3143">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="460d8-3144">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3144">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="460d8-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="460d8-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="460d8-3146">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3146">Add docs for az lock update.</span></span> <span data-ttu-id="460d8-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="460d8-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="460d8-3148">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3148">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="460d8-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="460d8-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="460d8-3150">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3150">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="460d8-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="460d8-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="460d8-3152">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="460d8-3152">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="460d8-3153">역할</span><span class="sxs-lookup"><span data-stu-id="460d8-3153">Role</span></span>

* <span data-ttu-id="460d8-3154">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="460d8-3154">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="460d8-3155">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="460d8-3155">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="460d8-3156">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="460d8-3156">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="460d8-3157">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="460d8-3157">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="460d8-3158">SQL</span><span class="sxs-lookup"><span data-stu-id="460d8-3158">SQL</span></span>

* <span data-ttu-id="460d8-3159">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="460d8-3159">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="460d8-3160">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="460d8-3160">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="460d8-3161">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-3161">Storage</span></span>

* <span data-ttu-id="460d8-3162">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="460d8-3162">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="460d8-3163">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3163">Add support for incremental blob copy</span></span>
* <span data-ttu-id="460d8-3164">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3164">Add support for large block blob upload</span></span>
* <span data-ttu-id="460d8-3165">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="460d8-3165">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-3166">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-3166">VM</span></span>

* <span data-ttu-id="460d8-3167">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="460d8-3167">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="460d8-3168">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="460d8-3168">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="460d8-3169">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="460d8-3169">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="460d8-3170">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="460d8-3170">az vm/vmss disk</span></span>
  3. <span data-ttu-id="460d8-3171">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3171">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="460d8-3172">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="460d8-3172">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="460d8-3173">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="460d8-3173">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="460d8-3174">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="460d8-3174">April 3, 2017</span></span>

<span data-ttu-id="460d8-3175">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="460d8-3175">Version 2.0.2</span></span>

<span data-ttu-id="460d8-3176">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3176">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="460d8-3177">핵심</span><span class="sxs-lookup"><span data-stu-id="460d8-3177">Core</span></span>

* <span data-ttu-id="460d8-3178">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="460d8-3178">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="460d8-3179">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="460d8-3179">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="460d8-3180">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="460d8-3180">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="460d8-3181">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="460d8-3181">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="460d8-3182">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="460d8-3182">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="460d8-3183">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="460d8-3183">Add prompting for missing template parameters.</span></span> <span data-ttu-id="460d8-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="460d8-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="460d8-3185">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-3185">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="460d8-3186">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="460d8-3186">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="460d8-3187">ACS</span><span class="sxs-lookup"><span data-stu-id="460d8-3187">ACS</span></span>

* <span data-ttu-id="460d8-3188">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="460d8-3188">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="460d8-3189">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="460d8-3189">Add support for ssh key password prompting.</span></span> <span data-ttu-id="460d8-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="460d8-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="460d8-3191">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="460d8-3191">Add support for windows clusters.</span></span> <span data-ttu-id="460d8-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="460d8-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="460d8-3193">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="460d8-3193">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="460d8-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="460d8-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="460d8-3195">AppService</span><span class="sxs-lookup"><span data-stu-id="460d8-3195">AppService</span></span>

* <span data-ttu-id="460d8-3196">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="460d8-3196">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="460d8-3197">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="460d8-3197">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="460d8-3198">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="460d8-3198">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="460d8-3199">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="460d8-3199">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="460d8-3200">DataLake</span><span class="sxs-lookup"><span data-stu-id="460d8-3200">DataLake</span></span>

* <span data-ttu-id="460d8-3201">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-3201">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="460d8-3202">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="460d8-3202">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="460d8-3203">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="460d8-3203">DocuemntDB</span></span>

* <span data-ttu-id="460d8-3204">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="460d8-3204">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="460d8-3205">VM</span><span class="sxs-lookup"><span data-stu-id="460d8-3205">VM</span></span>

* <span data-ttu-id="460d8-3206">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="460d8-3206">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="460d8-3207">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="460d8-3207">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="460d8-3208">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="460d8-3208">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="460d8-3209">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="460d8-3209">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="460d8-3210">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="460d8-3210">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="460d8-3211">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="460d8-3211">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="460d8-3212">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="460d8-3212">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="460d8-3213">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="460d8-3213">February 27, 2017</span></span>

<span data-ttu-id="460d8-3214">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="460d8-3214">Version 2.0.0</span></span>

<span data-ttu-id="460d8-3215">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3215">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="460d8-3216">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="460d8-3216">Container Service (acs)</span></span>
- <span data-ttu-id="460d8-3217">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="460d8-3217">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="460d8-3218">네트워킹</span><span class="sxs-lookup"><span data-stu-id="460d8-3218">Networking</span></span>
- <span data-ttu-id="460d8-3219">스토리지</span><span class="sxs-lookup"><span data-stu-id="460d8-3219">Storage</span></span>

<span data-ttu-id="460d8-3220">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3220">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="460d8-3221">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3221">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="460d8-3222">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3222">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="460d8-3223">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3223">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="460d8-3224">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="460d8-3224">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="460d8-3225">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460d8-3225">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="460d8-3226">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="460d8-3226">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="460d8-3227">제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="460d8-3227">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="460d8-3228">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="460d8-3228">Provide feedback from the command line with the `az feedback` command</span></span>


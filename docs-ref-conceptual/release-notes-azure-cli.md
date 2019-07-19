---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/16/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8cb0e2f43a3f40fdf15a00ebc7bdb931bf8f41f0
ms.sourcegitcommit: 49e1dea60942fce02d9c3ce249ac633a83f303e7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2019
ms.locfileid: "68246915"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="927ea-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="927ea-103">Azure CLI release notes</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="927ea-104">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="927ea-104">July 16, 2019</span></span>

<span data-ttu-id="927ea-105">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="927ea-105">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-106">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-106">Appservice</span></span>

* <span data-ttu-id="927ea-107">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-107">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="927ea-108">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-108">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="927ea-109">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-109">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="927ea-110">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-110">Core</span></span>

* <span data-ttu-id="927ea-111">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-111">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-112">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-112">Batch</span></span>

* <span data-ttu-id="927ea-113">[호환성이 손상되는 변경] `batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="927ea-113">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="927ea-114">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-114">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="927ea-115">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-115">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="927ea-116">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-116">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="927ea-117">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="927ea-117">Eventhubs</span></span>

* <span data-ttu-id="927ea-118">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-118">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-119">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-119">RDBMS</span></span>

* <span data-ttu-id="927ea-120">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-120">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="927ea-121">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-121">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="927ea-122">릴레이</span><span class="sxs-lookup"><span data-stu-id="927ea-122">Relay</span></span>

* <span data-ttu-id="927ea-123">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-123">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="927ea-124">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-124">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="927ea-125">Servicebus</span><span class="sxs-lookup"><span data-stu-id="927ea-125">Servicebus</span></span>

* <span data-ttu-id="927ea-126">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-126">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-127">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-127">Storage</span></span>

* <span data-ttu-id="927ea-128">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-128">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="927ea-129">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-129">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="927ea-130">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="927ea-130">July 2, 2019</span></span>

<span data-ttu-id="927ea-131">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="927ea-131">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="927ea-132">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-132">Core</span></span>

* <span data-ttu-id="927ea-133">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-133">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="927ea-134">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-134">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="927ea-135">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-135">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-136">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-136">ACR</span></span>

* <span data-ttu-id="927ea-137">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-137">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-138">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-138">Appservice</span></span>

* <span data-ttu-id="927ea-139">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-139">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="927ea-140">[호환성이 손상되는 변경] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-140">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="927ea-141">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-141">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="927ea-142">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-142">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="927ea-143">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="927ea-143">Cosmos DB</span></span>

* <span data-ttu-id="927ea-144">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-144">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="927ea-145">DLS</span><span class="sxs-lookup"><span data-stu-id="927ea-145">DLS</span></span>

* <span data-ttu-id="927ea-146">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="927ea-146">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="927ea-147">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="927ea-147">Feedback</span></span>

* <span data-ttu-id="927ea-148">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-148">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-149">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-149">HDInsight</span></span>

* <span data-ttu-id="927ea-150">[호환성이 손상되는 변경] `oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-150">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="927ea-151">[호환성이 손상되는 변경] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-151">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="927ea-152">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-152">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="927ea-153">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-153">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="927ea-154">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-154">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="927ea-155">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-155">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="927ea-156">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-156">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="927ea-157">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-157">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="927ea-158">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-158">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="927ea-159">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="927ea-159">Managed Services</span></span>

* <span data-ttu-id="927ea-160">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="927ea-160">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-161">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-161">Profile</span></span>
* <span data-ttu-id="927ea-162">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-162">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="927ea-163">RBAC</span><span class="sxs-lookup"><span data-stu-id="927ea-163">RBAC</span></span>

* <span data-ttu-id="927ea-164">[호환성이 손상되는 변경] `create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-164">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="927ea-165">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-165">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="927ea-166">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-166">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="927ea-167">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-167">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-168">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-168">RDBMS</span></span>

* <span data-ttu-id="927ea-169">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-169">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-170">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-170">SQL</span></span>

* <span data-ttu-id="927ea-171">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="927ea-171">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-172">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-172">Storage</span></span>

* <span data-ttu-id="927ea-173">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="927ea-173">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="927ea-174">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="927ea-174">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="927ea-175">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-175">VM</span></span>

* <span data-ttu-id="927ea-176">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-176">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="927ea-177">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-177">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="927ea-178">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-178">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="927ea-179">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-179">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="927ea-180">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="927ea-180">June 18, 2019</span></span>

<span data-ttu-id="927ea-181">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="927ea-181">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="927ea-182">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-182">Core</span></span>

<span data-ttu-id="927ea-183">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-183">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="927ea-184">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-184">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="927ea-185">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-185">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="927ea-186">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-186">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="927ea-187">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-187">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="927ea-188">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-188">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="927ea-189">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-189">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-190">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-190">ACR</span></span>
* <span data-ttu-id="927ea-191">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-191">Added 'acr check-health' command</span></span>
* <span data-ttu-id="927ea-192">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="927ea-192">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-193">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-193">ACS</span></span>
* <span data-ttu-id="927ea-194">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="927ea-194">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-195">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-195">AMS</span></span>
* <span data-ttu-id="927ea-196">[호환성이 손상되는 변경] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-196">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-197">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-197">AppService</span></span>
* <span data-ttu-id="927ea-198">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-198">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="927ea-199">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-199">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="927ea-200">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-200">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="927ea-201">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-201">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="927ea-202">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-202">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="927ea-203">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-203">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-204">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-204">Batch</span></span>
* <span data-ttu-id="927ea-205">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-205">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-206">BatchAI</span><span class="sxs-lookup"><span data-stu-id="927ea-206">BatchAI</span></span>
* <span data-ttu-id="927ea-207">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="927ea-207">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-208">BotService</span><span class="sxs-lookup"><span data-stu-id="927ea-208">BotService</span></span>
* <span data-ttu-id="927ea-209">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-209">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-210">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-210">CosmosDB</span></span>
* <span data-ttu-id="927ea-211">[사용 되지 않음] `cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-211">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="927ea-212">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="927ea-212">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="927ea-213">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-213">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="927ea-214">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-214">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="927ea-215">EventGrid</span><span class="sxs-lookup"><span data-stu-id="927ea-215">EventGrid</span></span>
* <span data-ttu-id="927ea-216">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-216">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="927ea-217">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-217">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="927ea-218">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-218">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="927ea-219">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-219">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="927ea-220">[호환성이 손상되는 변경] `eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-220">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-221">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-221">HDInsight</span></span>
* <span data-ttu-id="927ea-222">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-222">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-223">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-223">IoT</span></span>
* <span data-ttu-id="927ea-224">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-224">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="927ea-225">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-225">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="927ea-226">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-226">Network</span></span>
* <span data-ttu-id="927ea-227">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-227">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="927ea-228">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-228">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="927ea-229">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-229">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="927ea-230">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-230">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-231">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-231">Resource</span></span>
* <span data-ttu-id="927ea-232">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-232">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="927ea-233">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-233">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="927ea-234">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="927ea-234">ServiceBus</span></span>
* <span data-ttu-id="927ea-235">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-235">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-236">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-236">SQL</span></span>
* <span data-ttu-id="927ea-237">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-237">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="927ea-238">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-238">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="927ea-239">SQLVm</span><span class="sxs-lookup"><span data-stu-id="927ea-239">SQLVm</span></span>
* <span data-ttu-id="927ea-240">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-240">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="927ea-241">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-241">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-242">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-242">Storage</span></span>
* <span data-ttu-id="927ea-243">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-243">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="927ea-244">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-244">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-245">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-245">VM</span></span>
* <span data-ttu-id="927ea-246">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-246">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="927ea-247">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="927ea-247">June 4, 2019</span></span>

<span data-ttu-id="927ea-248">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="927ea-248">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="927ea-249">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-249">Core</span></span>
* <span data-ttu-id="927ea-250">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-250">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-251">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-251">ACR</span></span>
* <span data-ttu-id="927ea-252">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-252">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-253">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-253">ACS</span></span>
* <span data-ttu-id="927ea-254">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-254">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="927ea-255">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="927ea-255">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-256">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-256">Batch</span></span>
* <span data-ttu-id="927ea-257">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-257">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-258">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-258">IoT</span></span>
* <span data-ttu-id="927ea-259">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-259">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="927ea-260">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-260">Network</span></span>
* <span data-ttu-id="927ea-261">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-261">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="927ea-262">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-262">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="927ea-263">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-263">Resource</span></span>
* <span data-ttu-id="927ea-264">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-264">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="927ea-265">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-265">Role</span></span>
* <span data-ttu-id="927ea-266">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-266">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="927ea-267">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="927ea-267">Compute</span></span>
* <span data-ttu-id="927ea-268">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-268">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="927ea-269">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="927ea-269">May 21, 2019</span></span>

<span data-ttu-id="927ea-270">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="927ea-270">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="927ea-271">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-271">Core</span></span>
* <span data-ttu-id="927ea-272">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-272">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="927ea-273">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-273">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="927ea-274">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-274">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-275">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-275">ACR</span></span>
* <span data-ttu-id="927ea-276">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-276">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-277">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-277">ACS</span></span>
* <span data-ttu-id="927ea-278">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-278">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-279">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-279">AppService</span></span>
* <span data-ttu-id="927ea-280">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-280">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="927ea-281">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-281">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="927ea-282">[호환성이 손상되는 변경] `functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-282">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="927ea-283">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-283">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="927ea-284">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-284">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="927ea-285">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-285">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="927ea-286">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-286">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-287">BotService</span><span class="sxs-lookup"><span data-stu-id="927ea-287">BotService</span></span>
* <span data-ttu-id="927ea-288">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-288">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="927ea-289">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-289">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-290">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-290">Consumption</span></span>
* <span data-ttu-id="927ea-291">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-291">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-292">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-292">IoT</span></span>
* <span data-ttu-id="927ea-293">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-293">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="927ea-294">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-294">Network</span></span>
* [호환성이 손상되는 변경]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="927ea-296">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-296">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="927ea-297">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-297">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-298">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-298">RDBMS</span></span>
* <span data-ttu-id="927ea-299">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-299">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="927ea-300">RBAC</span><span class="sxs-lookup"><span data-stu-id="927ea-300">RBAC</span></span>
* <span data-ttu-id="927ea-301">`role assignment`에 관리 그룹 범위가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-301">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-302">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-302">Storage</span></span>
* <span data-ttu-id="927ea-303">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-303">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="927ea-304">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="927ea-304">Compute</span></span>
* <span data-ttu-id="927ea-305">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-305">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="927ea-306">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-306">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="927ea-307">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="927ea-307">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="927ea-308">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-308">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="927ea-309">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="927ea-309">May 6, 2019</span></span>

<span data-ttu-id="927ea-310">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="927ea-310">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-311">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-311">ACS</span></span>
* <span data-ttu-id="927ea-312">[호환성이 손상되는 변경] `openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-312">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="927ea-313">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-313">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="927ea-314">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-314">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="927ea-315">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-315">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-316">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-316">Appservice</span></span>
* <span data-ttu-id="927ea-317">[사용 되지 않음] `functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-317">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="927ea-318">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-318">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="927ea-319">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-319">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="927ea-320">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-320">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="927ea-321">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-321">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="927ea-322">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-322">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="927ea-323">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-323">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="927ea-324">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-324">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="927ea-325">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-325">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="927ea-326">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-326">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-327">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-327">Batch</span></span>
* <span data-ttu-id="927ea-328">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-328">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-329">Botservice</span><span class="sxs-lookup"><span data-stu-id="927ea-329">Botservice</span></span>
* <span data-ttu-id="927ea-330">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="927ea-330">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="927ea-331">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-331">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="927ea-332">[호환성이 손상되는 변경] `--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-332">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="927ea-333">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="927ea-333">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="927ea-334">[호환성이 손상되는 변경] `--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-334">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="927ea-335">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="927ea-335">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="927ea-336">[호환성이 손상되는 변경] `bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-336">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="927ea-337">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-337">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="927ea-338">[호환성이 손상되는 변경] `bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-338">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="927ea-339">[호환성이 손상되는 변경] `bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-339">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="927ea-340">[호환성이 손상되는 변경] `bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-340">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="927ea-341">[호환성이 손상되는 변경] `--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-341">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="927ea-342">[호환성이 손상되는 변경] `Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-342">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="927ea-343">[호환성이 손상되는 변경] `bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-343">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="927ea-344">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="927ea-344">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="927ea-345">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-345">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="927ea-346">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-346">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="927ea-347">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-347">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="927ea-348">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-348">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="927ea-349">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-349">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="927ea-350">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-350">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="927ea-351">구성</span><span class="sxs-lookup"><span data-stu-id="927ea-351">Configure</span></span>
* <span data-ttu-id="927ea-352">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-352">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="927ea-353">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="927ea-353">Eventhubs</span></span>
* <span data-ttu-id="927ea-354">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-354">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="927ea-355">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-355">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-356">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-356">Network</span></span>
* <span data-ttu-id="927ea-357">[호환성이 손상되는 변경] `vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="927ea-357">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="927ea-358">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="927ea-358">Policy Insights</span></span>
* <span data-ttu-id="927ea-359">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-359">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="927ea-360">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-360">Role</span></span>
* <span data-ttu-id="927ea-361">[사용 되지 않음] `create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-361">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="927ea-362">Service Bus</span><span class="sxs-lookup"><span data-stu-id="927ea-362">Service Bus</span></span>
* <span data-ttu-id="927ea-363">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-363">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="927ea-364">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-364">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="927ea-365">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-365">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-366">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-366">SQL</span></span>
* <span data-ttu-id="927ea-367">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-367">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-368">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-368">VM</span></span>
* <span data-ttu-id="927ea-369">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-369">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="927ea-370">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-370">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="927ea-371">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-371">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="927ea-372">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-372">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="927ea-373">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-373">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="927ea-374">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-374">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="927ea-375">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="927ea-375">April 23, 2019</span></span>

<span data-ttu-id="927ea-376">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="927ea-376">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-377">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-377">ACS</span></span>
* <span data-ttu-id="927ea-378">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-378">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="927ea-379">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-379">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-380">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-380">AMS</span></span>
* <span data-ttu-id="927ea-381">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-381">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-382">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-382">AppService</span></span>
* <span data-ttu-id="927ea-383">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-383">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="927ea-384">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-384">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="927ea-385">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-385">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="927ea-386">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-386">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="927ea-387">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-387">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="927ea-388">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-388">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="927ea-389">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-389">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="927ea-390">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-390">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="927ea-391">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-391">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="927ea-392">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="927ea-392">Deployment Manager</span></span>
* <span data-ttu-id="927ea-393">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="927ea-393">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="927ea-394">랩</span><span class="sxs-lookup"><span data-stu-id="927ea-394">Lab</span></span>
* <span data-ttu-id="927ea-395">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-395">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="927ea-396">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-396">Network</span></span>
* <span data-ttu-id="927ea-397">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-397">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-398">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-398">Resource</span></span>
* <span data-ttu-id="927ea-399">[사용 되지 않음] `resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="927ea-399">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="927ea-400">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="927ea-400">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="927ea-401">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-401">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="927ea-402">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-402">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-403">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-403">SQL</span></span>
* <span data-ttu-id="927ea-404">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-404">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="927ea-405">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-405">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="927ea-406">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-406">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="927ea-407">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-407">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-408">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-408">Storage</span></span>
* <span data-ttu-id="927ea-409">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-409">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-410">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-410">VM</span></span>
* <span data-ttu-id="927ea-411">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-411">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="927ea-412">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-412">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="927ea-413">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-413">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="927ea-414">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="927ea-414">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="927ea-415">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-415">Core</span></span>
* <span data-ttu-id="927ea-416">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-416">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-417">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-417">ACR</span></span>
* <span data-ttu-id="927ea-418">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-418">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-419">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-419">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="927ea-422">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-422">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="927ea-423">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-423">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-424">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-424">AppService</span></span>
* <span data-ttu-id="927ea-425">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-425">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="927ea-426">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-426">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="927ea-427">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="927ea-427">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="927ea-428">[호환성이 손상되는 변경] `devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="927ea-428">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="927ea-429">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-429">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="927ea-430">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-430">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="927ea-431">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-431">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-432">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-432">CDN</span></span>
* <span data-ttu-id="927ea-433">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-433">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="927ea-434">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="927ea-434">Feedback</span></span>
* <span data-ttu-id="927ea-435">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-435">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="927ea-436">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-436">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="927ea-437">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-437">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-438">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-438">Monitor</span></span>
* <span data-ttu-id="927ea-439">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-439">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="927ea-440">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-440">Network</span></span>
* <span data-ttu-id="927ea-441">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-441">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="927ea-442">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-442">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="927ea-443">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-443">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="927ea-444">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-444">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="927ea-445">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="927ea-445">PrivateDNS</span></span>
* <span data-ttu-id="927ea-446">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-446">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-447">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-447">Resource</span></span>
* <span data-ttu-id="927ea-448">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-448">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="927ea-449">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-449">Role</span></span>
* <span data-ttu-id="927ea-450">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-450">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="927ea-451">[호환성이 손상되는 변경] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-451">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-452">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-452">SQL</span></span>
* <span data-ttu-id="927ea-453">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-453">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-454">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-454">Storage</span></span>
* <span data-ttu-id="927ea-455">[호환성이 손상되는 변경] `storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-455">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="927ea-456">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-456">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="927ea-457">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-457">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="927ea-458">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-458">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="927ea-459">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="927ea-459">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="927ea-460">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-460">Core</span></span>
* <span data-ttu-id="927ea-461">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-461">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="927ea-462">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-462">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="927ea-463">클라우드</span><span class="sxs-lookup"><span data-stu-id="927ea-463">Cloud</span></span>
* <span data-ttu-id="927ea-464">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-464">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-465">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-465">ACR</span></span>
* <span data-ttu-id="927ea-466">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-466">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="927ea-467">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-467">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="927ea-468">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-468">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="927ea-469">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-469">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-470">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-470">AppService</span></span>
* <span data-ttu-id="927ea-471">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-471">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="927ea-472">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-472">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="927ea-473">BOT Service</span><span class="sxs-lookup"><span data-stu-id="927ea-473">BOT Service</span></span>
* <span data-ttu-id="927ea-474">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-474">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="927ea-475">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-475">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="927ea-476">[호환성이 손상되는 변경] `bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-476">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="927ea-477">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-477">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-478">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-478">CDN</span></span>
* <span data-ttu-id="927ea-479">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-479">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [호환성이 손상되는 변경]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="927ea-481">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-481">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="927ea-482">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-482">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-483">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="927ea-483">Cosmosdb</span></span>
* <span data-ttu-id="927ea-484">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-484">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="927ea-485">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-485">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-486">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-486">Interactive</span></span>
* <span data-ttu-id="927ea-487">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-487">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-488">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-488">Monitor</span></span>
* <span data-ttu-id="927ea-489">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-489">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-490">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-490">Network</span></span>
* <span data-ttu-id="927ea-491">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-491">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-492">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-492">Profile</span></span>
* <span data-ttu-id="927ea-493">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-493">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="927ea-494">Postgres</span><span class="sxs-lookup"><span data-stu-id="927ea-494">Postgres</span></span> 
* <span data-ttu-id="927ea-495">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-495">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="927ea-496">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-496">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-497">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-497">Resource</span></span>
* <span data-ttu-id="927ea-498">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-498">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="927ea-499">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-499">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="927ea-500">그래프</span><span class="sxs-lookup"><span data-stu-id="927ea-500">Graph</span></span>
* <span data-ttu-id="927ea-501">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-501">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="927ea-502">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-502">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="927ea-503">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-503">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="927ea-504">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-504">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="927ea-505">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-505">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-506">저장소</span><span class="sxs-lookup"><span data-stu-id="927ea-506">storage</span></span>
* <span data-ttu-id="927ea-507">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-507">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="927ea-508">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-508">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="927ea-509">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-509">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="927ea-510">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-510">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-511">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-511">VM</span></span>
* <span data-ttu-id="927ea-512">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-512">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="927ea-513">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="927ea-513">March 12, 2019</span></span>

<span data-ttu-id="927ea-514">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="927ea-514">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="927ea-515">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-515">Core</span></span>

* <span data-ttu-id="927ea-516">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-516">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-517">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-517">ACR</span></span>

* <span data-ttu-id="927ea-518">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-518">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-519">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-519">ACS</span></span>

* <span data-ttu-id="927ea-520">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-520">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="927ea-521">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-521">AppService</span></span>

* <span data-ttu-id="927ea-522">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-522">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="927ea-523">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="927ea-523">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="927ea-524">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-524">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="927ea-525">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-525">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-526">Botservice</span><span class="sxs-lookup"><span data-stu-id="927ea-526">Botservice</span></span>

* <span data-ttu-id="927ea-527">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-527">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="927ea-528">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-528">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="927ea-529">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-529">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="927ea-530">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-530">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="927ea-531">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-531">Container</span></span>

* <span data-ttu-id="927ea-532">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-532">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="927ea-533">EventHub</span><span class="sxs-lookup"><span data-stu-id="927ea-533">EventHub</span></span>

* <span data-ttu-id="927ea-534">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-534">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="927ea-535">찾기</span><span class="sxs-lookup"><span data-stu-id="927ea-535">Find</span></span>

* <span data-ttu-id="927ea-536">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-536">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-537">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-537">HDInsight</span></span>

* <span data-ttu-id="927ea-538">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-538">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="927ea-539">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-539">Network</span></span>

* <span data-ttu-id="927ea-540">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-540">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-541">Rdbms</span><span class="sxs-lookup"><span data-stu-id="927ea-541">Rdbms</span></span>

* <span data-ttu-id="927ea-542">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-542">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="927ea-543">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-543">Role</span></span>

* <span data-ttu-id="927ea-544">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-544">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="927ea-545">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-545">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="927ea-546">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="927ea-546">Service Fabric</span></span>

* <span data-ttu-id="927ea-547">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-547">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="927ea-548">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="927ea-548">February 26, 2019</span></span>

<span data-ttu-id="927ea-549">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="927ea-549">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="927ea-550">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-550">Core</span></span>

* <span data-ttu-id="927ea-551">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-551">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-552">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-552">ACR</span></span>

* <span data-ttu-id="927ea-553">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-553">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="927ea-554">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-554">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-555">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-555">ACS</span></span>

* <span data-ttu-id="927ea-556">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-556">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-557">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-557">AppService</span></span>

* <span data-ttu-id="927ea-558">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-558">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-559">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-559">Batch</span></span>
* <span data-ttu-id="927ea-560">[호환성이 손상되는 변경] `batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-560">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="927ea-561">[호환성이 손상되는 변경] `Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-561">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="927ea-562">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-562">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="927ea-563">[호환성이 손상되는 변경] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-563">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="927ea-564">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-564">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="927ea-565">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-565">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-566">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-566">CosmosDB</span></span>

* <span data-ttu-id="927ea-567">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-567">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="927ea-568">Kusto</span><span class="sxs-lookup"><span data-stu-id="927ea-568">Kusto</span></span>

* <span data-ttu-id="927ea-569">[호환성이 손상되는 변경] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-569">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="927ea-570">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-570">Network</span></span>

* <span data-ttu-id="927ea-571">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-571">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="927ea-572">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-572">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="927ea-573">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-573">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="927ea-574">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="927ea-574">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="927ea-575">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-575">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="927ea-576">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-576">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="927ea-577">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-577">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-578">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-578">Resource</span></span>

* <span data-ttu-id="927ea-579">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-579">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="927ea-580">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-580">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="927ea-581">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-581">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="927ea-582">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-582">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="927ea-583">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-583">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="927ea-584">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-584">Role</span></span>

* <span data-ttu-id="927ea-585">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-585">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-586">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-586">VM</span></span>

* <span data-ttu-id="927ea-587">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-587">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="927ea-588">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="927ea-588">February 12, 2019</span></span>

<span data-ttu-id="927ea-589">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="927ea-589">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="927ea-590">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-590">Core</span></span>

* <span data-ttu-id="927ea-591">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-591">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="927ea-592">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-592">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-593">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-593">ACR</span></span>
* <span data-ttu-id="927ea-594">[호환성이 손상되는 변경] `acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-594">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="927ea-595">[호환성이 손상되는 변경] `acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-595">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-596">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-596">ACS</span></span>
* <span data-ttu-id="927ea-597">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-597">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="927ea-598">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-598">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="927ea-599">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-599">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-600">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-600">AMS</span></span>
* <span data-ttu-id="927ea-601">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-601">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="927ea-602">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-602">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-603">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-603">Appservice</span></span>
* <span data-ttu-id="927ea-604">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-604">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="927ea-605">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-605">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="927ea-606">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-606">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="927ea-607">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-607">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="927ea-608">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-608">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-609">Botservice</span><span class="sxs-lookup"><span data-stu-id="927ea-609">Botservice</span></span>
* <span data-ttu-id="927ea-610">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-610">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="927ea-611">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-611">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="927ea-612">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-612">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="927ea-613">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-613">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="927ea-614">[사용 되지 않음] `--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-614">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="927ea-615">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-615">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="927ea-616">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-616">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="927ea-617">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-617">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="927ea-618">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-618">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="927ea-619">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-619">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="927ea-620">Key Vault</span><span class="sxs-lookup"><span data-stu-id="927ea-620">Key Vault</span></span>
* <span data-ttu-id="927ea-621">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-621">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-622">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-622">Monitor</span></span>
* <span data-ttu-id="927ea-623">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-623">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-624">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-624">Network</span></span>
* <span data-ttu-id="927ea-625">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-625">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="927ea-626">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-626">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="927ea-627">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-627">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="927ea-628">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-628">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="927ea-629">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="927ea-629">Policy Insights</span></span>
* <span data-ttu-id="927ea-630">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-630">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-631">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-631">RDBMS</span></span>
* <span data-ttu-id="927ea-632">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-632">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="927ea-633">Redis</span><span class="sxs-lookup"><span data-stu-id="927ea-633">Redis</span></span>
* <span data-ttu-id="927ea-634">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-634">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="927ea-635">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-635">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="927ea-636">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-636">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="927ea-637">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-637">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="927ea-638">[호환성이 손상되는 변경] `redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-638">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="927ea-639">[호환성이 손상되는 변경] `redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-639">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="927ea-640">[사용 되지 않음] `redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-640">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="927ea-641">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-641">Role</span></span>
* <span data-ttu-id="927ea-642">[호환성이 손상되는 변경] `vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-642">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="927ea-643">SQL VM</span><span class="sxs-lookup"><span data-stu-id="927ea-643">SQL VM</span></span>
* <span data-ttu-id="927ea-644">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-644">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-645">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-645">VM</span></span>
* <span data-ttu-id="927ea-646">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-646">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="927ea-647">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-647">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="927ea-648">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-648">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="927ea-649">[호환성이 손상되는 변경] `az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-649">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="927ea-650">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="927ea-650">January 31, 2019</span></span>

<span data-ttu-id="927ea-651">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="927ea-651">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="927ea-652">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-652">Core</span></span>

* <span data-ttu-id="927ea-653">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-653">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="927ea-654">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="927ea-654">January 28, 2019</span></span>

<span data-ttu-id="927ea-655">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="927ea-655">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-656">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-656">ACR</span></span>
* <span data-ttu-id="927ea-657">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-657">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-658">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-658">ACS</span></span>
* <span data-ttu-id="927ea-659">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-659">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="927ea-660">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-660">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="927ea-661">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-661">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-662">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-662">AMS</span></span>
* <span data-ttu-id="927ea-663">[호환성이 손상되는 변경] `ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-663">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="927ea-664">[호환성이 손상되는 변경] `ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-664">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-665">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-665">Appservice</span></span>
* <span data-ttu-id="927ea-666">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-666">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="927ea-667">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-667">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="927ea-668">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-668">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="927ea-669">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-669">Container</span></span>
* <span data-ttu-id="927ea-670">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-670">Added `container start` command</span></span>
* <span data-ttu-id="927ea-671">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-671">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="927ea-672">EventGrid</span><span class="sxs-lookup"><span data-stu-id="927ea-672">EventGrid</span></span>
* <span data-ttu-id="927ea-673">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-673">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="927ea-674">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-674">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="927ea-675">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-675">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="927ea-676">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-676">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="927ea-677">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-677">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-678">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-678">HDInsight</span></span>
* <span data-ttu-id="927ea-679">[호환성이 손상되는 변경] `hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-679">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="927ea-680">[호환성이 손상되는 변경] `hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-680">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="927ea-681">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-681">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="927ea-682">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-682">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="927ea-683">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-683">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="927ea-684">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-684">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-685">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-685">IoT</span></span>
* <span data-ttu-id="927ea-686">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-686">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="927ea-687">Kusto</span><span class="sxs-lookup"><span data-stu-id="927ea-687">Kusto</span></span>
* <span data-ttu-id="927ea-688">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-688">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-689">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-689">Monitor</span></span>
* <span data-ttu-id="927ea-690">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-690">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-691">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-691">Profile</span></span>
* <span data-ttu-id="927ea-692">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-692">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-693">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-693">Network</span></span>
* <span data-ttu-id="927ea-694">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-694">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="927ea-695">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-695">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-696">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-696">Resource</span></span>
* <span data-ttu-id="927ea-697">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-697">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="927ea-698">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-698">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="927ea-699">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="927ea-699">SQL Virtual Machine</span></span>
* <span data-ttu-id="927ea-700">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-700">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-701">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-701">Storage</span></span>
* <span data-ttu-id="927ea-702">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-702">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="927ea-703">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-703">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-704">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-704">VM</span></span>
* <span data-ttu-id="927ea-705">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-705">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="927ea-706">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-706">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="927ea-707">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="927ea-707">January 15, 2019</span></span>

<span data-ttu-id="927ea-708">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="927ea-708">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-709">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-709">ACR</span></span>
* <span data-ttu-id="927ea-710">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-710">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="927ea-711">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-711">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="927ea-712">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="927ea-712">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="927ea-713">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-713">ACS</span></span>
* <span data-ttu-id="927ea-714">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-714">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-715">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-715">Appservice</span></span>
* <span data-ttu-id="927ea-716">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-716">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="927ea-717">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-717">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="927ea-718">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-718">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="927ea-719">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-719">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-720">Botservice</span><span class="sxs-lookup"><span data-stu-id="927ea-720">Botservice</span></span>
* <span data-ttu-id="927ea-721">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-721">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="927ea-722">구성</span><span class="sxs-lookup"><span data-stu-id="927ea-722">Configure</span></span>
* <span data-ttu-id="927ea-723">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-723">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-724">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-724">CosmosDB</span></span>
* <span data-ttu-id="927ea-725">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-725">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-726">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-726">HDInsight</span></span>
* <span data-ttu-id="927ea-727">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-727">Added commands for managing applications</span></span>
* <span data-ttu-id="927ea-728">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-728">Added commands for managing script actions</span></span>
* <span data-ttu-id="927ea-729">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-729">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="927ea-730">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-730">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="927ea-731">[호환성이 손상되는 변경] `hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-731">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-732">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-732">Network</span></span>
* <span data-ttu-id="927ea-733">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-733">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="927ea-734">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-734">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="927ea-735">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-735">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="927ea-736">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-736">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="927ea-737">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-737">Role</span></span>
* <span data-ttu-id="927ea-738">[사용 되지 않음] `create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-738">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="927ea-739">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-739">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="927ea-740">보안</span><span class="sxs-lookup"><span data-stu-id="927ea-740">Security</span></span>
* <span data-ttu-id="927ea-741">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-741">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-742">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-742">Storage</span></span>
* <span data-ttu-id="927ea-743">[호환성이 손상되는 변경] `storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-743">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="927ea-744">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-744">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="927ea-745">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-745">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="927ea-746">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-746">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="927ea-747">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-747">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-748">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-748">VM</span></span>
* <span data-ttu-id="927ea-749">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-749">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="927ea-750">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-750">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="927ea-751">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-751">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="927ea-752">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-752">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="927ea-753">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-753">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="927ea-754">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-754">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="927ea-755">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="927ea-755">December 20, 2018</span></span>

<span data-ttu-id="927ea-756">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="927ea-756">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="927ea-757">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-757">Appservice</span></span>
* <span data-ttu-id="927ea-758">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-758">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="927ea-759">웹앱 스냅숏 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-759">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="927ea-760">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-760">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="927ea-761">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="927ea-761">IoTCentral</span></span>
* <span data-ttu-id="927ea-762">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-762">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="927ea-763">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-763">Role</span></span>
* <span data-ttu-id="927ea-764">[호환성이 손상되는 변경] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-764">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-765">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-765">SQL</span></span>
* <span data-ttu-id="927ea-766">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-766">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-767">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-767">VM</span></span>
* <span data-ttu-id="927ea-768">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-768">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="927ea-769">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="927ea-769">December 18, 2018</span></span>

<span data-ttu-id="927ea-770">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="927ea-770">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="927ea-771">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-771">ACR</span></span>
* <span data-ttu-id="927ea-772">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-772">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="927ea-773">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="927ea-773">Condensed the table layout for task list</span></span>
* <span data-ttu-id="927ea-774">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-774">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-775">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-775">ACS</span></span>
* <span data-ttu-id="927ea-776">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-776">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="927ea-777">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="927ea-777">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="927ea-778">[사용 되지 않음] `az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-778">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="927ea-779">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-779">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="927ea-780">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-780">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="927ea-781">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="927ea-781">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-782">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-782">Appservice</span></span>
* <span data-ttu-id="927ea-783">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-783">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="927ea-784">Botservice</span><span class="sxs-lookup"><span data-stu-id="927ea-784">Botservice</span></span>
* <span data-ttu-id="927ea-785">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-785">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="927ea-786">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="927ea-786">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="927ea-787">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="927ea-787">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="927ea-788">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="927ea-788">Reduced Kudu network calls</span></span>
* <span data-ttu-id="927ea-789">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-789">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-790">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-790">Consumption</span></span>
* <span data-ttu-id="927ea-791">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-791">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-792">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-792">CosmosDB</span></span>
* <span data-ttu-id="927ea-793">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-793">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="927ea-794">지도</span><span class="sxs-lookup"><span data-stu-id="927ea-794">Maps</span></span>
* <span data-ttu-id="927ea-795">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-795">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-796">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-796">Network</span></span>
* <span data-ttu-id="927ea-797">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-797">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="927ea-798">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="927ea-798">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-799">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-799">Resource</span></span>
* <span data-ttu-id="927ea-800">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-800">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="927ea-801">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-801">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-802">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-802">Storage</span></span>
*  <span data-ttu-id="927ea-803">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-803">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-804">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-804">VM</span></span>
* <span data-ttu-id="927ea-805">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-805">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="927ea-806">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="927ea-806">December 4, 2018</span></span>

<span data-ttu-id="927ea-807">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="927ea-807">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="927ea-808">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-808">Core</span></span>
* <span data-ttu-id="927ea-809">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-809">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="927ea-810">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-810">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-811">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-811">Appservice</span></span>
* <span data-ttu-id="927ea-812">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-812">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="927ea-813">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-813">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="927ea-814">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-814">Network</span></span>
* <span data-ttu-id="927ea-815">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-815">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="927ea-816">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-816">Role</span></span>
* <span data-ttu-id="927ea-817">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-817">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="927ea-818">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-818">VM</span></span>
* <span data-ttu-id="927ea-819">[사용 되지 않음] `vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-819">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="927ea-820">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-820">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="927ea-821">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-821">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="927ea-822">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-822">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="927ea-823">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="927ea-823">November 20, 2018</span></span>

<span data-ttu-id="927ea-824">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="927ea-824">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="927ea-825">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-825">Core</span></span>
* <span data-ttu-id="927ea-826">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-826">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-827">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-827">ACR</span></span>
* <span data-ttu-id="927ea-828">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-828">Added context token to task step</span></span>
* <span data-ttu-id="927ea-829">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-829">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="927ea-830">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-830">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-831">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-831">Appservice</span></span>
* <span data-ttu-id="927ea-832">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-832">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="927ea-833">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-833">Updated the default `node_version`.</span></span> <span data-ttu-id="927ea-834">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-834">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="927ea-835">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-835">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="927ea-836">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-836">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="927ea-837">IotCentral</span><span class="sxs-lookup"><span data-stu-id="927ea-837">IotCentral</span></span>
* <span data-ttu-id="927ea-838">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-838">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-839">KeyVault</span><span class="sxs-lookup"><span data-stu-id="927ea-839">KeyVault</span></span>
* <span data-ttu-id="927ea-840">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-840">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="927ea-841">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-841">Network</span></span>
* <span data-ttu-id="927ea-842">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-842">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="927ea-843">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="927ea-843">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="927ea-844">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-844">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="927ea-845">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="927ea-845">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-846">Rdbms</span><span class="sxs-lookup"><span data-stu-id="927ea-846">Rdbms</span></span>
* <span data-ttu-id="927ea-847">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-847">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="927ea-848">Rbac</span><span class="sxs-lookup"><span data-stu-id="927ea-848">Rbac</span></span>
* <span data-ttu-id="927ea-849">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-849">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="927ea-850">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-850">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="927ea-851">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-851">Storage</span></span>
* <span data-ttu-id="927ea-852">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-852">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="927ea-853">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-853">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="927ea-854">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-854">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="927ea-855">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-855">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-856">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-856">VM</span></span>
* <span data-ttu-id="927ea-857">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-857">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="927ea-858">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-858">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="927ea-859">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="927ea-859">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="927ea-860">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-860">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="927ea-861">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-861">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="927ea-862">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-862">Added `snapshot wait` command</span></span>
* <span data-ttu-id="927ea-863">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-863">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="927ea-864">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="927ea-864">November 6, 2018</span></span>

<span data-ttu-id="927ea-865">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="927ea-865">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="927ea-866">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-866">Core</span></span>
* <span data-ttu-id="927ea-867">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-867">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-868">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-868">ACR</span></span>
* <span data-ttu-id="927ea-869">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-869">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="927ea-870">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-870">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-871">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-871">ACS</span></span>
* <span data-ttu-id="927ea-872">[호환성이 손상되는 변경] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-872">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="927ea-873">Advisor</span><span class="sxs-lookup"><span data-stu-id="927ea-873">Advisor</span></span>
* <span data-ttu-id="927ea-874">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-874">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-875">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-875">AMS</span></span>
* <span data-ttu-id="927ea-876">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="927ea-876">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="927ea-877">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="927ea-877">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="927ea-878">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-878">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="927ea-879">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-879">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="927ea-880">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-880">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="927ea-881">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-881">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="927ea-882">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-882">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="927ea-883">[호환성이 손상되는 변경] `ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="927ea-883">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="927ea-884">[호환성이 손상되는 변경] `ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-884">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="927ea-885">[호환성이 손상되는 변경] `ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-885">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="927ea-886">[호환성이 손상되는 변경] `ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="927ea-886">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="927ea-887">[호환성이 손상되는 변경] `ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="927ea-887">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="927ea-888">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="927ea-888">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="927ea-889">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="927ea-889">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="927ea-890">[호환성이 손상되는 변경] `ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-890">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="927ea-891">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-891">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="927ea-892">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-892">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-893">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-893">AppService</span></span>
* <span data-ttu-id="927ea-894">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-894">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="927ea-895">구성</span><span class="sxs-lookup"><span data-stu-id="927ea-895">Configure</span></span>
* <span data-ttu-id="927ea-896">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-896">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="927ea-897">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-897">Container</span></span>
* <span data-ttu-id="927ea-898">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-898">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="927ea-899">EventHub</span><span class="sxs-lookup"><span data-stu-id="927ea-899">EventHub</span></span>
* <span data-ttu-id="927ea-900">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-900">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-901">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-901">Interactive</span></span>
* <span data-ttu-id="927ea-902">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-902">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-903">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-903">Monitor</span></span>
* <span data-ttu-id="927ea-904">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-904">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-905">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-905">Network</span></span>
* <span data-ttu-id="927ea-906">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-906">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="927ea-907">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-907">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="927ea-908">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-908">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="927ea-909">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-909">Profile</span></span>
* <span data-ttu-id="927ea-910">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-910">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-911">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-911">RDBMS</span></span>
* <span data-ttu-id="927ea-912">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-912">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-913">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-913">Resource</span></span>
* <span data-ttu-id="927ea-914">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-914">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="927ea-915">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-915">Role</span></span>
* <span data-ttu-id="927ea-916">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-916">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="927ea-917">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-917">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="927ea-918">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-918">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-919">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-919">Storage</span></span>
* <span data-ttu-id="927ea-920">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-920">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-921">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-921">VM</span></span>
* <span data-ttu-id="927ea-922">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-922">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="927ea-923">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-923">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="927ea-924">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-924">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="927ea-925">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-925">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="927ea-926">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="927ea-926">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="927ea-927">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-927">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="927ea-928">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="927ea-928">October 23, 2018</span></span>

<span data-ttu-id="927ea-929">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="927ea-929">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="927ea-930">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-930">Core</span></span>
* <span data-ttu-id="927ea-931">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-931">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="927ea-932">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-932">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-933">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-933">ACR</span></span>
* <span data-ttu-id="927ea-934">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-934">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-935">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-935">CDN</span></span>
* <span data-ttu-id="927ea-936">[호환성이 손상되는 변경] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-936">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="927ea-937">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-937">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="927ea-938">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-938">Container</span></span>
* <span data-ttu-id="927ea-939">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-939">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="927ea-940">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-940">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="927ea-941">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-941">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="927ea-942">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-942">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="927ea-943">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-943">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="927ea-944">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-944">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="927ea-945">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-945">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-946">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-946">CosmosDB</span></span>
* <span data-ttu-id="927ea-947">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-947">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-948">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-948">Interactive</span></span>
* <span data-ttu-id="927ea-949">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-949">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="927ea-950">IoT Central</span><span class="sxs-lookup"><span data-stu-id="927ea-950">IoT Central</span></span>
* <span data-ttu-id="927ea-951">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-951">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="927ea-952">[호환성이 손상되는 변경] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-952">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-953">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-953">Monitor</span></span>
* <span data-ttu-id="927ea-954">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="927ea-954">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="927ea-955">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-955">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="927ea-956">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-956">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="927ea-957">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-957">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="927ea-958">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-958">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="927ea-959">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-959">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="927ea-960">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="927ea-960">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="927ea-961">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-961">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="927ea-962">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-962">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="927ea-963">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-963">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-964">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-964">Network</span></span>
* <span data-ttu-id="927ea-965">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-965">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="927ea-966">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-966">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="927ea-967">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="927ea-967">ServiceBus</span></span>
* <span data-ttu-id="927ea-968">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-968">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-969">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-969">SQL</span></span>
* <span data-ttu-id="927ea-970">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-970">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-971">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-971">Storage</span></span>
* <span data-ttu-id="927ea-972">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-972">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="927ea-973">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-973">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-974">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-974">VM</span></span>
* <span data-ttu-id="927ea-975">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-975">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="927ea-976">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-976">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="927ea-977">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-977">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="927ea-978">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="927ea-978">October 16, 2018</span></span>

<span data-ttu-id="927ea-979">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="927ea-979">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-980">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-980">VM</span></span>
* <span data-ttu-id="927ea-981">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-981">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="927ea-982">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="927ea-982">October 9, 2018</span></span>

<span data-ttu-id="927ea-983">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="927ea-983">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="927ea-984">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-984">Core</span></span>
* <span data-ttu-id="927ea-985">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-985">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-986">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-986">ACR</span></span>
* <span data-ttu-id="927ea-987">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-987">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-988">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-988">ACS</span></span>
* <span data-ttu-id="927ea-989">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="927ea-989">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="927ea-990">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-990">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="927ea-991">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-991">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="927ea-992">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-992">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="927ea-993">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-993">Container</span></span>
* <span data-ttu-id="927ea-994">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-994">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="927ea-995">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-995">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="927ea-996">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="927ea-996">Event Hub</span></span>
* <span data-ttu-id="927ea-997">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-997">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="927ea-998">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-998">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="927ea-999">확장</span><span class="sxs-lookup"><span data-stu-id="927ea-999">Extensions</span></span>
* <span data-ttu-id="927ea-1000">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1000">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="927ea-1001">HDInsight</span><span class="sxs-lookup"><span data-stu-id="927ea-1001">HDInsight</span></span>
* <span data-ttu-id="927ea-1002">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1002">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1003">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1003">IoT</span></span>
* <span data-ttu-id="927ea-1004">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1004">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-1005">KeyVault</span><span class="sxs-lookup"><span data-stu-id="927ea-1005">KeyVault</span></span>
* <span data-ttu-id="927ea-1006">최신 API 프로필에 keyvault 저장소 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1006">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1007">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1007">Network</span></span>
* <span data-ttu-id="927ea-1008">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1008">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="927ea-1009">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="927ea-1009">See #6052</span></span>
* <span data-ttu-id="927ea-1010">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="927ea-1010">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="927ea-1011">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1011">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="927ea-1012">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1012">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="927ea-1013">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1013">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="927ea-1014">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1014">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="927ea-1015">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1015">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1016">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1016">Role</span></span>
* <span data-ttu-id="927ea-1017">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1017">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="927ea-1018">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1018">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="927ea-1019">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1019">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="927ea-1020">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1020">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="927ea-1021">Service Bus</span><span class="sxs-lookup"><span data-stu-id="927ea-1021">Service Bus</span></span>
* <span data-ttu-id="927ea-1022">[호환성이 손상되는 변경] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1022">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1023">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1023">VM</span></span>
* <span data-ttu-id="927ea-1024">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1024">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="927ea-1025">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1025">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="927ea-1026">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1026">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="927ea-1027">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1027">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="927ea-1028">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1028">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="927ea-1029">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1029">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="927ea-1030">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="927ea-1030">September 21, 2018</span></span>

<span data-ttu-id="927ea-1031">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="927ea-1031">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1032">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1032">ACR</span></span>
* <span data-ttu-id="927ea-1033">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1033">Added ACR Task commands</span></span>
* <span data-ttu-id="927ea-1034">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1034">Added quick run command</span></span>
* <span data-ttu-id="927ea-1035">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1035">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="927ea-1036">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1036">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="927ea-1037">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1037">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="927ea-1038">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1038">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1039">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1039">ACS</span></span>
* <span data-ttu-id="927ea-1040">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1040">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="927ea-1041">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1041">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1042">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1042">AppService</span></span>

* <span data-ttu-id="927ea-1043">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1043">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="927ea-1044">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1044">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="927ea-1045">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1045">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="927ea-1046">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1046">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1047">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1047">Batch</span></span>
* <span data-ttu-id="927ea-1048">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1048">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="927ea-1049">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1049">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="927ea-1050">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1050">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="927ea-1051">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1051">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="927ea-1052">Batch AI</span><span class="sxs-lookup"><span data-stu-id="927ea-1052">Batch AI</span></span> 
* <span data-ttu-id="927ea-1053">`batchai cluster create` 명령에서 자동 저장소 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1053">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="927ea-1054">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="927ea-1054">Cognitive Services</span></span>
* <span data-ttu-id="927ea-1055">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1055">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="927ea-1056">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1056">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="927ea-1057">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1057">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="927ea-1058">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1058">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="927ea-1059">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1059">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="927ea-1060">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1060">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1061">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1061">Container</span></span>
* <span data-ttu-id="927ea-1062">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1062">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="927ea-1063">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1063">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="927ea-1064">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1064">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="927ea-1065">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1065">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="927ea-1066">Datalake</span><span class="sxs-lookup"><span data-stu-id="927ea-1066">Datalake</span></span>
* <span data-ttu-id="927ea-1067">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1067">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="927ea-1068">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="927ea-1068">Interactive Shell</span></span>
* <span data-ttu-id="927ea-1069">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1069">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="927ea-1070">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1070">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1071">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1071">IoT</span></span>
* <span data-ttu-id="927ea-1072">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1072">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="927ea-1073">Key Vault</span><span class="sxs-lookup"><span data-stu-id="927ea-1073">Key Vault</span></span>
* <span data-ttu-id="927ea-1074">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1074">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1075">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1075">Network</span></span>
* <span data-ttu-id="927ea-1076">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1076">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="927ea-1077">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1077">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="927ea-1078">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1078">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="927ea-1079">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1079">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="927ea-1080">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1080">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="927ea-1081">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1081">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="927ea-1082">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1082">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="927ea-1083">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1083">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="927ea-1084">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1084">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="927ea-1085">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1085">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="927ea-1086">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1086">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="927ea-1087">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1087">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="927ea-1088">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1088">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="927ea-1089">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-1089">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="927ea-1090">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1090">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="927ea-1091">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1091">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="927ea-1092">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1092">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="927ea-1093">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1093">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-1094">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1094">RDBMS</span></span>
* <span data-ttu-id="927ea-1095">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1095">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="927ea-1096">예약</span><span class="sxs-lookup"><span data-stu-id="927ea-1096">Reservation</span></span>
* <span data-ttu-id="927ea-1097">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1097">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="927ea-1098">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1098">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="927ea-1099">앱 관리</span><span class="sxs-lookup"><span data-stu-id="927ea-1099">Manage App</span></span>
* <span data-ttu-id="927ea-1100">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1100">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="927ea-1101">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1101">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1102">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1102">Role</span></span>
* <span data-ttu-id="927ea-1103">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1103">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="927ea-1104">SignalR</span><span class="sxs-lookup"><span data-stu-id="927ea-1104">SignalR</span></span>
* <span data-ttu-id="927ea-1105">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1105">First release</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1106">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1106">Storage</span></span>
* <span data-ttu-id="927ea-1107">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1107">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="927ea-1108">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1108">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1109">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1109">VM</span></span>
* <span data-ttu-id="927ea-1110">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="927ea-1110">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="927ea-1111">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1111">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="927ea-1112">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="927ea-1112">August 28, 2018</span></span>

<span data-ttu-id="927ea-1113">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="927ea-1113">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1114">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1114">Core</span></span>

* <span data-ttu-id="927ea-1115">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1115">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="927ea-1116">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1116">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1117">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1117">ACR</span></span>

* <span data-ttu-id="927ea-1118">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1118">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="927ea-1119">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1119">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1120">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1120">ACS</span></span>

* <span data-ttu-id="927ea-1121">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1121">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="927ea-1122">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1122">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1123">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1123">AppService</span></span>

* <span data-ttu-id="927ea-1124">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1124">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="927ea-1125">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1125">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="927ea-1126">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1126">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="927ea-1127">Backup</span><span class="sxs-lookup"><span data-stu-id="927ea-1127">Backup</span></span>

* <span data-ttu-id="927ea-1128">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1128">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="927ea-1129">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="927ea-1129">Bot Service</span></span>

* <span data-ttu-id="927ea-1130">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1130">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="927ea-1131">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="927ea-1131">Cognitive Services</span></span>

* <span data-ttu-id="927ea-1132">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1132">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1133">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1133">IoT</span></span>

* <span data-ttu-id="927ea-1134">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1134">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1135">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1135">Monitor</span></span>

* <span data-ttu-id="927ea-1136">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1136">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="927ea-1137">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="927ea-1137">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1138">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1138">Network</span></span>

* <span data-ttu-id="927ea-1139">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1139">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1140">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1140">Resource</span></span>

* <span data-ttu-id="927ea-1141">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1141">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1142">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1142">Storage</span></span>

* <span data-ttu-id="927ea-1143">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1143">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1144">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1144">VM</span></span>

* <span data-ttu-id="927ea-1145">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1145">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="927ea-1146">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="927ea-1146">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="927ea-1147">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="927ea-1147">Auguest 14, 2018</span></span>

<span data-ttu-id="927ea-1148">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="927ea-1148">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1149">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1149">Core</span></span>

* <span data-ttu-id="927ea-1150">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1150">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="927ea-1151">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="927ea-1151">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="927ea-1152">원격 분석</span><span class="sxs-lookup"><span data-stu-id="927ea-1152">Telemetry</span></span>

* <span data-ttu-id="927ea-1153">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="927ea-1153">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1154">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1154">ACR</span></span>

* <span data-ttu-id="927ea-1155">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1155">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="927ea-1156">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1156">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1157">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1157">ACS</span></span>

* <span data-ttu-id="927ea-1158">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1158">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="927ea-1159">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1159">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="927ea-1160">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1160">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="927ea-1161">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1161">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="927ea-1162">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1162">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="927ea-1163">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1163">AppService</span></span>

* <span data-ttu-id="927ea-1164">외부 리소스 그룹에 저장소 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1164">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="927ea-1165">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1165">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-1166">BatchAI</span><span class="sxs-lookup"><span data-stu-id="927ea-1166">BatchAI</span></span>

* <span data-ttu-id="927ea-1167">자동 저장소 계정 만들기가 "리소스 *그룹*"을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1167">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="927ea-1168">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1168">Container</span></span>

* <span data-ttu-id="927ea-1169">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1169">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="927ea-1170">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1170">IoT</span></span>

* <span data-ttu-id="927ea-1171">[호환성이 손상되는 변경] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="927ea-1171">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="927ea-1172">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1172">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="927ea-1173">Iot Central</span><span class="sxs-lookup"><span data-stu-id="927ea-1173">Iot Central</span></span>

* <span data-ttu-id="927ea-1174">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1174">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-1175">KeyVault</span><span class="sxs-lookup"><span data-stu-id="927ea-1175">KeyVault</span></span>


* <span data-ttu-id="927ea-1176">저장소 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1176">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="927ea-1177">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1177">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="927ea-1178">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1178">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="927ea-1179">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1179">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="927ea-1180">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1180">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="927ea-1181">릴레이</span><span class="sxs-lookup"><span data-stu-id="927ea-1181">Relay</span></span>

* <span data-ttu-id="927ea-1182">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1182">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1183">Sql</span><span class="sxs-lookup"><span data-stu-id="927ea-1183">Sql</span></span>

* <span data-ttu-id="927ea-1184">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1184">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1185">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1185">Storage</span></span>

* <span data-ttu-id="927ea-1186">[호환성이 손상되는 변경] `--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1186">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="927ea-1187">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1187">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="927ea-1188">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1188">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="927ea-1189">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="927ea-1189">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="927ea-1190">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1190">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1191">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1191">VM</span></span>

* <span data-ttu-id="927ea-1192">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1192">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="927ea-1193">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="927ea-1193">July 31, 2018</span></span>

<span data-ttu-id="927ea-1194">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="927ea-1194">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1195">ACR</span></span>

* <span data-ttu-id="927ea-1196">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1196">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="927ea-1197">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1197">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1198">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1198">ACS</span></span>

* <span data-ttu-id="927ea-1199">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1199">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1200">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1200">Batch</span></span>

* <span data-ttu-id="927ea-1201">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1201">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1202">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1202">Container</span></span>

* <span data-ttu-id="927ea-1203">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1203">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1204">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1204">Network</span></span>

* <span data-ttu-id="927ea-1205">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1205">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="927ea-1206">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1206">Resource</span></span>

* <span data-ttu-id="927ea-1207">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="927ea-1207">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="927ea-1208">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1208">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1209">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1209">Role</span></span>

* <span data-ttu-id="927ea-1210">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1210">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="927ea-1211">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1211">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="927ea-1212">검색</span><span class="sxs-lookup"><span data-stu-id="927ea-1212">Search</span></span>

* <span data-ttu-id="927ea-1213">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1213">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="927ea-1214">Service Bus</span><span class="sxs-lookup"><span data-stu-id="927ea-1214">Service Bus</span></span>

* <span data-ttu-id="927ea-1215">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1215">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="927ea-1216">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1216">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="927ea-1217">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="927ea-1217">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="927ea-1218">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="927ea-1218">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1219">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1219">Storage</span></span>

* <span data-ttu-id="927ea-1220">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1220">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="927ea-1221">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="927ea-1221">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1222">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1222">VM</span></span>

* <span data-ttu-id="927ea-1223">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1223">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="927ea-1224">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1224">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="927ea-1225">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1225">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="927ea-1226">[호환성이 손상되는 변경] `[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1226">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="927ea-1227">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="927ea-1227">July 18, 2018</span></span>

<span data-ttu-id="927ea-1228">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="927ea-1228">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1229">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1229">Core</span></span>

* <span data-ttu-id="927ea-1230">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1230">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="927ea-1231">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1231">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="927ea-1232">[호환성이 손상되는 변경] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1232">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1233">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1233">ACR</span></span>

* <span data-ttu-id="927ea-1234">[호환성이 손상되는 변경] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1234">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="927ea-1235">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1235">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="927ea-1236">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1236">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="927ea-1237">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1237">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1238">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1238">ACS</span></span>

* <span data-ttu-id="927ea-1239">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1239">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1240">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1240">AppService</span></span>

* <span data-ttu-id="927ea-1241">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1241">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1242">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1242">Batch</span></span>

* <span data-ttu-id="927ea-1243">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1243">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="927ea-1244">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1244">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="927ea-1245">Batch AI</span><span class="sxs-lookup"><span data-stu-id="927ea-1245">Batch AI</span></span>

* <span data-ttu-id="927ea-1246">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1246">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1247">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1247">Container</span></span>

* <span data-ttu-id="927ea-1248">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1248">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="927ea-1249">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1249">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1250">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1250">Network</span></span>

* <span data-ttu-id="927ea-1251">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1251">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="927ea-1252">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1252">Added `network nic wait`</span></span>
* <span data-ttu-id="927ea-1253">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1253">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="927ea-1254">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1254">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="927ea-1255">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1255">Resource</span></span>

* <span data-ttu-id="927ea-1256">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1256">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="927ea-1257">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1257">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="927ea-1258">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1258">Added `deployment wait` command</span></span>
* <span data-ttu-id="927ea-1259">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1259">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1260">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1260">SQL</span></span>

* <span data-ttu-id="927ea-1261">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1261">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="927ea-1262">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1262">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="927ea-1263">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="927ea-1263">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1264">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1264">Storage</span></span>

* <span data-ttu-id="927ea-1265">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1265">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1266">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1266">VM</span></span>

* <span data-ttu-id="927ea-1267">[호환성이 손상되는 변경] `vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1267">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="927ea-1268">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1268">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="927ea-1269">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1269">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="927ea-1270">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="927ea-1270">July 3, 2018</span></span>

<span data-ttu-id="927ea-1271">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="927ea-1271">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="927ea-1272">AKS</span><span class="sxs-lookup"><span data-stu-id="927ea-1272">AKS</span></span>

* <span data-ttu-id="927ea-1273">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1273">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="927ea-1274">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="927ea-1274">July 3, 2018</span></span>

<span data-ttu-id="927ea-1275">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="927ea-1275">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1276">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1276">Core</span></span>

* <span data-ttu-id="927ea-1277">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1277">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1278">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1278">ACR</span></span>

* <span data-ttu-id="927ea-1279">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1279">Added polling build status</span></span>
* <span data-ttu-id="927ea-1280">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1280">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="927ea-1281">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1281">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1282">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1282">ACS</span></span>

* <span data-ttu-id="927ea-1283">[호환성이 손상되는 변경]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1283">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="927ea-1284">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1284">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="927ea-1285">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-1285">Updated options for `aks browse` command.</span></span> <span data-ttu-id="927ea-1286">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1286">Added `--listen-port` support</span></span>
* <span data-ttu-id="927ea-1287">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1287">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="927ea-1288">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-1288">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="927ea-1289">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1289">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1290">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1290">AppService</span></span>

* <span data-ttu-id="927ea-1291">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1291">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="927ea-1292">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1292">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="927ea-1293">Backup</span><span class="sxs-lookup"><span data-stu-id="927ea-1293">Backup</span></span>

* <span data-ttu-id="927ea-1294">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1294">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-1295">BatchAI</span><span class="sxs-lookup"><span data-stu-id="927ea-1295">BatchAI</span></span>

* <span data-ttu-id="927ea-1296">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1296">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="927ea-1297">클라우드</span><span class="sxs-lookup"><span data-stu-id="927ea-1297">Cloud</span></span>

* <span data-ttu-id="927ea-1298">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1298">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1299">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1299">Container</span></span>

* <span data-ttu-id="927ea-1300">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1300">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="927ea-1301">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1301">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="927ea-1302">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1302">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1303">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1303">Extension</span></span>

* <span data-ttu-id="927ea-1304">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1304">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1305">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1305">Network</span></span>

* <span data-ttu-id="927ea-1306">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="927ea-1306">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-1307">Rdbms</span><span class="sxs-lookup"><span data-stu-id="927ea-1307">Rdbms</span></span>

* <span data-ttu-id="927ea-1308">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1308">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1309">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1309">Resource</span></span>

* <span data-ttu-id="927ea-1310">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1310">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1311">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1311">VM</span></span>

* <span data-ttu-id="927ea-1312">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1312">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="927ea-1313">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="927ea-1313">June 25, 2018</span></span>

<span data-ttu-id="927ea-1314">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="927ea-1314">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="927ea-1315">CLI</span><span class="sxs-lookup"><span data-stu-id="927ea-1315">CLI</span></span>

* <span data-ttu-id="927ea-1316">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1316">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="927ea-1317">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="927ea-1317">June 19, 2018</span></span>

<span data-ttu-id="927ea-1318">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="927ea-1318">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1319">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1319">Core</span></span>

* <span data-ttu-id="927ea-1320">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1320">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1321">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1321">ACR</span></span>

* <span data-ttu-id="927ea-1322">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1322">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="927ea-1323">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1323">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1324">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1324">ACS</span></span>

* <span data-ttu-id="927ea-1325">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-1325">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="927ea-1326">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1326">Added `--update` support</span></span>
* <span data-ttu-id="927ea-1327">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1327">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="927ea-1328">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="927ea-1328">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="927ea-1329">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1329">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="927ea-1330">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1330">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="927ea-1331">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1331">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="927ea-1332">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1332">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1333">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1333">AppService</span></span>

* <span data-ttu-id="927ea-1334">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1334">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="927ea-1335">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1335">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1336">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1336">Batch</span></span>

* <span data-ttu-id="927ea-1337">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1337">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="927ea-1338">Batch AI</span><span class="sxs-lookup"><span data-stu-id="927ea-1338">Batch AI</span></span>

* <span data-ttu-id="927ea-1339">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="927ea-1339">Added support for workspaces.</span></span> <span data-ttu-id="927ea-1340">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1340">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="927ea-1341">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="927ea-1341">Added support for experiments.</span></span> <span data-ttu-id="927ea-1342">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1342">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="927ea-1343">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1343">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="927ea-1344">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-1344">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="927ea-1345">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1345">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="927ea-1346">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1346">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="927ea-1347">[호환성이 손상되는 변경] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="927ea-1347">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="927ea-1348">[호환성이 손상되는 변경] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="927ea-1348">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="927ea-1349">[호환성이 손상되는 변경] `cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="927ea-1349">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="927ea-1350">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="927ea-1350">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="927ea-1351">[호환성이 손상되는 변경] `job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="927ea-1351">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="927ea-1352">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="927ea-1352">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="927ea-1353">[호환성이 손상되는 변경] `location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="927ea-1353">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="927ea-1354">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1354">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="927ea-1355">[호환성이 손상되는 변경] `job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1355">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="927ea-1356">[호환성이 손상되는 변경] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="927ea-1356">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="927ea-1357">[`--config`, `-c`]를 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="927ea-1357">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="927ea-1358">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="927ea-1358">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="927ea-1359">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="927ea-1359">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="927ea-1360">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="927ea-1360">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="927ea-1361">지도</span><span class="sxs-lookup"><span data-stu-id="927ea-1361">Maps</span></span>

* <span data-ttu-id="927ea-1362">[호환성이 손상되는 변경] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1362">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1363">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1363">Network</span></span>

* <span data-ttu-id="927ea-1364">`https`에 대한 지원이 `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1364">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="927ea-1365">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1365">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="927ea-1366">#6502</span><span class="sxs-lookup"><span data-stu-id="927ea-1366">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="927ea-1367">예약</span><span class="sxs-lookup"><span data-stu-id="927ea-1367">Reservations</span></span>

* <span data-ttu-id="927ea-1368">[호환성이 손상되는 변경] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1368">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="927ea-1369">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1369">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="927ea-1370">[호환성이 손상되는 변경] `ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1370">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="927ea-1371">[호환성이 손상되는 변경] `Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1371">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="927ea-1372">[호환성이 손상되는 변경] `Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1372">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="927ea-1373">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1373">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1374">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1374">Role</span></span>

* <span data-ttu-id="927ea-1375">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="927ea-1375">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1376">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1376">SQL</span></span>

* <span data-ttu-id="927ea-1377">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1377">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1378">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1378">Storage</span></span>

* <span data-ttu-id="927ea-1379">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1379">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1380">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1380">VM</span></span>

* <span data-ttu-id="927ea-1381">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-1381">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="927ea-1382">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1382">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="927ea-1383">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1383">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="927ea-1384">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="927ea-1384">June 13, 2018</span></span>

<span data-ttu-id="927ea-1385">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="927ea-1385">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1386">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1386">Core</span></span>

* <span data-ttu-id="927ea-1387">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="927ea-1387">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="927ea-1388">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="927ea-1388">June 13, 2018</span></span>

<span data-ttu-id="927ea-1389">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="927ea-1389">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="927ea-1390">AKS</span><span class="sxs-lookup"><span data-stu-id="927ea-1390">AKS</span></span>

* <span data-ttu-id="927ea-1391">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1391">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="927ea-1392">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="927ea-1392">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="927ea-1393">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1393">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="927ea-1394">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1394">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="927ea-1395">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1395">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1396">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1396">AppService</span></span>

* <span data-ttu-id="927ea-1397">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1397">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="927ea-1398">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="927ea-1398">June 5, 2018</span></span>

<span data-ttu-id="927ea-1399">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="927ea-1399">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1400">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1400">Interactive</span></span>

* <span data-ttu-id="927ea-1401">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1401">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="927ea-1402">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="927ea-1402">June 5, 2018</span></span>

<span data-ttu-id="927ea-1403">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="927ea-1403">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1404">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1404">Core</span></span>

* <span data-ttu-id="927ea-1405">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1405">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="927ea-1406">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1406">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1407">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1407">ACR</span></span>

* <span data-ttu-id="927ea-1408">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1408">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="927ea-1409">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1409">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="927ea-1410">AKS</span><span class="sxs-lookup"><span data-stu-id="927ea-1410">AKS</span></span>

* <span data-ttu-id="927ea-1411">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-1411">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1412">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1412">Batch</span></span>

* <span data-ttu-id="927ea-1413">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="927ea-1413">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1414">IOT</span><span class="sxs-lookup"><span data-stu-id="927ea-1414">IOT</span></span>

* <span data-ttu-id="927ea-1415">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1415">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1416">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1416">Network</span></span>

* <span data-ttu-id="927ea-1417">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="927ea-1417">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="927ea-1418">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="927ea-1418">Policy Insights</span></span>

* <span data-ttu-id="927ea-1419">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1419">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="927ea-1420">ARM</span><span class="sxs-lookup"><span data-stu-id="927ea-1420">ARM</span></span>

* <span data-ttu-id="927ea-1421">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1421">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1422">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1422">SQL</span></span>

* <span data-ttu-id="927ea-1423">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="927ea-1423">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="927ea-1424">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1424">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="927ea-1425">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1425">Storage</span></span>

* <span data-ttu-id="927ea-1426">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="927ea-1426">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1427">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1427">VM</span></span>

* <span data-ttu-id="927ea-1428">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1428">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="927ea-1429">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1429">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="927ea-1430">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1430">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="927ea-1431">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="927ea-1431">May 22, 2018</span></span>

<span data-ttu-id="927ea-1432">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="927ea-1432">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1433">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1433">Core</span></span>

* <span data-ttu-id="927ea-1434">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1434">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1435">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1435">ACS</span></span>

* <span data-ttu-id="927ea-1436">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1436">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="927ea-1437">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1437">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1438">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-1438">AppService</span></span>

* <span data-ttu-id="927ea-1439">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1439">Improved generic update commands</span></span>
* <span data-ttu-id="927ea-1440">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1440">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1441">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1441">Container</span></span>

* <span data-ttu-id="927ea-1442">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1442">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="927ea-1443">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1443">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1444">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1444">Extension</span></span>

* <span data-ttu-id="927ea-1445">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1445">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1446">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1446">Interactive</span></span>

* <span data-ttu-id="927ea-1447">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-1447">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="927ea-1448">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1448">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-1449">KeyVault</span><span class="sxs-lookup"><span data-stu-id="927ea-1449">KeyVault</span></span>

* <span data-ttu-id="927ea-1450">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="927ea-1450">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1451">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1451">Network</span></span>

* <span data-ttu-id="927ea-1452">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1452">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="927ea-1453">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1453">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1454">SQL</span></span>

* <span data-ttu-id="927ea-1455">[호환성이 손상되는 변경] `db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="927ea-1455">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="927ea-1456">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="927ea-1456">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="927ea-1457">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1457">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="927ea-1458">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1458">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="927ea-1459">[호환성이 손상되는 변경] `db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1459">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="927ea-1460">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1460">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="927ea-1461">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1461">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="927ea-1462">`edition`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1462">`edition`.</span></span> <span data-ttu-id="927ea-1463">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1463">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="927ea-1464">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1464">`elasticPoolName`.</span></span> <span data-ttu-id="927ea-1465">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1465">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="927ea-1466">[호환성이 손상되는 변경] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1466">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="927ea-1467">`edition`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1467">`edition`.</span></span> <span data-ttu-id="927ea-1468">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-1468">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="927ea-1469">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1469">`dtu`.</span></span> <span data-ttu-id="927ea-1470">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-1470">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="927ea-1471">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1471">`databaseDtuMin`.</span></span> <span data-ttu-id="927ea-1472">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-1472">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="927ea-1473">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="927ea-1473">`databaseDtuMax`.</span></span> <span data-ttu-id="927ea-1474">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-1474">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="927ea-1475">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1475">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="927ea-1476">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1476">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1477">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1477">Storage</span></span>

* <span data-ttu-id="927ea-1478">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1478">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="927ea-1479">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1479">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1480">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1480">VM</span></span>

* <span data-ttu-id="927ea-1481">[호환성이 손상되는 변경] `vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="927ea-1481">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="927ea-1482">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-1482">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="927ea-1483">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1483">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="927ea-1484">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1484">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="927ea-1485">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1485">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="927ea-1486">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="927ea-1486">May 7, 2018</span></span>

<span data-ttu-id="927ea-1487">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="927ea-1487">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1488">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1488">Core</span></span>

* <span data-ttu-id="927ea-1489">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1489">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="927ea-1490">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1490">Added limited support for positional arguments</span></span>
* <span data-ttu-id="927ea-1491">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1491">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="927ea-1492">#5591</span><span class="sxs-lookup"><span data-stu-id="927ea-1492">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="927ea-1493">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1493">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="927ea-1494">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1494">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="927ea-1495">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1495">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="927ea-1496">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1496">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="927ea-1497">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1497">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1498">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1498">ACR</span></span>

* <span data-ttu-id="927ea-1499">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1499">Added ACR Build commands</span></span>
* <span data-ttu-id="927ea-1500">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1500">Improved resource not found error messages</span></span>
* <span data-ttu-id="927ea-1501">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1501">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="927ea-1502">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1502">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="927ea-1503">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1503">Improved repository commands error messages</span></span>
* <span data-ttu-id="927ea-1504">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1504">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1505">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1505">ACS</span></span>

* <span data-ttu-id="927ea-1506">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1506">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="927ea-1507">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1507">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="927ea-1508">AMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1508">AMS</span></span>

* <span data-ttu-id="927ea-1509">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="927ea-1509">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1510">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1510">Appservice</span></span>

* <span data-ttu-id="927ea-1511">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1511">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="927ea-1512">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1512">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="927ea-1513">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1513">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="927ea-1514">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1514">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="927ea-1515">Batch AI</span><span class="sxs-lookup"><span data-stu-id="927ea-1515">Batch AI</span></span>

* <span data-ttu-id="927ea-1516">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1516">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="927ea-1517">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="927ea-1517">Cognitive Services</span></span>

* <span data-ttu-id="927ea-1518">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1518">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-1519">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-1519">Consumption</span></span>

* <span data-ttu-id="927ea-1520">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1520">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1521">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1521">Container</span></span>

* <span data-ttu-id="927ea-1522">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1522">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="927ea-1523">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="927ea-1523">Cosmos DB</span></span>

* <span data-ttu-id="927ea-1524">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="927ea-1524">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="927ea-1525">DMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1525">DMS</span></span>

* <span data-ttu-id="927ea-1526">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1526">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1527">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1527">Extension</span></span>

* <span data-ttu-id="927ea-1528">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1528">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1529">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1529">Interactive</span></span>

* <span data-ttu-id="927ea-1530">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1530">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="927ea-1531">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="927ea-1531">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="927ea-1532">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1532">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="927ea-1533">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1533">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="927ea-1534">랩</span><span class="sxs-lookup"><span data-stu-id="927ea-1534">Lab</span></span>

* <span data-ttu-id="927ea-1535">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1535">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1536">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1536">Network</span></span>

* <span data-ttu-id="927ea-1537">[호환성이 손상되는 변경] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1537">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="927ea-1538">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1538">Profile</span></span>

* <span data-ttu-id="927ea-1539">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1539">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="927ea-1540">[호환성이 손상되는 변경] `--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1540">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="927ea-1541">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1541">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="927ea-1542">Redis</span><span class="sxs-lookup"><span data-stu-id="927ea-1542">Redis</span></span>

* <span data-ttu-id="927ea-1543">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1543">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="927ea-1544">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1544">Deprecated `redis list-all`.</span></span> <span data-ttu-id="927ea-1545">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1545">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="927ea-1546">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1546">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="927ea-1547">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1547">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1548">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1548">Role</span></span>

* <span data-ttu-id="927ea-1549">[호환성이 손상되는 변경] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1549">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1550">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1550">Storage</span></span>

* <span data-ttu-id="927ea-1551">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1551">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="927ea-1552">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="927ea-1552">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="927ea-1553">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="927ea-1553">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="927ea-1554">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1554">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="927ea-1555">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1555">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1556">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1556">VM</span></span>

* <span data-ttu-id="927ea-1557">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1557">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="927ea-1558">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1558">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="927ea-1559">[호환성이 손상되는 변경] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="927ea-1559">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="927ea-1560">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1560">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="927ea-1561">[호환성이 손상되는 변경] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1561">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="927ea-1562">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1562">Added write accelerator support</span></span>
* <span data-ttu-id="927ea-1563">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1563">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="927ea-1564">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1564">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="927ea-1565">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1565">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="927ea-1566">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="927ea-1566">April 10, 2018</span></span>

<span data-ttu-id="927ea-1567">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="927ea-1567">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1568">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1568">ACR</span></span>

* <span data-ttu-id="927ea-1569">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="927ea-1569">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1570">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1570">ACS</span></span>

* <span data-ttu-id="927ea-1571">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1571">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1572">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1572">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="927ea-1574">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1574">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-1575">BatchAI</span><span class="sxs-lookup"><span data-stu-id="927ea-1575">BatchAI</span></span>

* <span data-ttu-id="927ea-1576">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1576">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="927ea-1577">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="927ea-1577">Job level mounting</span></span>
  - <span data-ttu-id="927ea-1578">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="927ea-1578">Environment variables with secret values</span></span>
  - <span data-ttu-id="927ea-1579">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1579">Performance counters settings</span></span>
  - <span data-ttu-id="927ea-1580">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="927ea-1580">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="927ea-1581">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1581">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="927ea-1582">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="927ea-1582">Usage and limits reporting</span></span>
  - <span data-ttu-id="927ea-1583">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1583">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="927ea-1584">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1584">Support for custom images</span></span>
  - <span data-ttu-id="927ea-1585">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1585">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="927ea-1586">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1586">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="927ea-1587">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1587">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="927ea-1588">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1588">National clouds are supported</span></span>
* <span data-ttu-id="927ea-1589">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1589">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="927ea-1590">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="927ea-1590">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="927ea-1591">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1591">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="927ea-1592">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1592">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="927ea-1593">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="927ea-1593">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="927ea-1594">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="927ea-1594">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="927ea-1595">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1595">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="927ea-1596">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1596">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="927ea-1597">이 옵션을 사용하면 보다 쉽게 저장소 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1597">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="927ea-1598">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1598">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="927ea-1599">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1599">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="927ea-1600">[호환성이 손상되는 변경] `job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="927ea-1600">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="927ea-1601">[호환성이 손상되는 변경] `cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-1601">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="927ea-1602">결제</span><span class="sxs-lookup"><span data-stu-id="927ea-1602">Billing</span></span>

* <span data-ttu-id="927ea-1603">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1603">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-1604">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-1604">Consumption</span></span>

* <span data-ttu-id="927ea-1605">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1605">Added `marketplace` commands</span></span>
* <span data-ttu-id="927ea-1606">[호환성이 손상되는 변경] `reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1606">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="927ea-1607">[호환성이 손상되는 변경] `reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1607">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="927ea-1608">[호환성이 손상되는 변경] `reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1608">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="927ea-1609">[호환성이 손상되는 변경] `reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1609">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="927ea-1610">[호환성이 손상되는 변경] `pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1610">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1611">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1611">Container</span></span>

* <span data-ttu-id="927ea-1612">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path`를 추가함</span><span class="sxs-lookup"><span data-stu-id="927ea-1612">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="927ea-1613">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="927ea-1613">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1614">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1614">Extension</span></span>

* <span data-ttu-id="927ea-1615">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1615">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1616">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1616">Interactive</span></span>

* <span data-ttu-id="927ea-1617">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-1617">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="927ea-1618">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1618">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="927ea-1619">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1619">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1620">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1620">Network</span></span>

* <span data-ttu-id="927ea-1621">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1621">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="927ea-1622">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1622">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="927ea-1623">#4910</span><span class="sxs-lookup"><span data-stu-id="927ea-1623">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="927ea-1624">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1624">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="927ea-1625">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="927ea-1625">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="927ea-1626">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1626">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="927ea-1627">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1627">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="927ea-1628">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1628">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-1629">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1629">Profile</span></span>

* <span data-ttu-id="927ea-1630">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1630">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="927ea-1631">[호환성이 손상되는 변경] `--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1631">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-1632">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1632">RDBMS</span></span>

* <span data-ttu-id="927ea-1633">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1633">Added `georestore` command</span></span>
* <span data-ttu-id="927ea-1634">`create` 명령에서 저장소 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1634">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1635">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1635">Resource</span></span>

* <span data-ttu-id="927ea-1636">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1636">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="927ea-1637">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1637">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1638">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1638">SQL</span></span>

* <span data-ttu-id="927ea-1639">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1639">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1640">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1640">Storage</span></span>

* <span data-ttu-id="927ea-1641">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1641">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1642">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1642">VM</span></span>

* <span data-ttu-id="927ea-1643">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1643">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="927ea-1644">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-1644">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="927ea-1646">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1646">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="927ea-1647">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1647">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="927ea-1648">#5718</span><span class="sxs-lookup"><span data-stu-id="927ea-1648">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="927ea-1649">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1649">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="927ea-1650">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="927ea-1650">March 27, 2018</span></span>

<span data-ttu-id="927ea-1651">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="927ea-1651">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1652">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1652">Core</span></span>

* <span data-ttu-id="927ea-1653">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="927ea-1653">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1654">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1654">ACS</span></span>

* <span data-ttu-id="927ea-1655">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1655">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1656">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1656">Appservice</span></span>

* <span data-ttu-id="927ea-1657">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1657">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="927ea-1658">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1658">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="927ea-1659">Backup</span><span class="sxs-lookup"><span data-stu-id="927ea-1659">Backup</span></span>

* <span data-ttu-id="927ea-1660">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1660">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="927ea-1661">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1661">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="927ea-1662">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1662">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="927ea-1663">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1663">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1664">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1664">Container</span></span>

* <span data-ttu-id="927ea-1665">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1665">Added `container exec` command.</span></span> <span data-ttu-id="927ea-1666">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1666">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="927ea-1667">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-1667">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1668">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1668">Extension</span></span>

* <span data-ttu-id="927ea-1669">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1669">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="927ea-1670">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1670">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="927ea-1671">[호환성이 손상되는 변경] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1671">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1672">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1672">Interactive</span></span>

* <span data-ttu-id="927ea-1673">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="927ea-1673">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="927ea-1674">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1674">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="927ea-1675">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1675">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="927ea-1676">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1676">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="927ea-1677">랩</span><span class="sxs-lookup"><span data-stu-id="927ea-1677">Lab</span></span>

* <span data-ttu-id="927ea-1678">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1678">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1679">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1679">Monitor</span></span>

* <span data-ttu-id="927ea-1680">`--top`, `--orderby`, `--namespace`에 대한 지원이 `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1680">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="927ea-1681">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="927ea-1681">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="927ea-1682">`--namespace`에 대한 지원이 `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1682">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1683">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1683">Network</span></span>

* <span data-ttu-id="927ea-1684">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1684">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-1685">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1685">Profile</span></span>

* <span data-ttu-id="927ea-1686">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1686">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-1687">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1687">RDBMS</span></span>

* <span data-ttu-id="927ea-1688">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1688">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1689">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1689">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="927ea-1691">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1691">Role</span></span>

* <span data-ttu-id="927ea-1692">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1692">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="927ea-1693">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1693">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="927ea-1694">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1694">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="927ea-1695">[호환성이 손상되는 변경] `az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1695">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="927ea-1696">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1696">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1697">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1697">Storage</span></span>

* <span data-ttu-id="927ea-1698">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1698">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="927ea-1699">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="927ea-1699">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1700">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1700">VM</span></span>

* <span data-ttu-id="927ea-1701">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1701">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="927ea-1702">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1702">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="927ea-1703">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1703">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="927ea-1704">[호환성이 손상되는 변경] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1704">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="927ea-1705">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="927ea-1705">March 13, 2018</span></span>

<span data-ttu-id="927ea-1706">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="927ea-1706">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1707">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1707">ACR</span></span>

* <span data-ttu-id="927ea-1708">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1708">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="927ea-1709">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1709">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="927ea-1710">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1710">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1711">ACS</span></span>

* <span data-ttu-id="927ea-1712">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1712">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="927ea-1713">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1713">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="927ea-1714">Advisor</span><span class="sxs-lookup"><span data-stu-id="927ea-1714">Advisor</span></span>

* <span data-ttu-id="927ea-1715">[호환성이 손상되는 변경] `advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1715">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="927ea-1716">[호환성이 손상되는 변경] `advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1716">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="927ea-1717">[호환성이 손상되는 변경] `advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1717">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="927ea-1718">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1718">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="927ea-1719">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1719">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1720">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1720">Appservice</span></span>

* <span data-ttu-id="927ea-1721">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1721">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="927ea-1722">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1722">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="927ea-1723">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="927ea-1723">Eventhubs</span></span>

* <span data-ttu-id="927ea-1724">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1724">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1725">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1725">Extension</span></span>

* <span data-ttu-id="927ea-1726">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1726">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1727">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1727">Interactive</span></span>

* <span data-ttu-id="927ea-1728">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="927ea-1728">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="927ea-1729">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="927ea-1729">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="927ea-1730">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1730">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="927ea-1731">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1731">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1732">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1732">Monitor</span></span>

* <span data-ttu-id="927ea-1733">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1733">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="927ea-1734">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1734">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="927ea-1735">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1735">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="927ea-1736">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1736">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1737">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1737">Network</span></span>

* <span data-ttu-id="927ea-1738">[호환성이 손상되는 변경] `route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1738">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="927ea-1739">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="927ea-1739">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="927ea-1740">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1740">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="927ea-1741">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1741">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-1742">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1742">Profile</span></span>

* <span data-ttu-id="927ea-1743">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1743">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="927ea-1744">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1744">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-1745">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-1745">RDBMS</span></span>

* <span data-ttu-id="927ea-1746">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1746">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="927ea-1747">Service Bus</span><span class="sxs-lookup"><span data-stu-id="927ea-1747">Service Bus</span></span>

* <span data-ttu-id="927ea-1748">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1748">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1749">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1749">Storage</span></span>

* <span data-ttu-id="927ea-1750">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1750">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="927ea-1751">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1751">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1752">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1752">VM</span></span>

* <span data-ttu-id="927ea-1753">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1753">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="927ea-1754">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-1754">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="927ea-1755">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1755">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="927ea-1756">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1756">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="927ea-1757">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="927ea-1757">February 27, 2018</span></span>

<span data-ttu-id="927ea-1758">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="927ea-1758">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1759">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1759">Core</span></span>

* <span data-ttu-id="927ea-1760">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="927ea-1760">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="927ea-1761">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1761">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="927ea-1762">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1762">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1763">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1763">ACS</span></span>

* <span data-ttu-id="927ea-1764">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1764">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="927ea-1765">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="927ea-1765">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="927ea-1766">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1766">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="927ea-1767">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1767">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1768">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1768">Appservice</span></span>

* <span data-ttu-id="927ea-1769">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="927ea-1769">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="927ea-1770">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1770">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="927ea-1771">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="927ea-1771">Cognitive Services</span></span>

* <span data-ttu-id="927ea-1772">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1772">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-1773">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-1773">Consumption</span></span>

* <span data-ttu-id="927ea-1774">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1774">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="927ea-1775">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1775">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1776">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1776">Container</span></span>

* <span data-ttu-id="927ea-1777">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1777">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1778">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1778">Network</span></span>

* <span data-ttu-id="927ea-1779">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1779">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1780">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1780">Resource</span></span>

* <span data-ttu-id="927ea-1781">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1781">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1782">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1782">Role</span></span>

* <span data-ttu-id="927ea-1783">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1783">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1784">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1784">SQL</span></span>

* <span data-ttu-id="927ea-1785">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1785">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1786">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1786">Storage</span></span>

* <span data-ttu-id="927ea-1787">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="927ea-1787">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1788">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1788">VM</span></span>

* <span data-ttu-id="927ea-1789">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1789">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="927ea-1790">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="927ea-1790">February 13, 2018</span></span>

<span data-ttu-id="927ea-1791">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="927ea-1791">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1792">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1792">Core</span></span>

* <span data-ttu-id="927ea-1793">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1793">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1794">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1794">ACS</span></span>

* <span data-ttu-id="927ea-1795">[호환성이 손상되는 변경] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1795">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="927ea-1796">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1796">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="927ea-1797">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1797">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="927ea-1798">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="927ea-1798">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="927ea-1799">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1799">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="927ea-1800">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-1800">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="927ea-1801">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1801">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="927ea-1802">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1802">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1803">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1803">Appservice</span></span>

* <span data-ttu-id="927ea-1804">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1804">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="927ea-1805">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1805">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-1806">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-1806">CDN</span></span>

* <span data-ttu-id="927ea-1807">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1807">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1808">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1808">Container</span></span>

* <span data-ttu-id="927ea-1809">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1809">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="927ea-1810">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1810">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-1811">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-1811">CosmosDB</span></span>

* <span data-ttu-id="927ea-1812">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1812">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-1813">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-1813">Extension</span></span>

* <span data-ttu-id="927ea-1814">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1814">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="927ea-1815">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1815">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="927ea-1816">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="927ea-1816">Feedback</span></span>

* <span data-ttu-id="927ea-1817">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1817">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1818">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1818">Interactive</span></span>

* <span data-ttu-id="927ea-1819">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1819">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="927ea-1820">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1820">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1821">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1821">IoT</span></span>

* <span data-ttu-id="927ea-1822">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1822">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="927ea-1823">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1823">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="927ea-1824">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1824">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="927ea-1825">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-1825">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1826">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1826">Monitor</span></span>

* <span data-ttu-id="927ea-1827">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1827">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1828">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1828">Network</span></span>

* <span data-ttu-id="927ea-1829">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1829">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="927ea-1830">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1830">Profile</span></span>

* <span data-ttu-id="927ea-1831">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1831">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1832">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1832">Resource</span></span>

* <span data-ttu-id="927ea-1833">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1833">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1834">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1834">Role</span></span>

* <span data-ttu-id="927ea-1835">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1835">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1836">SQL</span></span>

* <span data-ttu-id="927ea-1837">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1837">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="927ea-1838">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1838">Added `sql db rename`</span></span>
* <span data-ttu-id="927ea-1839">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1839">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1840">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1840">Storage</span></span>

* <span data-ttu-id="927ea-1841">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1841">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1842">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1842">VM</span></span>

* <span data-ttu-id="927ea-1843">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1843">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="927ea-1844">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1844">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="927ea-1845">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="927ea-1845">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="927ea-1846">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="927ea-1846">January 31, 2018</span></span>

<span data-ttu-id="927ea-1847">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="927ea-1847">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1848">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1848">Core</span></span>

* <span data-ttu-id="927ea-1849">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1849">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="927ea-1850">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1850">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="927ea-1851">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1851">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="927ea-1852">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="927ea-1852">Use `--verbose` to see</span></span>
* <span data-ttu-id="927ea-1853">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1853">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1854">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1854">ACS</span></span>

* <span data-ttu-id="927ea-1855">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1855">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="927ea-1856">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="927ea-1856">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1857">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1857">Appservice</span></span>

* <span data-ttu-id="927ea-1858">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="927ea-1858">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="927ea-1859">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-1859">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-1860">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-1860">CDN</span></span>

* <span data-ttu-id="927ea-1861">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1861">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-1862">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-1862">CosmosDB</span></span>

* <span data-ttu-id="927ea-1863">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1863">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1864">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1864">Interactive</span></span>

* <span data-ttu-id="927ea-1865">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1865">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1866">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1866">Network</span></span>

* <span data-ttu-id="927ea-1867">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1867">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="927ea-1868">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1868">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="927ea-1869">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1869">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="927ea-1870">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1870">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="927ea-1871">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1871">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="927ea-1872">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="927ea-1872">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="927ea-1873">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1873">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="927ea-1874">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1874">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="927ea-1875">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1875">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="927ea-1876">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="927ea-1876">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-1877">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1877">Profile</span></span>

* <span data-ttu-id="927ea-1878">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1878">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1879">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1879">Resource</span></span>

* <span data-ttu-id="927ea-1880">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1880">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1881">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1881">Storage</span></span>

* <span data-ttu-id="927ea-1882">저장소 V1 계정을 저장소 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-1882">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="927ea-1883">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1883">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="927ea-1884">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1884">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="927ea-1885">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1885">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="927ea-1886">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1886">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1887">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1887">VM</span></span>

* <span data-ttu-id="927ea-1888">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1888">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="927ea-1889">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-1889">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="927ea-1890">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1890">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="927ea-1891">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1891">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="927ea-1892">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="927ea-1892">January 17, 2018</span></span>

<span data-ttu-id="927ea-1893">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="927ea-1893">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-1894">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-1894">ACR</span></span>

* <span data-ttu-id="927ea-1895">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1895">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="927ea-1896">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1896">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1897">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1897">ACS</span></span>

* <span data-ttu-id="927ea-1898">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1898">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="927ea-1899">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1899">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1900">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1900">Appservice</span></span>

* <span data-ttu-id="927ea-1901">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1901">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="927ea-1902">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1902">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="927ea-1903">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1903">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="927ea-1904">Backup</span><span class="sxs-lookup"><span data-stu-id="927ea-1904">Backup</span></span>

* <span data-ttu-id="927ea-1905">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1905">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="927ea-1906">`backup restore restore-disks`에 저장소 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1906">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="927ea-1907">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1907">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="927ea-1908">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1908">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="927ea-1909">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1909">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-1910">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-1910">Batch</span></span>

* <span data-ttu-id="927ea-1911">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1911">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="927ea-1912">클라우드</span><span class="sxs-lookup"><span data-stu-id="927ea-1912">Cloud</span></span>

* <span data-ttu-id="927ea-1913">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1913">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-1914">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-1914">Consumption</span></span>

* <span data-ttu-id="927ea-1915">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1915">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="927ea-1916">Event Grid</span><span class="sxs-lookup"><span data-stu-id="927ea-1916">Event Grid</span></span>

* <span data-ttu-id="927ea-1917">[호환성이 손상되는 변경] `az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1917">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="927ea-1918">[호환성이 손상되는 변경] `az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1918">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="927ea-1919">[호환성이 손상되는 변경] `eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1919">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="927ea-1920">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="927ea-1920">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="927ea-1921">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1921">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="927ea-1922">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1922">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="927ea-1923">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1923">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="927ea-1924">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1924">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-1925">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-1925">Interactive</span></span>

* <span data-ttu-id="927ea-1926">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1926">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="927ea-1927">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1927">Fixed errors on startup</span></span>
* <span data-ttu-id="927ea-1928">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1928">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-1929">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-1929">IoT</span></span>

* <span data-ttu-id="927ea-1930">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1930">Added support for device provisioning service</span></span>
* <span data-ttu-id="927ea-1931">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1931">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="927ea-1932">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1932">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1933">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1933">Monitor</span></span>

* <span data-ttu-id="927ea-1934">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1934">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="927ea-1935">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="927ea-1935">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="927ea-1936">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1936">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1937">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1937">Network</span></span>

* <span data-ttu-id="927ea-1938">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1938">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="927ea-1939">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1939">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-1940">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-1940">Profile</span></span>

* <span data-ttu-id="927ea-1941">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1941">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1942">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1942">Role</span></span>

* <span data-ttu-id="927ea-1943">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1943">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="927ea-1944">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="927ea-1944">Service Fabric</span></span>

* <span data-ttu-id="927ea-1945">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1945">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="927ea-1946">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1946">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1947">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1947">VM</span></span>

* <span data-ttu-id="927ea-1948">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-1948">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="927ea-1949">[호환성이 손상되는 변경] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1949">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="927ea-1950">[호환성이 손상되는 변경] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1950">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="927ea-1951">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1951">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="927ea-1952">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1952">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="927ea-1953">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1953">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="927ea-1954">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1954">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="927ea-1955">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1955">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="927ea-1956">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="927ea-1956">December 19, 2017</span></span>

<span data-ttu-id="927ea-1957">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="927ea-1957">Version 2.0.23</span></span>

* <span data-ttu-id="927ea-1958">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1958">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1959">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1959">Container</span></span>

* <span data-ttu-id="927ea-1960">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1960">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="927ea-1961">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-1961">Network</span></span>

* <span data-ttu-id="927ea-1962">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1962">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="927ea-1963">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1963">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-1964">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-1964">Storage</span></span>

* <span data-ttu-id="927ea-1965">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1965">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-1966">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-1966">VM</span></span>

* <span data-ttu-id="927ea-1967">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1967">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="927ea-1968">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="927ea-1968">December 5, 2017</span></span>

<span data-ttu-id="927ea-1969">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="927ea-1969">Version 2.0.22</span></span>

* <span data-ttu-id="927ea-1970">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-1970">Removed `az component` commands.</span></span> <span data-ttu-id="927ea-1971">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="927ea-1971">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="927ea-1972">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-1972">Core</span></span>
* <span data-ttu-id="927ea-1973">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1973">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="927ea-1974">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1974">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-1975">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-1975">ACS</span></span>

* <span data-ttu-id="927ea-1976">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1976">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="927ea-1977">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1977">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="927ea-1978">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1978">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="927ea-1979">Advisor</span><span class="sxs-lookup"><span data-stu-id="927ea-1979">Advisor</span></span>

* <span data-ttu-id="927ea-1980">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-1980">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-1981">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-1981">Appservice</span></span>

* <span data-ttu-id="927ea-1982">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1982">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="927ea-1983">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1983">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="927ea-1984">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1984">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="927ea-1985">Consumption</span><span class="sxs-lookup"><span data-stu-id="927ea-1985">Consumption</span></span>

* <span data-ttu-id="927ea-1986">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1986">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="927ea-1987">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-1987">Container</span></span>

* <span data-ttu-id="927ea-1988">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1988">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-1989">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-1989">Monitor</span></span>

* <span data-ttu-id="927ea-1990">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1990">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-1991">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-1991">Resource</span></span>

* <span data-ttu-id="927ea-1992">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-1992">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="927ea-1993">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-1993">Role</span></span>

* <span data-ttu-id="927ea-1994">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1994">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="927ea-1995">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1995">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="927ea-1996">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1996">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-1997">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-1997">SQL</span></span>

* <span data-ttu-id="927ea-1998">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1998">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="927ea-1999">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-1999">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2000">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2000">VM</span></span>

* <span data-ttu-id="927ea-2001">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2001">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="927ea-2002">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="927ea-2002">November 14, 2017</span></span>

<span data-ttu-id="927ea-2003">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="927ea-2003">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-2004">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-2004">ACR</span></span>

* <span data-ttu-id="927ea-2005">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2005">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="927ea-2006">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2006">ACS</span></span>

* <span data-ttu-id="927ea-2007">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2007">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="927ea-2008">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="927ea-2008">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="927ea-2009">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2009">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="927ea-2010">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2010">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="927ea-2011">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2011">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2012">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2012">Appservice</span></span>

* <span data-ttu-id="927ea-2013">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2013">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="927ea-2014">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2014">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="927ea-2015">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2015">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="927ea-2016">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2016">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="927ea-2017">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2017">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="927ea-2018">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="927ea-2018">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-2019">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-2019">Batch</span></span>

* <span data-ttu-id="927ea-2020">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2020">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-2021">Batchai</span><span class="sxs-lookup"><span data-stu-id="927ea-2021">Batchai</span></span>

* <span data-ttu-id="927ea-2022">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2022">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="927ea-2023">저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2023">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="927ea-2024">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2024">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="927ea-2025">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2025">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="927ea-2026">클라우드</span><span class="sxs-lookup"><span data-stu-id="927ea-2026">Cloud</span></span>

* <span data-ttu-id="927ea-2027">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2027">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="927ea-2028">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-2028">Container</span></span>

* <span data-ttu-id="927ea-2029">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2029">Added support to open multiple ports</span></span>
* <span data-ttu-id="927ea-2030">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2030">Added container group restart policy</span></span>
* <span data-ttu-id="927ea-2031">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2031">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="927ea-2032">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="927ea-2032">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="927ea-2033">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="927ea-2033">Data Lake Analytics</span></span>

* <span data-ttu-id="927ea-2034">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2034">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="927ea-2035">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="927ea-2035">Data Lake Store</span></span>

* <span data-ttu-id="927ea-2036">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2036">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-2037">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-2037">Extension</span></span>

* <span data-ttu-id="927ea-2038">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2038">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="927ea-2039">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2039">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-2040">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-2040">IoT</span></span>

* <span data-ttu-id="927ea-2041">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2041">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-2042">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-2042">Monitor</span></span>

* <span data-ttu-id="927ea-2043">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2043">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2044">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2044">Network</span></span>

* <span data-ttu-id="927ea-2045">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2045">Added support for CAA DNS records</span></span>
* <span data-ttu-id="927ea-2046">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2046">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="927ea-2047">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2047">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="927ea-2048">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2048">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="927ea-2049">예약</span><span class="sxs-lookup"><span data-stu-id="927ea-2049">Reservations</span></span>

* <span data-ttu-id="927ea-2050">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2050">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2051">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2051">Resource</span></span>

* <span data-ttu-id="927ea-2052">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2052">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2053">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-2053">SQL</span></span>

* <span data-ttu-id="927ea-2054">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2054">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2055">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2055">Storage</span></span>

* <span data-ttu-id="927ea-2056">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2056">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="927ea-2057">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2057">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="927ea-2058">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2058">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="927ea-2059">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="927ea-2059">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="927ea-2060">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2060">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="927ea-2061">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2061">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="927ea-2062">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2062">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2063">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2063">VM</span></span>

* <span data-ttu-id="927ea-2064">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2064">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="927ea-2065">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2065">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="927ea-2066">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2066">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="927ea-2067">이름이 `vm format-secret`에서 `vm secret format`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2067">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="927ea-2068">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2068">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="927ea-2069">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="927ea-2069">October 24, 2017</span></span>

<span data-ttu-id="927ea-2070">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="927ea-2070">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="927ea-2071">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2071">Core</span></span>

* <span data-ttu-id="927ea-2072">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="927ea-2072">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-2073">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-2073">ACR</span></span>

* <span data-ttu-id="927ea-2074">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="927ea-2074">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="927ea-2075">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-2075">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="927ea-2076">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="927ea-2076">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2077">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2077">ACS</span></span>

* <span data-ttu-id="927ea-2078">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2078">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="927ea-2079">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2079">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2080">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2080">Appservice</span></span>

* <span data-ttu-id="927ea-2081">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2081">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="927ea-2082">구성 요소</span><span class="sxs-lookup"><span data-stu-id="927ea-2082">Component</span></span>

* <span data-ttu-id="927ea-2083">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2083">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-2084">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-2084">Monitor</span></span>

* <span data-ttu-id="927ea-2085">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2085">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2086">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2086">Resource</span></span>

* <span data-ttu-id="927ea-2087">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2087">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="927ea-2088">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2088">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2089">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2089">VM</span></span>

* <span data-ttu-id="927ea-2090">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2090">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="927ea-2091">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="927ea-2091">October 9, 2017</span></span>

<span data-ttu-id="927ea-2092">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="927ea-2092">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="927ea-2093">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2093">Core</span></span>

* <span data-ttu-id="927ea-2094">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2094">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2095">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2095">Appservice</span></span>

* <span data-ttu-id="927ea-2096">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2096">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-2097">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-2097">Batch</span></span>

* <span data-ttu-id="927ea-2098">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2098">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="927ea-2099">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2099">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="927ea-2100">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2100">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="927ea-2101">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2101">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="927ea-2102">Batchai</span><span class="sxs-lookup"><span data-stu-id="927ea-2102">Batchai</span></span>

* <span data-ttu-id="927ea-2103">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2103">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-2104">Keyvault</span><span class="sxs-lookup"><span data-stu-id="927ea-2104">Keyvault</span></span>

* <span data-ttu-id="927ea-2105">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2105">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="927ea-2106">(#4448)</span><span class="sxs-lookup"><span data-stu-id="927ea-2106">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="927ea-2107">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2107">Network</span></span>

* <span data-ttu-id="927ea-2108">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2108">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="927ea-2109">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2109">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2110">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2110">Resource</span></span>

* <span data-ttu-id="927ea-2111">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2111">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="927ea-2112">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2112">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="927ea-2113">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2113">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="927ea-2114">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2114">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2115">Sql</span><span class="sxs-lookup"><span data-stu-id="927ea-2115">Sql</span></span>

* <span data-ttu-id="927ea-2116">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2116">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="927ea-2117">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2117">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="927ea-2118">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2118">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2119">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2119">Storage</span></span>

* <span data-ttu-id="927ea-2120">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2120">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2121">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2121">Vm</span></span>

* <span data-ttu-id="927ea-2122">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2122">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="927ea-2123">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2123">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="927ea-2124">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2124">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="927ea-2125">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2125">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="927ea-2126">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2126">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="927ea-2127">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="927ea-2127">September 22, 2017</span></span>

<span data-ttu-id="927ea-2128">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="927ea-2128">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2129">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2129">Resource</span></span>

* <span data-ttu-id="927ea-2130">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2130">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="927ea-2131">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2131">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="927ea-2132">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2132">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="927ea-2133">[호환성이 손상되는 변경] `managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2133">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2134">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2134">Network</span></span>

* <span data-ttu-id="927ea-2135">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2135">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="927ea-2136">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2136">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="927ea-2137">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2137">Added `asg` application security group commands</span></span>
* <span data-ttu-id="927ea-2138">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2138">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="927ea-2139">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2139">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="927ea-2140">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2140">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="927ea-2141">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2141">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2142">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2142">Storage</span></span>

* <span data-ttu-id="927ea-2143">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2143">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="927ea-2144">Event Grid</span><span class="sxs-lookup"><span data-stu-id="927ea-2144">Eventgrid</span></span>

* <span data-ttu-id="927ea-2145">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="927ea-2145">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2146">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-2146">SQL</span></span>

* <span data-ttu-id="927ea-2147">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2147">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="927ea-2148">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2148">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="927ea-2149">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2149">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-2150">Keyvault</span><span class="sxs-lookup"><span data-stu-id="927ea-2150">Keyvault</span></span>

* <span data-ttu-id="927ea-2151">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2151">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2152">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2152">VM</span></span>

* <span data-ttu-id="927ea-2153">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2153">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="927ea-2154">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="927ea-2154">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="927ea-2155">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2155">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="927ea-2156">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2156">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="927ea-2157">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2157">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="927ea-2158">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2158">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2159">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2159">ACS</span></span>

* <span data-ttu-id="927ea-2160">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2160">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2161">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2161">Appservice</span></span>

* <span data-ttu-id="927ea-2162">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2162">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="927ea-2163">Backup</span><span class="sxs-lookup"><span data-stu-id="927ea-2163">Backup</span></span>

* <span data-ttu-id="927ea-2164">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2164">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="927ea-2165">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="927ea-2165">September 11, 2017</span></span>

<span data-ttu-id="927ea-2166">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="927ea-2166">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="927ea-2167">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2167">Core</span></span>

* <span data-ttu-id="927ea-2168">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2168">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="927ea-2169">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2169">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2170">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2170">Acs</span></span>

* <span data-ttu-id="927ea-2171">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2171">Added `acs list-locations` command</span></span>
* <span data-ttu-id="927ea-2172">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="927ea-2172">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2173">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2173">Appservice</span></span>

* <span data-ttu-id="927ea-2174">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2174">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-2175">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-2175">CDN</span></span>

* <span data-ttu-id="927ea-2176">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2176">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="927ea-2177">내선 번호</span><span class="sxs-lookup"><span data-stu-id="927ea-2177">Extension</span></span>

* <span data-ttu-id="927ea-2178">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2178">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-2179">Keyvault</span><span class="sxs-lookup"><span data-stu-id="927ea-2179">Keyvault</span></span>

* <span data-ttu-id="927ea-2180">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2180">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2181">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2181">Network</span></span>

* <span data-ttu-id="927ea-2182">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2182">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="927ea-2183">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2183">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="927ea-2184">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2184">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="927ea-2185">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2185">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="927ea-2186">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2186">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2187">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2187">Resource</span></span>

* <span data-ttu-id="927ea-2188">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-2188">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="927ea-2189">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-2189">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="927ea-2190">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-2190">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="927ea-2191">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="927ea-2191">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2192">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-2192">SQL</span></span>

* <span data-ttu-id="927ea-2193">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2193">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2194">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2194">VM</span></span>

* <span data-ttu-id="927ea-2195">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2195">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="927ea-2196">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="927ea-2196">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="927ea-2197">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2197">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="927ea-2198">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2198">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="927ea-2199">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2199">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="927ea-2200">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="927ea-2200">August 31, 2017</span></span>

<span data-ttu-id="927ea-2201">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="927ea-2201">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-2202">Keyvault</span><span class="sxs-lookup"><span data-stu-id="927ea-2202">Keyvault</span></span>

* <span data-ttu-id="927ea-2203">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2203">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="927ea-2204">Sf</span><span class="sxs-lookup"><span data-stu-id="927ea-2204">Sf</span></span>

* <span data-ttu-id="927ea-2205">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2205">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2206">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2206">Storage</span></span>

* <span data-ttu-id="927ea-2207">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2207">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="927ea-2208">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="927ea-2208">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="927ea-2209">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="927ea-2209">August 28, 2017</span></span>

<span data-ttu-id="927ea-2210">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="927ea-2210">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="927ea-2211">CLI</span><span class="sxs-lookup"><span data-stu-id="927ea-2211">CLI</span></span>

* <span data-ttu-id="927ea-2212">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2212">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2213">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2213">ACS</span></span>

* <span data-ttu-id="927ea-2214">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2214">Corrected preview regions</span></span>
* <span data-ttu-id="927ea-2215">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2215">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="927ea-2216">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2216">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2217">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2217">Appservice</span></span>

* <span data-ttu-id="927ea-2218">[호환성이 손상되는 변경] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2218">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="927ea-2219">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2219">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="927ea-2220">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2220">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="927ea-2221">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2221">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="927ea-2222">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="927ea-2222">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-2223">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-2223">IoT</span></span>

* <span data-ttu-id="927ea-2224">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2224">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2225">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2225">Network</span></span>

* <span data-ttu-id="927ea-2226">[호환성이 손상되는 변경] `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2226">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="927ea-2227">[호환성이 손상되는 변경] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2227">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="927ea-2228">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2228">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="927ea-2229">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2229">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="927ea-2230">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2230">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-2231">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-2231">Profile</span></span>

* <span data-ttu-id="927ea-2232">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2232">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="927ea-2233">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="927ea-2233">Service Fabric</span></span>

* <span data-ttu-id="927ea-2234">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2234">Preview release</span></span>
* <span data-ttu-id="927ea-2235">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2235">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="927ea-2236">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2236">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="927ea-2237">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2237">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2238">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2238">Storage</span></span>

* <span data-ttu-id="927ea-2239">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2239">Enabled setting blob tier</span></span>
* <span data-ttu-id="927ea-2240">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2240">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="927ea-2241">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2241">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="927ea-2242">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2242">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="927ea-2243">[호환성이 손상되는 변경] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2243">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="927ea-2244">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2244">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2245">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2245">VM</span></span>

* <span data-ttu-id="927ea-2246">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2246">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="927ea-2247">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2247">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="927ea-2248">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2248">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="927ea-2249">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2249">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="927ea-2250">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2250">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="927ea-2251">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2251">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="927ea-2252">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="927ea-2252">August 15, 2017</span></span>

<span data-ttu-id="927ea-2253">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="927ea-2253">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2254">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2254">ACS</span></span>

* <span data-ttu-id="927ea-2255">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2255">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2256">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2256">Appservice</span></span>

* <span data-ttu-id="927ea-2257">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2257">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="927ea-2258">Event Grid</span><span class="sxs-lookup"><span data-stu-id="927ea-2258">Event Grid</span></span>

* <span data-ttu-id="927ea-2259">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2259">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="927ea-2260">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="927ea-2260">August 11, 2017</span></span>

<span data-ttu-id="927ea-2261">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="927ea-2261">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2262">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2262">ACS</span></span>

* <span data-ttu-id="927ea-2263">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2263">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-2264">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-2264">Batch</span></span>

* <span data-ttu-id="927ea-2265">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2265">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="927ea-2266">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2266">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="927ea-2267">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2267">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="927ea-2268">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2268">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="927ea-2269">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2269">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="927ea-2270">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2270">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="927ea-2271">구성 요소</span><span class="sxs-lookup"><span data-stu-id="927ea-2271">Component</span></span>

* <span data-ttu-id="927ea-2272">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2272">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="927ea-2273">컨테이너</span><span class="sxs-lookup"><span data-stu-id="927ea-2273">Container</span></span>

* <span data-ttu-id="927ea-2274">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2274">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="927ea-2275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="927ea-2275">Data Lake Store</span></span>

* <span data-ttu-id="927ea-2276">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2276">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="927ea-2277">Event Grid</span><span class="sxs-lookup"><span data-stu-id="927ea-2277">Event Grid</span></span>

* <span data-ttu-id="927ea-2278">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2278">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2279">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2279">Network</span></span>

* <span data-ttu-id="927ea-2280">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2280">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="927ea-2281">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2281">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="927ea-2282">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2282">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="927ea-2283">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2283">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-2284">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-2284">Profile</span></span>

* <span data-ttu-id="927ea-2285">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2285">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2286">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2286">Storage</span></span>

* <span data-ttu-id="927ea-2287">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2287">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2288">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2288">VM</span></span>

* <span data-ttu-id="927ea-2289">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2289">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="927ea-2290">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2290">Exposed `list-skus` command</span></span>
* <span data-ttu-id="927ea-2291">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2291">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="927ea-2292">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2292">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="927ea-2293">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2293">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="927ea-2294">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="927ea-2294">July 28, 2017</span></span>

<span data-ttu-id="927ea-2295">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="927ea-2295">Version 2.0.12</span></span>

* <span data-ttu-id="927ea-2296">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2296">Added container commands</span></span>
* <span data-ttu-id="927ea-2297">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2297">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="927ea-2298">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2298">Core</span></span>

* <span data-ttu-id="927ea-2299">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2299">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="927ea-2300">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2300">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="927ea-2301">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-2301">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="927ea-2302">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="927ea-2302">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="927ea-2303">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="927ea-2303">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="927ea-2304">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="927ea-2304">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="927ea-2305">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="927ea-2305">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="927ea-2306">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="927ea-2306">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="927ea-2307">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="927ea-2307">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="927ea-2308">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-2308">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="927ea-2309">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="927ea-2309">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="927ea-2310">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="927ea-2310">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="927ea-2311">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2311">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="927ea-2312">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2312">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="927ea-2313">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2313">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="927ea-2314">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="927ea-2314">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="927ea-2315">ACR</span><span class="sxs-lookup"><span data-stu-id="927ea-2315">ACR</span></span>

* <span data-ttu-id="927ea-2316">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2316">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="927ea-2317">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2317">Support SKU update for managed registries</span></span>
* <span data-ttu-id="927ea-2318">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2318">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="927ea-2319">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2319">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="927ea-2320">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2320">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="927ea-2321">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2321">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2322">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2322">ACS</span></span>

* <span data-ttu-id="927ea-2323">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2323">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2324">App Service</span><span class="sxs-lookup"><span data-stu-id="927ea-2324">Appservice</span></span>

* <span data-ttu-id="927ea-2325">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2325">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="927ea-2326">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2326">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="927ea-2327">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2327">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="927ea-2328">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="927ea-2328">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="927ea-2329">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="927ea-2329">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="927ea-2330">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="927ea-2330">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="927ea-2331">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="927ea-2331">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="927ea-2332">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="927ea-2332">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="927ea-2333">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2333">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="927ea-2334">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2334">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="927ea-2335">Batch</span><span class="sxs-lookup"><span data-stu-id="927ea-2335">Batch</span></span>

* <span data-ttu-id="927ea-2336">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2336">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="927ea-2337">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2337">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="927ea-2338">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2338">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="927ea-2339">CDN</span><span class="sxs-lookup"><span data-stu-id="927ea-2339">CDN</span></span>

* <span data-ttu-id="927ea-2340">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2340">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="927ea-2341">클라우드</span><span class="sxs-lookup"><span data-stu-id="927ea-2341">Cloud</span></span>

* <span data-ttu-id="927ea-2342">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2342">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="927ea-2343">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2343">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="927ea-2344">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2344">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="927ea-2345">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2345">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="927ea-2346">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2346">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-2347">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-2347">CosmosDB</span></span>

* <span data-ttu-id="927ea-2348">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2348">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="927ea-2349">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2349">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="927ea-2350">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="927ea-2350">Data Lake Analytics</span></span>

* <span data-ttu-id="927ea-2351">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2351">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="927ea-2352">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2352">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="927ea-2353">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2353">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="927ea-2354">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="927ea-2354">Data Lake Store</span></span>

* <span data-ttu-id="927ea-2355">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2355">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="927ea-2356">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2356">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="927ea-2357">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2357">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="927ea-2358">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="927ea-2358">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="927ea-2359">대화형</span><span class="sxs-lookup"><span data-stu-id="927ea-2359">Interactive</span></span>

* <span data-ttu-id="927ea-2360">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2360">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="927ea-2361">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2361">Increased test coverage</span></span>
* <span data-ttu-id="927ea-2362">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2362">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="927ea-2363">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="927ea-2363">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="927ea-2364">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="927ea-2364">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="927ea-2365">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="927ea-2365">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="927ea-2366">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="927ea-2366">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="927ea-2367">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2367">Added `--progress` flag</span></span>
* <span data-ttu-id="927ea-2368">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2368">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="927ea-2369">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="927ea-2369">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="927ea-2370">IoT</span><span class="sxs-lookup"><span data-stu-id="927ea-2370">IoT</span></span>

* <span data-ttu-id="927ea-2371">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2371">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="927ea-2372">(#3934)</span><span class="sxs-lookup"><span data-stu-id="927ea-2372">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="927ea-2373">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="927ea-2373">Key vault</span></span>

* <span data-ttu-id="927ea-2374">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="927ea-2374">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="927ea-2375">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="927ea-2375">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="927ea-2376">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="927ea-2376">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="927ea-2377">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="927ea-2377">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="927ea-2378">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="927ea-2378">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="927ea-2379">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="927ea-2379">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="927ea-2380">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2380">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="927ea-2381">(#3307)</span><span class="sxs-lookup"><span data-stu-id="927ea-2381">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="927ea-2382">랩</span><span class="sxs-lookup"><span data-stu-id="927ea-2382">Lab</span></span>

* <span data-ttu-id="927ea-2383">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2383">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="927ea-2384">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2384">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-2385">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-2385">Monitor</span></span>

* <span data-ttu-id="927ea-2386">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="927ea-2386">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="927ea-2387">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2387">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="927ea-2388">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2388">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="927ea-2389">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2389">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="927ea-2390">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2390">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="927ea-2391">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="927ea-2391">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="927ea-2392">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2392">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="927ea-2393">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2393">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="927ea-2394">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2394">`location` no longer required</span></span>
  * <span data-ttu-id="927ea-2395">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2395">Add name and ID support for target</span></span>
  * <span data-ttu-id="927ea-2396">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2396">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="927ea-2397">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2397">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="927ea-2398">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2398">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="927ea-2399">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2399">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="927ea-2400">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2400">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="927ea-2401">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2401">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2402">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2402">Network</span></span>

* <span data-ttu-id="927ea-2403">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2403">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="927ea-2404">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2404">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="927ea-2405">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2405">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="927ea-2406">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2406">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="927ea-2407">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2407">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="927ea-2408">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2408">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="927ea-2409">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="927ea-2409">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="927ea-2410">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="927ea-2410">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="927ea-2411">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="927ea-2411">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="927ea-2412">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="927ea-2412">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="927ea-2413">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="927ea-2413">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="927ea-2414">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="927ea-2414">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="927ea-2415">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="927ea-2415">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="927ea-2416">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="927ea-2416">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="927ea-2417">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2417">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="927ea-2418">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2418">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="927ea-2419">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2419">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="927ea-2420">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2420">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="927ea-2421">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2421">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="927ea-2422">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2422">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="927ea-2423">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2423">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="927ea-2424">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2424">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="927ea-2425">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2425">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="927ea-2426">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2426">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="927ea-2427">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2427">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="927ea-2428">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2428">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="927ea-2429">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2429">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-2430">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-2430">Profile</span></span>

* <span data-ttu-id="927ea-2431">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2431">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="927ea-2432">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2432">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="927ea-2433">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2433">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="927ea-2434">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2434">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="927ea-2435">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2435">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="927ea-2436">RDBMS</span><span class="sxs-lookup"><span data-stu-id="927ea-2436">RDBMS</span></span>

* <span data-ttu-id="927ea-2437">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="927ea-2437">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="927ea-2438">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="927ea-2438">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="927ea-2439">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="927ea-2439">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="927ea-2440">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="927ea-2440">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2441">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2441">Resource</span></span>

* <span data-ttu-id="927ea-2442">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2442">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="927ea-2443">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2443">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="927ea-2444">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2444">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="927ea-2445">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2445">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="927ea-2446">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="927ea-2446">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="927ea-2447">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2447">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="927ea-2448">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="927ea-2448">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="927ea-2449">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2449">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="927ea-2450">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-2450">Role</span></span>

* <span data-ttu-id="927ea-2451">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2451">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="927ea-2452">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="927ea-2452">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="927ea-2453">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2453">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="927ea-2454">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2454">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="927ea-2455">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2455">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="927ea-2456">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="927ea-2456">Service Fabric</span></span>
* <span data-ttu-id="927ea-2457">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="927ea-2457">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="927ea-2458">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="927ea-2458">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="927ea-2459">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="927ea-2459">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2460">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-2460">SQL</span></span>

* <span data-ttu-id="927ea-2461">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2461">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="927ea-2462">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2462">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="927ea-2463">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2463">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2464">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2464">Storage</span></span>

* <span data-ttu-id="927ea-2465">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="927ea-2465">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="927ea-2466">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-2466">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="927ea-2467">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="927ea-2467">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="927ea-2468">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2468">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="927ea-2469">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="927ea-2469">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="927ea-2470">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="927ea-2470">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2471">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2471">VM</span></span>

* <span data-ttu-id="927ea-2472">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2472">Support configuring nsg</span></span>
* <span data-ttu-id="927ea-2473">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2473">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="927ea-2474">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2474">Support managed service identities</span></span>
* <span data-ttu-id="927ea-2475">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2475">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="927ea-2476">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2476">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="927ea-2477">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="927ea-2477">May 10, 2017</span></span>

<span data-ttu-id="927ea-2478">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="927ea-2478">Version 2.0.6</span></span>

* <span data-ttu-id="927ea-2479">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="927ea-2479">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="927ea-2480">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2480">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="927ea-2481">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="927ea-2481">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="927ea-2482">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="927ea-2482">Include Cognitive Services module</span></span>
* <span data-ttu-id="927ea-2483">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="927ea-2483">Include Service Fabric module</span></span>
* <span data-ttu-id="927ea-2484">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="927ea-2484">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="927ea-2485">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2485">Add support for CDN commands</span></span>
* <span data-ttu-id="927ea-2486">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-2486">Remove Container module</span></span>
* <span data-ttu-id="927ea-2487">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="927ea-2487">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="927ea-2488">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="927ea-2488">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="927ea-2489">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2489">Core</span></span>

* <span data-ttu-id="927ea-2490">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="927ea-2490">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="927ea-2491">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="927ea-2491">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="927ea-2492">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="927ea-2492">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="927ea-2493">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="927ea-2493">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="927ea-2494">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="927ea-2494">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="927ea-2495">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="927ea-2495">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="927ea-2496">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="927ea-2496">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="927ea-2497">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="927ea-2497">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="927ea-2498">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="927ea-2498">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="927ea-2499">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="927ea-2499">core: Improved performance</span></span>
* <span data-ttu-id="927ea-2500">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2500">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="927ea-2501">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="927ea-2501">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2502">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2502">ACS</span></span>

* <span data-ttu-id="927ea-2503">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2503">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="927ea-2504">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="927ea-2504">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="927ea-2505">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="927ea-2505">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="927ea-2506">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="927ea-2506">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2507">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-2507">AppService</span></span>

* <span data-ttu-id="927ea-2508">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="927ea-2508">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="927ea-2509">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2509">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="927ea-2510">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="927ea-2510">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="927ea-2511">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="927ea-2511">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="927ea-2512">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="927ea-2512">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="927ea-2513">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="927ea-2513">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="927ea-2514">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2514">support slot swap with preview</span></span>
* <span data-ttu-id="927ea-2515">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="927ea-2515">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="927ea-2516">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="927ea-2516">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="927ea-2517">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="927ea-2517">CosmosDB</span></span>

* <span data-ttu-id="927ea-2518">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="927ea-2518">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="927ea-2519">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2519">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="927ea-2520">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2520">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="927ea-2521">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2521">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="927ea-2522">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="927ea-2522">Data Lake Analytics</span></span>

* <span data-ttu-id="927ea-2523">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2523">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="927ea-2524">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2524">Add support for new catalog item type: package.</span></span> <span data-ttu-id="927ea-2525">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="927ea-2525">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="927ea-2526">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="927ea-2526">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="927ea-2527">테이블</span><span class="sxs-lookup"><span data-stu-id="927ea-2527">Table</span></span>
  * <span data-ttu-id="927ea-2528">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="927ea-2528">Table valued function</span></span>
  * <span data-ttu-id="927ea-2529">보기</span><span class="sxs-lookup"><span data-stu-id="927ea-2529">View</span></span>
  * <span data-ttu-id="927ea-2530">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="927ea-2530">Table Statistics.</span></span> <span data-ttu-id="927ea-2531">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="927ea-2531">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="927ea-2532">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="927ea-2532">Data Lake Store</span></span>

* <span data-ttu-id="927ea-2533">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="927ea-2533">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="927ea-2534">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="927ea-2534">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="927ea-2535">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="927ea-2535">missed help for access show.</span></span> <span data-ttu-id="927ea-2536">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2536">adding it.</span></span> <span data-ttu-id="927ea-2537">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="927ea-2537">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="927ea-2538">찾기</span><span class="sxs-lookup"><span data-stu-id="927ea-2538">Find</span></span>

* <span data-ttu-id="927ea-2539">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="927ea-2539">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="927ea-2540">KeyVault</span><span class="sxs-lookup"><span data-stu-id="927ea-2540">KeyVault</span></span>

* <span data-ttu-id="927ea-2541">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2541">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="927ea-2542">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="927ea-2542">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="927ea-2543">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2543">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="927ea-2544">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2544">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="927ea-2545">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="927ea-2545">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="927ea-2546">랩</span><span class="sxs-lookup"><span data-stu-id="927ea-2546">Lab</span></span>

* <span data-ttu-id="927ea-2547">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2547">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="927ea-2548">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2548">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="927ea-2549">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="927ea-2549">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="927ea-2550">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="927ea-2550">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="927ea-2551">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2551">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="927ea-2552">모니터</span><span class="sxs-lookup"><span data-stu-id="927ea-2552">Monitor</span></span>

* <span data-ttu-id="927ea-2553">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="927ea-2553">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="927ea-2554">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="927ea-2554">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="927ea-2555">네트워크</span><span class="sxs-lookup"><span data-stu-id="927ea-2555">Network</span></span>

* <span data-ttu-id="927ea-2556">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2556">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="927ea-2557">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2557">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="927ea-2558">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2558">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="927ea-2559">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2559">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="927ea-2560">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2560">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="927ea-2561">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2561">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="927ea-2562">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2562">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="927ea-2563">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2563">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="927ea-2564">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2564">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="927ea-2565">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2565">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="927ea-2566">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="927ea-2566">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="927ea-2567">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2567">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="927ea-2568">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2568">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="927ea-2569">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2569">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="927ea-2570">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="927ea-2570">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="927ea-2571">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2571">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="927ea-2572">프로필</span><span class="sxs-lookup"><span data-stu-id="927ea-2572">Profile</span></span>

* <span data-ttu-id="927ea-2573">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="927ea-2573">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="927ea-2574">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="927ea-2574">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="927ea-2575">Redis</span><span class="sxs-lookup"><span data-stu-id="927ea-2575">Redis</span></span>

* <span data-ttu-id="927ea-2576">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2576">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="927ea-2577">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="927ea-2577">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="927ea-2578">리소스</span><span class="sxs-lookup"><span data-stu-id="927ea-2578">Resource</span></span>

* <span data-ttu-id="927ea-2579">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="927ea-2579">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="927ea-2580">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="927ea-2580">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="927ea-2581">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="927ea-2581">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="927ea-2582">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2582">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="927ea-2583">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="927ea-2583">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="927ea-2584">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2584">Add docs for az lock update.</span></span> <span data-ttu-id="927ea-2585">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="927ea-2585">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="927ea-2586">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2586">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="927ea-2587">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="927ea-2587">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="927ea-2588">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2588">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="927ea-2589">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="927ea-2589">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="927ea-2590">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="927ea-2590">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="927ea-2591">역할</span><span class="sxs-lookup"><span data-stu-id="927ea-2591">Role</span></span>

* <span data-ttu-id="927ea-2592">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="927ea-2592">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="927ea-2593">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="927ea-2593">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="927ea-2594">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="927ea-2594">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="927ea-2595">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="927ea-2595">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="927ea-2596">SQL</span><span class="sxs-lookup"><span data-stu-id="927ea-2596">SQL</span></span>

* <span data-ttu-id="927ea-2597">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="927ea-2597">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="927ea-2598">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="927ea-2598">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="927ea-2599">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2599">Storage</span></span>

* <span data-ttu-id="927ea-2600">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="927ea-2600">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="927ea-2601">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2601">Add support for incremental blob copy</span></span>
* <span data-ttu-id="927ea-2602">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2602">Add support for large block blob upload</span></span>
* <span data-ttu-id="927ea-2603">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="927ea-2603">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2604">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2604">VM</span></span>

* <span data-ttu-id="927ea-2605">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="927ea-2605">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="927ea-2606">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="927ea-2606">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="927ea-2607">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="927ea-2607">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="927ea-2608">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="927ea-2608">az vm/vmss disk</span></span>
  3. <span data-ttu-id="927ea-2609">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2609">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="927ea-2610">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="927ea-2610">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="927ea-2611">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="927ea-2611">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="927ea-2612">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="927ea-2612">April 3, 2017</span></span>

<span data-ttu-id="927ea-2613">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="927ea-2613">Version 2.0.2</span></span>

<span data-ttu-id="927ea-2614">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2614">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="927ea-2615">코어</span><span class="sxs-lookup"><span data-stu-id="927ea-2615">Core</span></span>

* <span data-ttu-id="927ea-2616">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="927ea-2616">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="927ea-2617">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="927ea-2617">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="927ea-2618">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="927ea-2618">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="927ea-2619">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="927ea-2619">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="927ea-2620">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="927ea-2620">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="927ea-2621">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="927ea-2621">Add prompting for missing template parameters.</span></span> <span data-ttu-id="927ea-2622">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="927ea-2622">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="927ea-2623">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2623">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="927ea-2624">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="927ea-2624">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="927ea-2625">ACS</span><span class="sxs-lookup"><span data-stu-id="927ea-2625">ACS</span></span>

* <span data-ttu-id="927ea-2626">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="927ea-2626">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="927ea-2627">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="927ea-2627">Add support for ssh key password prompting.</span></span> <span data-ttu-id="927ea-2628">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="927ea-2628">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="927ea-2629">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="927ea-2629">Add support for windows clusters.</span></span> <span data-ttu-id="927ea-2630">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="927ea-2630">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="927ea-2631">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="927ea-2631">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="927ea-2632">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="927ea-2632">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="927ea-2633">AppService</span><span class="sxs-lookup"><span data-stu-id="927ea-2633">AppService</span></span>

* <span data-ttu-id="927ea-2634">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="927ea-2634">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="927ea-2635">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="927ea-2635">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="927ea-2636">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="927ea-2636">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="927ea-2637">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="927ea-2637">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="927ea-2638">DataLake</span><span class="sxs-lookup"><span data-stu-id="927ea-2638">DataLake</span></span>

* <span data-ttu-id="927ea-2639">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2639">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="927ea-2640">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="927ea-2640">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="927ea-2641">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="927ea-2641">DocuemntDB</span></span>

* <span data-ttu-id="927ea-2642">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="927ea-2642">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="927ea-2643">VM</span><span class="sxs-lookup"><span data-stu-id="927ea-2643">VM</span></span>

* <span data-ttu-id="927ea-2644">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="927ea-2644">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="927ea-2645">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="927ea-2645">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="927ea-2646">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="927ea-2646">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="927ea-2647">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="927ea-2647">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="927ea-2648">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="927ea-2648">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="927ea-2649">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="927ea-2649">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="927ea-2650">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="927ea-2650">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="927ea-2651">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="927ea-2651">February 27, 2017</span></span>

<span data-ttu-id="927ea-2652">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="927ea-2652">Version 2.0.0</span></span>

<span data-ttu-id="927ea-2653">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2653">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="927ea-2654">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="927ea-2654">Container Service (acs)</span></span>
- <span data-ttu-id="927ea-2655">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="927ea-2655">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="927ea-2656">네트워킹</span><span class="sxs-lookup"><span data-stu-id="927ea-2656">Networking</span></span>
- <span data-ttu-id="927ea-2657">Storage</span><span class="sxs-lookup"><span data-stu-id="927ea-2657">Storage</span></span>

<span data-ttu-id="927ea-2658">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2658">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="927ea-2659">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2659">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="927ea-2660">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2660">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="927ea-2661">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2661">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="927ea-2662">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="927ea-2662">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="927ea-2663">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="927ea-2663">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="927ea-2664">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="927ea-2664">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="927ea-2665">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="927ea-2665">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="927ea-2666">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="927ea-2666">Provide feedback from the command line with the `az feedback` command</span></span>


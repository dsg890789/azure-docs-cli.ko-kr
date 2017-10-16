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
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="85a43-104">Azure CLI 2.0 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="85a43-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="85a43-105">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="85a43-105">October 9, 2017</span></span>

<span data-ttu-id="85a43-106">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="85a43-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="85a43-107">코어</span><span class="sxs-lookup"><span data-stu-id="85a43-107">Core</span></span>

* <span data-ttu-id="85a43-108">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-109">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-109">Appservice</span></span>

* <span data-ttu-id="85a43-110">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="85a43-111">배치</span><span class="sxs-lookup"><span data-stu-id="85a43-111">Batch</span></span>

* <span data-ttu-id="85a43-112">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="85a43-113">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="85a43-114">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="85a43-115">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="85a43-116">Batchai</span><span class="sxs-lookup"><span data-stu-id="85a43-116">Batchai</span></span>

* <span data-ttu-id="85a43-117">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="85a43-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="85a43-118">Keyvault</span><span class="sxs-lookup"><span data-stu-id="85a43-118">Keyvault</span></span>

* <span data-ttu-id="85a43-119">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="85a43-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="85a43-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="85a43-121">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-121">Network</span></span>

* <span data-ttu-id="85a43-122">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="85a43-123">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="85a43-124">리소스</span><span class="sxs-lookup"><span data-stu-id="85a43-124">Resource</span></span>

* <span data-ttu-id="85a43-125">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="85a43-126">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="85a43-127">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="85a43-128">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="85a43-129">Sql</span><span class="sxs-lookup"><span data-stu-id="85a43-129">Sql</span></span>

* <span data-ttu-id="85a43-130">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="85a43-131">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="85a43-132">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-133">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-133">Storage</span></span>

* <span data-ttu-id="85a43-134">파일 공유 스냅숏에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-135">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-135">Vm</span></span>

* <span data-ttu-id="85a43-136">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="85a43-137">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="85a43-138">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="85a43-139">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="85a43-140">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="85a43-141">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="85a43-141">September 22, 2017</span></span>

<span data-ttu-id="85a43-142">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="85a43-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="85a43-143">리소스</span><span class="sxs-lookup"><span data-stu-id="85a43-143">Resource</span></span>

* <span data-ttu-id="85a43-144">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="85a43-145">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="85a43-146">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="85a43-147">[주요 변경 내용] `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 `managedapp` 리소스 종류 변경</span><span class="sxs-lookup"><span data-stu-id="85a43-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="85a43-148">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-148">Network</span></span>

* <span data-ttu-id="85a43-149">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="85a43-150">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="85a43-151">`asg` 응용 프로그램 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="85a43-152">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="85a43-153">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="85a43-154">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="85a43-155">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-156">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-156">Storage</span></span>

* <span data-ttu-id="85a43-157">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="85a43-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="85a43-158">Event Grid</span><span class="sxs-lookup"><span data-stu-id="85a43-158">Eventgrid</span></span>

* <span data-ttu-id="85a43-159">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="85a43-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="85a43-160">SQL</span><span class="sxs-lookup"><span data-stu-id="85a43-160">SQL</span></span>

* <span data-ttu-id="85a43-161">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="85a43-162">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="85a43-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="85a43-163">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="85a43-164">Keyvault</span><span class="sxs-lookup"><span data-stu-id="85a43-164">Keyvault</span></span>

* <span data-ttu-id="85a43-165">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-166">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-166">VM</span></span>

* <span data-ttu-id="85a43-167">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="85a43-168">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="85a43-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="85a43-169">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="85a43-170">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="85a43-171">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="85a43-172">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-173">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-173">ACS</span></span>

* <span data-ttu-id="85a43-174">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-175">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-175">Appservice</span></span>

* <span data-ttu-id="85a43-176">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="85a43-177">백업</span><span class="sxs-lookup"><span data-stu-id="85a43-177">Backup</span></span>

* <span data-ttu-id="85a43-178">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="85a43-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="85a43-179">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="85a43-179">September 11, 2017</span></span>

<span data-ttu-id="85a43-180">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="85a43-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="85a43-181">코어</span><span class="sxs-lookup"><span data-stu-id="85a43-181">Core</span></span>

* <span data-ttu-id="85a43-182">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="85a43-183">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-184">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-184">Acs</span></span>

* <span data-ttu-id="85a43-185">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="85a43-186">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="85a43-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-187">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-187">Appservice</span></span>

* <span data-ttu-id="85a43-188">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="85a43-189">CDN</span><span class="sxs-lookup"><span data-stu-id="85a43-189">CDN</span></span>

* <span data-ttu-id="85a43-190">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="85a43-191">내선 번호</span><span class="sxs-lookup"><span data-stu-id="85a43-191">Extension</span></span>

* <span data-ttu-id="85a43-192">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="85a43-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="85a43-193">Keyvault</span><span class="sxs-lookup"><span data-stu-id="85a43-193">Keyvault</span></span>

* <span data-ttu-id="85a43-194">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="85a43-195">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-195">Network</span></span>

* <span data-ttu-id="85a43-196">이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="85a43-197">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="85a43-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="85a43-198">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="85a43-199">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="85a43-200">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="85a43-201">리소스</span><span class="sxs-lookup"><span data-stu-id="85a43-201">Resource</span></span>

* <span data-ttu-id="85a43-202">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="85a43-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="85a43-203">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="85a43-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="85a43-204">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="85a43-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="85a43-205">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="85a43-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="85a43-206">SQL</span><span class="sxs-lookup"><span data-stu-id="85a43-206">SQL</span></span>

* <span data-ttu-id="85a43-207">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-208">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-208">VM</span></span>

* <span data-ttu-id="85a43-209">수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="85a43-210">수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함</span><span class="sxs-lookup"><span data-stu-id="85a43-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="85a43-211">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="85a43-212">수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="85a43-213">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="85a43-214">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="85a43-214">August 31, 2017</span></span>

<span data-ttu-id="85a43-215">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="85a43-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="85a43-216">Keyvault</span><span class="sxs-lookup"><span data-stu-id="85a43-216">Keyvault</span></span>

* <span data-ttu-id="85a43-217">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="85a43-218">Sf</span><span class="sxs-lookup"><span data-stu-id="85a43-218">Sf</span></span>

* <span data-ttu-id="85a43-219">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-220">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-220">Storage</span></span>

* <span data-ttu-id="85a43-221">저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="85a43-222">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="85a43-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="85a43-223">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="85a43-223">August 28, 2017</span></span>

<span data-ttu-id="85a43-224">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="85a43-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="85a43-225">CLI</span><span class="sxs-lookup"><span data-stu-id="85a43-225">CLI</span></span>

* <span data-ttu-id="85a43-226">`--version`에 법적 정보가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-227">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-227">ACS</span></span>

* <span data-ttu-id="85a43-228">미리 보기 지역이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-228">Corrected preview regions.</span></span>
* <span data-ttu-id="85a43-229">`dns_name_prefix`의 기본 형식이 올바르게 지정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="85a43-230">acs 명령 출력이 최적화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-231">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-231">Appservice</span></span>

* <span data-ttu-id="85a43-232">[주요 변경 내용] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="85a43-233">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="85a43-234">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="85a43-235">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="85a43-236">슬롯 설정을 올바르게 검색하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="85a43-237">IoT</span><span class="sxs-lookup"><span data-stu-id="85a43-237">IoT</span></span>

* <span data-ttu-id="85a43-238">#3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="85a43-239">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-239">Network</span></span>

* <span data-ttu-id="85a43-240">[주요 변경 내용] 이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="85a43-241">[주요 변경 내용] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="85a43-242">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="85a43-243">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="85a43-244">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="85a43-245">프로필</span><span class="sxs-lookup"><span data-stu-id="85a43-245">Profile</span></span>

* <span data-ttu-id="85a43-246">가상 컴퓨터의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="85a43-247">서비스 패브릭</span><span class="sxs-lookup"><span data-stu-id="85a43-247">Service Fabric</span></span>

* <span data-ttu-id="85a43-248">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="85a43-248">Preview release</span></span>
* <span data-ttu-id="85a43-249">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="85a43-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="85a43-250">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="85a43-251">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-252">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-252">Storage</span></span>

* <span data-ttu-id="85a43-253">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="85a43-254">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="85a43-255">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="85a43-256">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="85a43-257">[주요 변경 내용] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="85a43-258">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-259">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-259">VM</span></span>

* <span data-ttu-id="85a43-260">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="85a43-261">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="85a43-262">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="85a43-263">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="85a43-264">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="85a43-265">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="85a43-266">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="85a43-266">August 15, 2017</span></span>

<span data-ttu-id="85a43-267">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="85a43-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-268">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-268">ACS</span></span>

* <span data-ttu-id="85a43-269">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-270">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-270">Appservice</span></span>

* <span data-ttu-id="85a43-271">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="85a43-272">Event Grid</span><span class="sxs-lookup"><span data-stu-id="85a43-272">Event Grid</span></span>

* <span data-ttu-id="85a43-273">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="85a43-274">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="85a43-274">August 11, 2017</span></span>

<span data-ttu-id="85a43-275">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="85a43-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-276">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-276">ACS</span></span>

* <span data-ttu-id="85a43-277">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="85a43-278">배치</span><span class="sxs-lookup"><span data-stu-id="85a43-278">Batch</span></span>

* <span data-ttu-id="85a43-279">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="85a43-280">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="85a43-281">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="85a43-282">배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="85a43-283">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="85a43-284">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="85a43-285">구성 요소</span><span class="sxs-lookup"><span data-stu-id="85a43-285">Component</span></span>

* <span data-ttu-id="85a43-286">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="85a43-287">컨테이너</span><span class="sxs-lookup"><span data-stu-id="85a43-287">Container</span></span>

* <span data-ttu-id="85a43-288">`create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="85a43-289">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-289">Data Lake Store</span></span>

* <span data-ttu-id="85a43-290">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="85a43-291">Event Grid</span><span class="sxs-lookup"><span data-stu-id="85a43-291">Event Grid</span></span>

* <span data-ttu-id="85a43-292">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="85a43-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="85a43-293">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-293">Network</span></span>

* <span data-ttu-id="85a43-294">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="85a43-295">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="85a43-296">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="85a43-297">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="85a43-298">프로필</span><span class="sxs-lookup"><span data-stu-id="85a43-298">Profile</span></span>

* <span data-ttu-id="85a43-299">`account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-300">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-300">Storage</span></span>

* <span data-ttu-id="85a43-301">시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-302">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-302">VM</span></span>

* <span data-ttu-id="85a43-303">`availability-set`: 변환 시 오류 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="85a43-304">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="85a43-305">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="85a43-306">데이터 디스크 연결 시 저장소 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="85a43-307">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="85a43-308">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="85a43-308">July 28, 2017</span></span>

<span data-ttu-id="85a43-309">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="85a43-309">Version 2.0.12</span></span>

* <span data-ttu-id="85a43-310">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-310">Added container commands</span></span>
* <span data-ttu-id="85a43-311">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="85a43-312">코어</span><span class="sxs-lookup"><span data-stu-id="85a43-312">Core</span></span>

* <span data-ttu-id="85a43-313">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="85a43-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="85a43-314">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="85a43-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="85a43-315">현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="85a43-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="85a43-316">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="85a43-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="85a43-317">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="85a43-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="85a43-318">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="85a43-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="85a43-319">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="85a43-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="85a43-320">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="85a43-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="85a43-321">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="85a43-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="85a43-322">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="85a43-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="85a43-323">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="85a43-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="85a43-324">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="85a43-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="85a43-325">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="85a43-326">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="85a43-327">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="85a43-328">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="85a43-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="85a43-329">ACR</span><span class="sxs-lookup"><span data-stu-id="85a43-329">ACR</span></span>

* <span data-ttu-id="85a43-330">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="85a43-331">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="85a43-332">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="85a43-333">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="85a43-334">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="85a43-335">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-336">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-336">ACS</span></span>

* <span data-ttu-id="85a43-337">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-338">App Service</span><span class="sxs-lookup"><span data-stu-id="85a43-338">Appservice</span></span>

* <span data-ttu-id="85a43-339">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="85a43-340">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="85a43-341">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="85a43-342">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="85a43-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="85a43-343">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="85a43-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="85a43-344">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="85a43-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="85a43-345">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="85a43-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="85a43-346">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="85a43-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="85a43-347">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="85a43-348">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="85a43-349">배치</span><span class="sxs-lookup"><span data-stu-id="85a43-349">Batch</span></span>

* <span data-ttu-id="85a43-350">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="85a43-351">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="85a43-352">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="85a43-353">CDN</span><span class="sxs-lookup"><span data-stu-id="85a43-353">CDN</span></span>

* <span data-ttu-id="85a43-354">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="85a43-355">클라우드</span><span class="sxs-lookup"><span data-stu-id="85a43-355">Cloud</span></span>

* <span data-ttu-id="85a43-356">클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="85a43-357">갤러리 끝점이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="85a43-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="85a43-358">ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="85a43-359">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="85a43-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="85a43-360">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="85a43-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="85a43-361">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="85a43-361">CosmosDB</span></span>

* <span data-ttu-id="85a43-362">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="85a43-363">컬렉션 기본 TTL에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="85a43-364">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="85a43-364">Data Lake Analytics</span></span>

* <span data-ttu-id="85a43-365">`dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="85a43-366">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="85a43-367">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="85a43-368">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-368">Data Lake Store</span></span>

* <span data-ttu-id="85a43-369">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="85a43-370">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="85a43-371">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="85a43-372">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="85a43-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="85a43-373">대화형</span><span class="sxs-lookup"><span data-stu-id="85a43-373">Interactive</span></span>

* <span data-ttu-id="85a43-374">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="85a43-375">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-375">Increased test coverage</span></span>
* <span data-ttu-id="85a43-376">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="85a43-377">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="85a43-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="85a43-378">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="85a43-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="85a43-379">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="85a43-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="85a43-380">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="85a43-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="85a43-381">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-381">Added `--progress` flag</span></span>
* <span data-ttu-id="85a43-382">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="85a43-383">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="85a43-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="85a43-384">IoT</span><span class="sxs-lookup"><span data-stu-id="85a43-384">IoT</span></span>

* <span data-ttu-id="85a43-385">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="85a43-386">(#3934)</span><span class="sxs-lookup"><span data-stu-id="85a43-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="85a43-387">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="85a43-387">Key vault</span></span>

* <span data-ttu-id="85a43-388">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="85a43-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="85a43-389">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="85a43-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="85a43-390">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="85a43-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="85a43-391">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="85a43-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="85a43-392">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="85a43-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="85a43-393">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="85a43-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="85a43-394">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="85a43-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="85a43-395">(#3307)</span><span class="sxs-lookup"><span data-stu-id="85a43-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="85a43-396">랩</span><span class="sxs-lookup"><span data-stu-id="85a43-396">Lab</span></span>

* <span data-ttu-id="85a43-397">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="85a43-398">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="85a43-399">모니터</span><span class="sxs-lookup"><span data-stu-id="85a43-399">Monitor</span></span>

* <span data-ttu-id="85a43-400">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="85a43-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="85a43-401">이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="85a43-402">이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="85a43-403">이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="85a43-404">이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="85a43-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="85a43-405">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="85a43-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="85a43-406">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="85a43-407">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="85a43-408">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-408">`location` no longer required</span></span>
  * <span data-ttu-id="85a43-409">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="85a43-410">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="85a43-411">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="85a43-412">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="85a43-413">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="85a43-414">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="85a43-415">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="85a43-416">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-416">Network</span></span>

* <span data-ttu-id="85a43-417">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="85a43-418">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="85a43-419">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="85a43-420">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="85a43-421">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="85a43-422">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="85a43-423">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="85a43-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="85a43-424">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="85a43-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="85a43-425">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="85a43-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="85a43-426">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="85a43-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="85a43-427">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="85a43-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="85a43-428">`application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="85a43-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="85a43-429">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="85a43-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="85a43-430">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="85a43-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="85a43-431">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="85a43-432">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="85a43-433">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="85a43-434">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="85a43-435">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="85a43-436">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="85a43-437">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="85a43-438">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="85a43-439">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="85a43-440">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="85a43-441">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="85a43-442">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="85a43-443">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="85a43-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="85a43-444">프로필</span><span class="sxs-lookup"><span data-stu-id="85a43-444">Profile</span></span>

* <span data-ttu-id="85a43-445">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="85a43-446">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="85a43-447">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="85a43-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="85a43-448">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="85a43-449">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="85a43-450">RDBMS</span><span class="sxs-lookup"><span data-stu-id="85a43-450">RDBMS</span></span>

* <span data-ttu-id="85a43-451">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="85a43-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="85a43-452">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="85a43-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="85a43-453">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="85a43-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="85a43-454">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="85a43-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="85a43-455">리소스</span><span class="sxs-lookup"><span data-stu-id="85a43-455">Resource</span></span>

* <span data-ttu-id="85a43-456">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="85a43-457">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="85a43-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="85a43-458">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="85a43-459">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="85a43-460">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="85a43-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="85a43-461">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="85a43-462">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="85a43-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="85a43-463">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="85a43-464">역할</span><span class="sxs-lookup"><span data-stu-id="85a43-464">Role</span></span>

* <span data-ttu-id="85a43-465">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="85a43-466">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="85a43-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="85a43-467">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="85a43-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="85a43-468">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="85a43-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="85a43-469">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="85a43-470">서비스 패브릭</span><span class="sxs-lookup"><span data-stu-id="85a43-470">Service Fabric</span></span>
* <span data-ttu-id="85a43-471">업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="85a43-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="85a43-472">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="85a43-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="85a43-473">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="85a43-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="85a43-474">SQL</span><span class="sxs-lookup"><span data-stu-id="85a43-474">SQL</span></span>

* <span data-ttu-id="85a43-475">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="85a43-476">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="85a43-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="85a43-477">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-478">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-478">Storage</span></span>

* <span data-ttu-id="85a43-479">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="85a43-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="85a43-480">HTTPS 전용 저장소 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="85a43-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="85a43-481">저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="85a43-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="85a43-482">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="85a43-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="85a43-483">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="85a43-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="85a43-484">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="85a43-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-485">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-485">VM</span></span>

* <span data-ttu-id="85a43-486">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-486">Support configuring nsg</span></span>
* <span data-ttu-id="85a43-487">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="85a43-488">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="85a43-488">Support managed service identities</span></span>
* <span data-ttu-id="85a43-489">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="85a43-490">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="85a43-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="85a43-491">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="85a43-491">May 10, 2017</span></span>

<span data-ttu-id="85a43-492">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="85a43-492">Version 2.0.6</span></span>

* <span data-ttu-id="85a43-493">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="85a43-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="85a43-494">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="85a43-495">Data Lake Analytics 및 Data Lake Store 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="85a43-496">Cognitive Services 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="85a43-497">Service Fabric 모듈을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="85a43-498">대화형 모듈(az-shell 이름 바꾸기)을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="85a43-499">CDN 명령에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="85a43-500">컨테이너 모듈을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-500">Remove Container module.</span></span>
* <span data-ttu-id="85a43-501">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="85a43-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="85a43-502">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="85a43-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="85a43-503">코어</span><span class="sxs-lookup"><span data-stu-id="85a43-503">Core</span></span>

* <span data-ttu-id="85a43-504">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="85a43-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="85a43-505">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="85a43-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="85a43-506">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="85a43-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="85a43-507">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="85a43-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="85a43-508">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="85a43-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="85a43-509">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="85a43-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="85a43-510">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="85a43-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="85a43-511">core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="85a43-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="85a43-512">core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="85a43-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="85a43-513">core: 향상된 성능</span><span class="sxs-lookup"><span data-stu-id="85a43-513">core: Improved performance</span></span>
* <span data-ttu-id="85a43-514">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="85a43-515">core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용</span><span class="sxs-lookup"><span data-stu-id="85a43-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="85a43-516">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-516">ACS</span></span>

* <span data-ttu-id="85a43-517">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="85a43-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="85a43-518">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="85a43-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="85a43-519">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="85a43-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="85a43-520">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="85a43-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="85a43-521">AppService</span><span class="sxs-lookup"><span data-stu-id="85a43-521">AppService</span></span>

* <span data-ttu-id="85a43-522">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="85a43-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="85a43-523">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="85a43-524">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="85a43-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="85a43-525">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="85a43-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="85a43-526">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="85a43-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="85a43-527">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="85a43-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="85a43-528">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-528">support slot swap with preview</span></span>
* <span data-ttu-id="85a43-529">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="85a43-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="85a43-530">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="85a43-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="85a43-531">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="85a43-531">CosmosDB</span></span>

* <span data-ttu-id="85a43-532">documentdb 모듈 이름을 cosmosdb로 바꿈</span><span class="sxs-lookup"><span data-stu-id="85a43-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="85a43-533">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="85a43-534">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="85a43-535">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="85a43-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="85a43-536">데이터 레이크 분석</span><span class="sxs-lookup"><span data-stu-id="85a43-536">Data Lake Analytics</span></span>

* <span data-ttu-id="85a43-537">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="85a43-538">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="85a43-539">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="85a43-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="85a43-540">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="85a43-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="85a43-541">테이블</span><span class="sxs-lookup"><span data-stu-id="85a43-541">Table</span></span>
  * <span data-ttu-id="85a43-542">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="85a43-542">Table valued function</span></span>
  * <span data-ttu-id="85a43-543">보기</span><span class="sxs-lookup"><span data-stu-id="85a43-543">View</span></span>
  * <span data-ttu-id="85a43-544">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="85a43-544">Table Statistics.</span></span> <span data-ttu-id="85a43-545">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="85a43-546">데이터 레이크 저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-546">Data Lake Store</span></span>

* <span data-ttu-id="85a43-547">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 대해 보다 나은 지원을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="85a43-548">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="85a43-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="85a43-549">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="85a43-549">missed help for access show.</span></span> <span data-ttu-id="85a43-550">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-550">adding it.</span></span> <span data-ttu-id="85a43-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="85a43-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="85a43-552">찾기</span><span class="sxs-lookup"><span data-stu-id="85a43-552">Find</span></span>

* <span data-ttu-id="85a43-553">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="85a43-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="85a43-554">KeyVault</span><span class="sxs-lookup"><span data-stu-id="85a43-554">KeyVault</span></span>

* <span data-ttu-id="85a43-555">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="85a43-556">BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="85a43-557">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="85a43-558">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="85a43-559">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="85a43-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="85a43-560">랩</span><span class="sxs-lookup"><span data-stu-id="85a43-560">Lab</span></span>

* <span data-ttu-id="85a43-561">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="85a43-562">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="85a43-563">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="85a43-564">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="85a43-565">랩 내에서 비밀을 관리하는 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="85a43-566">모니터</span><span class="sxs-lookup"><span data-stu-id="85a43-566">Monitor</span></span>

* <span data-ttu-id="85a43-567">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="85a43-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="85a43-568">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="85a43-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="85a43-569">네트워크</span><span class="sxs-lookup"><span data-stu-id="85a43-569">Network</span></span>

* <span data-ttu-id="85a43-570">`network watcher test-connectivity` 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="85a43-571">`network watcher packet-capture create`에 대한 `--filters` 매개 변수 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="85a43-572">Application Gateway 연결 드레이닝에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="85a43-573">Application Gateway WAF 규칙 집합 구성에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="85a43-574">ExpressRoute 경로 필터 및 규칙에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="85a43-575">TrafficManager 지리적 라우팅에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="85a43-576">VPN 연결 정책 기반 트래픽 선택기에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="85a43-577">VPN 연결 IPSec 정책에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="85a43-578">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create`를 사용하여 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="85a43-579">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="85a43-580">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="85a43-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="85a43-581">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="85a43-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="85a43-582">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="85a43-583">레코드가 제대로 가져와지지 않는 `dns zone import`의 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="85a43-584">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="85a43-585">'network watcher' 미리 보기 명령을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="85a43-586">프로필</span><span class="sxs-lookup"><span data-stu-id="85a43-586">Profile</span></span>

* <span data-ttu-id="85a43-587">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="85a43-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="85a43-588">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="85a43-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="85a43-589">Redis</span><span class="sxs-lookup"><span data-stu-id="85a43-589">Redis</span></span>

* <span data-ttu-id="85a43-590">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="85a43-591">'update-settings' 명령은 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="85a43-592">리소스</span><span class="sxs-lookup"><span data-stu-id="85a43-592">Resource</span></span>

* <span data-ttu-id="85a43-593">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="85a43-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="85a43-594">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="85a43-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="85a43-595">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="85a43-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="85a43-596">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="85a43-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="85a43-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="85a43-598">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-598">Add docs for az lock update.</span></span> <span data-ttu-id="85a43-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="85a43-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="85a43-600">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="85a43-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="85a43-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="85a43-602">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="85a43-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="85a43-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="85a43-604">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="85a43-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="85a43-605">역할</span><span class="sxs-lookup"><span data-stu-id="85a43-605">Role</span></span>

* <span data-ttu-id="85a43-606">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="85a43-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="85a43-607">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="85a43-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="85a43-608">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="85a43-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="85a43-609">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="85a43-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="85a43-610">SQL</span><span class="sxs-lookup"><span data-stu-id="85a43-610">SQL</span></span>

* <span data-ttu-id="85a43-611">az sql server list-usages 및 az sql db list-usages 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="85a43-612">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="85a43-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="85a43-613">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-613">Storage</span></span>

* <span data-ttu-id="85a43-614">기본 위치를 `storage account create`에 대한 리소스 그룹 위치로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="85a43-615">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="85a43-616">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="85a43-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="85a43-617">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="85a43-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-618">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-618">VM</span></span>

* <span data-ttu-id="85a43-619">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="85a43-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="85a43-620">note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.</span><span class="sxs-lookup"><span data-stu-id="85a43-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="85a43-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="85a43-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="85a43-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="85a43-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="85a43-623">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="85a43-624">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="85a43-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="85a43-625">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="85a43-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="85a43-626">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="85a43-626">April 3, 2017</span></span>

<span data-ttu-id="85a43-627">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="85a43-627">Version 2.0.2</span></span>

<span data-ttu-id="85a43-628">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 출시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="85a43-629">코어</span><span class="sxs-lookup"><span data-stu-id="85a43-629">Core</span></span>

* <span data-ttu-id="85a43-630">기본 목록에 acr, 랩, 모니터 및 찾기 모듈을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="85a43-631">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="85a43-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="85a43-632">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="85a43-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="85a43-633">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="85a43-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="85a43-634">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="85a43-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="85a43-635">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="85a43-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="85a43-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="85a43-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="85a43-637">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="85a43-638">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="85a43-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="85a43-639">ACS</span><span class="sxs-lookup"><span data-stu-id="85a43-639">ACS</span></span>

* <span data-ttu-id="85a43-640">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="85a43-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="85a43-641">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="85a43-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="85a43-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="85a43-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="85a43-643">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="85a43-643">Add support for windows clusters.</span></span> <span data-ttu-id="85a43-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="85a43-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="85a43-645">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="85a43-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="85a43-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="85a43-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="85a43-647">AppService</span><span class="sxs-lookup"><span data-stu-id="85a43-647">AppService</span></span>

* <span data-ttu-id="85a43-648">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="85a43-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="85a43-649">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="85a43-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="85a43-650">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="85a43-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="85a43-651">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="85a43-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="85a43-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="85a43-652">DataLake</span></span>

* <span data-ttu-id="85a43-653">Data Lake Analytics 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="85a43-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="85a43-654">Data Lake Store 모듈의 초기 릴리스.</span><span class="sxs-lookup"><span data-stu-id="85a43-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="85a43-655">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="85a43-655">DocuemntDB</span></span>

* <span data-ttu-id="85a43-656">DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="85a43-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="85a43-657">VM</span><span class="sxs-lookup"><span data-stu-id="85a43-657">VM</span></span>

* <span data-ttu-id="85a43-658">[Compute] 가상 컴퓨터 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="85a43-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="85a43-659">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="85a43-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="85a43-660">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="85a43-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="85a43-661">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="85a43-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="85a43-662">가상 컴퓨터 확장 집합: vm의 인스턴스 보기를 나열하는 * 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="85a43-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="85a43-663">VM 및 가상 컴퓨터 확장 집합에 --secrets 추가([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="85a43-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="85a43-664">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="85a43-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="85a43-665">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="85a43-665">February 27, 2017</span></span>

<span data-ttu-id="85a43-666">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="85a43-666">Version 2.0.0</span></span>

<span data-ttu-id="85a43-667">Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="85a43-668">일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="85a43-669">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="85a43-669">Container Service (acs)</span></span>
- <span data-ttu-id="85a43-670">Compute(Resource Manager, VM, 가상 컴퓨터 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="85a43-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="85a43-671">네트워킹</span><span class="sxs-lookup"><span data-stu-id="85a43-671">Networking</span></span>
- <span data-ttu-id="85a43-672">저장소</span><span class="sxs-lookup"><span data-stu-id="85a43-672">Storage</span></span>

<span data-ttu-id="85a43-673">이러한 명령은 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="85a43-674">Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 개설할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="85a43-675">[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="85a43-676">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="85a43-677">CLI 버전을 확인하려면 `az --version`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="85a43-678">출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="85a43-679">일부 명령 모듈에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="85a43-680">이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="85a43-681">CLI 야간 미리 보기 빌드도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="85a43-682">자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85a43-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="85a43-683">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85a43-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="85a43-684">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="85a43-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="85a43-685">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.</span><span class="sxs-lookup"><span data-stu-id="85a43-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="85a43-686">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공.</span><span class="sxs-lookup"><span data-stu-id="85a43-686">Provide feedback from the command line with the `az feedback` command.</span></span>


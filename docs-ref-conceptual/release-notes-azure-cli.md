---
title: Azure CLI 릴리스 정보
description: Azure CLI 최신 업데이트 알아보기
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/13/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3ecb6fb41ee0ae60af58a02c934f2c295133f998
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913715"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="56085-103">Azure CLI 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="56085-103">Azure CLI release notes</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="56085-104">2020년 1월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-104">January 13, 2020</span></span>

<span data-ttu-id="56085-105">버전 2.0.80</span><span class="sxs-lookup"><span data-stu-id="56085-105">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="56085-106">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-106">Compute</span></span>

* <span data-ttu-id="56085-107">디스크 업데이트: --disk-encryption-set 및 --encryption-type 추가</span><span class="sxs-lookup"><span data-stu-id="56085-107">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="56085-108">스냅샷 만들기/업데이트: --disk-encryption-set 및 --encryption-type 추가</span><span class="sxs-lookup"><span data-stu-id="56085-108">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="56085-109">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-109">Storage</span></span>

* <span data-ttu-id="56085-110">azure-mgmt-storage 버전을 7.1.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="56085-110">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="56085-111">`az storage account create`: 테이블 및 큐 암호화 서비스를 지원하기 위해 `--encryption-key-type-for-table` 및 `--encryption-key-type-for-queue` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-111">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="56085-112">2020년 1월 7일</span><span class="sxs-lookup"><span data-stu-id="56085-112">January 07, 2020</span></span>

<span data-ttu-id="56085-113">버전 2.0.79</span><span class="sxs-lookup"><span data-stu-id="56085-113">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="56085-114">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-114">ACR</span></span>

* <span data-ttu-id="56085-115">[주요 변경 사항] 'acr build', 'acr task create/update', 'acr run' 및 'acr pack'에서 '--os' 매개 변수 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-115">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="56085-116">대신 '--platform'을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="56085-116">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="56085-117">AppConfig</span><span class="sxs-lookup"><span data-stu-id="56085-117">AppConfig</span></span>

* <span data-ttu-id="56085-118">기능 플래그 가져오기/내보내기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-118">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="56085-119">keyvault 참조를 만들려면 새 명령 'az appconfig kv set-keyvault' 추가</span><span class="sxs-lookup"><span data-stu-id="56085-119">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="56085-120">기능 플래그를 파일로 내보낼 때 다양한 명명 규칙 지원</span><span class="sxs-lookup"><span data-stu-id="56085-120">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-121">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-121">AppService</span></span>

* <span data-ttu-id="56085-122">이슈 #7154 해결: 작은따옴표 대신 백틱을 사용하도록 명령 <>에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-122">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="56085-123">이슈 #11287 해결: webapp up: up을 사용하여 만든 앱은 기본적으로 'SSL 사용'으로 설정되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-123">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="56085-124">이슈 #11592 해결: html 정적 사이트에 대한 az webapp up 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="56085-124">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="56085-125">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-125">ARM</span></span>

* <span data-ttu-id="56085-126">`az resource tag` 해결: Recovery Services 자격 증명 모음 태그를 업데이트할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-126">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="56085-127">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-127">Backup</span></span>

* <span data-ttu-id="56085-128">IaasVM 워크로드의 일시 삭제 기능을 지원하기 위해 새 명령 'backup protection undelete' 추가</span><span class="sxs-lookup"><span data-stu-id="56085-128">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="56085-129">backup-properties 명령을 설정하기 위해 새 매개 변수 '--soft-delete-feature-state' 추가</span><span class="sxs-lookup"><span data-stu-id="56085-129">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="56085-130">IaasVM 워크로드에 대한 디스크 제외 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-130">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="56085-131">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-131">Compute</span></span>

* <span data-ttu-id="56085-132">Azure Stack 프로필에서 `vm create` 오류 해결.</span><span class="sxs-lookup"><span data-stu-id="56085-132">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="56085-133">vm monitor metrics tail/list-definitions: vm에 쿼리 메트릭 및 목록 정의 지원</span><span class="sxs-lookup"><span data-stu-id="56085-133">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="56085-134">az vm의 새로운 다시 적용 명령 작업 추가</span><span class="sxs-lookup"><span data-stu-id="56085-134">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-135">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-135">HDInsight</span></span>

* <span data-ttu-id="56085-136">Kafka Rest 프록시로 Kafka 클러스터 생성 지원</span><span class="sxs-lookup"><span data-stu-id="56085-136">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="56085-137">azure-mgmt-hdinsight를 1.3.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="56085-137">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="56085-138">기타</span><span class="sxs-lookup"><span data-stu-id="56085-138">Misc.</span></span>

* <span data-ttu-id="56085-139">기본적으로 JSON 형식 또는 --output으로 구성된 형식으로 Azure CLI 모듈 및 확장 버전을 표시하기 위해 미리 보기 명령 `az version show` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-139">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="56085-140">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="56085-140">Event Hubs</span></span>

* <span data-ttu-id="56085-141">[주요 변경 사항] 'az eventhubs eventhub update' 및 'az eventhubs eventhub create' 명령에서 'ReceiveDisabled' 상태 옵션 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-141">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="56085-142">이 옵션은 이벤트 허브 항목에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-142">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="56085-143">Service Bus</span><span class="sxs-lookup"><span data-stu-id="56085-143">Service Bus</span></span>

* <span data-ttu-id="56085-144">[주요 변경 사항] 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' 및 'az servicebus queue update' 명령에서 'ReceiveDisabled' 상태 옵션 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-144">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="56085-145">이 옵션은 Service Bus 항목 및 큐에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-145">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-146">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-146">RBAC</span></span>

* <span data-ttu-id="56085-147">#11712 해결: 애플리케이션 또는 서비스 주체가 없을 때 `az ad app/sp show`가 종료 코드 3을 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-147">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="56085-148">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-148">Storage</span></span>

* <span data-ttu-id="56085-149">`az storage account create`: --enable-hierarchical-namespace 매개 변수에 대한 미리 보기 플래그 제거</span><span class="sxs-lookup"><span data-stu-id="56085-149">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="56085-150">api 버전 2019-06-01을 사용하도록 azure-mgmt-storage 버전이 7.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-150">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="56085-151">스토리지 계정 blob-service-properties에 대한 보존 정책 삭제 관리를 지원하도록 새 매개 변수 `--enable-delete-retention` 및 `--delete-retention-days` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-151">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="56085-152">2019년 12월 17일</span><span class="sxs-lookup"><span data-stu-id="56085-152">December 17, 2019</span></span>

<span data-ttu-id="56085-153">2.0.78</span><span class="sxs-lookup"><span data-stu-id="56085-153">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="56085-154">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-154">ACR</span></span>

* <span data-ttu-id="56085-155">acr task run에 로컬 컨텍스트 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-155">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="56085-156">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-156">ACS</span></span>

* <span data-ttu-id="56085-157">[주요 변경 사항]az openshift create: `--workspace-resource-id`에서 `--workspace-id`로 이름이 변경됨.</span><span class="sxs-lookup"><span data-stu-id="56085-157">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="56085-158">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-158">AMS</span></span>

* <span data-ttu-id="56085-159">리소스를 찾을 수 없을 때 3을 반환하도록 show 명령 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-159">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="56085-160">AppConfig</span><span class="sxs-lookup"><span data-stu-id="56085-160">AppConfig</span></span>

* <span data-ttu-id="56085-161">요청 url에 api-version을 추가할 때 버그 해결.</span><span class="sxs-lookup"><span data-stu-id="56085-161">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="56085-162">기존 해결책은 페이지 매김과 함께 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-162">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="56085-163">백 엔드 서비스에서 세계화를 위한 유니코드를 지원함에 따라 영어 이외의 언어를 표시하는 지원 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-163">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-164">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-164">AppService</span></span>

* <span data-ttu-id="56085-165">이슈 #11217 해결: webapp: az webapp config ssl upload가 슬롯 매개 변수를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-165">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="56085-166">이슈 #10965 해결: 오류: 이름을 비워 둘 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-166">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="56085-167">ip_address 및 subnet으로 제거 허용</span><span class="sxs-lookup"><span data-stu-id="56085-167">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="56085-168">Key Vault `az webapp config ssl import`에서 인증서 가져오기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-168">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="56085-169">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-169">ARM</span></span>

* <span data-ttu-id="56085-170">6\.0.0을 사용하도록 azure-mgmt-resource 패키지가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-170">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="56085-171">새 매개 변수 `--aux-subs`를 추가하여 `az group deployment create` 명령에 대한 교차 테넌트 지원</span><span class="sxs-lookup"><span data-stu-id="56085-171">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="56085-172">정책 세트 정의에 대한 메타데이터 정보 추가를 지원하기 위해 새 매개 변수 `--metadata` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-172">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="56085-173">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-173">Backup</span></span>

* <span data-ttu-id="56085-174">SQL 및 SAP Hana 워크로드에 대한 Backup 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-174">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-175">BotService</span><span class="sxs-lookup"><span data-stu-id="56085-175">BotService</span></span>

* <span data-ttu-id="56085-176">[주요 변경 사항] 미리 보기 명령 'az bot create'에서 '--version' 플래그 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-176">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="56085-177">v4 SDK 봇만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-177">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="56085-178">'az bot create'에 대한 이름 가용성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="56085-178">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="56085-179">'az bot update'를 통해 봇의 아이콘 URL 업데이트에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-179">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="56085-180">'az bot directline update'를 통해 Direct Line 채널을 업데이트하는 기능에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-180">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="56085-181">'az bot directline create'에 '--enable-enhanced-auth' 플래그 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-181">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="56085-182">'az bot authsetting' 명령 그룹은 미리 보기 상태가 아니라 GA입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-182">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="56085-183">'az bot'의 'create', 'prepare-deploy', 'show', 'delete', 'update' 명령은 미리 보기 상태가 아니라 GA입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-183">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="56085-184">'--proj-file-path' 값을 소문자로 변경(예: "Test.csproj"를 "test.csproj"로)하는 'az bot prepare-deploy' 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="56085-184">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="56085-185">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-185">Compute</span></span>

* <span data-ttu-id="56085-186">vmss create/update: VMSS를 축소할 때 어떤 가상 머신을 제거할지 결정하는 --scale-in-policy 추가</span><span class="sxs-lookup"><span data-stu-id="56085-186">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="56085-187">vm/vmss update: --priority 추가</span><span class="sxs-lookup"><span data-stu-id="56085-187">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="56085-188">vm/vmss update: --max-price 추가</span><span class="sxs-lookup"><span data-stu-id="56085-188">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="56085-189">disk-encryption-set 명령 그룹(create, show, update, delete, list) 추가</span><span class="sxs-lookup"><span data-stu-id="56085-189">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="56085-190">disk create: --encryption-type 및 --disk-encryption-set 추가</span><span class="sxs-lookup"><span data-stu-id="56085-190">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="56085-191">vm/vmss create: --os-disk-encryption-set 및 --data-disk-encryption-sets 추가</span><span class="sxs-lookup"><span data-stu-id="56085-191">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="56085-192">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-192">Core</span></span>

* <span data-ttu-id="56085-193">Python 3.4에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="56085-193">Removed support for Python 3.4</span></span>
* <span data-ttu-id="56085-194">여러 명령에 HaTS 설문 조사 연결</span><span class="sxs-lookup"><span data-stu-id="56085-194">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="56085-195">DLS</span><span class="sxs-lookup"><span data-stu-id="56085-195">DLS</span></span>

* <span data-ttu-id="56085-196">ADLS sdk 버전이 업데이트되었습니다(0.0.48).</span><span class="sxs-lookup"><span data-stu-id="56085-196">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="56085-197">설치</span><span class="sxs-lookup"><span data-stu-id="56085-197">Install</span></span>

* <span data-ttu-id="56085-198">설치 스크립트 지원(python 3.8)</span><span class="sxs-lookup"><span data-stu-id="56085-198">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="56085-199">IOT</span><span class="sxs-lookup"><span data-stu-id="56085-199">IOT</span></span>

* <span data-ttu-id="56085-200">[주요 변경 사항] manual-failover에서 --failover-region 매개 변수 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-200">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="56085-201">이제 할당된, 지리적으로 연결된 보조 지역으로 장애 조치(failover)됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-201">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-202">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-202">Key Vault</span></span>

* <span data-ttu-id="56085-203">#8095 해결: `az keyvault storage remove`: 도움말 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="56085-203">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="56085-204">#8921 해결: `az keyvault key/secret/certificate list/list-deleted/list-versions`: 매개 변수 `--maxresults`의 유효성 검사 버그 해결</span><span class="sxs-lookup"><span data-stu-id="56085-204">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="56085-205">#10512 해결: `az keyvault set-policy`: `--object-id`, `--spn` 또는 `--upn`이 지정된 경우 오류 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="56085-205">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="56085-206">#10846 해결: `az keyvault secret show-deleted`: `--id`가 지정된 경우 `--name/-n`이 필요 없습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-206">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="56085-207">#11084 해결: `az keyvault secret download`: 매개 변수 `--encoding`의 도움말 메시지 개선</span><span class="sxs-lookup"><span data-stu-id="56085-207">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="56085-208">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-208">Network</span></span>

* <span data-ttu-id="56085-209">az network application-gateway probe: 생성 및 업데이트 시 백엔드 서버를 검색할 포트를 지정하는 --port 옵션에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-209">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="56085-210">az network application-gateway url-path-map create/update: `--waf-policy`에 대한 버그 해결</span><span class="sxs-lookup"><span data-stu-id="56085-210">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="56085-211">az network application-gateway: `--rewrite-rule-set` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-211">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="56085-212">az network list-service-aliases: 서비스 엔드포인트 정책에 사용할 수 있는 지원 목록 서비스 별칭 추가</span><span class="sxs-lookup"><span data-stu-id="56085-212">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="56085-213">az network dns zone import: 레코드 이름에 .@ 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-213">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="56085-214">패키징</span><span class="sxs-lookup"><span data-stu-id="56085-214">Packaging</span></span>

* <span data-ttu-id="56085-215">pip 설치를 위한 백 에지 빌드 추가</span><span class="sxs-lookup"><span data-stu-id="56085-215">Added back edge builds for pip install</span></span>
* <span data-ttu-id="56085-216">Ubuntu eoan 패키지 추가</span><span class="sxs-lookup"><span data-stu-id="56085-216">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="56085-217">정책</span><span class="sxs-lookup"><span data-stu-id="56085-217">Policy</span></span>

* <span data-ttu-id="56085-218">정책 API 버전 2019-09-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-218">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="56085-219">az policy set-definition: 정책 세트 정의 내에서 `--definition-groups` 매개 변수를 사용한 그룹화 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-219">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="56085-220">Redis</span><span class="sxs-lookup"><span data-stu-id="56085-220">Redis</span></span>

* <span data-ttu-id="56085-221">`az redis create` 명령에 `--replicas-per-master` 미리 보기 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-221">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="56085-222">azure-mgmt-redis가 6.0.0에서 7.0.0rc1로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-222">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="56085-223">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="56085-223">ServiceFabric</span></span>

* <span data-ttu-id="56085-224">#10963을 포함한 노드 유형 추가 논리 이슈 해결: 내구성 수준이 Gold인 새 노드 유형을 추가할 때마다 CLI 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-224">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="56085-225">생성 템플릿에서 ServiceFabricNodeVmExt 버전이 1.1로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-225">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="56085-226">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-226">SQL</span></span>

* <span data-ttu-id="56085-227">읽기 확장 관리를 지원하도록 sql db create 및 update 명령에 "--read-scale" 및 "--read-replicas" 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-227">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="56085-228">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-228">Storage</span></span>

* <span data-ttu-id="56085-229">스토리지 계정 만들기 및 업데이트 명령의 GA 릴리스 대용량 파일 공유 속성</span><span class="sxs-lookup"><span data-stu-id="56085-229">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="56085-230">GA 릴리스 사용자 위임 SAS 토큰 지원</span><span class="sxs-lookup"><span data-stu-id="56085-230">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="56085-231">스토리지 계정의 blob service 속성을 관리하기 위해 새 명령 `az storage account blob-service-properties show` 및 `az storage account blob-service-properties update --enable-change-feed` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-231">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="56085-232">[예정된 호환성이 손상되는 변경] `az storage copy`: `*` 문자는 더 이상 URL에서 와일드카드로 지원되지 않지만 `*` 와일드카드 지원과 함께 새 매개 변수 --include-pattern 및 --exclude-pattern이 추가될 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-232">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="56085-233">이슈 #11043 해결: `az storage remove` 명령에서 전체 컨테이너/공유를 제거하는 지원 기능 추가</span><span class="sxs-lookup"><span data-stu-id="56085-233">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="56085-234">2019년 11월 26일</span><span class="sxs-lookup"><span data-stu-id="56085-234">November 26, 2019</span></span>

<span data-ttu-id="56085-235">버전 2.0.77</span><span class="sxs-lookup"><span data-stu-id="56085-235">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="56085-236">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-236">ACR</span></span>

* <span data-ttu-id="56085-237">acr task create/update의 `--branch` 매개 변수가 더 이상 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-237">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="56085-238">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="56085-238">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="56085-239">`--workspace-resource-id` 플래그가 추가되어 모니터링으로 Azure Red Hat Openshift 클러스터 생성 가능</span><span class="sxs-lookup"><span data-stu-id="56085-239">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="56085-240">모니터링으로 Azure Red Hat OpenShift 클러스터를 만드는 `monitor_profile`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-240">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="56085-241">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-241">AKS</span></span>

* <span data-ttu-id="56085-242">"az aks rotate-certs"를 사용한 지원 클러스터 인증서 순환 작업이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-242">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="56085-243">AppConfig</span><span class="sxs-lookup"><span data-stu-id="56085-243">AppConfig</span></span>

* <span data-ttu-id="56085-244">":"을 `as az appconfig kv import` 구분 기호로 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-244">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="56085-245">Null 레이블을 포함하여 여러 레이블이 있는 키 값을 나열하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-245">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="56085-246">관리 평면 sdk, azure-mgmt-appconfiguration이 버전 0.3.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-246">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="56085-247">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-247">AppService</span></span>

* <span data-ttu-id="56085-248">#11100 문제가 해결됨: 서비스 계획을 만들 때 az webapp up의 AttributeError</span><span class="sxs-lookup"><span data-stu-id="56085-248">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="56085-249">az webapp up: 지원되는 언어를 위해 사이트를 만들거나 배포하도록 적용하면 기본값이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-249">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="56085-250">App Service Environment에 대한 지원 추가t: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="56085-250">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="56085-251">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-251">Backup</span></span>

* <span data-ttu-id="56085-252">az backup policy list-associated-items 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-252">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="56085-253">선택적 BackupManagementType 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-253">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="56085-254">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-254">Compute</span></span>

* <span data-ttu-id="56085-255">컴퓨팅, 디스크, 스냅샷의 API 버전이 2019-07-01로 업그레이드되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-255">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="56085-256">vmss create: --orchestration-mode 개선</span><span class="sxs-lookup"><span data-stu-id="56085-256">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="56085-257">sig image-definition create: --os-state가 추가되어 이 이미지로 생성된 가상 머신이 'Generalized'인지 아니면 'Specialized'인지 지정 가능</span><span class="sxs-lookup"><span data-stu-id="56085-257">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="56085-258">sig image-definition create: --hyper-v-generation이 추가되어 하이퍼바이저 세대 지정 가능</span><span class="sxs-lookup"><span data-stu-id="56085-258">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="56085-259">sig image-version create: 지원 --os-snapshot 및 --data-snapshots 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-259">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="56085-260">image create: --data-disk-caching이 추가되어 데이터 디스크의 캐싱 설정을 지정할 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-260">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="56085-261">Python Compute SDK를 10.0.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="56085-261">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="56085-262">vm/vmss create: 'Priority' 열거형 속성에 'Spot' 추가</span><span class="sxs-lookup"><span data-stu-id="56085-262">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="56085-263">[주요 변경 사항] Swagger 및 Powershell cmdlet과 일치하도록 VM 및 VMSS에 대한 '--max-billing' 매개 변수의 이름이 '--max-price'로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-263">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="56085-264">vm monitor log show: 연결된 로그 분석 작업 영역을 통한 로그 쿼리에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-264">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="56085-265">IOT</span><span class="sxs-lookup"><span data-stu-id="56085-265">IOT</span></span>

* <span data-ttu-id="56085-266">#2531 수정됨: 허브 업데이트에 대한 편의 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-266">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="56085-267">#8323 수정됨: 스토리지 사용자 지정 엔드포인트를 만드는 누락된 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-267">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="56085-268">재발 버그 수정: 기본 스토리지 엔드포인트를 재정의하는 변경 사항을 되돌렸습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-268">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-269">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-269">Key Vault</span></span>

* <span data-ttu-id="56085-270">#11121 수정됨: `az keyvault certificate list`를 사용하는 경우 `--include-pending`을 전달할 때 이제 `true` 또는 `false` 값이 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-270">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="56085-271">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="56085-271">NetAppFiles</span></span>

* <span data-ttu-id="56085-272">azure-mgmt-netapp이 0.7.0으로 업그레이드되고, 여기에는 향후 복제 작업과 연결된 몇 가지 추가 볼륨 속성이 포함됨</span><span class="sxs-lookup"><span data-stu-id="56085-272">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="56085-273">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-273">Network</span></span>

* <span data-ttu-id="56085-274">application-gateway waf-config: 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-274">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="56085-275">application-gateway waf-policy: 관리형 규칙 집합과 제외 규칙을 관리하는 하위 그룹 managed-rules가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-275">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="56085-276">application-gateway waf-policy: waf-policy의 글로벌 구성을 관리하는 하위 그룹 policy-setting이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-276">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="56085-277">[주요 변경 사항] application-gateway waf-policy: 하위 그룹 규칙의 이름이 custom-rule로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-277">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="56085-278">application-gateway http-listener: 생성 시 --firewall-policy가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-278">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="56085-279">application-gateway url-path-map 규칙: 생성 시 --firewall-policy가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-279">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="56085-280">패키징</span><span class="sxs-lookup"><span data-stu-id="56085-280">Packaging</span></span>

* <span data-ttu-id="56085-281">az wrapper가 Python으로 다시 작성됨</span><span class="sxs-lookup"><span data-stu-id="56085-281">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="56085-282">Python 3.8에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-282">Added support for Python 3.8</span></span>
* <span data-ttu-id="56085-283">RPM 패키지의 경우 Python 3으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-283">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="56085-284">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-284">Profile</span></span>

* <span data-ttu-id="56085-285">Microsoft 계정으로 `az login -u {} -p {}` 실행 시 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-285">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="56085-286">자체 서명된 루트 인증서로 프록시 뒤에서 `az login` 실행 시 `SSLError`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-286">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="56085-287">#10578 수정됨: Windows 또는 WSL에서 동시에 둘 이상의 인스턴스가 시작되면 `az login`이 중단됨</span><span class="sxs-lookup"><span data-stu-id="56085-287">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="56085-288">#11059 수정됨: 테넌트에 구독이 있는 경우`az login --allow-no-subscriptions`가 실패함</span><span class="sxs-lookup"><span data-stu-id="56085-288">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="56085-289">#11238 수정됨: 구독 이름을 바꾼 후 MSI로 로그인하면 동일한 구독이 두 번 나타남</span><span class="sxs-lookup"><span data-stu-id="56085-289">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-290">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-290">RBAC</span></span>

* <span data-ttu-id="56085-291">#10996 수정됨: `--password`가 지정되지 않은 경우 `az ad user update`의 `--force-change-password-next-login`에 대한 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-291">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="56085-292">Redis</span><span class="sxs-lookup"><span data-stu-id="56085-292">Redis</span></span>

* <span data-ttu-id="56085-293">#2902 수정됨: 기본 SKU 캐시를 업데이트하는 동안 메모리 구성을 설정하지 마십시오</span><span class="sxs-lookup"><span data-stu-id="56085-293">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="56085-294">예약</span><span class="sxs-lookup"><span data-stu-id="56085-294">Reservations</span></span>

* <span data-ttu-id="56085-295">SDK 버전을 0.6.0으로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="56085-295">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="56085-296">Get-Gatalogs를 호출한 후 billingplan 세부 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-296">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="56085-297">예약 가격을 계산하는 새 명령 `az reservations reservation-order calculate`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-297">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="56085-298">새 예약을 구입하는 `az reservations reservation-order purchase`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-298">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="56085-299">REST</span><span class="sxs-lookup"><span data-stu-id="56085-299">Rest</span></span>
* <span data-ttu-id="56085-300">`az rest`가 GA로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-300">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="56085-301">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-301">SQL</span></span>

* <span data-ttu-id="56085-302">azure-mgmt-sql이 버전 0.15.0으로 업그레이드됨</span><span class="sxs-lookup"><span data-stu-id="56085-302">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="56085-303">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-303">Storage</span></span>

* <span data-ttu-id="56085-304">storage account create: Blob service에서 파일 시스템 의미 체계를 지원하는 --enable-hierarchical-namespace가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-304">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="56085-305">오류 메시지에서 관련되지 않은 예외가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-305">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="56085-306">잘못된 오류 메시지 "이 작업을 수행하는 데 필요한 권한이 없습니다." 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-306">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="56085-307">네트워크 규칙 또는 AuthenticationFailed로 차단된 경우</span><span class="sxs-lookup"><span data-stu-id="56085-307">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="56085-308">2019년 11월 4일</span><span class="sxs-lookup"><span data-stu-id="56085-308">November 4, 2019</span></span>

<span data-ttu-id="56085-309">버전 2.0.76</span><span class="sxs-lookup"><span data-stu-id="56085-309">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="56085-310">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-310">ACR</span></span>

* <span data-ttu-id="56085-311">`az acr pack build` 명령에 `--pack-image-tag` 미리 보기 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-311">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="56085-312">레지스트리 생성에 대한 감사를 가능하게 하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-312">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="56085-313">리포지토리 범위 RBAC에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-313">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="56085-314">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-314">AKS</span></span>

* <span data-ttu-id="56085-315">노드 풀에 대한 클러스터 자동 크기 조정기를 사용할 수 있도록 `--enable-cluster-autoscaler`, `--min-count` 및 `--max-count`를 `az aks create` 명령에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-315">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="56085-316">위의 플래그뿐만 아니라 클러스터 자동 크기 조정기를 업데이트할 수 있도록 `--update-cluster-autoscaler` 및 `--disable-cluster-autoscaler`도 `az aks update` 명령에 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-316">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="56085-317">AppConfig</span><span class="sxs-lookup"><span data-stu-id="56085-317">AppConfig</span></span>

* <span data-ttu-id="56085-318">App Configuration에 저장된 기능 플래그를 관리하는 appconfig 기능 명령 그룹을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-318">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="56085-319">appconfig kv export to file 명령에 대한 사소한 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-319">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="56085-320">내보내는 동안 대상 파일 콘텐츠 읽기를 중지합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-320">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-321">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-321">AppService</span></span>

* <span data-ttu-id="56085-322">`az appservice plan create`: appservice plan create에서 'persitescaling'을 설정하는 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-322">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="56085-323">webapp config ssl bind 작업이 리소스에서 기존 태그를 제거하는 문제를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-323">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="56085-324">함수 앱을 배포하는 동안 원격 빌드 작업을 지원하기 위해 `az functionapp deployment source config-zip`에 대해 `--build-remote` 플래그를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-324">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="56085-325">Windows의 경우 함수 앱의 기본 노드 버전을 ~10으로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-325">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="56085-326">`az functionapp create`에 `--runtime-version` 속성 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-326">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="56085-327">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-327">ARM</span></span>

* <span data-ttu-id="56085-328">`az deployment/group deployment validate`: 배포 시 json 템플릿에서 여러 줄과 주석을 지원하기 위해 `--handle-extended-json-format` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-328">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="56085-329">azure-mgmt-resource가 2019-07-01로 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-329">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="56085-330">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-330">Backup</span></span>

* <span data-ttu-id="56085-331">AzureFiles 백업 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-331">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="56085-332">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-332">Compute</span></span>

* <span data-ttu-id="56085-333">`az vm create`: 가속화된 네트워킹 및 기존 NIC를 함께 지정하는 경우 경고를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-333">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="56085-334">`az vm create`: 가상 머신을 할당해야 하는 기존 가상 머신 확장 집합을 지정하는 `--vmss`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-334">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="56085-335">`az vm/vmss create`: 제한된 네트워크 환경에서 액세스할 수 있도록 이미지 별칭 파일의 로컬 복사본을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-335">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="56085-336">`az vmss create`: 확장 집합에서 가상 머신을 관리하는 방법을 지정하는 `--orchestration-mode`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-336">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="56085-337">`az vm/vmss update`: Ultra SSD 설정 업데이트를 허용하는 `--ultra-ssd-enabled`를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-337">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="56085-338">[호환성이 손상되는 변경] `az vm extension set`: 사용자가 `--ids`를 사용하여 VM에서 확장을 설정할 수 없는 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-338">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="56085-339">Azure Marketplace 이미지 용어를 관리하는 `az vm image terms accept/cancel/show` 명령을 새로 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-339">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="56085-340">VMAccessForLinux가 버전 1.5로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-340">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-341">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-341">CosmosDB</span></span>

* <span data-ttu-id="56085-342">[호환성이 손상되는 변경] `az sql container create`: `--partition-key-path`가 필수 매개 변수로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-342">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="56085-343">[호환성이 손상되는 변경] `az gremlin graph create`: `--partition-key-path`가 필수 매개 변수로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-343">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="56085-344">`az sql container create`: `--unique-key-policy` 및 `--conflict-resolution-policy`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-344">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="56085-345">`az sql container create/update`: `--idx` 기본 스키마가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-345">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="56085-346">`gremlin graph create`: `--conflict-resolution-policy`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-346">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="56085-347">`gremlin graph create/update`: `--idx` 기본 스키마가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-347">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="56085-348">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="56085-348">Fixed typo in help message</span></span>
* <span data-ttu-id="56085-349">데이터베이스: 사용 중단 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-349">database: Added deprecation infomation</span></span>
* <span data-ttu-id="56085-350">컬렉션: 사용 중단 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-350">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="56085-351">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-351">IoT</span></span>

* <span data-ttu-id="56085-352">새 라우팅 원본 유형이 추가됨: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="56085-352">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="56085-353">`az iot hub create`에서 누락된 기능이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-353">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-354">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-354">Key Vault</span></span>

* <span data-ttu-id="56085-355">인증서 파일이 없을 때 발생하는 예기치 않은 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-355">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="56085-356">`az keyvault recover/purge`가 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-356">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="56085-357">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="56085-357">NetAppFiles</span></span>

* <span data-ttu-id="56085-358">API 버전 2019-07-01을 사용 하도록 azure-mgmt-netapp을 0.6.0으로 업그레이드했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-358">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="56085-359">이 새로운 API 버전에는 다음이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-359">This new API version includes:</span></span>

    - <span data-ttu-id="56085-360">볼륨 만들기 `--protocol-types`에서 이제는 "NFSv4"가 아닌 "NFSv4.1"이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-360">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="56085-361">볼륨 내보내기 정책 속성의 이름은 이제 'nfsv4'가 아닌 'nfsv41'입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-361">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="56085-362">볼륨 `--creation-token`의 이름이 `--file-path`로 바뀌었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-362">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="56085-363">스냅샷 생성 날짜가 이제 'created'라는 이름으로만 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-363">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="56085-364">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-364">Network</span></span>

* <span data-ttu-id="56085-365">`az network private-dns link vnet create/update`: 교차 테넌트 가상 네트워킹 연결을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-365">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="56085-366">[호환성이 손상되는 변경] `az network vnet subnet list`: `--resource-group` 및 `--vnet-name`이 이제 필수 항목으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-366">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="56085-367">`az network public-ip prefix create`: 생성 시 IP 주소 버전(IPv4, IPv6)을 지정하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-367">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="56085-368">azure-mgmt-network를 7.0.0으로 향상시키고 api-version을 2019-09-01로 증가함</span><span class="sxs-lookup"><span data-stu-id="56085-368">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="56085-369">`az network vrouter`: 새 서비스 가상 라우터 및 가상 라우터 피어링에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-369">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="56085-370">`az network express-route gateway connection`: `--internet-security`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-370">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-371">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-371">Profile</span></span>

* <span data-ttu-id="56085-372">`az account get-access-token --resource-type ms-graph`가 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-372">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="56085-373">`az login`에서 경고 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-373">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-374">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-374">RBAC</span></span>

* <span data-ttu-id="56085-375">`az ad app update --id {} --display-name {}`이 작동하지 않는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-375">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="56085-376">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="56085-376">ServiceFabric</span></span>

* <span data-ttu-id="56085-377">`az sf cluster create`: service fabric linux 및 windows template.json compute vmss를 표준에서 관리 디스크로 수정하여 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-377">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="56085-378">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-378">SQL</span></span>

* <span data-ttu-id="56085-379">새 SQL Database 제품에 대한 CRUD 작업을 지원하기 위해 `--compute-model`, `--auto-pause-delay` 및 `--min-capacity` 매개 변수를 추가했습니다. 서버리스 컴퓨팅 모델.</span><span class="sxs-lookup"><span data-stu-id="56085-379">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="56085-380">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-380">Storage</span></span>

* <span data-ttu-id="56085-381">`az storage account create/update`: --enable-files-adds 매개 변수 및 Azure Active Directory 속성 인수 그룹이 추가되어 Azure Files Active Directory 도메인 서비스 인증을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-381">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="56085-382">스토리지 계정의 Kerberos 키 나열 또는 다시 생성을 지원하도록 `az storage account keys list/renew`를 확장했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-382">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="56085-383">2019년 10월 15일</span><span class="sxs-lookup"><span data-stu-id="56085-383">October 15, 2019</span></span>

<span data-ttu-id="56085-384">버전 2.0.75</span><span class="sxs-lookup"><span data-stu-id="56085-384">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="56085-385">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-385">AKS</span></span>

* <span data-ttu-id="56085-386">Kubernetes 버전에서 지원되는 경우 `--load-balancer-sku` 기본값이 `standard`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-386">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="56085-387">Kubernetes 버전에서 지원되는 경우 `--vm-set-type` 기본값이 `virtualmachinescalesets`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-387">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="56085-388">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-388">AMS</span></span>

* <span data-ttu-id="56085-389">[주요 변경 사항]`job start`의 이름이 `job create`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-389">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="56085-390">[주요 변경 사항] UTF8 대신 32자 16진수 문자열을 사용하도록 `content-key-policy create`의 `--ask` 매개 변수가 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-390">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-391">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-391">AppService</span></span>

* <span data-ttu-id="56085-392">`webapp config access-restriction show|set|add|remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-392">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="56085-393">`webapp up`에 더 나은 오류 처리 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-393">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="56085-394">`Isolated` SKU에 대한 지원이 `appservice plan update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-394">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="56085-395">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-395">ARM</span></span>

* <span data-ttu-id="56085-396">json 템플릿에서 여러 줄과 주석을 지원하기 위해 `--handle-extended-json-format` 매개 변수가 `deployment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-396">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="56085-397">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-397">Compute</span></span>

* <span data-ttu-id="56085-398">`--enable-agent` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-398">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="56085-399">영역 사용 시 표준 공용 IP SKU를 자동으로 사용하도록 `vm create`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-399">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="56085-400">VM에 대해 유효한 컴퓨터 이름을 자동으로 만들도록 `vm create`이 변경됨(제공되지 않은 경우)</span><span class="sxs-lookup"><span data-stu-id="56085-400">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="56085-401">VMSS에서 가상 머신의 사용자 지정 컴퓨터 이름 접두사를 지원하기 위해 `vmss create`에 `--computer-name-prefix` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-401">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="56085-402">로그 분석 작업 영역을 자동으로 사용하도록 `vm create`에 `--workspace` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-402">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="56085-403">갤러리 API 버전이 2019-07-01로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-403">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="56085-404">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-404">Core</span></span>

* <span data-ttu-id="56085-405">일반 업데이트 명령에 `--set` 매개 변수에 대한 구문 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-405">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="56085-406">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-406">IoT</span></span>

* <span data-ttu-id="56085-407">`iot hub show`에서 "리소스를 찾을 수 없음" 오류가 잘못 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-407">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-408">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-408">Monitor</span></span>

* <span data-ttu-id="56085-409">CRUD에 대한 지원이 `monitor log-analytics workspace`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-409">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="56085-410">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-410">Network</span></span>

* <span data-ttu-id="56085-411">교차 테넌트 가상 연결에 대한 지원이 `network private-dns link vnet [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-411">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="56085-412">[주요 변경 사항]`--resource-group` 및 `--vnet-name` 매개 변수가 필수 매개 변수가 되도록 `network vnet subnet list`가 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-412">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="56085-413">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-413">SQL</span></span>

* <span data-ttu-id="56085-414">관리형 인스턴스에서 AAD 관리자 설정을 지원하는 명령이 `sql mi ad-admin`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-414">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="56085-415">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-415">Storage</span></span>

* <span data-ttu-id="56085-416">서비스에서 서비스로 복사하는 동안 액세스 계층을 유지하기 위해 `storage copy`에 `--preserve-s2s-access-tier` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-416">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="56085-417">스토리지 계정에 대한 대용량 파일 공유를 지원하기 위해 `storage account [create|update]`에 `--enable-large-file-share` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-417">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="56085-418">2019년 9월 24일</span><span class="sxs-lookup"><span data-stu-id="56085-418">September 24, 2019</span></span>

<span data-ttu-id="56085-419">버전 2.0.74</span><span class="sxs-lookup"><span data-stu-id="56085-419">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="56085-420">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-420">ACR</span></span>

* <span data-ttu-id="56085-421">`acr config retention update`에 필수 `--type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-421">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="56085-422">[주요 변경 사항] `--name -n` 매개 변수가 `acr config` 명령 그룹에 대한 `--registry -r `로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-422">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="56085-423">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-423">AKS</span></span>

* <span data-ttu-id="56085-424">`aks create` 명령에 `--load-balancer-sku` 매개 변수가 추가되어 SLB로 AKS 클러스터를 만들 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-424">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="56085-425">`aks [create|update]` 명령에 `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` 및 `--load-balancer-outbound-ip-prefixes` 매개 변수가 추가되어 SLB로 AKS 클러스터의 부하 분산 장치 프로필을 업데이트할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-425">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="56085-426">`aks create` 명령에 `--vm-set-type` 매개 변수가 추가되어 AKS 클러스터의 vm 유형을 지정할 수 있게 되었습니다(vmas 또는 vmss).</span><span class="sxs-lookup"><span data-stu-id="56085-426">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="56085-427">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-427">ARM</span></span>

* <span data-ttu-id="56085-428">json 템플릿에서 여러 줄과 주석을 지원할 수 있도록 `group deployment create` 명령에 `--handle-extended-json-format` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-428">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="56085-429">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-429">Compute</span></span>

* <span data-ttu-id="56085-430">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss [create|update]` 명령에 `--terminate-notification-time` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-430">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="56085-431">예약된 이벤트 종료 구성 기능을 지원하기 위해 `vmss update` 명령에 `--enable-terminate-notification` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-431">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="56085-432">`[vm|vmss] create` 명령에 `--priority,` `--eviction-policy,` `--max-billing` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-432">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="56085-433">디스크 업로드의 정확한 크기를 지정할 수 있도록 `disk create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-433">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="56085-434">관리 디스크의 증분 스냅샷에 대한 지원이 `snapshot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-434">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="56085-435">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="56085-435">Cosmos DB</span></span>

* <span data-ttu-id="56085-436">키, 읽기 전용 키 또는 연결 문자열을 표시하도록 `cosmosdb keys list` 명령에 `--type <key-type>` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-436">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="56085-437">`cosmosdb keys regenerate` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-437">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="56085-438">[사용 되지 않음]`cosmosdb list-connection-strings`, `cosmosdb regenerate-key` 및 `cosmosdb list-read-only-keys` 명령이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-438">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="56085-439">EventGrid</span><span class="sxs-lookup"><span data-stu-id="56085-439">EventGrid</span></span>

* <span data-ttu-id="56085-440">오른쪽 매개 변수를 참조하도록 엔드포인트 도움말 텍스트가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-440">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-441">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-441">Key Vault</span></span>

* <span data-ttu-id="56085-442">테넌트(`login -t`)로 로그인하면 `keyvault create`가 실패할 수 있는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-442">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-443">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-443">Monitor</span></span>

* <span data-ttu-id="56085-444">`--condition` 인수에서 `:` 문자가 허용되지 않아 `monitor metrics alert create` 할 수 없는 이슈가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-444">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="56085-445">정책</span><span class="sxs-lookup"><span data-stu-id="56085-445">Policy</span></span>

* <span data-ttu-id="56085-446">정책 API 버전 2019-06-01에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-446">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="56085-447">`policy assignment create` 명령에 `--enforcement-mode` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-447">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="56085-448">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-448">Storage</span></span>

* <span data-ttu-id="56085-449">`az storage copy` 명령에 `--blob-type` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-449">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="56085-450">2019년 9월 10일</span><span class="sxs-lookup"><span data-stu-id="56085-450">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="56085-451">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-451">ACR</span></span>

* <span data-ttu-id="56085-452">보존 정책을 구성하는 `acr config retention` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-452">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="56085-453">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-453">AKS</span></span>

* <span data-ttu-id="56085-454">다음 명령을 통해 ACR 통합 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-454">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="56085-455">AKS 클러스터에 ACR을 연결하는 `--attach-acr` 매개 변수가 `aks [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-455">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="56085-456">AKS 클러스터에서 ACR을 분리하는 `--detach-acr` 매개 변수가 `aks update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-456">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="56085-457">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-457">ARM</span></span>

* <span data-ttu-id="56085-458">2019-05-10 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-458">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="56085-459">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-459">Batch</span></span>

* <span data-ttu-id="56085-460">`batch pool create`에 대한 `--json-file`에 새 JSON 구성 설정이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-460">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="56085-461">파일 시스템을 탑재하기 위한 `MountConfigurations`가 추가됨(자세한 내용은 https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="56085-461">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="56085-462">`NetworkConfiguration`에 풀의 공용 IP에 대한 선택적 속성 `publicIPs`가 추가됨(자세한 내용은 https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body 참조)</span><span class="sxs-lookup"><span data-stu-id="56085-462">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="56085-463">공유 이미지 갤러리에 대한 지원이 `--image`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-463">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="56085-464">[주요 변경 사항]`batch pool create`의 기본값 `--start-task-wait-for-success`가 `true`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-464">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="56085-465">[주요 변경 사항]`AutoUserSpecification`의 `Scope` 기본값이 항상 풀이 되도록 변경됨(Windows 노드에서는 `Task`, Linux 노드에서는 `Pool`이었음)</span><span class="sxs-lookup"><span data-stu-id="56085-465">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="56085-466">이 인수는 `--json-file`을 사용하여 JSON 구성에서만 설정 가능</span><span class="sxs-lookup"><span data-stu-id="56085-466">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-467">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-467">HDInsight</span></span>

* <span data-ttu-id="56085-468">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-468">GA release</span></span>
* <span data-ttu-id="56085-469">[주요 변경 사항]`az hdinsight resize`의 `--workernode-count/-c` 매개 변수가 필수 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-469">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-470">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-470">Key Vault</span></span>

* <span data-ttu-id="56085-471">네트워크 규칙에서 서브넷을 삭제할 수 없는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="56085-471">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="56085-472">중복 서브넷 및 IP 주소를 네트워크 규칙에 추가할 수 있는 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="56085-472">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="56085-473">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-473">Network</span></span>

* <span data-ttu-id="56085-474">트래픽 분석 간격 값을 설정하는 `--interval` 매개 변수가 `network watcher flow-log`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-474">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="56085-475">게이트웨이 ID를 관리하는 `network application-gateway identity`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-475">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="56085-476">Key Vault ID 설정 지원이 `network application-gateway ssl-cert`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-476">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="56085-477">`network express-route peering peer-connection [show|list]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-477">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="56085-478">정책</span><span class="sxs-lookup"><span data-stu-id="56085-478">Policy</span></span>

* <span data-ttu-id="56085-479">2019-01-01 API 버전을 사용하도록 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-479">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="56085-480">2019년 8월 27일</span><span class="sxs-lookup"><span data-stu-id="56085-480">August 27, 2019</span></span>

<span data-ttu-id="56085-481">버전 2.0.72</span><span class="sxs-lookup"><span data-stu-id="56085-481">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="56085-482">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-482">ACR</span></span>

* <span data-ttu-id="56085-483">[주요 변경 사항]`classic` SKU 지원이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-483">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="56085-484">API Management</span><span class="sxs-lookup"><span data-stu-id="56085-484">API Management</span></span>

* <span data-ttu-id="56085-485">[미리 보기] `apim` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-485">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-486">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-486">AppService</span></span>

* <span data-ttu-id="56085-487">슬롯 지정 시의 `webapp webjob continuous start` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-487">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="56085-488">`env` 폴더를 검색하고 배포에 사용된 파일에서 제거하도록 `webapp up`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-488">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-489">Keyvault</span><span class="sxs-lookup"><span data-stu-id="56085-489">Keyvault</span></span>

* <span data-ttu-id="56085-490">`--expires` 인수를 무시한 `keyvault secret set`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-490">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="56085-491">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-491">Network</span></span>

* <span data-ttu-id="56085-492">`--private-ip-address-version` 인수에 IPv6 주소 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-492">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="56085-493">프라이빗 엔드포인트를 관리하기 위한 새 `network private-endpoint [create|update|list-types]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-493">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="56085-494">`network private-link-service` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-494">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="56085-495">`--private-endpoint-network-policies` 및 `--private-link-service-network-policies` 인수를 `network vnet subnet update`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-495">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-496">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-496">RBAC</span></span>

* <span data-ttu-id="56085-497">홈페이지가 업데이트되지 않는 `ad app update --homepage` 명령 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-497">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="56085-498">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="56085-498">ServiceFabric</span></span>

* <span data-ttu-id="56085-499">대/소문자가 혼합된 Key Vault 이름 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-499">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="56085-500">Key Vault에서 인증서를 사용할 때 발생하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-500">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="56085-501">PFX 인증서 파일의 사용 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-501">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="56085-502">Key Vault 리소스 그룹이 지정되지 않은 `sf cluster certificate add` 관련 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-502">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="56085-503">`sf cluster set`가 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-503">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="56085-504">SignalR</span><span class="sxs-lookup"><span data-stu-id="56085-504">SignalR</span></span>

* <span data-ttu-id="56085-505">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="56085-505">Added new commands:</span></span>
  * <span data-ttu-id="56085-506">`signalr cors`: SignalR CORS 관리</span><span class="sxs-lookup"><span data-stu-id="56085-506">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="56085-507">`signalr restart`: SignalR Service 다시 시작</span><span class="sxs-lookup"><span data-stu-id="56085-507">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="56085-508">`signalr update`: SignalR Service 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-508">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="56085-509">`--service-mode` 인수를 `signalr create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-509">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-510">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-510">Storage</span></span>

* <span data-ttu-id="56085-511">`storage account revoke-delegation-keys` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-511">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="56085-512">2019년 8월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-512">August 13, 2019</span></span>

<span data-ttu-id="56085-513">버전 2.0.71</span><span class="sxs-lookup"><span data-stu-id="56085-513">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-514">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-514">AppService</span></span>

* <span data-ttu-id="56085-515">슬롯에 대해 `webapp webjob continuous` 명령이 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-515">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-516">BotService</span><span class="sxs-lookup"><span data-stu-id="56085-516">BotService</span></span>

* <span data-ttu-id="56085-517">[주요 변경 사항] v3 SDK 봇 만들기에 대한 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-517">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="56085-518">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="56085-518">CognitiveServices</span></span>

* <span data-ttu-id="56085-519">`cognitiveservices account network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-519">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="56085-520">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="56085-520">Cosmos DB</span></span>

* <span data-ttu-id="56085-521">여러 쓰기 위치 업데이트 시의 경고가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-521">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="56085-522">CosmosDB SQL, MongoDB, Cassandra, Gremlin 및 Table 리소스 및 리소스 처리량에 대한 CRUD 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-522">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-523">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-523">HDInsight</span></span>

<span data-ttu-id="56085-524">이 릴리스에는 호환성이 손상되는 변경이 많이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-524">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="56085-525">[주요 변경 사항]`hdinsight create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-525">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="56085-526">`--storage-default-container`에서 `--storage-container`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-526">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="56085-527">`--storage-default-filesystem`에서 `--storage-filesystem`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-527">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="56085-528">[주요 변경 사항]`application create`의 `--name` 인수에서 클러스터 이름 대신 애플리케이션 이름을 나타내도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-528">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="56085-529">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 `application create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-529">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="56085-530">[주요 변경 사항]`application create`에 대한 매개 변수의 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-530">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="56085-531">`--application-type`에서 `--type`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-531">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="56085-532">`--marketplace-identifier`에서 `--marketplace-id`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-532">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="56085-533">`--https-endpoint-access-mode`에서 `--access-mode`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-533">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="56085-534">이름이 `--https-endpoint-destination-port`에서 `--destination-port`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-534">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="56085-535">[주요 변경 사항]`application create`에 대한 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-535">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="56085-536">[호환성이 손상되는 변경] `hdinsight resize`에 대한 이름이 `--target-instance-count`에서 `--workernode-count`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-536">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="56085-537">[주요 변경 사항]`hdinsight script-action` 그룹의 모든 명령에서 `--name` 매개 변수를 스크립트 작업 이름으로 사용하도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="56085-537">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="56085-538">이전 `--name` 기능을 대체하기 위해 `--cluster-name` 인수가 모든 `hdinsight script-action` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-538">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="56085-539">[주요 변경 사항] 모든 `hdinsight script-action` 명령에 대한 이름이 `--script-execution-id`에서 `--execution-id`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-539">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="56085-540">[주요 변경 사항]`hdinsight script-action show`에서 `hdinsight script-action show-execution-details`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-540">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="56085-541">[호환성이 손상되는 변경] `hdinsight script-action execute --roles`의 매개 변수에서 쉼표로 구분하는 대신 공백으로 구분하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-541">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="56085-542">[주요 변경 사항]`hdinsight script-action list`의 `--persisted` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-542">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="56085-543">`hdinsight create --cluster-configurations` 매개 변수에서 로컬 JSON 파일 또는 JSON 문자열에 대한 경로를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-543">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="56085-544">명령 `hdinsight script-action list-execution-history` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-544">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="56085-545">`hdinsight monitor enable --workspace`에서 Log Analytics 작업 영역 ID 또는 작업 영역 이름을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-545">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="56085-546">작업 영역 ID가 매개 변수로 제공되는 경우 필요한 `hdinsight monitor enable --primary-key` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-546">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="56085-547">도움말 메시지에 대한 추가 예제 및 업데이트된 설명이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-547">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-548">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-548">Interactive</span></span>

* <span data-ttu-id="56085-549">로드 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-549">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="56085-550">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="56085-550">Kubernetes</span></span>

* <span data-ttu-id="56085-551">대시보드 컨테이너 포트에서 `https`를 사용하는 경우 `https`를 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-551">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="56085-552">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-552">Network</span></span>

* <span data-ttu-id="56085-553">`--yes` 인수가 `network dns record-set cname delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-553">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-554">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-554">Profile</span></span>

* <span data-ttu-id="56085-555">리소스 액세스 토큰을 가져오기 위해 `--resource-type` 인수가 `account get-access-token`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-555">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="56085-556">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="56085-556">ServiceFabric</span></span>

* <span data-ttu-id="56085-557">sf 클러스터를 만드는 데 지원되는 모든 os 버전이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-557">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="56085-558">기본 인증서 유효성 검사 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-558">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="56085-559">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-559">Storage</span></span>

* <span data-ttu-id="56085-560">명령 `storage copy` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-560">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="56085-561">2019년 7월 30일</span><span class="sxs-lookup"><span data-stu-id="56085-561">July 30, 2019</span></span>

<span data-ttu-id="56085-562">버전 2.0.70</span><span class="sxs-lookup"><span data-stu-id="56085-562">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="56085-563">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-563">ACR</span></span>

* <span data-ttu-id="56085-564">#9952 문제(`acr pack build` 명령의 회귀)가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-564">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="56085-565">`acr pack build`의 기본 작성기 이미지 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-565">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-566">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-566">Appservice</span></span>

* <span data-ttu-id="56085-567">리소스를 찾을 수 없는 경우 메시지를 표시 하도록 `webapp config ssl`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-567">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="56085-568">`functionapp create`에서 `Standard_RAGRS` 스토리지 계정 유형을 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-568">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="56085-569">이전 버전의 python을 사용하여 실행할 경우 `webapp up`이(가) 실패하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-569">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="56085-570">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-570">Network</span></span>

* <span data-ttu-id="56085-571">`network nic ip-config add`에서 잘못된 매개 변수 `--ids` 제거됨(#9861 수정)</span><span class="sxs-lookup"><span data-stu-id="56085-571">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="56085-572">#9604 수정.</span><span class="sxs-lookup"><span data-stu-id="56085-572">Fixes #9604.</span></span> <span data-ttu-id="56085-573">사용자가 신뢰할 수 있는 루트 인증서를 연결할 수 있도록 `network application-gateway http-settings [create|update]`에 `--root-certs` 매개 변수를 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-573">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="56085-574">`network dns record-set ns create`(#9965)에 대해 인수 `--subscription`을 수정</span><span class="sxs-lookup"><span data-stu-id="56085-574">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-575">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-575">RBAC</span></span>

* <span data-ttu-id="56085-576">`user update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-576">Added `user update` command</span></span>
* <span data-ttu-id="56085-577">[사용 되지 않음] 사용자 관련 명령 중 `--upn-or-object-id`가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-577">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="56085-578">대체 인수 `--id` 사용</span><span class="sxs-lookup"><span data-stu-id="56085-578">Use replacement argument `--id`</span></span>
* <span data-ttu-id="56085-579">사용자 관련 명령에 `--id` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-579">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="56085-580">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-580">SQL</span></span>

* <span data-ttu-id="56085-581">관리형 인스턴스 키 및 TDE 보호기에 대한 관리 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-581">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="56085-582">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-582">Storage</span></span>

* <span data-ttu-id="56085-583">`storage remove` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-583">Added `storage remove` command</span></span>
* <span data-ttu-id="56085-584">`storage blob update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-584">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-585">VM</span><span class="sxs-lookup"><span data-stu-id="56085-585">VM</span></span>

* <span data-ttu-id="56085-586">새로운 API 버전을 사용하여 영역 세부 정보를 출력하도록 `list-skus`를 변경</span><span class="sxs-lookup"><span data-stu-id="56085-586">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="56085-587">`vmss create`에 대한 `--single-placement-group`의 기본값을 `false`로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-587">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="56085-588">`[snapshot|disk] create`에 대한 ZRS 스토리지 SKU를 선택하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-588">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="56085-589">전용 호스트를 지원하는 새로운 명령 그룹 `vm host`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-589">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="56085-590">VM 전용 호스트를 설정하기 위해 `vm create`에 매개 변수 `--host` 및 `--host-group` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-590">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="56085-591">2019년 7월 16일</span><span class="sxs-lookup"><span data-stu-id="56085-591">July 16, 2019</span></span>

<span data-ttu-id="56085-592">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="56085-592">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-593">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-593">Appservice</span></span>

* <span data-ttu-id="56085-594">ResourceGroupName 또는 애플리케이션 이름이 유효하지 않은 경우 올바른 오류 메시지를 반환하도록 `webapp identity` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-594">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="56085-595">ResourceGroup이 제공되지 않은 경우 numberOfSites에 대한 올바른 값을 반환하도록 `webapp list` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-595">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="56085-596">`appservice plan create` 및 `webapp create`의 부작용 수정</span><span class="sxs-lookup"><span data-stu-id="56085-596">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="56085-597">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-597">Core</span></span>

* <span data-ttu-id="56085-598">적용할 수 없음에도 불구하고 `--subscription`이 나타나는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-598">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="56085-599">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-599">Batch</span></span>

* <span data-ttu-id="56085-600">[주요 변경 사항]`batch pool node-agent-skus list`를 `batch pool supported-images list`로 대체</span><span class="sxs-lookup"><span data-stu-id="56085-600">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="56085-601">`batch pool create network`의 `--json-file` 옵션을 사용할 때 트래픽의 소스 포트를 기반으로 풀에 대한 네트워크 액세스를 차단하는 보안 규칙에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-601">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="56085-602">`batch task create`의 `--json-file` 옵션을 사용할 때 컨테이너 작업 디렉터리 또는 일괄 처리 작업 디렉터리에서 작업을 실행하도록 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-602">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="56085-603">`batch pool create`의 `--application-package-references` 옵션에서 기본값으로만 작동하는 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-603">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="56085-604">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="56085-604">Eventhubs</span></span>

* <span data-ttu-id="56085-605">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-605">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-606">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-606">RDBMS</span></span>

* <span data-ttu-id="56085-607">복제본 명령을 만들기 위해 복제본 SKU를 지정하는 선택적 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-607">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="56085-608">MySQL 복제본 생성 시 CI 테스트 실패 문제 수정</span><span class="sxs-lookup"><span data-stu-id="56085-608">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="56085-609">릴레이</span><span class="sxs-lookup"><span data-stu-id="56085-609">Relay</span></span>

* <span data-ttu-id="56085-610">클라이언트 인증이 비활성화[#8775](https://github.com/azure/azure-cli/issues/8775)된 경우의 하이브리드 연결 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-610">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="56085-611">`--requires-transport-security` 매개 변수가 `relay wcfrelay create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-611">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="56085-612">Servicebus</span><span class="sxs-lookup"><span data-stu-id="56085-612">Servicebus</span></span>

* <span data-ttu-id="56085-613">`authorizationrule` 명령의 `--rights` 매개 변수에 대한 유효성 검사를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-613">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="56085-614">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-614">Storage</span></span>

* <span data-ttu-id="56085-615">스토리지 계정 업데이트를 위해 파일 AADDS 사용 설정</span><span class="sxs-lookup"><span data-stu-id="56085-615">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="56085-616">문제 `storage blob service-properties update --set` 해결</span><span class="sxs-lookup"><span data-stu-id="56085-616">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="56085-617">2019년 7월 2일</span><span class="sxs-lookup"><span data-stu-id="56085-617">July 2, 2019</span></span>

<span data-ttu-id="56085-618">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="56085-618">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="56085-619">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-619">Core</span></span>

* <span data-ttu-id="56085-620">명령 모듈은 이제 단일 Python 배포 패키지로 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-620">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="56085-621">따라서 PyPI의 많은 `azure-cli-` 패키지를 직접 사용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-621">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="56085-622">이를 통해 설치 크기를 줄이고 `pip`를 통해 직접 설치한 사용자에게만 영향을 주게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-622">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="56085-623">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-623">ACR</span></span>

* <span data-ttu-id="56085-624">작업에 타이머 트리거에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-624">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-625">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-625">Appservice</span></span>

* <span data-ttu-id="56085-626">기본값으로 애플리케이션 인사이트를 사용하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-626">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="56085-627">[주요 변경 사항] 사용되지 않는 `functionapp devops-build` 제거</span><span class="sxs-lookup"><span data-stu-id="56085-627">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="56085-628">대신 새 명령 `az functionapp devops-pipeline` 사용</span><span class="sxs-lookup"><span data-stu-id="56085-628">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="56085-629">`functionapp deployment config-zip`에 Linux 사용 함수 앱 계획 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-629">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="56085-630">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="56085-630">Cosmos DB</span></span>

* <span data-ttu-id="56085-631">TTL을 사용하지 않도록 설정하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-631">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="56085-632">DLS</span><span class="sxs-lookup"><span data-stu-id="56085-632">DLS</span></span>

* <span data-ttu-id="56085-633">업데이트된 ADLS 버전(0.0.45)</span><span class="sxs-lookup"><span data-stu-id="56085-633">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="56085-634">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="56085-634">Feedback</span></span>

* <span data-ttu-id="56085-635">실패한 확장 명령을 보고할 때, `az feedback`은 이제 브라우저에서 인덱스 확장의 프로젝트/리포지토리 URL을 열려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-635">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-636">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-636">HDInsight</span></span>

* <span data-ttu-id="56085-637">[주요 변경 사항]`oms` 명령 그룹 이름을 `monitor`로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-637">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="56085-638">[주요 변경 사항] 필수 매개 변수로 `--http-password/-p` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-638">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="56085-639">`--cluster-admin-account` 및 `cluster-users-group-dns` 매개 변수 완성자에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="56085-639">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="56085-640">`—esp`가 있을 때 `cluster-users-group-dns` 매개 변수가 필수가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-640">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="56085-641">모든 기존 인수 자동-완성자에 대한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="56085-641">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="56085-642">리소스 이름을 리소스 ID로 변환하기 위한 시간 제한 추가</span><span class="sxs-lookup"><span data-stu-id="56085-642">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="56085-643">자동 완성자를 모든 리소스 그룹에서 리소스를 선택하도록 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-643">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="56085-644">`-g`로 지정한 리소스 그룹과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-644">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="56085-645">`hdinsight application create` 명령에서 `--sub-domain-suffix` 및 `--disable_gateway_auth` 매개 변수에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-645">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="56085-646">관리 서비스</span><span class="sxs-lookup"><span data-stu-id="56085-646">Managed Services</span></span>

* <span data-ttu-id="56085-647">미리 보기 관리 서비스 명령 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="56085-647">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="56085-648">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-648">Profile</span></span>
* <span data-ttu-id="56085-649">로그 아웃 명령에 대한 `--subscription` 인수 표시하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-649">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-650">RBAC</span></span>

* <span data-ttu-id="56085-651">[주요 변경 사항]`create-for-rbac`에 대한 `--password` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-651">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="56085-652">AAD 그래프 서버 복제 대기 시간으로 인한 일시적인 실패를 피하기 위해 `create` 명령에 `--assignee-principal-type` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-652">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="56085-653">소유 개체를 나열할 때 `ad signed-in-user`에서의 충돌 수정</span><span class="sxs-lookup"><span data-stu-id="56085-653">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="56085-654">`ad sp`가 서비스 주체로부터 올바른 애플리케이션을 찾지 못하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-654">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-655">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-655">RDBMS</span></span>

* <span data-ttu-id="56085-656">MariaDB에 대한 복제 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-656">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="56085-657">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-657">SQL</span></span>

* <span data-ttu-id="56085-658">`sql db create --sample-name`에 허용되는 값이 문서화됨</span><span class="sxs-lookup"><span data-stu-id="56085-658">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-659">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-659">Storage</span></span>

* <span data-ttu-id="56085-660">`--as-user`를 사용하여 `storage blob generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="56085-660">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="56085-661">`--as-user`를 사용하여 `storage container generate-sas`에 사용자 위임 SAS 토큰 지원을 추가함</span><span class="sxs-lookup"><span data-stu-id="56085-661">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="56085-662">VM</span><span class="sxs-lookup"><span data-stu-id="56085-662">VM</span></span>

* <span data-ttu-id="56085-663">`vmss create`가 `--no-wait`와 실행될 때 오류 메시지를 반환하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-663">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="56085-664">`vmss create --single-placement-group`에 대한 클라이언트 측 유효성 검사 제거</span><span class="sxs-lookup"><span data-stu-id="56085-664">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="56085-665">`--single-placement-group`이 `true`로 설정되고 `--instance-count`이 100보다 크거나 가용성 영역이 지정되면 실패하지 않지만, 이 유효성 검사는 컴퓨팅 서비스에 남겨 둡니다.</span><span class="sxs-lookup"><span data-stu-id="56085-665">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="56085-666">`[vm|vmss] extension image list`가 `--latest`와 함께 사용하면 실패하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-666">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="56085-667">2019년 6월 18일</span><span class="sxs-lookup"><span data-stu-id="56085-667">June 18, 2019</span></span>

<span data-ttu-id="56085-668">2\.0.67 버전</span><span class="sxs-lookup"><span data-stu-id="56085-668">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="56085-669">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-669">Core</span></span>

<span data-ttu-id="56085-670">이 릴리스에서는 명령 그룹, 명령 또는 인수가 미리 보기 상태에 있을 때 고객에게 보다 명확하게 알릴 수 있는 새로운 [미리 보기] 태그가 도입되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-670">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="56085-671">이것은 이전에 도움말 텍스트에서 호출되었거나 명령 모듈 버전 번호에 의해 암시적으로 전달되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-671">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="56085-672">CLI는 앞으로 개별 패키지의 버전 번호를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-672">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="56085-673">명령이 미리 보기 상태이면 해당 인수도 모두 같습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-673">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="56085-674">명령 그룹이 미리 보기로 레이블링된 경우 모든 명령과 인수도 미리 보기로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-674">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="56085-675">이 변경으로 인해 여러 명령 그룹이 "갑자기" 이 릴리스의 미리 보기 상태에 있는 것처럼 보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-675">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="56085-676">실제로는 대부분의 패키지가 미리 보기 상태였지만 이 릴리스에서는 GA로 간주됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-676">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="56085-677">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-677">ACR</span></span>
* <span data-ttu-id="56085-678">'acr check-health' 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-678">Added 'acr check-health' command</span></span>
* <span data-ttu-id="56085-679">AAD 토큰 및 외부 명령 검색의 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="56085-679">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="56085-680">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-680">ACS</span></span>
* <span data-ttu-id="56085-681">사용되지 않는 ACS 명령이 도움말 보기에서 숨겨짐</span><span class="sxs-lookup"><span data-stu-id="56085-681">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="56085-682">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-682">AMS</span></span>
* <span data-ttu-id="56085-683">[주요 변경 사항] archive-window-length 및 key-frame-interval-duration에 대한 ISO 8601 시간 문자열을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-683">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-684">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-684">AppService</span></span>
* <span data-ttu-id="56085-685">`webapp deleted list` 및 `webapp deleted restore`에 대한 위치 기반 라우팅을 추가</span><span class="sxs-lookup"><span data-stu-id="56085-685">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="56085-686">Azure Cloud Shell에서 웹앱의 업로깅된 대상 URL("...에서 앱을 시작할 수 있습니다")을 클릭할 수 없는 이슈가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-686">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="56085-687">AlwaysOn 오류로 일부 SKU가 포함된 앱을 만들지 못하는 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-687">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="56085-688">추가 사전 유효성 검사를 `[appservice|webapp] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-688">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="56085-689">올바른 actionHostName을 사용하도록 `[webapp|functionapp] traffic-routing` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-689">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="56085-690">`functionapp` 명령에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-690">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="56085-691">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-691">Batch</span></span>
* <span data-ttu-id="56085-692">공유 키 인증에 대한 과도한 오류 보고로 인해 AAD 인증 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-692">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-693">BatchAI</span><span class="sxs-lookup"><span data-stu-id="56085-693">BatchAI</span></span>
* <span data-ttu-id="56085-694">BatchAI 명령은 이제 사용되지 않고 숨겨집니다</span><span class="sxs-lookup"><span data-stu-id="56085-694">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-695">BotService</span><span class="sxs-lookup"><span data-stu-id="56085-695">BotService</span></span>
* <span data-ttu-id="56085-696">v3 SDK를 지원하는 명령에 대한 "지원 중단"/ "유지 관리 모드" 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="56085-696">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-697">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-697">CosmosDB</span></span>
* <span data-ttu-id="56085-698">[사용 되지 않음]`cosmosdb list-keys` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-698">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="56085-699">`cosmosdb keys list` 명령이 추가됨 - `cosmosdb list-keys` 명령을 대체</span><span class="sxs-lookup"><span data-stu-id="56085-699">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="56085-700">`cosmsodb create/update`: "isZoneRedundant"속성을 설정할 수 있도록 --location에 대한 새로운 형식이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-700">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="56085-701">이전 형식은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-701">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="56085-702">EventGrid</span><span class="sxs-lookup"><span data-stu-id="56085-702">EventGrid</span></span>
* <span data-ttu-id="56085-703">도메인 CRUD 작업에 `eventgrid domain` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-703">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="56085-704">도메인 토픽 CRUD 작업에 `eventgrid domain topic` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-704">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="56085-705">OData 구문을 사용하여 결과를 필터링하기 위해 `eventgrid [topic|event-subscription] list`에 `--odata-query` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-705">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="56085-706">`event-subscription create/update`: `--endpoint-type` 매개 변수의 새 값으로 servicebusqueue 추가</span><span class="sxs-lookup"><span data-stu-id="56085-706">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="56085-707">[주요 변경 사항]`eventgrid event-subscription [create|update]`를 사용하여 `--included-event-types All`에 대한 지원 제거</span><span class="sxs-lookup"><span data-stu-id="56085-707">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-708">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-708">HDInsight</span></span>
* <span data-ttu-id="56085-709">`hdinsight create` 명령에서 `--ssh-public-key` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-709">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="56085-710">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-710">IoT</span></span>
* <span data-ttu-id="56085-711">권한 부여 정책 키를 다시 생성하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-711">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="56085-712">DigitalTwin Repository Provisioning Service에 대한 SDK 및 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-712">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="56085-713">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-713">Network</span></span>
* <span data-ttu-id="56085-714">Nat 게이트웨이에 대한 영역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-714">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="56085-715">명령 `network list-service-tags` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-715">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="56085-716">사용자가 와일드카드 A 레코드를 가져올 수 없는 `dns zone import` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-716">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="56085-717">특정 영역에서 흐름 로깅을 활성화할 수 없는 `watcher flow-log configure` 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-717">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="56085-718">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-718">Resource</span></span>
* <span data-ttu-id="56085-719">REST 호출 마킹을 위한 `az rest` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-719">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="56085-720">리소스 그룹 또는 구독 수준 `--scope`에 `policy assignment list`를 사용할 때의 오류 수정</span><span class="sxs-lookup"><span data-stu-id="56085-720">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="56085-721">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="56085-721">ServiceBus</span></span>
* <span data-ttu-id="56085-722">`servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319) 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-722">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="56085-723">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-723">SQL</span></span>
* <span data-ttu-id="56085-724">`sql [server|mi] create`에 대해 `--location`을 선택 사항으로 변경했습니다 - 지정되지 않은 경우 리소스 그룹 위치를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-724">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="56085-725">`sql db list-editions --available`에 대해 “’NoneType’ 객체 반복 불가” 오류를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-725">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="56085-726">SQLVm</span><span class="sxs-lookup"><span data-stu-id="56085-726">SQLVm</span></span>
* <span data-ttu-id="56085-727">[호환성이 손상되는 변경] `--license-type` 매개 변수가 필수 매개 변수가 되도록 `sql vm create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-727">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="56085-728">sql vm을 만들거나 업데이트하는 경우 SQL 이미지 SKU 설정을 허용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-728">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="56085-729">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-729">Storage</span></span>
* <span data-ttu-id="56085-730">`storage container generate-sas`에 대한 계정 키 누락 이슈가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-730">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="56085-731">Linux에서 `storage blob sync` 이슈 해결</span><span class="sxs-lookup"><span data-stu-id="56085-731">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="56085-732">VM</span><span class="sxs-lookup"><span data-stu-id="56085-732">VM</span></span>
* <span data-ttu-id="56085-733">[미리 보기] VM 이미지 작성을 위해 `vm image template` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-733">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="56085-734">2019년 6월 4일</span><span class="sxs-lookup"><span data-stu-id="56085-734">June 4, 2019</span></span>

<span data-ttu-id="56085-735">버전 2.0.66</span><span class="sxs-lookup"><span data-stu-id="56085-735">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="56085-736">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-736">Core</span></span>
* <span data-ttu-id="56085-737">`--output yaml`을 `--query`와 함께 사용하는 경우 명령이 실패하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-737">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="56085-738">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-738">ACR</span></span>
* <span data-ttu-id="56085-739">빌드 팩을 사용하여 빠른 빌드 작업을 만드는 'acr pack' 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-739">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="56085-740">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-740">ACS</span></span>
* <span data-ttu-id="56085-741">AKS kube-dashboard 추가 기능에 대한 사용/사용 안 함 설정이 허용됨</span><span class="sxs-lookup"><span data-stu-id="56085-741">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="56085-742">구독이 Azure Red Hat OpenShift를 사용하기 위한 허용 목록에 없는 경우 친숙한 메시지가 출력됨</span><span class="sxs-lookup"><span data-stu-id="56085-742">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="56085-743">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-743">Batch</span></span>
* <span data-ttu-id="56085-744">계정에 로그인되지 않는 \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\] 오류에 대한 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-744">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="56085-745">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-745">IoT</span></span>
* <span data-ttu-id="56085-746">수동 장애 조치 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-746">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="56085-747">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-747">Network</span></span>
* <span data-ttu-id="56085-748">사용자 지정 WAF 규칙을 지원하는 `network application-gateway waf-policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-748">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="56085-749">`--waf-policy` 및 `--max-capacity` 인수를 `network application-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-749">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="56085-750">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-750">Resource</span></span>
* <span data-ttu-id="56085-751">사용 가능한 TTY가 없을 때 `deployment create`에서 나타나는 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-751">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="56085-752">역할</span><span class="sxs-lookup"><span data-stu-id="56085-752">Role</span></span>
* <span data-ttu-id="56085-753">도움말 텍스트가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-753">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="56085-754">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-754">Compute</span></span>
* <span data-ttu-id="56085-755">0에서 시작하지 않거나 숫자를 건너뛰는 데이터 디스크 LUN이 있는 관리형 이미지의 VM에 대한 `vm create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-755">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="56085-756">2019년 5월 21일</span><span class="sxs-lookup"><span data-stu-id="56085-756">May 21, 2019</span></span>

<span data-ttu-id="56085-757">버전 2.0.65</span><span class="sxs-lookup"><span data-stu-id="56085-757">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="56085-758">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-758">Core</span></span>
* <span data-ttu-id="56085-759">인증 오류에 대한 더 나은 피드백이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-759">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="56085-760">CLI가 코어 버전과 호환되지 않는 확장을 로드하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-760">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="56085-761">`clouds.config`가 손상된 경우 시작과 관련된 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-761">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="56085-762">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-762">ACR</span></span>
* <span data-ttu-id="56085-763">Tasks에 관리 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-763">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="56085-764">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-764">ACS</span></span>
* <span data-ttu-id="56085-765">고객 AAD 클라이언트에서 사용되는 `openshift create` 명령의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-765">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-766">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-766">AppService</span></span>
* <span data-ttu-id="56085-767">[사용 되지 않음]`functionapp devops-build` 명령이 사용되지 않음 - 다음 릴리스에서 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-767">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="56085-768">`functionapp devops-pipeline`에서 Azure DevOps의 빌드 로그를 자세한 정보 표시 모드로 가져오도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-768">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="56085-769">[주요 변경 사항]`functionapp devops-pipeline` 명령에서 `--use_local_settings` 플래그가 제거됨 - 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-769">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="56085-770">`--logs`를 사용하지 않으면 `webapp up`에서 JSON 출력을 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-770">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="56085-771">`webapp up`에 대한 로컬 구성에 기본 리소스를 작성할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-771">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="56085-772">`webapp up`에서 `--location` 인수를 사용하지 않고 앱을 다시 배포할 수 있도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-772">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="56085-773">Linux SKU ASP 평가판을 만들 때 작동하지 않는 SKU 값을 Free로 사용하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-773">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-774">BotService</span><span class="sxs-lookup"><span data-stu-id="56085-774">BotService</span></span>
* <span data-ttu-id="56085-775">명령에 대한 `--lang` 매개 변수에서 모든 대/소문자 구분을 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-775">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="56085-776">명령 모듈에 대한 설명이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-776">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-777">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-777">Consumption</span></span>
* <span data-ttu-id="56085-778">`consumption usage list --billing-period-name`을 실행할 때 누락된 필수 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-778">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="56085-779">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-779">IoT</span></span>
* <span data-ttu-id="56085-780">모든 키를 나열하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-780">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="56085-781">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-781">Network</span></span>
* [주요 변경 사항]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="56085-783">NAT 게이트웨이에 연결하기 위해 `network vnet subnet [create|update]`에 `--nat-gateway` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-783">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="56085-784">레코드 이름이 레코드 유형과 일치하지 않는 `dns zone import` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-784">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-785">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-785">RDBMS</span></span>
* <span data-ttu-id="56085-786">지역 복제에 postgres 및 mysql이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-786">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-787">RBAC</span><span class="sxs-lookup"><span data-stu-id="56085-787">RBAC</span></span>
* <span data-ttu-id="56085-788">`role assignment`에 관리 그룹 범위 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-788">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-789">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-789">Storage</span></span>
* <span data-ttu-id="56085-790">`storage blob sync`: 스토리지 Blob에 대한 sync 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-790">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="56085-791">컴퓨팅</span><span class="sxs-lookup"><span data-stu-id="56085-791">Compute</span></span>
* <span data-ttu-id="56085-792">VM의 컴퓨터 이름을 설정하기 위해 `--computer-name`이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-792">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="56085-793">`[vm|vmss] create`에 대한 `--ssh-key-value` 이름이 `--ssh-key-values`로 변경됨 - 이제 여러 개의 ssh 공개 키 값 또는 경로를 허용할 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-793">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="56085-794">__참고__: 호환성이 손상되는 변경이 **아님** - `--ssh-key-value`가 `--ssh-key-values`와만 일치하므로 올바르게 구문 분석됨</span><span class="sxs-lookup"><span data-stu-id="56085-794">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="56085-795">`ppg create`의 `--type` 인수가 선택적 항목으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-795">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="56085-796">2019년 5월 6일</span><span class="sxs-lookup"><span data-stu-id="56085-796">May 6, 2019</span></span>

<span data-ttu-id="56085-797">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="56085-797">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="56085-798">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-798">ACS</span></span>
* <span data-ttu-id="56085-799">[주요 변경 사항]`openshift` 명령에서 `--fqdn` 플래그가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-799">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="56085-800">Azure Red Hat Openshift GA API 버전을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-800">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="56085-801">`customer-admin-group-id` 플래그가 `openshift create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-801">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="56085-802">[GA] `aks create` 옵션인 `--network-policy`에서 `(PREVIEW)`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-802">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-803">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-803">Appservice</span></span>
* <span data-ttu-id="56085-804">[사용 되지 않음]`functionapp devops-build` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-804">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="56085-805">`functionapp devops-pipeline`으로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-805">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="56085-806">`webapp up` 실패를 야기하는 cloudshell의 올바른 사용자 이름을 가져오는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-806">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="56085-807">지원되는 appserviceplans를 반영하도록 업데이트된 `appservice plan --sku` 설명서가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-807">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="56085-808">리소스 그룹 및 계획을 위한 선택적 인수가 `webapp up`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-808">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="56085-809">`webapp ssh`에 환경 변수 `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-809">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="56085-810">Linux Free SKU에 대한 `appserviceplan create` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-810">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="56085-811">Kudu 콜드 스타트 처리를 위해 `SCM_DO_BUILD_DURING_DEPLOYMENT=true`를 설정한 후 `webapp up`이 30초 동안 일시 중지하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-811">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="56085-812">Windows에서 `powershell` 런타임에 대한 지원이 `functionapp create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-812">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="56085-813">`create-remote-connection` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-813">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="56085-814">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-814">Batch</span></span>
* <span data-ttu-id="56085-815">`--application-package-references` 옵션에 대한 유효성 검사기의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-815">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-816">Botservice</span><span class="sxs-lookup"><span data-stu-id="56085-816">Botservice</span></span>
* <span data-ttu-id="56085-817">[주요 변경 사항]`bot create -v v4 -k webapp`에서 기본적으로 빈 Web App 봇을 만들도록 변경됨(즉, 봇이 App Service에 배포되지 않음)</span><span class="sxs-lookup"><span data-stu-id="56085-817">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="56085-818">`-v v4`에서 이전 동작을 사용하도록 `--echo` 플래그가 `bot create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-818">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="56085-819">[주요 변경 사항]`--version`의 기본값이 `v4`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-819">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="56085-820">__참고:__ `bot prepare-publish`는 이전의 기본값을 계속 사용함</span><span class="sxs-lookup"><span data-stu-id="56085-820">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="56085-821">[주요 변경 사항]`--lang`에서 `Csharp`이 더 이상 기본값으로 설정되지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-821">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="56085-822">명령에 `--lang`이 필요하지만 제공되지 않으면 이제 명령에서 오류가 발생함</span><span class="sxs-lookup"><span data-stu-id="56085-822">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="56085-823">[주요 변경 사항]`bot create`에서 `--appid` 및 `--password` 인수가 필수 항목이 되도록 변경되었으며 이제 `ad app create`를 통해 만들어질 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-823">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="56085-824">`--appid` 및 `--password` 유효성 검사가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-824">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="56085-825">[주요 변경 사항]`bot create -v v4`에서 Storage 계정 또는 Application Insights를 만들거나 사용하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-825">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="56085-826">[주요 변경 사항]`bot create -v v3`에서 Application Insights를 사용할 수 있는 지역을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-826">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="56085-827">[주요 변경 사항]`bot update`에서 이제 봇의 특정 속성에만 영향을 주도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-827">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="56085-828">[주요 변경 사항]`--lang` 플래그에서 `Node` 대신 `Javascript`를 허용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-828">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="56085-829">[주요 변경 사항]`Node`가 허용되는 `--lang` 값으로 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-829">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="56085-830">[주요 변경 사항]`bot create -v v4 -k webapp`에서 `SCM_DO_BUILD_DURING_DEPLOYMENT`가 더 이상 true로 설정되지 않도록 변경됨.</span><span class="sxs-lookup"><span data-stu-id="56085-830">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="56085-831">Kudu를 통한 모든 배포가 해당 기본 동작에 따라 작동함</span><span class="sxs-lookup"><span data-stu-id="56085-831">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="56085-832">`.bot` 파일이 없는 봇에 대한 `bot download`에서 해당 봇에 대한 애플리케이션 설정 값을 사용하여 언어별 구성 파일을 만들도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-832">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="56085-833">`bot prepare-deploy`에 `Typescript` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-833">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="56085-834">`--code-dir`에 `package.json`이 포함되어 있지 않은 경우 `Javascript` 및 `Typescript` 봇에 대한 경고 메시지가 `bot prepare-deploy`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-834">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="56085-835">성공하면 `bot prepare-deploy`에서 `true`를 반환하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-835">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="56085-836">`bot prepare-deploy`에 자세한 정보 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-836">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="56085-837">`az bot create -v v3`에 더 많은 사용 가능한 Application Insights 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-837">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="56085-838">구성</span><span class="sxs-lookup"><span data-stu-id="56085-838">Configure</span></span>
* <span data-ttu-id="56085-839">폴더 기반 인수 기본값 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-839">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="56085-840">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="56085-840">Eventhubs</span></span>
* <span data-ttu-id="56085-841">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-841">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="56085-842">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-842">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="56085-843">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-843">Network</span></span>
* <span data-ttu-id="56085-844">[주요 변경 사항]`vnet [create|update]`에 대한 `--cache` 인수가 `--defer`로 바뀜</span><span class="sxs-lookup"><span data-stu-id="56085-844">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="56085-845">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="56085-845">Policy Insights</span></span>
* <span data-ttu-id="56085-846">`--expand PolicyEvaluationDetails`에서 리소스에 대한 정책 평가 세부 정보를 쿼리하도록 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-846">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="56085-847">역할</span><span class="sxs-lookup"><span data-stu-id="56085-847">Role</span></span>
* <span data-ttu-id="56085-848">[사용 되지 않음]`create-for-rbac` hide '- password' 인수 변경 - 2019년 5월에 지원이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-848">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="56085-849">Service Bus</span><span class="sxs-lookup"><span data-stu-id="56085-849">Service Bus</span></span>
* <span data-ttu-id="56085-850">`namespace network-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-850">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="56085-851">네트워크 규칙에 대한 `--default-action` 인수가 `namespace [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-851">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="56085-852">`topic [create|update]`의 `--max-size`에서 프리미엄 SKU를 통해 10, 20, 40 및 80GB 값을 지원할 수 있도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-852">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="56085-853">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-853">SQL</span></span>
* <span data-ttu-id="56085-854">`sql virtual-cluster [list|show|delete]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-854">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="56085-855">VM</span><span class="sxs-lookup"><span data-stu-id="56085-855">VM</span></span>
* <span data-ttu-id="56085-856">VMSS VM 인스턴스의 보호 정책 업데이트를 사용하도록 설정하기 위해 `--protect-from-scale-in` 및 `--protect-from-scale-set-actions`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-856">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="56085-857">VMSS VM 인스턴스의 일반 업데이트를 사용하도록 설정하기 위해 `--instance-id`가 `vmss update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-857">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="56085-858">`vmss wait`에 `--instance-id` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-858">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="56085-859">근접 배치 그룹 관리를 위해 새 `ppg` 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-859">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="56085-860">PPG 관리를 위해 `--ppg`가 `[vm|vmss] create` 및 `vm availability-set create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-860">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="56085-861">`--hyper-v-generation` 매개 변수가 `image create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-861">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="56085-862">2019년 4월 23일</span><span class="sxs-lookup"><span data-stu-id="56085-862">April 23, 2019</span></span>

<span data-ttu-id="56085-863">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="56085-863">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="56085-864">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-864">ACS</span></span>
* <span data-ttu-id="56085-865">`aks get-credentials`를 중복 값을 덮어쓸지 묻는 메시지로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-865">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="56085-866">Dev Space 명령 "aks use-dev-spaces" 및 "aks remove-dev-spaces"명령에서 `(PREVIEW)` 제거</span><span class="sxs-lookup"><span data-stu-id="56085-866">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="56085-867">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-867">AMS</span></span>
* <span data-ttu-id="56085-868">자산 및 계정 필터 업데이트 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-868">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-869">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-869">AppService</span></span>
* <span data-ttu-id="56085-870">`webapp ssh`에 ASE 및 시간 제한에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-870">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="56085-871">Github 리포지토리에서 함수 앱에 이르는 Azure DevOps 파이프라인에 CI CD를 설치할 수 있도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-871">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="56085-872">Github 개인용 액세스 토큰을 받기 위해 `functionapp devops-build create`에 `--github-pat` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-872">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="56085-873">functionapp 소스 코드가 포함된 Github 리포지토리를 수락하기 위해 `functionapp devops-build create`에 `--github-repository` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-873">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="56085-874">`az webapp up --logs`가 오류로 실패하고 기본 .NETCORE 버전을 2.1로 업데이트하는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-874">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="56085-875">소비 계획이 있는 함수 앱을 만들 때 불필요한 functionapp 설정을 제거</span><span class="sxs-lookup"><span data-stu-id="56085-875">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="56085-876">기본 ASP 문자열이 끝에 숫자를 추가하여 SKU 옵션에 따라 새로운 ASP를 만들도록 `webapp up`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-876">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="56085-877">브라우저에서 앱을 실행하기 위해 `-b`를 `webapp up`에 대한 옵션으로 추가</span><span class="sxs-lookup"><span data-stu-id="56085-877">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="56085-878">`AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` 환경 변수를 처리하도록 `webapp deployment source config zip` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-878">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="56085-879">배포 관리자</span><span class="sxs-lookup"><span data-stu-id="56085-879">Deployment Manager</span></span>
* <span data-ttu-id="56085-880">[PREVIEW] 출시를 지원하는 아티팩트 생성 및 관리</span><span class="sxs-lookup"><span data-stu-id="56085-880">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="56085-881">랩</span><span class="sxs-lookup"><span data-stu-id="56085-881">Lab</span></span>
* <span data-ttu-id="56085-882">조기 종료를 유발하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-882">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="56085-883">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-883">Network</span></span>
* <span data-ttu-id="56085-884">자식 영역 생성 중 부모의 `dns zone create`에 자동 이름 서버 위임이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-884">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="56085-885">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-885">Resource</span></span>
* <span data-ttu-id="56085-886">[사용 되지 않음]`resource link`의 사용되지 않는 `--link-id`, `--target-id` 및 `--filter-string` 인수</span><span class="sxs-lookup"><span data-stu-id="56085-886">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="56085-887">대신 `--link`, `--target` 및 `--filter` 인수를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="56085-887">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="56085-888">`resource link [create|update]` 명령이 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-888">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="56085-889">오류가 발생하여 리소스 ID를 사용하는 삭제가 중단되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-889">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="56085-890">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-890">SQL</span></span>
* <span data-ttu-id="56085-891">관리형 인스턴스에 사용자 지정 표준 시간대 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-891">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="56085-892">탄력적 풀 이름을 `sql db update`와 함께 사용할 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-892">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="56085-893">`sql server [create|update]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-893">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="56085-894">명령 `sql server wait` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-894">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-895">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-895">Storage</span></span>
* <span data-ttu-id="56085-896">`storage blob generate-sas`의 이중 인코딩 SAS 토큰으로 인한 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-896">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-897">VM</span><span class="sxs-lookup"><span data-stu-id="56085-897">VM</span></span>
* <span data-ttu-id="56085-898">종료하지 않고 VM 전원을 끄기 위해 `--skip-shutdown` 플래그를 `vm|vmss stop`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-898">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="56085-899">게시 프로필의 계정 유형을 설정하기 위해 `--storage-account-type` 인수가 `sig image-version create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-899">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="56085-900">Azure 지역별 스토리지 계정 유형을 설정할 수 있도록 `sig image-version create`에 `--target-regions` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-900">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="56085-901">2019년 4월 9일</span><span class="sxs-lookup"><span data-stu-id="56085-901">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="56085-902">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-902">Core</span></span>
* <span data-ttu-id="56085-903">일부 확장이 버전을 `Unknown`으로 표시하고 업데이트할 수 없었던 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-903">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="56085-904">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-904">ACR</span></span>
* <span data-ttu-id="56085-905">이미지를 컨텍스트 없이 실행하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-905">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="56085-906">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-906">AMS</span></span>
* [사용 되지 않음]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [호환성이 손상되는 변경]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="56085-909">`ams streaming-policy create`에 새로운 암호화 매개 변수 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-909">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="56085-910">새로운 매개 변수 `--filters`가 `ams streaming-locator create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-910">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-911">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-911">AppService</span></span>
* <span data-ttu-id="56085-912">`webapp up`에 `--logs` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-912">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="56085-913">`functionapp devops-build create` 명령 `azure-pipelines.yml` 생성 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-913">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="56085-914">`unctionapp devops-build create` 오류 처리 및 표시기 개선</span><span class="sxs-lookup"><span data-stu-id="56085-914">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="56085-915">[주요 변경 사항]`devops-build` 명령에 대한 `--local-git` 플래그 제거, Azure DevOps 파이프라인을 만드는 경우 강제 로컬 git 검색 및 처리</span><span class="sxs-lookup"><span data-stu-id="56085-915">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="56085-916">Linux 함수 플랜을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-916">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="56085-917">`functionapp update --plan`을 사용하여 함수 앱 아래에 계획을 전환하는 기능이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-917">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="56085-918">Azure Functions 프리미엄 플랜 확장 설정에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-918">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-919">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-919">CDN</span></span>
* <span data-ttu-id="56085-920">`Microsoft_Standard` 및 `Standard_ChinaCdn`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-920">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="56085-921">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="56085-921">Feedback</span></span>
* <span data-ttu-id="56085-922">최근 실행한 명령에 대한 메타데이터를 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-922">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="56085-923">브라우저를 열고 문제 템플릿을 사용하여 문제 생성 프로세스에서 도움이 되는 프롬프트를 사용자에게 표시하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-923">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="56085-924">'--verbose'를 사용하여 실행할 때 문제 본문을 출력하도록 `feedback`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-924">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-925">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-925">Monitor</span></span>
* <span data-ttu-id="56085-926">`metrics alert [create|update]`에서 "count"가 허용된 값이 아닌 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-926">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="56085-927">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-927">Network</span></span>
* <span data-ttu-id="56085-928">`vnet-gateway list-bgp-peer-status`로 테이블 형식이 표시되지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-928">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="56085-929">`list-request-headers` 및 `list-response-headers` 명령을 `application-gateway rewrite-rule`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-929">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="56085-930">`list-server-variables` 명령을 `application-gateway rewrite-rule condition`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-930">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="56085-931">급행 경로 포트 상의 링크 상태를 업데이트할 때 알 수 없는 속성 예외 `express-route port update`가 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="56085-931">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="56085-932">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="56085-932">PrivateDNS</span></span>
* <span data-ttu-id="56085-933">프라이빗 DNS 영역에 대한 `network private-dns` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-933">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="56085-934">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-934">Resource</span></span>
* <span data-ttu-id="56085-935">`deployment create` 및 `group deployment create`에서 빈 매개 변수 세트를 포함하는 매개 변수 파일이 작동하지 않을 수 있는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-935">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="56085-936">역할</span><span class="sxs-lookup"><span data-stu-id="56085-936">Role</span></span>
* <span data-ttu-id="56085-937">`--years`를 올바르게 처리하도록 `create-for-rbac` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-937">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="56085-938">[주요 변경 사항] 구독 아래의 모든 할당을 무조건 삭제하는 경우 프롬프트를 표시하도록 `role assignment delete` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-938">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="56085-939">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-939">SQL</span></span>
* <span data-ttu-id="56085-940">속성 proxyOverride 및 publicDataEndpointEnabled로 `sql mi [create|update]` 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-940">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="56085-941">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-941">Storage</span></span>
* <span data-ttu-id="56085-942">[주요 변경 사항]`storage blob delete`의 결과 제거</span><span class="sxs-lookup"><span data-stu-id="56085-942">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="56085-943">SAS를 포함하는 BLOB에 대해 전체 URI를 만드는 `--full-uri`을 `storage blob generate-sas`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-943">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="56085-944">스냅샷에서 파일을 복사하는 `--file-snapshot`을 `storage file copy start`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-944">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="56085-945">NoPendingCopyOperation에 대해 예외 대신 오류만 표시하도록 `storage blob copy cancel` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-945">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="56085-946">2019년 3월 26일</span><span class="sxs-lookup"><span data-stu-id="56085-946">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="56085-947">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-947">Core</span></span>
* <span data-ttu-id="56085-948">개발 확장이 호환되지 않는 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-948">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="56085-949">이제 오류 처리 시 고객에게 문제 페이지를 가리킵니다.</span><span class="sxs-lookup"><span data-stu-id="56085-949">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="56085-950">클라우드</span><span class="sxs-lookup"><span data-stu-id="56085-950">Cloud</span></span>
* <span data-ttu-id="56085-951">`cloud set`의 '구독을 찾을 수 없음' 오류가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-951">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="56085-952">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-952">ACR</span></span>
* <span data-ttu-id="56085-953">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="56085-953">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="56085-954">`--auth-mode`가 `acr build`, `acr run`, `acr task create` 및 `acr task update` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-954">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="56085-955">작업에 대한 자격 증명을 관리하는 'acr task credential' 명령 그룹이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-955">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="56085-956">'--no-wait'가 `acr build` 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-956">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-957">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-957">AppService</span></span>
* <span data-ttu-id="56085-958">`webapp up`가 빈 디렉터리 또는 알 수 없는 코드 시나리오에서 제대로 실행되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-958">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="56085-959">슬롯이 `[webapp|functionapp] config ssl bind`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-959">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="56085-960">BOT Service</span><span class="sxs-lookup"><span data-stu-id="56085-960">BOT Service</span></span>
* <span data-ttu-id="56085-961">`webapp`을 통한 봇 배포를 준비하는 `bot prepare-deploy`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-961">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="56085-962">암호가 제공되지 않으면 암호를 표시하도록 `bot create --kind registration`이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-962">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="56085-963">[주요 변경 사항]`bot create --kind registration`의 `--endpoint`가 기본적으로 필수 문자열 대신 빈 문자열로 지정되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-963">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="56085-964">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-964">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-965">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-965">CDN</span></span>
* <span data-ttu-id="56085-966">`--no-wait`에 대한 지원이 `cdn endpoint [create|update|start|stop|delete|load|purge]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-966">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [주요 변경 사항]: `cdn endpoint create` 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="56085-968">더 이상 "IgnoreQueryString"이 기본값으로 지정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-968">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="56085-969">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-969">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-970">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="56085-970">Cosmosdb</span></span>
* <span data-ttu-id="56085-971">계정 업데이트 시 `--enable-multiple-write-locations` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-971">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="56085-972">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-972">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-973">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-973">Interactive</span></span>
* <span data-ttu-id="56085-974">azdev를 통해 설치된 대화형 확장과 호환되지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-974">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-975">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-975">Monitor</span></span>
* <span data-ttu-id="56085-976">`monitor metrics alert [create|update]`에 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-976">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="56085-977">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-977">Network</span></span>
* <span data-ttu-id="56085-978">`rewrite-rule` 명령 그룹이 `application-gateway`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-978">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-979">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-979">Profile</span></span>
* <span data-ttu-id="56085-980">관리 서비스 ID에 대한 테넌트 수준 계정 지원이 `login`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-980">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="56085-981">Postgres</span><span class="sxs-lookup"><span data-stu-id="56085-981">Postgres</span></span> 
* <span data-ttu-id="56085-982">postgresql `replica` 명령 및 `restart server` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-982">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="56085-983">서버를 만드는 데 제공되지 않은 경우 리소스 그룹에서 기본 위치를 가져오고 보존 기간(일)에 대한 유효성 검사를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-983">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="56085-984">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-984">Resource</span></span>
* <span data-ttu-id="56085-985">`deployment [create|list|show]`의 테이블 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-985">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="56085-986">secureObject 형식이 인식되지 않는 `deployment [create|validate]` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-986">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="56085-987">그래프</span><span class="sxs-lookup"><span data-stu-id="56085-987">Graph</span></span>
* <span data-ttu-id="56085-988">`--end-date`에 대한 지원이 `ad [app|sp] credential reset`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-988">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="56085-989">`ad app permission add`를 사용하여 권한을 추가할 수 있도록 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-989">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="56085-990">권한이 없는 `ad app permission list` 관련 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-990">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="56085-991">현재 계정에 구독이 없는 경우 역할 할당 삭제를 건너뛰도록 `ad sp delete`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-991">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="56085-992">목록이 제공되지 않는 경우 `--identifier-uris`에서 기본적으로 빈 목록을 지정하도록 `ad app create`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-992">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="56085-993">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-993">storage</span></span>
* <span data-ttu-id="56085-994">공유 스냅샷에서 다운로드할 수 있도록 `--snapshot`이 `storage file download-batch`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-994">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="56085-995">자세한 정보를 줄이고 현재 Blob을 표시하도록 `storage blob [download-batch|upload-batch]` 진행 표시줄이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-995">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="56085-996">암호화 매개 변수를 업데이트하는 `storage account update` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-996">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="56085-997">oauth(`--auth-mode=login`)를 사용하면 `storage blob show`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-997">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="56085-998">VM</span><span class="sxs-lookup"><span data-stu-id="56085-998">VM</span></span>
* <span data-ttu-id="56085-999">`image update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-999">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="56085-1000">2019년 3월 12일</span><span class="sxs-lookup"><span data-stu-id="56085-1000">March 12, 2019</span></span>

<span data-ttu-id="56085-1001">2\.0.60 버전</span><span class="sxs-lookup"><span data-stu-id="56085-1001">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="56085-1002">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1002">Core</span></span>

* <span data-ttu-id="56085-1003">구독이 발견되지 않는 문제를 `cloud set`에서 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1003">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1004">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1004">ACR</span></span>

* <span data-ttu-id="56085-1005">이미지 가져오기에서 중복 소스 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1005">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1006">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1006">ACS</span></span>

* <span data-ttu-id="56085-1007">kubectl에서 지원되지 않는 경우 `aks browse`에 대한 `--listen-address` 매개 변수를 무시하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1007">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="56085-1008">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1008">AppService</span></span>

* <span data-ttu-id="56085-1009">Kudu 게시 url 및 해당 자격 증명을 가져오도록 `[webapp|functionapp] deployment list-publishing-credentials` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1009">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="56085-1010">`webapp auth update`에 대한 잘못된 인쇄 문 삭제</span><span class="sxs-lookup"><span data-stu-id="56085-1010">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="56085-1011">Linux App Service 계획에서 런타임에 올바른 이미지를 설정하도록 `functionapp` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1011">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="56085-1012">`webapp up`에 대한 미리보기 태그 제거 및 명령 개선 사항 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1012">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-1013">Botservice</span><span class="sxs-lookup"><span data-stu-id="56085-1013">Botservice</span></span>

* <span data-ttu-id="56085-1014">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `SCM_DO_BUILD_DURING_DEPLOYMENT`를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1014">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="56085-1015">v4 웹앱 봇에 대한 ARM 템플릿의 애플리케이션 설정에 `Microsoft-BotFramework-AppId` 및 `Microsoft-BotFramework-AppPassword` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1015">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="56085-1016">`bot create`의 끝에 `bot publish` 명령 출력에서 작은 따옴표 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1016">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="56085-1017">`bot publish`를 비동기로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1017">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="56085-1018">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1018">Container</span></span>

* <span data-ttu-id="56085-1019">`--no-wait` 인수를 `container [start|restart]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1019">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="56085-1020">EventHub</span><span class="sxs-lookup"><span data-stu-id="56085-1020">EventHub</span></span>

* <span data-ttu-id="56085-1021">캡처에서 빈 보관을 지원하기 위해 `--skip-empty-archives` 플래그를 `eventhub create|update`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1021">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="56085-1022">찾기</span><span class="sxs-lookup"><span data-stu-id="56085-1022">Find</span></span>

* <span data-ttu-id="56085-1023">주요 기능 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1023">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-1024">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-1024">HDInsight</span></span>

* <span data-ttu-id="56085-1025">ADLS Gen2 MSI를 지원하기 위해 `hdinsight create`에 `--storage-account-managed-identity` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1025">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="56085-1026">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1026">Network</span></span>

* <span data-ttu-id="56085-1027">다른 구독의 게이트웨이 간 VPN 연결을 업데이트하지 못하는 `vpn-connection update` 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1027">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1028">Rdbms</span><span class="sxs-lookup"><span data-stu-id="56085-1028">Rdbms</span></span>

* <span data-ttu-id="56085-1029">서버 생성 시 제공되지 않은 경우 리소스 그룹에서 기본 위치를 얻고 재방문 주기에 대한 유효성 검사를 추가하는 사소한 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1029">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="56085-1030">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1030">Role</span></span>

* <span data-ttu-id="56085-1031">정의를 올바르게 확인하기 위해 ID를 사용하도록 `role definition update` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1031">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="56085-1032">`ad app credential reset`을 앱의 서비스 사용자가 항상 존재한다는 가정을 제거하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1032">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="56085-1033">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="56085-1033">Service Fabric</span></span>

* <span data-ttu-id="56085-1034">`sf cluster list`가 반복 가능하지 않은 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1034">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="56085-1035">2019년 2월 26일</span><span class="sxs-lookup"><span data-stu-id="56085-1035">February 26, 2019</span></span>

<span data-ttu-id="56085-1036">버전 2.0.59</span><span class="sxs-lookup"><span data-stu-id="56085-1036">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="56085-1037">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1037">Core</span></span>

* <span data-ttu-id="56085-1038">`--subscription NAME`을 사용하는 일부 인스턴스에서 예외가 발생하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1038">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1039">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1039">ACR</span></span>

* <span data-ttu-id="56085-1040">`acr build`, `acr task create` 및 `acr task update` 명령에 대한 `--target` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1040">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="56085-1041">Azure에 로그인하지 않은 경우 런타임 명령에 대한 오류 처리 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1041">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1042">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1042">ACS</span></span>

* <span data-ttu-id="56085-1043">`--listen-address` 옵션을 `aks port-forward`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1043">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1044">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1044">AppService</span></span>

* <span data-ttu-id="56085-1045">`functionapp devops-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1045">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1046">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1046">Batch</span></span>
* <span data-ttu-id="56085-1047">[주요 변경 사항]`batch pool upgrade os` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-1047">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="56085-1048">[주요 변경 사항]`Application` 응답에서 `Pacakges` 속성 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-1048">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="56085-1049">애플리케이션 패키지를 나열하는 `batch application package list` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1049">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="56085-1050">[주요 변경 사항] 모든 `batch application` 명령에서 `--application-id`가 `--application-name`으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1050">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="56085-1051">원시 API 응답을 요청하는 명령에 `--json-file` 인수 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1051">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="56085-1052">모든 엔드포인트에 `https://`가 누락된 경우 이를 자동으로 포함하도록 유효성 검사 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-1052">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-1053">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-1053">CosmosDB</span></span>

* <span data-ttu-id="56085-1054">Cosmos DB 계정의 VNET 규칙을 관리하기 위한 `add`, `remove` 및 `list` 명령으로 `network-rule` 하위 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1054">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="56085-1055">Kusto</span><span class="sxs-lookup"><span data-stu-id="56085-1055">Kusto</span></span>

* <span data-ttu-id="56085-1056">[주요 변경 사항] 포맷하는 동안 데이터베이스의 `hot_cache_period` 및 `soft_delete_period` 유형이 ISO8601로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1056">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="56085-1057">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1057">Network</span></span>

* <span data-ttu-id="56085-1058">`--express-route-gateway-bypass` 인수를 `vpn-connection [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1058">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="56085-1059">`express-route` 확장의 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1059">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="56085-1060">`express-route gateway` 및 `express-route port` 명령 그룹 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1060">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="56085-1061">`express-route peering [create|update]`에 추가된 인수: `--legacy-mode`</span><span class="sxs-lookup"><span data-stu-id="56085-1061">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="56085-1062">`--allow-classic-operations` 및 `--express-route-port` 인수를 `express-route [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1062">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="56085-1063">`--gateway-default-site` 인수를 `vnet-gateway [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1063">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="56085-1064">`ipsec-policy` 명령이 `vnet-gateway`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1064">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1065">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1065">Resource</span></span>

* <span data-ttu-id="56085-1066">유형 입력란이 대소문자를 구분하는 `deployment create` 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1066">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="56085-1067">URI 기반 매개 변수 파일에 대한 지원이 `policy assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1067">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="56085-1068">URI 기반 매개 변수 및 정의에 대한 지원이 `policy set-definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1068">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="56085-1069">`policy definition update`에 대한 매개 변수 및 규칙 처리 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1069">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="56085-1070">교차 구독 ID가 구독 ID를 제대로 인식하지 않는 `resource show/update/delete/tag/invoke-action` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1070">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="56085-1071">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1071">Role</span></span>

* <span data-ttu-id="56085-1072">앱 역할에 대한 지원이 `ad app [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1072">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1073">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1073">VM</span></span>

* <span data-ttu-id="56085-1074">Ubuntu 18.0에서 `vm create where ` --accelerated-networking\`이 기본값으로 사용되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1074">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="56085-1075">2019년 2월 12일</span><span class="sxs-lookup"><span data-stu-id="56085-1075">February 12, 2019</span></span>

<span data-ttu-id="56085-1076">버전 2.0.58</span><span class="sxs-lookup"><span data-stu-id="56085-1076">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="56085-1077">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1077">Core</span></span>

* <span data-ttu-id="56085-1078">업데이트할 수 있는 패키지가 있는 경우 이제 `az --version`에서 알림을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1078">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="56085-1079">JSON 출력에서 `--ids`를 더 이상 사용할 수 없었던 회귀가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1079">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1080">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1080">ACR</span></span>
* <span data-ttu-id="56085-1081">[주요 변경 사항]`acr build-task` 명령 그룹이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1081">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="56085-1082">[주요 변경 사항]`acr repository delete`에서 `--tag` 및 `--manifest` 옵션이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1082">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1083">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1083">ACS</span></span>
* <span data-ttu-id="56085-1084">대/소문자를 구분하지 않는 이름에 대한 지원이 `aks [enable-addons|disable-addons]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1084">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="56085-1085">`aks update-credentials --reset-aad`를 사용하여 Azure Active Directory를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1085">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="56085-1086">`aks get-credentials`에 대한 `--output`은 무시된다는 설명이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1086">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="56085-1087">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-1087">AMS</span></span>
* <span data-ttu-id="56085-1088">`ams streaming-endpoint [start | stop | create | update] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1088">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="56085-1089">`ams live-event [create | start | stop | reset] wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1089">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1090">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1090">Appservice</span></span>
* <span data-ttu-id="56085-1091">ACR 컨테이너를 사용하여 함수를 만들고 구성할 수 있는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1091">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="56085-1092">json을 통해 웹앱 구성을 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1092">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="56085-1093">`appservice-plan-update`에 대한 도움말이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1093">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="56085-1094">App Insights에서 함수 앱을 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1094">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="56085-1095">웹앱 SSH 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1095">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-1096">Botservice</span><span class="sxs-lookup"><span data-stu-id="56085-1096">Botservice</span></span>
* <span data-ttu-id="56085-1097">`bot publish`에 대한 UX가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1097">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="56085-1098">`az bot publish` 중에 `npm install`을 실행할 때 시간 제한에 대한 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1098">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="56085-1099">`az bot create`의 `--name`에서 잘못된 `.` 문자가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1099">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="56085-1100">Azure Storage, App Service 계획, Function/Web App 및 Application Insights를 만들 때 리소스 이름에 대한 임의 지정을 중지하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1100">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="56085-1101">[사용 되지 않음]`--proj-file-path`를 위해 `--proj-name` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1101">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="56085-1102">가져온 IIS Node.js 배포 파일이 아직 없으면 `az bot publish`에서 이를 제거하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1102">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="56085-1103">App Service에서 `node_modules` 폴더를 삭제하지 않도록 `--keep-node-modules` 인수가 `az bot publish`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1103">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="56085-1104">Azure Function 또는 Web App 봇을 만들 때의 `az bot create`의 출력에 `"publishCommand"` 키-값 쌍이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1104">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="56085-1105">`"publishCommand"` 값은 새로 만든 봇을 게시하는 데 필요한 매개 변수가 미리 채워진 `az bot publish` 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1105">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="56085-1106">v4 SDK 봇에서 8.9.4 대신 10.14.1을 사용하도록 ARM 템플릿의 `"WEBSITE_NODE_DEFAULT_VERSION"`이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1106">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-1107">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-1107">Key Vault</span></span>
* <span data-ttu-id="56085-1108">`--id`를 사용할 때 일부 사용자가 `unexpected_keyword` 오류를 받은 `keyvault secret backup` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1108">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-1109">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-1109">Monitor</span></span>
* <span data-ttu-id="56085-1110">`monitor metrics alert [create|update]`에서 `*` 차원 값을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1110">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1111">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1111">Network</span></span>
* <span data-ttu-id="56085-1112">`dns zone export`에서 내보낸 CNAME이 FQDN인지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1112">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="56085-1113">애플리케이션 게이트웨이 백 엔드 주소 풀을 지원하도록 `--gateway-name` 매개 변수가 `nic ip-config address-pool [add|remove]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1113">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="56085-1114">Log Analytics 작업 영역을 통해 트래픽을 분석할 수 있도록 `--traffic-analytics` 및 `--workspace` 인수가 `network watcher flow-log configure`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1114">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="56085-1115">`--idle-timeout` 및 `--floating-ip`가 `lb inbound-nat-pool [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1115">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="56085-1116">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="56085-1116">Policy Insights</span></span>
* <span data-ttu-id="56085-1117">리소스 정책 업데이트 관리 기능을 지원하는 `policy remediation` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1117">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1118">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-1118">RDBMS</span></span>
* <span data-ttu-id="56085-1119">도움말 메시지 및 명령 매개 변수가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1119">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="56085-1120">Redis</span><span class="sxs-lookup"><span data-stu-id="56085-1120">Redis</span></span>
* <span data-ttu-id="56085-1121">방화벽 규칙을 관리하기 위한 명령(create, update, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1121">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="56085-1122">서버 링크를 관리하기 위한 명령(create, delete, show, list)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1122">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="56085-1123">패치 일정을 관리하기 위한 명령(create, update, delete, show)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1123">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="56085-1124">가용성 영역 및 최소 TLS 버전에 대한 지원이 'redis create'에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1124">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="56085-1125">[주요 변경 사항]`redis update-settings` 및 `redis list-all` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1125">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="56085-1126">[주요 변경 사항]`redis create`: '테넌트 설정' 매개 변수가 key[=value] 형식으로 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1126">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="56085-1127">[사용 되지 않음]`redis import-method` 명령이 사용되지 않는다는 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1127">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="56085-1128">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1128">Role</span></span>
* <span data-ttu-id="56085-1129">[주요 변경 사항]`vm` 명령에서 `az identity` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1129">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="56085-1130">SQL VM</span><span class="sxs-lookup"><span data-stu-id="56085-1130">SQL VM</span></span>
* <span data-ttu-id="56085-1131">[사용 되지 않음] 오타로 인해 `--boostrap-acc-pwd` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1131">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1132">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1132">VM</span></span>
* <span data-ttu-id="56085-1133">`vm list-skus`에서 `--all true` 대신 `--all`을 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1133">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="56085-1134">`vmss run-command [invoke | list | show]`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1134">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="56085-1135">이전에 실행하면 `vmss encryption enable`이 실패했던 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1135">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="56085-1136">[주요 변경 사항]`az identity` 명령이 `role` 명령으로 전환되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1136">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="56085-1137">2019년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="56085-1137">January 31, 2019</span></span>

<span data-ttu-id="56085-1138">버전 2.0.57</span><span class="sxs-lookup"><span data-stu-id="56085-1138">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="56085-1139">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1139">Core</span></span>

* <span data-ttu-id="56085-1140">[8399 문제](https://github.com/Azure/azure-cli/issues/8399)에 대한 핫 픽스입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1140">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="56085-1141">2019년 1월 28일</span><span class="sxs-lookup"><span data-stu-id="56085-1141">January 28, 2019</span></span>

<span data-ttu-id="56085-1142">버전 2.0.56</span><span class="sxs-lookup"><span data-stu-id="56085-1142">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1143">ACR</span></span>
* <span data-ttu-id="56085-1144">VNet/IP 규칙에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1144">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1145">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1145">ACS</span></span>
* <span data-ttu-id="56085-1146">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1146">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="56085-1147">Managed OpenShift 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1147">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="56085-1148">`aks update-credentials -reset-service-principal`을 사용하여 서비스 주체를 업데이트할 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1148">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="56085-1149">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-1149">AMS</span></span>
* <span data-ttu-id="56085-1150">[주요 변경 사항]`ams asset get-streaming-locators`에서 `ams asset list-streaming-locators`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1150">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="56085-1151">[주요 변경 사항]`ams streaming-locator get-content-keys`에서 `ams streaming-locator list-content-keys`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1151">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1152">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1152">Appservice</span></span>
* <span data-ttu-id="56085-1153">App Insights에서 `functionapp create`를 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1153">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="56085-1154">App Service 계획 만들기(탄력성 프리미엄 포함)에 대한 지원이 함수 앱에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1154">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="56085-1155">탄력적 프리미엄 요금제와 관련된 앱 설정 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1155">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="56085-1156">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1156">Container</span></span>
* <span data-ttu-id="56085-1157">`container start` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1157">Added `container start` command</span></span>
* <span data-ttu-id="56085-1158">컨테이너를 만드는 동안 10진수 값을 CPU에 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1158">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="56085-1159">EventGrid</span><span class="sxs-lookup"><span data-stu-id="56085-1159">EventGrid</span></span>
* <span data-ttu-id="56085-1160">`--deadletter-endpoint` 매개 변수가 `event-subscription [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1160">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="56085-1161">storagequeue 및 hybridconnection이 'event-subscription [create|update] --endpoint-type'에 대한 새 값으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1161">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="56085-1162">이벤트에 대한 재시도 정책을 지정하는 `--max-delivery-attempts` 및 `--event-ttl` 매개 변수가 `event-subscription create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1162">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="56085-1163">이벤트 구독에 대상으로 웹후크를 사용하는 경우에 대한 경고 메시지가 `event-subscription [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1163">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="56085-1164">모든 이벤트 구독 관련 명령에 대한 source-resource-id 매개 변수가 추가되었고, 다른 모든 원본 리소스 관련 매개 변수가 더 이상 사용되지 않는 것으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1164">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-1165">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-1165">HDInsight</span></span>
* <span data-ttu-id="56085-1166">[주요 변경 사항]`hdinsight [application] create`에서 `--virtual-network` 및 `--subnet-name` 매개 변수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1166">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="56085-1167">[주요 변경 사항]`hdinsight create --storage-account`에서 Blob 엔드포인트 대신 스토리지 계정의 이름 또는 ID를 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1167">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="56085-1168">`hdinsight create`에 `--vnet-name` 및 `--subnet-name` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1168">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="56085-1169">Enterprise Security Package 및 디스크 암호화에 대한 지원이 `hdinsight create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1169">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="56085-1170">`hdinsight rotate-disk-encryption-key` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1170">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="56085-1171">`hdinsight update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1171">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="56085-1172">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-1172">IoT</span></span>
* <span data-ttu-id="56085-1173">인코딩 형식이 routing-endpoint 명령에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1173">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="56085-1174">Kusto</span><span class="sxs-lookup"><span data-stu-id="56085-1174">Kusto</span></span>
* <span data-ttu-id="56085-1175">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1175">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-1176">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-1176">Monitor</span></span>
* <span data-ttu-id="56085-1177">ID 비교에서 대/소문자를 구분하지 않도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1177">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="56085-1178">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-1178">Profile</span></span>
* <span data-ttu-id="56085-1179">`login`에서 관리 서비스 ID에 대한 테넌트 수준 계정을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1179">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1180">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1180">Network</span></span>
* <span data-ttu-id="56085-1181">`--bandwidth` 인수가 무시되었던 `express-route update`: 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1181">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="56085-1182">집합 이해력으로 인해 스택 추적이 발생했던 `ddos-protection update` 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1182">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1183">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1183">Resource</span></span>
* <span data-ttu-id="56085-1184">URI 매개 변수 파일에 대한 지원이 `group deployment create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1184">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="56085-1185">관리 ID에 대한 지원이 `policy assignment [create|list|show]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1185">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="56085-1186">SQL Virtual Machine</span><span class="sxs-lookup"><span data-stu-id="56085-1186">SQL Virtual Machine</span></span>
* <span data-ttu-id="56085-1187">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1187">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1188">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1188">Storage</span></span>
* <span data-ttu-id="56085-1189">수정 프로그램을 통해 동일한 개체에서 변경된 속성만 업데이트하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1189">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="56085-1190">반환될 때 2진수 데이터가 Base 64로 인코딩되는 #8021 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1190">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1191">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1191">VM</span></span>
* <span data-ttu-id="56085-1192">`vm encryption enable`에서 디스크 암호화 키 자격 증명 모음의 유효성을 검사하고 해당 키 암호화 키 자격 증명 모음이 있는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1192">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="56085-1193">`--force` 플래그가 `vm encryption enable`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1193">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="56085-1194">2019년 1월 15일</span><span class="sxs-lookup"><span data-stu-id="56085-1194">January 15, 2019</span></span>

<span data-ttu-id="56085-1195">버전 2.0.55</span><span class="sxs-lookup"><span data-stu-id="56085-1195">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1196">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1196">ACR</span></span>
* <span data-ttu-id="56085-1197">존재하지 않는 helm 차트를 강제로 푸시하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1197">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="56085-1198">ARM 요청 없이 런타임 작업을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1198">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="56085-1199">[사용 되지 않음] 다음 명령의 `--resource-group` 매개 변수가 사용되지 않음:</span><span class="sxs-lookup"><span data-stu-id="56085-1199">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="56085-1200">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1200">ACS</span></span>
* <span data-ttu-id="56085-1201">새 ACI 지역에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1201">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1202">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1202">Appservice</span></span>
* <span data-ttu-id="56085-1203">ASE RG 및 App RG가 다른 ASE에서 호스팅되는 앱에 대한 인증서 업로드 관련 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1203">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="56085-1204">`webapp up`에서 SKU P1V1을 Linux에 대한 기본값으로 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1204">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="56085-1205">배포가 실패하면 `[webapp|functionapp] deployment source config-zip`에서 올바른 오류 메시지를 표시하도록 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1205">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="56085-1206">`webapp ssh` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1206">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-1207">Botservice</span><span class="sxs-lookup"><span data-stu-id="56085-1207">Botservice</span></span>
* <span data-ttu-id="56085-1208">배포 상태 업데이트가 `bot create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1208">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="56085-1209">구성</span><span class="sxs-lookup"><span data-stu-id="56085-1209">Configure</span></span>
* <span data-ttu-id="56085-1210">`none`이 구성 가능한 출력 형식으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1210">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-1211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-1211">CosmosDB</span></span>
* <span data-ttu-id="56085-1212">공유 처리량을 사용하여 데이터베이스를 만들 수 있도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1212">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-1213">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-1213">HDInsight</span></span>
* <span data-ttu-id="56085-1214">애플리케이션 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1214">Added commands for managing applications</span></span>
* <span data-ttu-id="56085-1215">스크립트 작업 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1215">Added commands for managing script actions</span></span>
* <span data-ttu-id="56085-1216">OMS(Operation Management Suite) 관리 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1216">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="56085-1217">지역별 사용량 나열에 대한 지원이 `hdinsight list-usage`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1217">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="56085-1218">[주요 변경 사항]`hdinsight create`에서 기본 클러스터 유형이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1218">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1219">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1219">Network</span></span>
* <span data-ttu-id="56085-1220">`--custom-headers` 및 `--status-code-ranges` 인수를 `traffic-manager profile [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1220">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="56085-1221">새 라우팅 유형으로 Subnet 및 Multivalue가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1221">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="56085-1222">`--custom-headers` 및 `--subnets` 인수를 `traffic-manager endpoint [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1222">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="56085-1223">`--vnets ""`를 `ddos-protection update`에 제공함으로써 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1223">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="56085-1224">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1224">Role</span></span>
* <span data-ttu-id="56085-1225">[사용 되지 않음]`create-for-rbac`에 대한 `--password` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1225">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="56085-1226">대신 CLI에서 생성된 보안 암호를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1226">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="56085-1227">보안</span><span class="sxs-lookup"><span data-stu-id="56085-1227">Security</span></span>
* <span data-ttu-id="56085-1228">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1228">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1229">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1229">Storage</span></span>
* <span data-ttu-id="56085-1230">[주요 변경 사항]`storage [blob|file|container|share] list`의 기본 결과 수가 5,000개가 되도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1230">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="56085-1231">모든 결과를 반환하는 원래 동작에는 `--num-results *`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1231">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="56085-1232">`--marker` 매개 변수가 `storage [blob|file|container|share] list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1232">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="56085-1233">다음 페이지에 대한 로그 표식이 `storage [blob|file|container|share] list`의 STDERR에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1233">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="56085-1234">정적 웹 사이트를 지원하는 `storage blob service-properties update` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1234">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1235">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1235">VM</span></span>
* <span data-ttu-id="56085-1236">`vm [disk|unmanaged-disk]` 및 `vmss disk`에서 더 일관된 매개 변수를 사용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1236">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="56085-1237">`[vm|vmss] create`를 참조하는 테넌트 간 이미지에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1237">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="56085-1238">`vm diagnostics get-default-config --windows-os`에서 기본 구성과 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1238">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="56085-1239">설정되기 전에 프로비저닝해야 하는 확장을 정의하기 위해 `--provision-after-extensions` 인수가 `vmss extension set`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1239">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="56085-1240">기본 복제 수를 설정하기 위해 `--replica-count` 인수가 `sig image-version update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1240">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="56085-1241">전체 리소스 ID가 제공되는 경우에도 원본 OS 디스크가 동일한 이름의 VM으로 잘못 인식되는 `image create --source`와 관련된 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1241">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="56085-1242">2018년 12월 20일</span><span class="sxs-lookup"><span data-stu-id="56085-1242">December 20, 2018</span></span>

<span data-ttu-id="56085-1243">버전 2.0.54</span><span class="sxs-lookup"><span data-stu-id="56085-1243">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="56085-1244">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1244">Appservice</span></span>
* <span data-ttu-id="56085-1245">`webapp up`의 재배포 실패 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1245">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="56085-1246">웹앱 스냅샷 목록 및 복원에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1246">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="56085-1247">Windows 함수 앱 `--runtime` 플래그에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1247">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="56085-1248">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="56085-1248">IoTCentral</span></span>
* <span data-ttu-id="56085-1249">업데이트 명령 API 호출이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1249">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="56085-1250">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1250">Role</span></span>
* <span data-ttu-id="56085-1251">[주요 변경 사항] 기본적으로 처음 100개의 개체만 목록으로 표시하도록 `ad [app|sp] list`를 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-1251">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1252">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1252">SQL</span></span>
* <span data-ttu-id="56085-1253">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1253">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1254">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1254">VM</span></span>
* <span data-ttu-id="56085-1255">`---os-type` 매개 변수가 `disk create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1255">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="56085-1256">2018년 12월 18일</span><span class="sxs-lookup"><span data-stu-id="56085-1256">December 18, 2018</span></span>

<span data-ttu-id="56085-1257">버전 2.0.53</span><span class="sxs-lookup"><span data-stu-id="56085-1257">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="56085-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1258">ACR</span></span>
* <span data-ttu-id="56085-1259">외부 컨테이너 레지스트리에서 이미지 가져오기에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1259">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="56085-1260">작업 목록의 표 레이아웃을 좁게 축소함</span><span class="sxs-lookup"><span data-stu-id="56085-1260">Condensed the table layout for task list</span></span>
* <span data-ttu-id="56085-1261">Azure DevOps URL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1261">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1262">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1262">ACS</span></span>
* <span data-ttu-id="56085-1263">가상 노드 미리 보기 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1263">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="56085-1264">`aks create`에 대한 AAD 인수에서 "(미리 보기)"를 제거함</span><span class="sxs-lookup"><span data-stu-id="56085-1264">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="56085-1265">[사용 되지 않음]`az acs` 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1265">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="56085-1266">ACS 서비스가 2020년 1월 31일 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1266">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="56085-1267">새 AKS 클러스터를 만들 때 네트워크 정책에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1267">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="56085-1268">노드 풀이 하나뿐일 경우 `aks scale`에 `--nodepool-name` 인수 요구사항 삭제</span><span class="sxs-lookup"><span data-stu-id="56085-1268">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1269">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1269">Appservice</span></span>
* <span data-ttu-id="56085-1270">`webapp config container`에서 `--slot` 매개 변수를 적용할 수 없던 문제 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1270">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="56085-1271">Botservice</span><span class="sxs-lookup"><span data-stu-id="56085-1271">Botservice</span></span>
* <span data-ttu-id="56085-1272">`bot show`를 호출할 때 `.bot` 파일 구문 분석에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1272">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="56085-1273">AppInsights 프로비전 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="56085-1273">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="56085-1274">파일 경로를 처리할 때 공백 버그를 수정함</span><span class="sxs-lookup"><span data-stu-id="56085-1274">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="56085-1275">Kudu 네트워크 호출이 감소함</span><span class="sxs-lookup"><span data-stu-id="56085-1275">Reduced Kudu network calls</span></span>
* <span data-ttu-id="56085-1276">일반 명령 UX 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1276">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-1277">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-1277">Consumption</span></span>
* <span data-ttu-id="56085-1278">알림을 표시하도록 예산 API 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1278">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-1279">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-1279">CosmosDB</span></span>
* <span data-ttu-id="56085-1280">다중 마스터에서 단일 마스터로의 계정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1280">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="56085-1281">지도</span><span class="sxs-lookup"><span data-stu-id="56085-1281">Maps</span></span>
* <span data-ttu-id="56085-1282">S1 SKU에 대한 지원이 `maps account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1282">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1283">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1283">Network</span></span>
* <span data-ttu-id="56085-1284">`--format` 및 `--log-version`에 대한 지원이 `watcher flow-log configure`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1284">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="56085-1285">""을(를) 사용하여 해결과 등록을 지워도 VNet이 작동하지 않을 경우 `dns zone update`을(를) 통해 문제를 해결함</span><span class="sxs-lookup"><span data-stu-id="56085-1285">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1286">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1286">Resource</span></span>
* <span data-ttu-id="56085-1287">`policy assignment [create|list|delete|show|update]`에서 관리 그룹에 대한 범위 매개 변수 처리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1287">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="56085-1288">새 명령 `resource wait`이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1288">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1289">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1289">Storage</span></span>
*  <span data-ttu-id="56085-1290">스토리지 서비스를 위한 로그 스키마 버전 업데이트 기능이 `storage logging update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1290">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1291">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1291">VM</span></span>
* <span data-ttu-id="56085-1292">지정된 vm에 할당된 관리 서비스가 없는 경우 `vm identity remove`에서 크래시가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1292">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="56085-1293">2018년 12월 4일</span><span class="sxs-lookup"><span data-stu-id="56085-1293">December 4, 2018</span></span>

<span data-ttu-id="56085-1294">버전 2.0.52</span><span class="sxs-lookup"><span data-stu-id="56085-1294">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="56085-1295">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1295">Core</span></span>
* <span data-ttu-id="56085-1296">다중 테넌트 서비스 주체에 대한 교차 테넌트 리소스 프로 비전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1296">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="56085-1297">tsv 출력을 사용한 명령에서 파이프된 id의 구문 분석이 잘못되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1297">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1298">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1298">Appservice</span></span>
* <span data-ttu-id="56085-1299">[미리 보기] 애플리케이션에 콘텐츠 생성 및 배포를 돕는 `webapp up` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1299">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="56085-1300">백 엔드 변경으로 인해 컨테이너 기반의 Windows 앱에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1300">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="56085-1301">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1301">Network</span></span>
* <span data-ttu-id="56085-1302">WAF 제외를 지원하기 위해 `--exclusion` 인수를 `application-gateway waf-config set`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1302">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="56085-1303">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1303">Role</span></span>
* <span data-ttu-id="56085-1304">암호 자격 증명을 위해 사용자 지정 식별자에 대해 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1304">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="56085-1305">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1305">VM</span></span>
* <span data-ttu-id="56085-1306">[사용 되지 않음]`vm extension [show|wait] --expand` 매개 변수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1306">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="56085-1307">응답 없는 VM을 다시 배포하기 위해 `--force` 매개 변수를 `vm restart`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1307">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="56085-1308">암호와 SSH 인증을 사용하여 VM을 생성하기 위해 "all"을 허용하도록 `[vm|vmss] create --authentication-type` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1308">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="56085-1309">이미지에 OS 디스크 캐싱을 설정하기 위해 `image create --os-disk-caching` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1309">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="56085-1310">2018년 11월 20일</span><span class="sxs-lookup"><span data-stu-id="56085-1310">November 20, 2018</span></span>

<span data-ttu-id="56085-1311">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="56085-1311">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="56085-1312">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1312">Core</span></span>
* <span data-ttu-id="56085-1313">ID에서 구독 이름을 재사용하지 않도록 MSI 로그인 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1313">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1314">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1314">ACR</span></span>
* <span data-ttu-id="56085-1315">작업 단계에 대해 컨텍스트 토큰 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1315">Added context token to task step</span></span>
* <span data-ttu-id="56085-1316">acr 작업을 미러링하도록 acr에서 비밀을 설정하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1316">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="56085-1317">`show-tags` 및 `show-manifests` 명령에 대한 `--top` 및 `--orderby`에 대한 지원 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1317">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1318">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1318">Appservice</span></span>
* <span data-ttu-id="56085-1319">zip 배포 기본 시간 제한을 변경하여 해당 상태에 대한 폴링이 5 분으로 증가하고 시간 제한 속성을 추가하여 이 값을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1319">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="56085-1320">기본값을 `node_version`으로 업데이트 했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1320">Updated the default `node_version`.</span></span> <span data-ttu-id="56085-1321">2단계 스왑 중에 슬롯 스왑 동작을 재설정하면 모든 appsettings 및 연결 문자열이 보존됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1321">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="56085-1322">Linux App Service 계획 만들기에 대한 클라이언트 쪽 SKU 확인 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1322">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="56085-1323">Zipdeploy 상태를 가져오기 하려고 할 때의 오류가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1323">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="56085-1324">IotCentral</span><span class="sxs-lookup"><span data-stu-id="56085-1324">IotCentral</span></span>
* <span data-ttu-id="56085-1325">IoT Central 애플리케이션을 만들 때 하위 도메인 가용성 확인 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1325">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-1326">KeyVault</span><span class="sxs-lookup"><span data-stu-id="56085-1326">KeyVault</span></span>
* <span data-ttu-id="56085-1327">오류가 무시되었을 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1327">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="56085-1328">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1328">Network</span></span>
* <span data-ttu-id="56085-1329">신뢰할 수 있는 루트 인증서를 처리하기 위해 `root-cert` 하위 명령을 `application-gateway`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1329">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="56085-1330">`--min-capacity` 및 `--custom-error-pages` 옵션을 `application-gateway [create|update]`에 추가:</span><span class="sxs-lookup"><span data-stu-id="56085-1330">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="56085-1331">`application-gateway create`에 가용성 영역 지원을 위해 `--zones` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1331">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="56085-1332">`application-gateway waf-config set`에 추가된 인수: `--file-upload-limit`, `--max-request-body-size`, `--request-body-check`</span><span class="sxs-lookup"><span data-stu-id="56085-1332">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1333">Rdbms</span><span class="sxs-lookup"><span data-stu-id="56085-1333">Rdbms</span></span>
* <span data-ttu-id="56085-1334">mariadb vnet 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1334">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="56085-1335">Rbac</span><span class="sxs-lookup"><span data-stu-id="56085-1335">Rbac</span></span>
* <span data-ttu-id="56085-1336">`ad app update`에서 변경할 수 없는 자격 증명을 업데이트 하려는 시도 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1336">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="56085-1337">`ad [app|sp] list`에 대한 가까운 장래의 호환성이 손상되는 변경을 알리는 출력 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1337">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="56085-1338">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1338">Storage</span></span>
* <span data-ttu-id="56085-1339">스토리지 복사 명령에 대한 코너 케이스의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-1339">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="56085-1340">대상 계정과 원본 계정이 같을 때 로그인 자격 증명을 사용하지 않는 `storage blob copy start-batch` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1340">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="56085-1341">`sas_token`이 URL에 통합되지 않은 `storage [blob|file] url`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1341">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="56085-1342">`[blob|container] list`에 호환성이 손상되는 변경 경고가 추가됨: 기본적으로 처음 5000개의 결과만 출력됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1342">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1343">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1343">VM</span></span>
* <span data-ttu-id="56085-1344">관리되는 OS 및 데이터 디스크에 대한 스토리지 계정 SKU를 별도로 지정하도록 `[vm|vmss] create --storage-sku`에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1344">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="56085-1345">`sig image-version`에 대한 버전 이름 매개 변수를 `--image-version -e`가 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1345">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="56085-1346">`--image-version-name`에 대한 `sig image-version` 인수가 사용되지 않으며 `--image-version`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="56085-1346">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="56085-1347">`[vm|vmss] create --ephemeral-os-disk`에 로컬 OS 디스크를 사용하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1347">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="56085-1348">`--no-wait`에 대한 지원이 `snapshot create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1348">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="56085-1349">`snapshot wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1349">Added `snapshot wait` command</span></span>
* <span data-ttu-id="56085-1350">`[vm|vmss] extension set --extension-instance-name` 인스턴스 이름을 사용하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1350">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="56085-1351">2018년 11월 6일</span><span class="sxs-lookup"><span data-stu-id="56085-1351">November 6, 2018</span></span>

<span data-ttu-id="56085-1352">버전 2.0.50</span><span class="sxs-lookup"><span data-stu-id="56085-1352">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="56085-1353">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1353">Core</span></span>
* <span data-ttu-id="56085-1354">서비스 주체 sn+issuer auth에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1354">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1355">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1355">ACR</span></span>
* <span data-ttu-id="56085-1356">작업 소스 트리거에 대한 커밋 및 끌어오기 요청 git 이벤트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1356">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="56085-1357">빌드 명령에서 기본 Dockerfile이 지정되지 않은 경우 기본 Dockerfile을 사용하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1357">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1358">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1358">ACS</span></span>
* <span data-ttu-id="56085-1359">[주요 변경 사항] 기본적으로 'az aks browse'을 기본적으로 사용하기 위해 `enable_cloud_console_aks_browse` 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-1359">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="56085-1360">Advisor</span><span class="sxs-lookup"><span data-stu-id="56085-1360">Advisor</span></span>
* <span data-ttu-id="56085-1361">GA 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1361">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="56085-1362">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-1362">AMS</span></span>
* <span data-ttu-id="56085-1363">새 명령 그룹이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="56085-1363">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="56085-1364">새 명령이 추가됨:</span><span class="sxs-lookup"><span data-stu-id="56085-1364">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="56085-1365">암호화 매개 변수 지원이 `ams streaming-policy create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1365">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="56085-1366">이제 제거할 출력 인덱스를 전달하여 `ams transform output remove`에 대한 추가 지원을 수행할 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-1366">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="56085-1367">`ams job` 명령 그룹에 `--correlation-data` 및 `--label` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1367">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="56085-1368">`ams asset` 명령 그룹에 `--storage-account` 및 `--container` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1368">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="56085-1369">`ams asset get-sas-url` 명령에서 만료 시간(현재+23h) 및 사용 권한(읽기)의 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1369">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="56085-1370">[주요 변경 사항]`ams streaming locator` 명령이 `ams streaming-locator`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="56085-1370">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="56085-1371">[주요 변경 사항]`ams streaming locator`의 `--content-keys` 인수가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-1371">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="56085-1372">[주요 변경 사항]`ams streaming locator` 명령에서 `--content-policy-name`에서 `--content-key-policy-name`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1372">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="56085-1373">[주요 변경 사항]`ams streaming policy` 명령이 `ams streaming-policy`로 대체됨</span><span class="sxs-lookup"><span data-stu-id="56085-1373">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="56085-1374">[주요 변경 사항]`ams transform` 명령 그룹에서 `--preset-names` 인수가 `--preset`으로 대체됨</span><span class="sxs-lookup"><span data-stu-id="56085-1374">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="56085-1375">이제 한 번에 1개의 출력/사전 설정만 설정할 수 있습니다(더 추가하려면 `ams transform output add`를 실행해야 함).</span><span class="sxs-lookup"><span data-stu-id="56085-1375">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="56085-1376">또한 사용자 정의 JSON에 경로를 전달하여 사용자 정의 StandardEncoderPreset을 설정할 수 있습니다</span><span class="sxs-lookup"><span data-stu-id="56085-1376">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="56085-1377">[주요 변경 사항]`ams job start` 명령에서 `--output-asset-names `에서 `--output-assets`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1377">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="56085-1378">이제 'assetName = label' 형식으로 공백으로 구분된 자산 목록을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1378">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="56085-1379">레이블이 없는 자산은 'assetName='과 같이 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1379">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1380">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1380">AppService</span></span>
* <span data-ttu-id="56085-1381">백업 스케쥴이 아직 설정되지 않은 경우 백업 스케쥴 설정을 방해하는 `az webapp config backup update`의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1381">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="56085-1382">구성</span><span class="sxs-lookup"><span data-stu-id="56085-1382">Configure</span></span>
* <span data-ttu-id="56085-1383">출력 형식 옵션에 YAML이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1383">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="56085-1384">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1384">Container</span></span>
* <span data-ttu-id="56085-1385">yaml에 컨테이너 그룹을 내보낼 때 ID를 표시하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1385">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="56085-1386">EventHub</span><span class="sxs-lookup"><span data-stu-id="56085-1386">EventHub</span></span>
* <span data-ttu-id="56085-1387">`eventhub namespace [create|update]`에서 Kafka를 지원하기 위해 `--enable-kafka` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1387">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-1388">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-1388">Interactive</span></span>
* <span data-ttu-id="56085-1389">이제 대화형이 `interactive` 확장을 설치하여 업데이트 및 지원이 더 빨라집니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1389">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-1390">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-1390">Monitor</span></span>
* <span data-ttu-id="56085-1391">`monitor metrics alert [create|update]`의 `--condition`에 슬래시(/)와 마침표(.) 문자를 포함하는 메트릭 이름에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1391">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1392">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1392">Network</span></span>
* <span data-ttu-id="56085-1393">`network private-endpoint`를 위해 `network interface-endpoint` 명령 이름 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1393">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="56085-1394">`express-route peering connection create`의 `--peer-circuit` 인수가 ID를 허용하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1394">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="56085-1395">`--ip-tags`가 `public-ip create`와 함께 제대로 작동하지 않는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1395">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="56085-1396">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-1396">Profile</span></span>
* <span data-ttu-id="56085-1397">cert auto-rolls로 서비스 주체 로그인을 위해 `--use-cert-sn-issuer`가 `az login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1397">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1398">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-1398">RDBMS</span></span>
* <span data-ttu-id="56085-1399">mysql 복제본 명령 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1399">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1400">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1400">Resource</span></span>
* <span data-ttu-id="56085-1401">관리 그룹 및 구독에 대한 지원이 `policy definition|set-definition` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1401">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="56085-1402">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1402">Role</span></span>
* <span data-ttu-id="56085-1403">API 권한 관리, 로그인 사용자 및 애플리케이션 암호 및 인증서 자격 증명 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1403">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="56085-1404">displayName과 서비스 주체 이름 간의 혼동을 방지하기 위해 `ad sp create-for-rbac`을 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-1404">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="56085-1405">AAD 앱에 권한을 부여하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1405">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1406">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1406">Storage</span></span>
* <span data-ttu-id="56085-1407">`Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`에 설명된 대로 SAS 및 엔드포인트(계정 이름 또는 키 없이)로만 스토리지 서비스에 연결하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1407">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1408">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1408">VM</span></span>
* <span data-ttu-id="56085-1409">이미지의 기본 스토리지 계정 유형 설정을 위해 `image create`에 `storage-sku` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1409">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="56085-1410">`vm resize`가 `--no-wait` 옵션으로 인해 명령이 충돌하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1410">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="56085-1411">`vm encryption show` 테이블 출력 형식을 상태 표시로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1411">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="56085-1412">`vm secret format`이 json/jsonc 출력을 요구하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1412">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="56085-1413">원하지 않는 출력 형식이 선택되면 사용자에게 경고하고 json을 기본값으로 출력</span><span class="sxs-lookup"><span data-stu-id="56085-1413">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="56085-1414">`vm create --image`에 대한 인수 유효성 검사가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1414">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="56085-1415">2018년 10월 23일</span><span class="sxs-lookup"><span data-stu-id="56085-1415">October 23, 2018</span></span>

<span data-ttu-id="56085-1416">버전 2.0.49</span><span class="sxs-lookup"><span data-stu-id="56085-1416">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="56085-1417">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1417">Core</span></span>
* <span data-ttu-id="56085-1418">`--subscription`이 `--ids`의 구독보다 우선적으로 적용되는 `--ids` 관련 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1418">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="56085-1419">`--ids`를 사용하여 매개 변수가 무시되는 경우 명시적 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1419">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1420">ACR</span></span>
* <span data-ttu-id="56085-1421">Python2에서 ACR Build 인코딩 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1421">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-1422">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-1422">CDN</span></span>
* <span data-ttu-id="56085-1423">[주요 변경 사항] "IgnoreQueryString"를 더 이상 기본값으로 설정하지 않도록 `cdn endpoint create`의 기본 쿼리 문자열 캐싱 동작이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1423">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="56085-1424">이제 서비스에 의해 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1424">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="56085-1425">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1425">Container</span></span>
* <span data-ttu-id="56085-1426">'--ip-address'를 전달하기 위해 `Private`이 올바른 유형으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1426">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="56085-1427">컨테이너 그룹에 대한 가상 네트워크를 설정하기 위해 서브넷 ID만 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1427">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="56085-1428">다른 리소스 그룹의 VNet을 사용하기 위해 VNet 이름 또는 리소스 ID를 사용할 수 있도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1428">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="56085-1429">MSI ID를 컨테이너 그룹에 추가하기 위해 `--assign-identity`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1429">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="56085-1430">시스템 할당 MSI ID에 대한 역할 할당을 만들기 위해 `--scope`가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1430">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="56085-1431">장기 실행 프로세스 없이 이미지를 사용하여 컨테이너 그룹을 만들 때 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1431">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="56085-1432">`list` 및 `show` 명령에 대한 테이블 출력 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1432">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-1433">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-1433">CosmosDB</span></span>
* <span data-ttu-id="56085-1434">`cosmosdb create`에 `--enable-multiple-write-locations` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1434">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-1435">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-1435">Interactive</span></span>
* <span data-ttu-id="56085-1436">글로벌 구독 매개 변수가 매개 변수에서 나타나는지 확인하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1436">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="56085-1437">IoT Central</span><span class="sxs-lookup"><span data-stu-id="56085-1437">IoT Central</span></span>
* <span data-ttu-id="56085-1438">IoT Central 애플리케이션 생성을 위해 템플릿 및 표시 이름 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1438">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="56085-1439">[주요 변경 사항] F1 SKU에 대한 지원이 제거되었습니다. 대신 S1 SKU를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1439">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-1440">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-1440">Monitor</span></span>
* <span data-ttu-id="56085-1441">`monitor activity-log list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="56085-1441">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="56085-1442">구독 수준에서 모든 이벤트를 나열하는 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1442">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="56085-1443">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1443">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="56085-1444">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1444">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="56085-1445">`--namespace`가 사용되지 않는 옵션 `--resource-provider`에 대한 별칭으로 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1445">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="56085-1446">강력한 형식의 옵션이 포함되지 않은 값이 서비스에서 지원되지 않으므로 `--filters`가 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1446">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="56085-1447">`monitor metrics list`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="56085-1447">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="56085-1448">시간 쿼리를 더 쉽게 만들기 위해 `--offset` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1448">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="56085-1449">넓은 범위의 ISO8601 형식 및 사용자에게 친숙한 날짜/시간 서식을 사용하기 위해 `--start-time` 및 `--end-time`에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1449">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="56085-1450">`monitor diagnostic-settings create`을 위한 `--event-hub` 및 `--event-hub-rule` 인수에 대한 유효성 검사가 개선되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1450">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="56085-1451">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1451">Network</span></span>
* <span data-ttu-id="56085-1452">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1452">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="56085-1453">NIC에 애플리케이션 게이트웨이 백 엔드 주소 풀을 추가하도록 지원하기 위해 `--app-gateway-address-pools` 및 `--gateway-name` 인수가 `nic ip-config create/update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1453">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="56085-1454">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="56085-1454">ServiceBus</span></span>
* <span data-ttu-id="56085-1455">현재 Service Bus Standard를 Premium 네스페이스 마이그레이션 상태로 표시하기 위해 읽기 전용 `migration_state`가 MigrationConfigProperties에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1455">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1456">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1456">SQL</span></span>
* <span data-ttu-id="56085-1457">수동 장애 조치 정책을 사용하기 위해 `sql failover-group create` 및 `sql failover-group update`가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1457">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1458">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1458">Storage</span></span>
* <span data-ttu-id="56085-1459">모든 항목이 올바른 "서비스" 키를 표시하도록 `az storage cors list` 출력 서식 지정이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1459">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="56085-1460">불변성 정책 차단 컨테이너를 삭제하기 위해 `--bypass-immutability-policy` 매개 변수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1460">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1461">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1461">VM</span></span>
* <span data-ttu-id="56085-1462">`[vm|vmss] create`에서 머신의 Lv/Lv2 시리즈에 대해 디스크 캐싱 모드가 `None`이 되도록 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1462">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="56085-1463">`vm create`에 대해 지원되는 크기 목록 지원 네트워킹 가속기가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1463">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="56085-1464">`disk create`에서 ultrassd iops 및 mbps configs에 대한 강력한 형식 인수가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1464">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="56085-1465">2018년 10월 16일</span><span class="sxs-lookup"><span data-stu-id="56085-1465">October 16, 2018</span></span>

<span data-ttu-id="56085-1466">버전 2.0.48</span><span class="sxs-lookup"><span data-stu-id="56085-1466">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1467">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1467">VM</span></span>
* <span data-ttu-id="56085-1468">Homebrew 설치가 실패하게 된 SDK 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1468">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="56085-1469">2018년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="56085-1469">October 9, 2018</span></span>

<span data-ttu-id="56085-1470">버전 2.0.47</span><span class="sxs-lookup"><span data-stu-id="56085-1470">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="56085-1471">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1471">Core</span></span>
* <span data-ttu-id="56085-1472">"잘못된 요청" 오류의 오류 처리를 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1472">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1473">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1473">ACR</span></span>
* <span data-ttu-id="56085-1474">helm 클라이언트와 유사한 테이블 형식에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1474">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1475">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1475">ACS</span></span>
* <span data-ttu-id="56085-1476">`aks [create|scale] --nodepool-name`을 추가하여 nodepool 이름 구성, 12 문자로 잘림, 기본값 - nodepool1</span><span class="sxs-lookup"><span data-stu-id="56085-1476">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="56085-1477">Parimiko가 실패할 때 'scp'로 되돌아가도록 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1477">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="56085-1478">`aks create`가 `--aad-tenant-id`를 요구하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1478">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="56085-1479">중복된 항목이 있을 때 Kubernetes 자격 증명에 대한 병합 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1479">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="56085-1480">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1480">Container</span></span>
* <span data-ttu-id="56085-1481">특정 런타임을 사용하여 Linux 소비 계획 형식 만들기를 지원하도록 `functionapp create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1481">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="56085-1482">[미리 보기] Windows 컨테이너에 웹앱을 호스트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1482">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="56085-1483">이벤트 허브</span><span class="sxs-lookup"><span data-stu-id="56085-1483">Event Hub</span></span>
* <span data-ttu-id="56085-1484">`eventhub update` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1484">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="56085-1485">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1485">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="56085-1486">확장</span><span class="sxs-lookup"><span data-stu-id="56085-1486">Extensions</span></span>
* <span data-ttu-id="56085-1487">이미 설치되어 있는 확장을 추가하려고 시도할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1487">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="56085-1488">HDInsight</span><span class="sxs-lookup"><span data-stu-id="56085-1488">HDInsight</span></span>
* <span data-ttu-id="56085-1489">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1489">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="56085-1490">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-1490">IoT</span></span>
* <span data-ttu-id="56085-1491">첫 번째 실행 배너에 확장 설치 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1491">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-1492">KeyVault</span><span class="sxs-lookup"><span data-stu-id="56085-1492">KeyVault</span></span>
* <span data-ttu-id="56085-1493">최신 API 프로필에 keyvault 스토리지 명령을 제한하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1493">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="56085-1494">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1494">Network</span></span>
* <span data-ttu-id="56085-1495">`network dns zone create` 수정됨: 사용자가 기본 위치를 구성한 경우에도 명령은 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1495">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="56085-1496">#6052 참조</span><span class="sxs-lookup"><span data-stu-id="56085-1496">See #6052</span></span>
* <span data-ttu-id="56085-1497">`network vnet peering create`에 `--remote-vnet-id`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="56085-1497">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="56085-1498">이름 또는 ID를 허용하는 `network vnet peering create`에 `--remote-vnet` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1498">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="56085-1499">서브넷에서 `--subnet-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet create`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1499">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="56085-1500">서브넷에서 `--address-prefixes`를 사용하는 여러 주소 접두사에 대한 지원이 `network vnet subnet [create|update]`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1500">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="56085-1501">`WAF_v2` 또는 `Standard_v2` SKU로 게이트웨이를 만들지 못하던 `network application-gateway create` 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1501">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="56085-1502">`--service-endpoint-policy` 편의 인수가 `network vnet subnet update`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1502">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="56085-1503">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1503">Role</span></span>
* <span data-ttu-id="56085-1504">`ad app owner`에 Azure AD 앱 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1504">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="56085-1505">`ad sp owner`에 Azure AD 서비스 주체 소유자를 나열하기 위한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1505">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="56085-1506">역할 정의 작성 및 업데이트 명령이 여러 권한 구성을 허용하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1506">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="56085-1507">홈 페이지 URI가 항상 "https"가 되도록 `ad sp create-for-rbac`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1507">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="56085-1508">Service Bus</span><span class="sxs-lookup"><span data-stu-id="56085-1508">Service Bus</span></span>
* <span data-ttu-id="56085-1509">[주요 변경 사항] 빈 목록을 표시하는 대신 일반적인 방법으로 resource(s) NotFound(404)에 대한 오류를 처리하도록 `list` 명령을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1509">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1510">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1510">VM</span></span>
* <span data-ttu-id="56085-1511">`disk grant-access` 내 빈 `accessSas` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1511">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="56085-1512">오버프로비저닝을 처리하기 위해 충분히 큰 프런트 엔드 포트 범위를 예약하도록 `vmss create`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1512">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="56085-1513">`sig`에 대한 업데이트 명령을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1513">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="56085-1514">`sig`에 이미지 버전 관리에 대한 `--no-wait` 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1514">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="56085-1515">공용 IP 주소 가용성 영역을 표시하도록 `vm list-ip-addresses`가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1515">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="56085-1516">디스크의 기본 lun을 첫 번째 사용 가능한 지점으로 설정하도록 `[vm|vmss] disk attach`를 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1516">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="56085-1517">2018년 9월 21일</span><span class="sxs-lookup"><span data-stu-id="56085-1517">September 21, 2018</span></span>

<span data-ttu-id="56085-1518">버전 2.0.46</span><span class="sxs-lookup"><span data-stu-id="56085-1518">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1519">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1519">ACR</span></span>
* <span data-ttu-id="56085-1520">ACR 작업 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1520">Added ACR Task commands</span></span>
* <span data-ttu-id="56085-1521">빠른 실행 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1521">Added quick run command</span></span>
* <span data-ttu-id="56085-1522">`build-task` 명령 그룹 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1522">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="56085-1523">ACR에서 Helm 차트 관리를 지원하기 위해 `helm` 명령 그룹 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1523">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="56085-1524">관리되는 레지스트리의 명등원 만들기를 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1524">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="56085-1525">빌드 로그 표시를 위한 비형식 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1525">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1526">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1526">ACS</span></span>
* <span data-ttu-id="56085-1527">AKS 마스터 FQDN 설정을 위한 `install-connector` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1527">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="56085-1528">서비스 주체 및 skip-role-assignemnt를 지정하지 않은 경우의 vnet-subnet-id에 대한 역할 할당 만들기 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1528">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1529">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1529">AppService</span></span>

* <span data-ttu-id="56085-1530">웹 작업(연속 및 트리거) 작업 관리 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1530">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="56085-1531">az webapp config set 지원 --fts-state 속성. functionapp config set 및 show 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1531">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="56085-1532">웹앱에 대한 Bring Your Own Storage 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1532">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="56085-1533">삭제된 웹앱 나열 및 복원을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1533">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1534">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1534">Batch</span></span>
* <span data-ttu-id="56085-1535">AddTaskCollectionParameter 구문 지원을 위해 `--json-file`을 통한 작업 추가 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1535">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="56085-1536">수락된 `--json-file` 형식에 대한 설명서 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1536">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="56085-1537">`batch pool create`에 `--max-tasks-per-node-option` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1537">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="56085-1538">옵션이 지정되지 않은 경우 현재 로그인된 계정을 표시하도록 `batch account` 동작 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1538">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="56085-1539">Batch AI</span><span class="sxs-lookup"><span data-stu-id="56085-1539">Batch AI</span></span> 
* <span data-ttu-id="56085-1540">`batchai cluster create` 명령에서 자동 스토리지 계정 만들기 오류 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1540">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="56085-1541">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="56085-1541">Cognitive Services</span></span>
* <span data-ttu-id="56085-1542">`--sku`, `--kind`, `--location` 인수에 대한 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1542">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="56085-1543">명령 `cognitiveservices account list-usage` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1543">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="56085-1544">명령 `cognitiveservices account list-kinds` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1544">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="56085-1545">명령 `cognitiveservices account list` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1545">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="56085-1546">`cognitiveservices list` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1546">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="56085-1547">`cognitiveservices account list-skus`에 대해 선택 사항으로 `--name` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1547">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="56085-1548">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1548">Container</span></span>
* <span data-ttu-id="56085-1549">실행 중인 컨테이너 그룹 다시 시작 및 중지 기능 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1549">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="56085-1550">네트워크 프로필 전달을 위한 `--network-profile` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1550">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="56085-1551">VNET에서 컨테이너 그룹 생성을 허용하도록 `--subnet`, `--vnet_name` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1551">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="56085-1552">컨테이너 그룹의 상태를 표시하도록 테이블 출력 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1552">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="56085-1553">Datalake</span><span class="sxs-lookup"><span data-stu-id="56085-1553">Datalake</span></span>
* <span data-ttu-id="56085-1554">가상 네트워크 규칙에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1554">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="56085-1555">대화형 셸</span><span class="sxs-lookup"><span data-stu-id="56085-1555">Interactive Shell</span></span>
* <span data-ttu-id="56085-1556">명령 실행이 실패하는 Windows 오류 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1556">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="56085-1557">사용되지 않는 개체로 인해 발생하는 대화식 명령 로드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1557">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="56085-1558">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-1558">IoT</span></span>
* <span data-ttu-id="56085-1559">IoT 허브 라우팅을 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1559">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-1560">Key Vault</span><span class="sxs-lookup"><span data-stu-id="56085-1560">Key Vault</span></span>
* <span data-ttu-id="56085-1561">RSA 키에 대한 Key Vault 키 가져오기 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1561">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="56085-1562">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1562">Network</span></span>
* <span data-ttu-id="56085-1563">공용 IP 접두사 기능을 지원하기 위한 `network public-ip prefix` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1563">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="56085-1564">서비스 엔드포인트 정책 기능을 지원하기 위한 `network service-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1564">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="56085-1565">표준 Load Balancer 아웃바운드 규칙 생성을 지원하기 위한 `network lb outbound-rule` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1565">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="56085-1566">공용 IP 접두사를 사용한 프런트 엔드 IP 구성 지원을 위해 `network lb frontend-ip create/update`에 `--public-ip-prefix` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1566">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="56085-1567">`network lb rule/inbound-nat-rule/inbound-nat-pool create/update`에 `--enable-tcp-reset` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1567">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="56085-1568">`network lb rule create/update`에 `--disable-outbound-snat` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1568">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="56085-1569">클래식 NSG에 `network watcher flow-log show/configure` 사용 허용</span><span class="sxs-lookup"><span data-stu-id="56085-1569">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="56085-1570">`network watcher run-configuration-diagnostic` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1570">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="56085-1571">`network watcher test-connectivity` 명령 수정 및 `--method`, `--valid-status-codes` 및 `--headers` 속성 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1571">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="56085-1572">`network express-route create/update`: `--allow-global-reach` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1572">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="56085-1573">`network vnet subnet create/update`: `--delegation`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1573">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="56085-1574">`network vnet subnet list-available-delegations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1574">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="56085-1575">`network traffic-manager profile create/update`: 모니터 구성을 위해 `--interval`, `--timeout`, `--max-failures`에 대한 지원이 추가됨 `--path`, `--port`, `--protocol`을(를) 위해 `--monitor-path`, `--monitor-port`, `--monitor-protocol` 옵션은 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1575">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="56085-1576">`network lb frontend-ip create/update`: 프라이빗 IP 할당 방법을 설정하는 논리가 수정됨. 개인 IP 주소가 제공되는 경우 정적 할당이 설정됨. 개인 IP 주소가 제공되지 않는 경우나 개인 IP 주소에 빈 문자열이 주어질 경우 동적 할당이 설정됨.</span><span class="sxs-lookup"><span data-stu-id="56085-1576">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="56085-1577">`dns record-set * create/update`: `--target-resource`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1577">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="56085-1578">인터페이스 엔드포인트 개체를 쿼리하기 위한 `network interface-endpoint` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1578">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="56085-1579">네트워크 프로필의 부분 관리를 위한 `network profile show/list/delete` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1579">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="56085-1580">ExpressRoute 간 피어링 연결을 관리하기 위한 `network express-route peering connection` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1580">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1581">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-1581">RDBMS</span></span>
* <span data-ttu-id="56085-1582">MariaDB 서비스 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1582">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="56085-1583">예약</span><span class="sxs-lookup"><span data-stu-id="56085-1583">Reservation</span></span>
* <span data-ttu-id="56085-1584">예약된 리소스 열거형 형식에 CosmosDb 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1584">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="56085-1585">패치 모델에서 이름 속성 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1585">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="56085-1586">앱 관리</span><span class="sxs-lookup"><span data-stu-id="56085-1586">Manage App</span></span>
* <span data-ttu-id="56085-1587">마켓플레이스 관리 앱의 인스턴스 생성이 충돌하는 `managedapp create --kind MarketPlace` 버그 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1587">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="56085-1588">지원되는 프로필로 제한되도록 `feature` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1588">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="56085-1589">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1589">Role</span></span>
* <span data-ttu-id="56085-1590">사용자 그룹 멤버 자격을 나열하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1590">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="56085-1591">SignalR</span><span class="sxs-lookup"><span data-stu-id="56085-1591">SignalR</span></span>
* <span data-ttu-id="56085-1592">첫번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1592">First release</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1593">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1593">Storage</span></span>
* <span data-ttu-id="56085-1594">blob 및 큐 권한 부여에 대한 사용자 로그자인 격 증명 사용을 위해 `--auth-mode login` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1594">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="56085-1595">변경할 수 없는 스토리지 관리를 위한 `storage container immutability-policy/legal-hold` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1595">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1596">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1596">VM</span></span>
* <span data-ttu-id="56085-1597">공개 키 파일이 누락된 경우 `vm create --generate-ssh-keys`가 프라이빗 키 파일을 덮어쓰는 문제 해결(#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="56085-1597">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="56085-1598">`az sig`를 통한 공유 이미지 갤러리에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1598">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="56085-1599">2018년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="56085-1599">August 28, 2018</span></span>

<span data-ttu-id="56085-1600">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="56085-1600">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="56085-1601">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1601">Core</span></span>

* <span data-ttu-id="56085-1602">빈 구성 파일을 로드하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1602">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="56085-1603">Azure Stack에 대해 `2018-03-01-hybrid` 프로필에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1603">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1604">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1604">ACR</span></span>

* <span data-ttu-id="56085-1605">ARM 요청 없이 런타임 작업에 대한 해결 방법 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1605">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="56085-1606">기본적으로 `build` 명령에서 버전 제어 파일 (예:.git,.gitignore)을 업로드된 tar에서 제외하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1606">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1607">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1607">ACS</span></span>

* <span data-ttu-id="56085-1608">`aks create`의 기본값을 `Standard_DS2_v2` VM으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1608">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="56085-1609">이제 새 api를 호출하여 클러스터 자격 증명을 가져오도록 `aks get-credentials` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1609">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1610">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1610">AppService</span></span>

* <span data-ttu-id="56085-1611">Functionapp 및 Webapp에서 CORS 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1611">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="56085-1612">명령 생성에 대한 ARM 태그 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1612">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="56085-1613">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `[webapp|functionapp] identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1613">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="56085-1614">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-1614">Backup</span></span>

* <span data-ttu-id="56085-1615">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `backup vault backup-properties show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1615">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="56085-1616">Bot 서비스</span><span class="sxs-lookup"><span data-stu-id="56085-1616">Bot Service</span></span>

* <span data-ttu-id="56085-1617">초기 Bot Service CLI 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1617">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="56085-1618">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="56085-1618">Cognitive Services</span></span>

* <span data-ttu-id="56085-1619">일부 서비스를 만드는 데 필요한 새 매개 변수 `--api-properties,` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1619">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="56085-1620">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-1620">IoT</span></span>

* <span data-ttu-id="56085-1621">연결된 허브 연관 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1621">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-1622">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-1622">Monitor</span></span>

* <span data-ttu-id="56085-1623">근 실시간 메트릭 경고에 대한 `monitor metrics alert` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1623">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="56085-1624">사용되지 않는 `monitor alert` 명령</span><span class="sxs-lookup"><span data-stu-id="56085-1624">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="56085-1625">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1625">Network</span></span>

* <span data-ttu-id="56085-1626">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `network application-gateway ssl-policy predefined show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1626">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1627">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1627">Resource</span></span>

* <span data-ttu-id="56085-1628">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `provider operation show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1628">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1629">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1629">Storage</span></span>

* <span data-ttu-id="56085-1630">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `storage share policy show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1630">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1631">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1631">VM</span></span>

* <span data-ttu-id="56085-1632">누락된 리소스 발생 시 코드 3을 사용하여 종료하도록 `vm/vmss identity show` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1632">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="56085-1633">`vm create`에 `--storage-caching`이 사용되지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="56085-1633">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="56085-1634">2018년 8월 14일</span><span class="sxs-lookup"><span data-stu-id="56085-1634">Auguest 14, 2018</span></span>

<span data-ttu-id="56085-1635">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="56085-1635">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="56085-1636">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1636">Core</span></span>

* <span data-ttu-id="56085-1637">`table` 출력에 숫자 표시 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1637">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="56085-1638">추가된 YAML 출력 형식</span><span class="sxs-lookup"><span data-stu-id="56085-1638">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="56085-1639">원격 분석</span><span class="sxs-lookup"><span data-stu-id="56085-1639">Telemetry</span></span>

* <span data-ttu-id="56085-1640">향상된 원격 분석 보고</span><span class="sxs-lookup"><span data-stu-id="56085-1640">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1641">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1641">ACR</span></span>

* <span data-ttu-id="56085-1642">`content-trust policy` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1642">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="56085-1643">`.dockerignore`가 제대로 처리되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1643">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1644">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1644">ACS</span></span>

* <span data-ttu-id="56085-1645">Windows에서 `%USERPROFILE%\.azure-kubectl` 하에서 설치하도록 `az acs/aks install-cli` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1645">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="56085-1646">클러스터에 RBAC가 있는지 감지하여 ACI 커넥터를 적절하게 구성하도록 `az aks install-connector` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1646">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="56085-1647">제공되는 서브넷에 대한 역할 할당 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1647">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="56085-1648">서브넷에 대해 제공하는 경우 "역할 할당 건너뛰기" 새 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1648">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="56085-1649">할당이 이미 있는 경우 서브넷으로의 역할 할당을 건너뛸 수 있도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1649">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="56085-1650">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1650">AppService</span></span>

* <span data-ttu-id="56085-1651">외부 리소스 그룹에 스토리지 계정을 사용하여 함수 앱을 만들지 못하도록 하는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1651">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="56085-1652">Zip 배포 충돌을 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1652">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-1653">BatchAI</span><span class="sxs-lookup"><span data-stu-id="56085-1653">BatchAI</span></span>

* <span data-ttu-id="56085-1654">자동 스토리지 계정 만들기가 &quot;리소스 *그룹*&quot;을 지정하도록 로거 출력 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1654">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="56085-1655">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1655">Container</span></span>

* <span data-ttu-id="56085-1656">보안 환경 변수 전달을 위해 컨테이너에 `--secure-environment-variables` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1656">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="56085-1657">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-1657">IoT</span></span>

* <span data-ttu-id="56085-1658">[주요 변경 사항] 사용되지 않는 명령을 제거하여 iot 확장으로 이동</span><span class="sxs-lookup"><span data-stu-id="56085-1658">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="56085-1659">`azure-devices.net` 도메인을 가정하지 않도록 요소를 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1659">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="56085-1660">Iot Central</span><span class="sxs-lookup"><span data-stu-id="56085-1660">Iot Central</span></span>

* <span data-ttu-id="56085-1661">IoT Central 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1661">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-1662">KeyVault</span><span class="sxs-lookup"><span data-stu-id="56085-1662">KeyVault</span></span>


* <span data-ttu-id="56085-1663">스토리지 계정 및 sas 정의를 관리하는 것에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1663">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="56085-1664">네트워크 규칙에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1664">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="56085-1665">비밀, 키 및 인증서 작업에 `--id` 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1665">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="56085-1666">KV mgmt 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1666">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="56085-1667">KV 데이터 평면 다중 api 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1667">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="56085-1668">릴레이</span><span class="sxs-lookup"><span data-stu-id="56085-1668">Relay</span></span>

* <span data-ttu-id="56085-1669">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1669">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1670">Sql</span><span class="sxs-lookup"><span data-stu-id="56085-1670">Sql</span></span>

* <span data-ttu-id="56085-1671">`sql failover-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1671">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1672">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1672">Storage</span></span>

* <span data-ttu-id="56085-1673">[주요 변경 사항]`--location` 매개 변수를 요구하도록 `storage account show-usage`를 변경하여 지역에 따라 나열됨</span><span class="sxs-lookup"><span data-stu-id="56085-1673">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="56085-1674">`--resource-group` 매개 변수가 `storage account` 명령에 대해 선택 사항이 되도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1674">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="56085-1675">단일 집계된 메시지에 대한 일괄 처리 명령에서 개별 오류에 대한 '전제 조건 실패’ 경고를 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1675">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="56085-1676">`[blob|file] delete-batch` 명령을 변경하여 더 이상 null 배열을 출력하지 않도록 함</span><span class="sxs-lookup"><span data-stu-id="56085-1676">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="56085-1677">컨테이너 url에서 sas 토큰을 읽도록 `blob [download|upload|delete-batch]` 명령 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1677">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1678">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1678">VM</span></span>

* <span data-ttu-id="56085-1679">사용 편의성을 위해 일반 필터를 `vm list-skus`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1679">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="56085-1680">2018년 7월 31일</span><span class="sxs-lookup"><span data-stu-id="56085-1680">July 31, 2018</span></span>

<span data-ttu-id="56085-1681">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="56085-1681">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1682">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1682">ACR</span></span>

* <span data-ttu-id="56085-1683">`--with-secure-properties` 플래그를 `acr build-task show` 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1683">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="56085-1684">`acr build-task update-build` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1684">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1685">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1685">ACS</span></span>

* <span data-ttu-id="56085-1686">`az aks browse`를 종료할 때 [Ctrl + C]를 눌러 return 0(성공)을 반환하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1686">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1687">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1687">Batch</span></span>

* <span data-ttu-id="56085-1688">cloudshell에서 AAD 토큰을 보여줄 때의 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1688">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="56085-1689">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1689">Container</span></span>

* <span data-ttu-id="56085-1690">집합 구독에서 이름 또는ID에 대한 `--log-analytics-workspace-key` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-1690">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="56085-1691">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1691">Network</span></span>

* <span data-ttu-id="56085-1692">Azure Stack에 대해 2017-03-09-profile에 dns 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1692">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="56085-1693">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1693">Resource</span></span>

* <span data-ttu-id="56085-1694">`group deployment create`에 `--rollback-on-error`를 추가하여 오류 시 성공한 배포를 실행하도록 함</span><span class="sxs-lookup"><span data-stu-id="56085-1694">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="56085-1695">`group deployment create`를 사용하여 `--parameters {}`에서 오류가 발생하는 문제를 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1695">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="56085-1696">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1696">Role</span></span>

* <span data-ttu-id="56085-1697">스택 프로필 2017-03-09-profile에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1697">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="56085-1698">`app update`에 다한 제네릭 업데이트 매개 변수가 올바르게 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1698">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="56085-1699">검색</span><span class="sxs-lookup"><span data-stu-id="56085-1699">Search</span></span>

* <span data-ttu-id="56085-1700">Azure Search 서비스에 대한 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1700">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="56085-1701">Service Bus</span><span class="sxs-lookup"><span data-stu-id="56085-1701">Service Bus</span></span>

* <span data-ttu-id="56085-1702">Service Bus 표준에서 프리미엄으로 네임 스페이스를 마이그레이션하는 추가 마이그레이션 명령 그룹이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1702">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="56085-1703">Service Bus 큐 및 구독에 새로운 선택적 속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1703">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="56085-1704">`queue` 내 `--enable-batched-operations` 및 `--enable-dead-lettering-on-message-expiration`</span><span class="sxs-lookup"><span data-stu-id="56085-1704">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="56085-1705">`subscriptions` 내 `--dead-letter-on-filter-exceptions`</span><span class="sxs-lookup"><span data-stu-id="56085-1705">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1706">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1706">Storage</span></span>

* <span data-ttu-id="56085-1707">단일 연결을 사용하는 대용량 파일 다운로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1707">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="56085-1708">리소스 누락으로 종료 코드 3으로 실패할 때 누락되었던 `show` 명령 변환</span><span class="sxs-lookup"><span data-stu-id="56085-1708">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1709">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1709">VM</span></span>

* <span data-ttu-id="56085-1710">구독 별로 가용성 집합을 리스팅하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1710">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="56085-1711">`StandardSSD_LRS`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1711">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="56085-1712">VM 확장 집합 생성 시 애플리케이션 보안 그룹에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1712">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="56085-1713">[주요 변경 사항]`[vm|vmss] create`, `[vm|vmss] identity assign`, 및 `[vm|vmss] identity remove`를 사전 형식으로 사용자 할당 ID를 출력하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1713">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="56085-1714">2018년 7월 18일</span><span class="sxs-lookup"><span data-stu-id="56085-1714">July 18, 2018</span></span>

<span data-ttu-id="56085-1715">버전 2.0.42</span><span class="sxs-lookup"><span data-stu-id="56085-1715">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="56085-1716">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1716">Core</span></span>

* <span data-ttu-id="56085-1717">WSL bash 창에서 브라우저 기반 로그인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1717">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="56085-1718">모든 일반 업데이트 명령에 `--force-string` 플래그 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1718">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="56085-1719">[주요 변경 사항] '표시' 명령이 리소스 누락 시 오류 메시지를 기록하고 종료 코드 3과 함께 실패하도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1719">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1720">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1720">ACR</span></span>

* <span data-ttu-id="56085-1721">[주요 변경 사항] '--no-push'를 'acr 빌드' 명령에서 순수 플래그로 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1721">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="56085-1722">`show` 및 `update` 명령이 `acr repository` 그룹 아래 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1722">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="56085-1723">세부 정보를 표시 하기 위해 `--detail` 플래그를 `show-manifests` 및 `show-tags`에 대해 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1723">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="56085-1724">`--image` 매개 변수를 이미지로 빌드 세부 사항이나 로그를 얻을 수 있도록 지원하기 위해 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1724">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1725">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1725">ACS</span></span>

* <span data-ttu-id="56085-1726">`--max-pods`가 5보다 작은 경우 오류가 발생하도록 `az aks create`을 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1726">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1727">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1727">AppService</span></span>

* <span data-ttu-id="56085-1728">PremiumV2 sku에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1728">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1729">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1729">Batch</span></span>

* <span data-ttu-id="56085-1730">클라우드 셸 모드에서 토큰 자격 증명을 사용할 때의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1730">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="56085-1731">JSON 입력을 대/소문자를 구분하지 않도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1731">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="56085-1732">Batch AI</span><span class="sxs-lookup"><span data-stu-id="56085-1732">Batch AI</span></span>

* <span data-ttu-id="56085-1733">`az batchai job exec` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1733">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="56085-1734">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1734">Container</span></span>

* <span data-ttu-id="56085-1735">비 dockerhub 레지스트리의 사용자 이름 및 암호에 대한 요구 사항을 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1735">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="56085-1736">yaml 파일에서 컨테이너 그룹을 만들 때 발생하는 오류 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1736">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="56085-1737">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1737">Network</span></span>

* <span data-ttu-id="56085-1738">`network nic [create|update|delete]`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1738">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="56085-1739">`network nic wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1739">Added `network nic wait`</span></span>
* <span data-ttu-id="56085-1740">`network vnet [subnet|peering] list`에 대한 `--ids` 인수가 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1740">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="56085-1741">`network nsg rule list` 출력의 기본 보안 규칙을 포함하도록 `--include-default` 플래그를 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1741">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="56085-1742">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1742">Resource</span></span>

* <span data-ttu-id="56085-1743">`group deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1743">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="56085-1744">`deployment delete`에 `--no-wait` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1744">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="56085-1745">`deployment wait` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1745">Added `deployment wait` command</span></span>
* <span data-ttu-id="56085-1746">구독 수준 `az deployment` 명령이 프로필 2017-03-09-profile에 잘못 표시되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1746">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1747">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1747">SQL</span></span>

* <span data-ttu-id="56085-1748">`sql db copy` 및 `sql db replica create` 명령에 탄력적 풀 이름을 지정할 때 ‘제공된 리소스 그룹의 이름이 ... URL 내의 이름과 일치하지 않습니다’ 오류가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1748">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="56085-1749">`az configure --defaults sql-server=<name>`를 실행하여 기본 SQL Server 구성 허용</span><span class="sxs-lookup"><span data-stu-id="56085-1749">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="56085-1750">`sql server`, `sql server firewall-rule`, `sql list-usages`, `sql show-usage` 명령에 테이블 포맷터를 구현함</span><span class="sxs-lookup"><span data-stu-id="56085-1750">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1751">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1751">Storage</span></span>

* <span data-ttu-id="56085-1752">페이지 Blob에 대해 채워질 `storage blob show` 출력에 `pageRanges` 속성을 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1752">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1753">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1753">VM</span></span>

* <span data-ttu-id="56085-1754">[주요 변경 사항]`vmss create`가 `Standard_DS1_v2`를 기본 인스턴스 크기로 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1754">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="56085-1755">`vm extension [set|delete]` 및 `vmss extension [set|delete]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1755">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="56085-1756">`vm extension wait`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1756">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="56085-1757">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="56085-1757">July 3, 2018</span></span>

<span data-ttu-id="56085-1758">버전 2.0.41</span><span class="sxs-lookup"><span data-stu-id="56085-1758">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="56085-1759">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-1759">AKS</span></span>

* <span data-ttu-id="56085-1760">구독 ID를 사용하도록 모니터링 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1760">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="56085-1761">2018년 7월 3일</span><span class="sxs-lookup"><span data-stu-id="56085-1761">July 3, 2018</span></span>

<span data-ttu-id="56085-1762">버전 2.0.40</span><span class="sxs-lookup"><span data-stu-id="56085-1762">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="56085-1763">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1763">Core</span></span>

* <span data-ttu-id="56085-1764">대화형 로그인에 대한 새 권한 부여 코드 흐름을 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1764">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1765">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1765">ACR</span></span>

* <span data-ttu-id="56085-1766">빌드 상태 폴링 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1766">Added polling build status</span></span>
* <span data-ttu-id="56085-1767">대/소문자 열거형 값에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1767">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="56085-1768">`show-manifests`에 `--top` 및 `--orderby` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1768">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1769">ACS</span></span>

* <span data-ttu-id="56085-1770">[주요 변경 사항]Kubernetes 역할 기반 액세스 제어를 기본값으로 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1770">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="56085-1771">`--disable-rbac` 인수를 추가 그리고 `--enable-rbac`가 기본값이므로 이제 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-1771">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="56085-1772">`aks browse` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="56085-1772">Updated options for `aks browse` command.</span></span> <span data-ttu-id="56085-1773">`--listen-port` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1773">Added `--listen-port` support</span></span>
* <span data-ttu-id="56085-1774">`aks install-connector` 명령에 대한 기본 helm 차트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1774">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="56085-1775">virtual-kubelet-for-aks-latest.tgz 사용</span><span class="sxs-lookup"><span data-stu-id="56085-1775">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="56085-1776">기존 클러스터 업데이트에 `aks enable-addons`과 `aks disable-addons` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1776">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1777">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1777">AppService</span></span>

* <span data-ttu-id="56085-1778">`webapp identity remove`를 통해 ID를 사용하지 않도록 하는 것에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1778">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="56085-1779">`preview` 태그의 ID 기능 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1779">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="56085-1780">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-1780">Backup</span></span>

* <span data-ttu-id="56085-1781">모듈 정의 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1781">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-1782">BatchAI</span><span class="sxs-lookup"><span data-stu-id="56085-1782">BatchAI</span></span>

* <span data-ttu-id="56085-1783">`batchai cluster node list`, `batchai job node list` 명령에 대한 테이블 출력이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1783">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="56085-1784">클라우드</span><span class="sxs-lookup"><span data-stu-id="56085-1784">Cloud</span></span>

* <span data-ttu-id="56085-1785">`acr login` 서버 접미사를 클라우드 구성에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1785">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="56085-1786">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1786">Container</span></span>

* <span data-ttu-id="56085-1787">`container create`의 기본값을 장기 실행 작업으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1787">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="56085-1788">Log Analytics 매개 변수를 `--log-analytics-workspace` 및 `--log-analytics-workspace-key`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1788">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="56085-1789">`--protocol` 매개 변수를 사용할 네트워크 프로토콜을 지정하도록 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1789">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="56085-1790">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-1790">Extension</span></span>

* <span data-ttu-id="56085-1791">CLI 버전과 호환되는 확장명만 표시하도록 `extension list-available` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1791">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="56085-1792">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1792">Network</span></span>

* <span data-ttu-id="56085-1793">레코드 형식이 대/소문자를 구분하는 문제 수정([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="56085-1793">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-1794">Rdbms</span><span class="sxs-lookup"><span data-stu-id="56085-1794">Rdbms</span></span>

* <span data-ttu-id="56085-1795">`[postgres|myql] server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1795">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="56085-1796">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-1796">Resource</span></span>

* <span data-ttu-id="56085-1797">새 작업 그룹 `deployment` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1797">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1798">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1798">VM</span></span>

* <span data-ttu-id="56085-1799">시스템 할당 ID를 제거하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1799">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="56085-1800">2018년 6월 25일</span><span class="sxs-lookup"><span data-stu-id="56085-1800">June 25, 2018</span></span>

<span data-ttu-id="56085-1801">버전 2.0.39</span><span class="sxs-lookup"><span data-stu-id="56085-1801">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="56085-1802">CLI</span><span class="sxs-lookup"><span data-stu-id="56085-1802">CLI</span></span>

* <span data-ttu-id="56085-1803">확장 설치 문제를 해결하기 위해 MSI 설치 관리자에서 파일 잘라내기 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1803">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="56085-1804">2018년 6월 19일</span><span class="sxs-lookup"><span data-stu-id="56085-1804">June 19, 2018</span></span>

<span data-ttu-id="56085-1805">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="56085-1805">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="56085-1806">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1806">Core</span></span>

* <span data-ttu-id="56085-1807">대부분의 명령으로 `--subscription`에 대한 전역 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1807">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1808">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1808">ACR</span></span>

* <span data-ttu-id="56085-1809">`azure-storage-blob`이 종속성으로 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1809">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="56085-1810">`acr build-task create`가 코어 2개를 사용하도록 기본 CPU 구성이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1810">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1811">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1811">ACS</span></span>

* <span data-ttu-id="56085-1812">`aks use-dev-spaces` 명령 옵션이 업데이트됨.</span><span class="sxs-lookup"><span data-stu-id="56085-1812">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="56085-1813">`--update` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1813">Added `--update` support</span></span>
* <span data-ttu-id="56085-1814">`$HOME/.kube/config` 안의 사용자 컨텍스트를 대체하지 않도록 `aks get-credentials --admin` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1814">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="56085-1815">읽기 전용 `nodeResourceGroup` 속성을 관리되는 클러스터에서 공개</span><span class="sxs-lookup"><span data-stu-id="56085-1815">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="56085-1816">`acs browse` 명령 오류 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1816">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="56085-1817">`aks install-connector`, `aks upgrade-connector` 및 `aks remove-connector`에 대해 `--connector-name`을 옵션으로 설정</span><span class="sxs-lookup"><span data-stu-id="56085-1817">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="56085-1818">`aks install-connector`에 대해 새 Azure 컨테이너 인스턴스 영역 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1818">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="56085-1819">helm 릴리스 이름과 `aks install-connector` 노드 이름에 정규화된 위치 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1819">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1820">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1820">AppService</span></span>

* <span data-ttu-id="56085-1821">Urllib의 최신 버전에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1821">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="56085-1822">`functionapp create`가 외부 리소스 그룹 제공 앱 서비스 계획을 사용하도록 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1822">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1823">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1823">Batch</span></span>

* <span data-ttu-id="56085-1824">`azure-batch-extensions` 종속성 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1824">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="56085-1825">Batch AI</span><span class="sxs-lookup"><span data-stu-id="56085-1825">Batch AI</span></span>

* <span data-ttu-id="56085-1826">작업 영역에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="56085-1826">Added support for workspaces.</span></span> <span data-ttu-id="56085-1827">그룹 클러스터, 파일 서버 및 그룹 내 실험에 작업 영역 허용, 리소스의 수에 대한 제한을 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1827">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="56085-1828">실험에 대한 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="56085-1828">Added support for experiments.</span></span> <span data-ttu-id="56085-1829">실험을 컬렉션의 그룹 작업에 허용, 생성된 작업의 수에 대한 제한 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1829">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="56085-1830">Docker 컨테이너에서 실행 중인 작업에 대해 `/dev/shm`을 구성하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1830">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="56085-1831">`batchai cluster node exec` 및 `batchai job node exec` 명령이 추가됨.</span><span class="sxs-lookup"><span data-stu-id="56085-1831">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="56085-1832">이 명령은 노드에서 직접 모든 명령을 실행하도록 허용하고 포트 포워드를 위한 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1832">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="56085-1833">`--ids`에 대한 지원이 `batchai` 명령에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1833">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="56085-1834">[주요 변경 사항] 모든 클러스터 및 파일 서버는 작업 영역에서 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="56085-1834">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="56085-1835">[주요 변경 사항] 실험 아래에 작업을 만들어야 합니다</span><span class="sxs-lookup"><span data-stu-id="56085-1835">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="56085-1836">[주요 변경 사항]`cluster create`, `job create` 명령에서 `--nfs-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="56085-1836">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="56085-1837">다른 작업 영역/리소스 그룹에 속한 NFS를 탑재하려면 `--nfs` 옵션을 통해 파일 서버의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="56085-1837">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="56085-1838">[주요 변경 사항]`job create` 명령에서 `--cluster-resource-group`제거.</span><span class="sxs-lookup"><span data-stu-id="56085-1838">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="56085-1839">다른 작업 영역/리소스 그룹에 속한 클러스터 상의 작업을 제출하려면 `--cluster` 옵션을 통해 클러스터의 ARM ID를 제공</span><span class="sxs-lookup"><span data-stu-id="56085-1839">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="56085-1840">[주요 변경 사항]`location` 특성을 작업, 클러스터 및 파일 서버에서 제거.</span><span class="sxs-lookup"><span data-stu-id="56085-1840">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="56085-1841">이제 이 위치는 작업 영역의 특성입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1841">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="56085-1842">[주요 변경 사항]`job create`, `cluster create`, `file-server create` 명령에서 `--location`제거</span><span class="sxs-lookup"><span data-stu-id="56085-1842">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="56085-1843">[주요 변경 사항] 보다 일관된 인터페이스를 위해 간단한 옵션의 이름을 변경:</span><span class="sxs-lookup"><span data-stu-id="56085-1843">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="56085-1844">[`--config`, `-c`]을 [`--config-file`, `-f`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="56085-1844">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="56085-1845">[`--cluster`, `-r`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="56085-1845">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="56085-1846">[`--cluster`, `-n`]을 [`--cluster`, `-c`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="56085-1846">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="56085-1847">[`--job`, `-n`]을 [`--job`, `-j`]로 이름 바꿈</span><span class="sxs-lookup"><span data-stu-id="56085-1847">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="56085-1848">지도</span><span class="sxs-lookup"><span data-stu-id="56085-1848">Maps</span></span>

* <span data-ttu-id="56085-1849">[주요 변경 사항] 대화형 프롬프트 또는 `--accept-tos` 플래그로 서비스 약관을 수락하도록 `maps account create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1849">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="56085-1850">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1850">Network</span></span>

* <span data-ttu-id="56085-1851">`network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)에 `https` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1851">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="56085-1852">`--endpoint-status`가 대/소문자를 구분하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1852">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="56085-1853">#6502</span><span class="sxs-lookup"><span data-stu-id="56085-1853">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="56085-1854">예약</span><span class="sxs-lookup"><span data-stu-id="56085-1854">Reservations</span></span>

* <span data-ttu-id="56085-1855">[주요 변경 사항] 필수 매개 변수 `ReservedResourceType`을 `reservations catalog show`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1855">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="56085-1856">`Location` 매개 변수가 `reservations catalog show`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1856">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="56085-1857">[주요 변경 사항]`ReservationProperties`에서 `kind`제거</span><span class="sxs-lookup"><span data-stu-id="56085-1857">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="56085-1858">[주요 변경 사항]`Catalog` 내에서 `capabilities`에서 `sku_properties`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-1858">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="56085-1859">[주요 변경 사항]`Catalog`에서 `size`, `tier` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1859">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="56085-1860">`InstanceFlexibility` 매개 변수가 `reservations reservation update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1860">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="56085-1861">역할</span><span class="sxs-lookup"><span data-stu-id="56085-1861">Role</span></span>

* <span data-ttu-id="56085-1862">오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="56085-1862">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1863">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1863">SQL</span></span>

* <span data-ttu-id="56085-1864">구독에 사용할 수 없는 위치에 대해 `az sql db list-editions` 실행 시 발생하는 혼란스러운 오류 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1864">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1865">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1865">Storage</span></span>

* <span data-ttu-id="56085-1866">`storage blob download`에 대한 출력 테이블을 가독성을 높이도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1866">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1867">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1867">VM</span></span>

* <span data-ttu-id="56085-1868">`vm create` 내 네트워킹 지원 가속화에 대한 구체화 vm 크기 확인 향상</span><span class="sxs-lookup"><span data-stu-id="56085-1868">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="56085-1869">기본 vm 크기가 `Standard_D1_v2`에서 `Standard_DS1_v2`로 전환된다는, `vmss create`에 대한 경고 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1869">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="56085-1870">구성이 변경되지 않은 경우에도 확장을 업데이트하도록 `--force-update`를 `[vm|vmss] extension set`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1870">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="56085-1871">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-1871">June 13, 2018</span></span>

<span data-ttu-id="56085-1872">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="56085-1872">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="56085-1873">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1873">Core</span></span>

* <span data-ttu-id="56085-1874">개선된 대화형 원격 분석</span><span class="sxs-lookup"><span data-stu-id="56085-1874">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="56085-1875">2018년 6월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-1875">June 13, 2018</span></span>

<span data-ttu-id="56085-1876">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="56085-1876">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="56085-1877">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-1877">AKS</span></span>

* <span data-ttu-id="56085-1878">고급 네트워킹 옵션이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1878">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="56085-1879">인수를  `aks create`에 추가하여 모니터링 및 HTTP 라우팅을 활성화</span><span class="sxs-lookup"><span data-stu-id="56085-1879">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="56085-1880">`--no-ssh-key` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1880">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="56085-1881">`--enable-rbac` 인수를 `aks create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1881">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="56085-1882">[미리 보기] Azure Active Directory 인증에 대한 지원이 `aks create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1882">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1883">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1883">AppService</span></span>

* <span data-ttu-id="56085-1884">호환되지 않는 urllib 버전 관련 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1884">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="56085-1885">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="56085-1885">June 5, 2018</span></span>

<span data-ttu-id="56085-1886">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="56085-1886">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-1887">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-1887">Interactive</span></span>

* <span data-ttu-id="56085-1888">대화형 모드의 종속성에 제한 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1888">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="56085-1889">2018년 6월 5일</span><span class="sxs-lookup"><span data-stu-id="56085-1889">June 5, 2018</span></span>

<span data-ttu-id="56085-1890">버전 2.0.34</span><span class="sxs-lookup"><span data-stu-id="56085-1890">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="56085-1891">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1891">Core</span></span>

* <span data-ttu-id="56085-1892">상호 테넌트 리소스 참조에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1892">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="56085-1893">원격 분석 업로드 신뢰성이 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-1893">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1894">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1894">ACR</span></span>

* <span data-ttu-id="56085-1895">원격 원본 위치로 VSTS 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1895">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="56085-1896">`acr import` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1896">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="56085-1897">AKS</span><span class="sxs-lookup"><span data-stu-id="56085-1897">AKS</span></span>

* <span data-ttu-id="56085-1898">보다 안전한 파일 시스템 권한으로 kube 구성 파일을 만들기 위해 `aks get-credentials`변경함</span><span class="sxs-lookup"><span data-stu-id="56085-1898">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="56085-1899">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-1899">Batch</span></span>

* <span data-ttu-id="56085-1900">풀 목록 표 서식수정 버그가 수정됨 [[문제 #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="56085-1900">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="56085-1901">IOT</span><span class="sxs-lookup"><span data-stu-id="56085-1901">IOT</span></span>

* <span data-ttu-id="56085-1902">기본 계층 IoT Hub 생성을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1902">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="56085-1903">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1903">Network</span></span>

* <span data-ttu-id="56085-1904">향상됨 `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="56085-1904">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="56085-1905">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="56085-1905">Policy Insights</span></span>

* <span data-ttu-id="56085-1906">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-1906">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="56085-1907">ARM</span><span class="sxs-lookup"><span data-stu-id="56085-1907">ARM</span></span>

* <span data-ttu-id="56085-1908">`account management-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1908">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1909">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1909">SQL</span></span>

* <span data-ttu-id="56085-1910">새로운 추가된 관리되는 인스턴스 명령:</span><span class="sxs-lookup"><span data-stu-id="56085-1910">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="56085-1911">관리형 새 데이터베이스 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1911">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="56085-1912">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1912">Storage</span></span>

* <span data-ttu-id="56085-1913">파일 확장명에서 유추할 수 있도록 json 및 javascript를 추가 mimetypes으로 추가함</span><span class="sxs-lookup"><span data-stu-id="56085-1913">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1914">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1914">VM</span></span>

* <span data-ttu-id="56085-1915">열을 고정시켜 사용하고 `Tier` 및 `Size`가 제거될 예정이라는 경고를 추가하도록 `vm list-skus` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1915">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="56085-1916">`--accelerated-networking` 옵션을 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1916">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="56085-1917">`identity create`에 `--tags` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1917">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="56085-1918">2018년 5월 22일</span><span class="sxs-lookup"><span data-stu-id="56085-1918">May 22, 2018</span></span>

<span data-ttu-id="56085-1919">버전 2.0.33</span><span class="sxs-lookup"><span data-stu-id="56085-1919">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="56085-1920">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1920">Core</span></span>

* <span data-ttu-id="56085-1921">파일 이름에 `@` 확장을 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1921">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1922">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1922">ACS</span></span>

* <span data-ttu-id="56085-1923">새 Dev-Space 명령 `aks use-dev-spaces` 및 `aks remove-dev-spaces` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1923">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="56085-1924">도움말 메시지 내 오류 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1924">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1925">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-1925">AppService</span></span>

* <span data-ttu-id="56085-1926">일반 업데이트 명령이 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-1926">Improved generic update commands</span></span>
* <span data-ttu-id="56085-1927">`webapp deployment source config-zip`에 대한 비동기 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1927">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="56085-1928">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-1928">Container</span></span>

* <span data-ttu-id="56085-1929">컨테이너 그룹을 yaml 형식으로 내보내기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1929">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="56085-1930">Yaml 파일을 사용하여 컨테이너 그룹 만들기 / 업데이트하기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1930">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="56085-1931">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-1931">Extension</span></span>

* <span data-ttu-id="56085-1932">확장 제거가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-1932">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-1933">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-1933">Interactive</span></span>

* <span data-ttu-id="56085-1934">완료 시 파서를 음소거하도록 로깅을 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-1934">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="56085-1935">잘못된 도움말 캐시의 처리가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-1935">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-1936">KeyVault</span><span class="sxs-lookup"><span data-stu-id="56085-1936">KeyVault</span></span>

* <span data-ttu-id="56085-1937">클라우드 셸 또는 id를 가진 Vm에서 실행 하도록 keyvault 명령을 수정함</span><span class="sxs-lookup"><span data-stu-id="56085-1937">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="56085-1938">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-1938">Network</span></span>

* <span data-ttu-id="56085-1939">`network watcher show-topology`이 vnet 및/또는 서브넷 이름[#6326](https://github.com/Azure/azure-cli/issues/6326)으로 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1939">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="56085-1940">`network watcher` 명령 결과 실제로 [#6264](https://github.com/Azure/azure-cli/issues/6264)인 영역에 대해 Network Watcher가 사용 가능하지 않다는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-1940">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="56085-1941">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-1941">SQL</span></span>

* <span data-ttu-id="56085-1942">[주요 변경 사항]`db` 및 `dw` 명령으로 리턴되는 응답 개체 변경 :</span><span class="sxs-lookup"><span data-stu-id="56085-1942">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="56085-1943">`serviceLevelObjective` 속성을 `currentServiceObjectiveName`로 이름을 바꿈</span><span class="sxs-lookup"><span data-stu-id="56085-1943">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="56085-1944">`currentServiceObjectiveId` 및 `requestedServiceObjectiveId` 속성 제거</span><span class="sxs-lookup"><span data-stu-id="56085-1944">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="56085-1945">`maxSizeBytes` 속성을 문자열 대신 정수값으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1945">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="56085-1946">[주요 변경 사항]`db` 및 `dw`를 읽기 전용 속성으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1946">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="56085-1947">`requestedServiceObjectiveName`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1947">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="56085-1948">업데이트하려면, `--service-objective` 매개 변수를 사용하거나 `sku.name` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="56085-1948">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="56085-1949">`edition`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1949">`edition`.</span></span> <span data-ttu-id="56085-1950">업데이트하려면, `--edition` 매개 변수를 사용하거나 `sku.tier` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="56085-1950">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="56085-1951">`elasticPoolName`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1951">`elasticPoolName`.</span></span> <span data-ttu-id="56085-1952">업데이트하려면, `--elastic-pool` 매개 변수를 사용하거나 `elasticPoolId` 속성 설정</span><span class="sxs-lookup"><span data-stu-id="56085-1952">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="56085-1953">[주요 변경 사항] 다음 `elastic-pool` 속성을 읽기 전용으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-1953">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="56085-1954">`edition`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1954">`edition`.</span></span> <span data-ttu-id="56085-1955">업데이트하려면 `--edition` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="56085-1955">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="56085-1956">`dtu`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1956">`dtu`.</span></span> <span data-ttu-id="56085-1957">업데이트하려면 `--capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="56085-1957">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="56085-1958">`databaseDtuMin`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1958">`databaseDtuMin`.</span></span> <span data-ttu-id="56085-1959">업데이트하려면 `--db-min-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="56085-1959">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="56085-1960">`databaseDtuMax`입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1960">`databaseDtuMax`.</span></span> <span data-ttu-id="56085-1961">업데이트하려면 `--db-max-capacity` 매개 변수를 사용</span><span class="sxs-lookup"><span data-stu-id="56085-1961">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="56085-1962">`db`,`dw`,`elastic-pool` 명령에 `--family`, `--capacity` 매개 변수 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1962">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="56085-1963">`elastic-pool` 명령에 `db`, `dw` 테이블 포맷터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-1963">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="56085-1964">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-1964">Storage</span></span>

* <span data-ttu-id="56085-1965">`--account-name` 인수에 완료자 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1965">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="56085-1966">`storage entity query`의 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1966">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-1967">VM</span><span class="sxs-lookup"><span data-stu-id="56085-1967">VM</span></span>

* <span data-ttu-id="56085-1968">[주요 변경 사항]`vm create`에서 `--write-accelerator`제거됨.</span><span class="sxs-lookup"><span data-stu-id="56085-1968">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="56085-1969">동일한 지원을 `vm update` 또는 `vm disk attach`를 통해 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-1969">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="56085-1970">`[vm|vmss] extension`에서 일치하는 확장 이미지 수정</span><span class="sxs-lookup"><span data-stu-id="56085-1970">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="56085-1971">부팅 로그를 캡처하기 위해 `vm create`에 `--boot-diagnostics-storage` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1971">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="56085-1972">`[vm|vmss] update`에 `--license-type` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-1972">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="56085-1973">2018년 5월 7일</span><span class="sxs-lookup"><span data-stu-id="56085-1973">May 7, 2018</span></span>

<span data-ttu-id="56085-1974">버전 2.0.32</span><span class="sxs-lookup"><span data-stu-id="56085-1974">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="56085-1975">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-1975">Core</span></span>

* <span data-ttu-id="56085-1976">인증서를 사용하여 서비스 사용자 계정에서 비밀을 검색할 때 처리되지 않는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1976">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="56085-1977">위치 인수에 대한 제한된 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1977">Added limited support for positional arguments</span></span>
* <span data-ttu-id="56085-1978">`--query`가 `--ids`와 함께 사용될 수 없는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1978">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="56085-1979">#5591</span><span class="sxs-lookup"><span data-stu-id="56085-1979">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="56085-1980">`--ids`를 사용하는 경우 명령의 파이핑 시나리오가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1980">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="56085-1981">쿼리가 지정된 `-o tsv` 또는 쿼리가 지정되지 않은 `-o json`을 지원</span><span class="sxs-lookup"><span data-stu-id="56085-1981">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="56085-1982">사용자의 명령에 오타가 있는 경우 오류에 대한 명령 제안이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1982">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="56085-1983">사용자가 `az ''`를 입력하는 경우 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1983">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="56085-1984">명령 모듈 및 확장에 대한 사용자 지정 리소스 유형 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1984">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="56085-1985">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-1985">ACR</span></span>

* <span data-ttu-id="56085-1986">ACR Build 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1986">Added ACR Build commands</span></span>
* <span data-ttu-id="56085-1987">리소스를 찾을 수 없음 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1987">Improved resource not found error messages</span></span>
* <span data-ttu-id="56085-1988">리소스 생성 성능 및 오류 처리가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1988">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="56085-1989">비표준 콘솔 및 WSL에서 acr 로그인이 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1989">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="56085-1990">리포지토리 명령 오류 메시지가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-1990">Improved repository commands error messages</span></span>
* <span data-ttu-id="56085-1991">테이블 열 및 순서 지정 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-1991">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="56085-1992">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-1992">ACS</span></span>

* <span data-ttu-id="56085-1993">`az aks`가 미리 보기 서비스라는 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-1993">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="56085-1994">`--aci-resource-group`이 지정되지 않은 경우 `aks install-connector`의 권한 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-1994">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="56085-1995">AMS</span><span class="sxs-lookup"><span data-stu-id="56085-1995">AMS</span></span>

* <span data-ttu-id="56085-1996">최초 릴리스 - Azure Media Services 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="56085-1996">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-1997">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-1997">Appservice</span></span>

* <span data-ttu-id="56085-1998">`--slot`이 제공되는 경우 `webapp delete` 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-1998">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="56085-1999">`webapp auth update`에서 `--runtime-version`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-1999">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="56085-2000">min\_tls\_version 및 https2.0에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2000">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="56085-2001">멀티 컨테이너 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2001">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="56085-2002">Batch AI</span><span class="sxs-lookup"><span data-stu-id="56085-2002">Batch AI</span></span>

* <span data-ttu-id="56085-2003">클러스터의 구성 파일에 구성된 VM 우선 순위를 존중하도록 `batchai create cluster` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2003">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="56085-2004">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="56085-2004">Cognitive Services</span></span>

* <span data-ttu-id="56085-2005">`cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)에 대한 예제의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2005">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-2006">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-2006">Consumption</span></span>

* <span data-ttu-id="56085-2007">예산 API에 대한 새로운 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2007">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="56085-2008">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2008">Container</span></span>

* <span data-ttu-id="56085-2009">레지스트리 서버가 이미지 이름에 포함될 때 `container create`에 대한 `--registry-server` 요구 사항이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2009">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="56085-2010">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="56085-2010">Cosmos DB</span></span>

* <span data-ttu-id="56085-2011">Azure CLI용 VNET 지원 소개 - Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="56085-2011">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="56085-2012">DMS</span><span class="sxs-lookup"><span data-stu-id="56085-2012">DMS</span></span>

* <span data-ttu-id="56085-2013">최초 릴리스 - Azure SQL 마이그레이션 시나리오에 대한 SQL 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2013">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2014">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2014">Extension</span></span>

* <span data-ttu-id="56085-2015">확장 메타데이터가 표시되지 않는 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2015">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2016">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2016">Interactive</span></span>

* <span data-ttu-id="56085-2017">대화형 completer가 위치 인수로 작동하도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2017">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="56085-2018">사용자가 '\'을 입력하면 사용자 친화적인 출력 표시</span><span class="sxs-lookup"><span data-stu-id="56085-2018">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="56085-2019">도움이 없는 매개 변수 완성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2019">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="56085-2020">명령 그룹에 대한 설명이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2020">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="56085-2021">랩</span><span class="sxs-lookup"><span data-stu-id="56085-2021">Lab</span></span>

* <span data-ttu-id="56085-2022">knack 전환으로부터 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2022">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="56085-2023">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2023">Network</span></span>

* <span data-ttu-id="56085-2024">[주요 변경 사항] 다음 항목에서 `--ids` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2024">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="56085-2025">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2025">Profile</span></span>

* <span data-ttu-id="56085-2026">`disk create` 원본 감지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2026">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="56085-2027">[주요 변경 사항]`--msi-port` 및 `--identity-port`가 더 이상 사용되지 않아서 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2027">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="56085-2028">`account get-access-token` 짧은 요약의 오타가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2028">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="56085-2029">Redis</span><span class="sxs-lookup"><span data-stu-id="56085-2029">Redis</span></span>

* <span data-ttu-id="56085-2030">`redis patch-schedule patch-schedule show`는 사용되지 않고 `redis patch-schedule show`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2030">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="56085-2031">`redis list-all`이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2031">Deprecated `redis list-all`.</span></span> <span data-ttu-id="56085-2032">이 기능은 `redis list`에 포함됨</span><span class="sxs-lookup"><span data-stu-id="56085-2032">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="56085-2033">`redis import-method`는 사용되지 않고 `redis import`가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2033">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="56085-2034">다양한 명령에 `--ids` 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2034">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="56085-2035">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2035">Role</span></span>

* <span data-ttu-id="56085-2036">[주요 변경 사항] 사용되지 않는 `ad sp reset-credentials`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2036">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2037">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2037">Storage</span></span>

* <span data-ttu-id="56085-2038">소스 sas 및 계정 키가 지정되지 않은 경우 Blob 복사본의 소스에 대상 sas-token이 적용되도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2038">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="56085-2039">Blob 업로드 및 다운로드에 대한 --socket-timeout이 노출</span><span class="sxs-lookup"><span data-stu-id="56085-2039">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="56085-2040">경로 구분 기호로 시작하는 BLOB 이름을 상대 경로로 처리</span><span class="sxs-lookup"><span data-stu-id="56085-2040">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="56085-2041">시작 쿼리 문자가 ?인 `storage blob copy --source-sas` 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2041">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="56085-2042">key=values 목록을 수락하도록 `storage entity query --marker`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2042">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2043">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2043">VM</span></span>

* <span data-ttu-id="56085-2044">관리되지 않는 Blob URI에 대한 잘못된 검색 논리가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2044">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="56085-2045">사용자가 제공한 서비스 사용자가 없는 디스크 암호화 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2045">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="56085-2046">[주요 변경 사항] MSI 지원에 VM 'ManagedIdentityExtension' 사용 금지</span><span class="sxs-lookup"><span data-stu-id="56085-2046">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="56085-2047">`vmss`에 대한 제거 정책이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2047">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="56085-2048">[주요 변경 사항] 다음 항목에서 `--ids`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2048">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="56085-2049">Write Accelerator 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2049">Added write accelerator support</span></span>
* <span data-ttu-id="56085-2050">`vmss perform-maintenance`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2050">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="56085-2051">VM의 OS 유형을 안정적으로 감지하도록 `vm diagnostics set`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2051">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="56085-2052">요청된 크기가 현재 설정과 다른지 확인하고 변경 시에만 업데이트하도록 `vm resize` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2052">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="56085-2053">2018년 4월 10일</span><span class="sxs-lookup"><span data-stu-id="56085-2053">April 10, 2018</span></span>

<span data-ttu-id="56085-2054">버전 2.0.31</span><span class="sxs-lookup"><span data-stu-id="56085-2054">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2055">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2055">ACR</span></span>

* <span data-ttu-id="56085-2056">Wincred 대체(fallback)의 향상된 오류 처리</span><span class="sxs-lookup"><span data-stu-id="56085-2056">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2057">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2057">ACS</span></span>

* <span data-ttu-id="56085-2058">SPN이 5년 동안 유효하도록 만든 aks 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2058">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2059">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2059">Appservice</span></span>

* [호환성이 손상되는 변경]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="56085-2061">존재하지 않는 webapp 계획에 대한 확인할 수 없는 예외가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2061">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-2062">BatchAI</span><span class="sxs-lookup"><span data-stu-id="56085-2062">BatchAI</span></span>

* <span data-ttu-id="56085-2063">2018-03-01 API에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2063">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="56085-2064">작업 수준 탑재</span><span class="sxs-lookup"><span data-stu-id="56085-2064">Job level mounting</span></span>
  - <span data-ttu-id="56085-2065">비밀 값을 가진 환경 변수</span><span class="sxs-lookup"><span data-stu-id="56085-2065">Environment variables with secret values</span></span>
  - <span data-ttu-id="56085-2066">성능 카운터 설정</span><span class="sxs-lookup"><span data-stu-id="56085-2066">Performance counters settings</span></span>
  - <span data-ttu-id="56085-2067">작업 특정 직선 세그먼트 보고</span><span class="sxs-lookup"><span data-stu-id="56085-2067">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="56085-2068">목록 파일 api의 하위 폴더 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2068">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="56085-2069">사용 및 제한 보고</span><span class="sxs-lookup"><span data-stu-id="56085-2069">Usage and limits reporting</span></span>
  - <span data-ttu-id="56085-2070">NFS 서버에 대한 캐싱 유형을 지정하도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2070">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="56085-2071">사용자 지정 이미지 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2071">Support for custom images</span></span>
  - <span data-ttu-id="56085-2072">pyTorch 툴킷 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2072">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="56085-2073">작업 완료를 기다리고 작업 종료 코드를 보고할 수 있도록 하는 `job wait` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2073">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="56085-2074">현재 Batch AI 리소스 사용을 나열하고 서로 다른 지역에 대해 제한하는 `usage show` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2074">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="56085-2075">국가별 클라우드가 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2075">National clouds are supported</span></span>
* <span data-ttu-id="56085-2076">구성 파일 외에도 파일 시스템을 작업 수준에 탑재하기 위한 작업 명령줄 인수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2076">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="56085-2077">클러스터를 사용자 지정하는 더 많은 옵션 추가 - vm 우선 순위, 서브넷, 자동 크기 조정 클러스터에 대한 초기 노드 수, 사용자 지정 이미지 지정</span><span class="sxs-lookup"><span data-stu-id="56085-2077">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="56085-2078">Batch AI 관리 NFS에 대한 캐싱 유형을 지정하는 명령줄 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2078">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="56085-2079">구성 파일에 파일 시스템 탑재를 간소화합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2079">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="56085-2080">이제 Azure File Share 및 Azure Blob Container에 대한 자격 증명을 생략 할 수 있습니다 - CLI는 명령줄 매개 변수를 통해 제공되거나 환경 변수를 통해 지정된 스토리지 계정 키를 사용하여 누락된 자격 증명을 채우거나 Azure Storage에서 키를 쿼리합니다.(스토리지 계정이 현재 구독에 속한 경우)</span><span class="sxs-lookup"><span data-stu-id="56085-2080">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="56085-2081">이제 작업 파일 스트림 명령은 작업이 완료될 때 자동 완료합니다.(성공, 실패, 종료 또는 삭제)</span><span class="sxs-lookup"><span data-stu-id="56085-2081">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="56085-2082">`show` 작업에 대한 `table` 출력이 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2082">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="56085-2083">클러스터 생성을 위해 `--use-auto-storage` 옵션이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2083">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="56085-2084">이 옵션을 사용하면 보다 쉽게 스토리지 계정을 관리하고 Azure File Share 및 Azure Blob Containers를 클러스터에 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2084">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="56085-2085">`--generate-ssh-keys` 옵션을 `cluster create` 및 `file-server create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2085">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="56085-2086">명령줄을 통해 노드 설정 작업을 제공하는 기능 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2086">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="56085-2087">[주요 변경 사항]`job stream-file` 및 `job list-files` 명령을 `job file`로 이동함</span><span class="sxs-lookup"><span data-stu-id="56085-2087">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="56085-2088">[주요 변경 사항]`cluster create` 명령과 호환되도록 `file-server create` 명령에서 `--admin-user-name`을 `--user-name`로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-2088">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="56085-2089">결제</span><span class="sxs-lookup"><span data-stu-id="56085-2089">Billing</span></span>

* <span data-ttu-id="56085-2090">등록 계정 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2090">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-2091">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-2091">Consumption</span></span>

* <span data-ttu-id="56085-2092">`marketplace` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2092">Added `marketplace` commands</span></span>
* <span data-ttu-id="56085-2093">[주요 변경 사항]`reservations summaries`에서 `reservation summary`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2093">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="56085-2094">[주요 변경 사항]`reservations details`에서 `reservation detail`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2094">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="56085-2095">[주요 변경 사항]`reservation` 명령에 대한 `--reservation-order-id`과 `--reservation-id` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2095">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="56085-2096">[주요 변경 사항]`reservation summary` 명령에 대한 `--grain` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2096">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="56085-2097">[주요 변경 사항]`pricesheet` 명령에 대한 `--include-meter-details` 짧은 옵션이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2097">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="56085-2098">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2098">Container</span></span>

* <span data-ttu-id="56085-2099">Git 리포지토리 볼륨 탑재 매개 변수 `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` 및 `--gitrepo-mount-path` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2099">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="56085-2100">[#5926](https://github.com/Azure/azure-cli/issues/5926) 수정됨: --컨테이너-이름이 지정될 때 `az container exec` 실패</span><span class="sxs-lookup"><span data-stu-id="56085-2100">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2101">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2101">Extension</span></span>

* <span data-ttu-id="56085-2102">배포 확인 메시지를 디버그 수준으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2102">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2103">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2103">Interactive</span></span>

* <span data-ttu-id="56085-2104">인식할 수 없는 명령이 있으면 완료를 중지하도록 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-2104">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="56085-2105">명령 하위 트리를 만들기 전과 후에 이벤트 후크 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2105">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="56085-2106">`--ids` 매개 변수에 대한 완료 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2106">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="56085-2107">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2107">Network</span></span>

* <span data-ttu-id="56085-2108">[#5936](https://github.com/Azure/azure-cli/issues/5936) 수정됨: `application-gateway create` 태그는 bet 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2108">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="56085-2109">`application-gateway http-settings [create|update]`에 대한 인증 인증서를 첨부하기 위해 인수 `--auth-certs`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2109">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="56085-2110">#4910</span><span class="sxs-lookup"><span data-stu-id="56085-2110">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="56085-2111">DDoS 보호 계획을 만들기 위해 `ddos-protection` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2111">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="56085-2112">VNet을 DDoS 보호 계획에 연결하기 위해 `--ddos-protection-plan`에 대한 지원을 `vnet [create|update]`에 추가함</span><span class="sxs-lookup"><span data-stu-id="56085-2112">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="56085-2113">`network route-table [create|update]`에서 `--disable-bgp-route-propagation` 플래그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2113">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="56085-2114">`network lb [create|update]`에 대해 더미 인수 `--public-ip-address-type` 및 `--subnet-type`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2114">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="56085-2115">`network dns zone [import|export]` 및 `network dns record-set txt add-record`에 대한 RFC 1035 이스케이프 시퀀스를 가진 TXT 레코드에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2115">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2116">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2116">Profile</span></span>

* <span data-ttu-id="56085-2117">`account list`에 있는 Azure Classic 계정에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2117">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="56085-2118">[주요 변경 사항]`--msi` & `--msi-port` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2118">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-2119">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-2119">RDBMS</span></span>

* <span data-ttu-id="56085-2120">`georestore` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2120">Added `georestore` command</span></span>
* <span data-ttu-id="56085-2121">`create` 명령에서 스토리지 크기 제한이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2121">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2122">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2122">Resource</span></span>

* <span data-ttu-id="56085-2123">`--metadata`에 대한 지원이 `policy definition create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2123">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="56085-2124">`--metadata`, `--set`, `--add`, `--remove`에 대한 지원이 `policy definition update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2124">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2125">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2125">SQL</span></span>

* <span data-ttu-id="56085-2126">`sql elastic-pool op list` 및 `sql elastic-pool op cancel`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2126">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2127">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2127">Storage</span></span>

* <span data-ttu-id="56085-2128">잘못된 형식의 연결 문자열에 대한 오류 메시지가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2128">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2129">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2129">VM</span></span>

* <span data-ttu-id="56085-2130">플랫폼 장애 도메인 수를 `vmss create`로 구성하는 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2130">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="56085-2131">영역, 대형 또는 단일 배치 그룹 비활성화 스케일 집합에 대해 `vmss create`을 기본값인 표준 LB로 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-2131">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [호환성이 손상되는 변경]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="56085-2133">공용-IP SKU에 대한 지원이 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2133">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="56085-2134">명령이 자격 증명 모음 ID를 확인할 수 없는 시나리오를 지원하기 위해 `--keyvault` 및 `--resource-group` 인수가 `vm secret format`에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2134">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="56085-2135">#5718</span><span class="sxs-lookup"><span data-stu-id="56085-2135">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="56085-2136">리소스 그룹의 위치에 영역 지원이 없는 경우 `[vm|vmss create]`에 대한 오류가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-2136">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="56085-2137">2018년 3월 27일</span><span class="sxs-lookup"><span data-stu-id="56085-2137">March 27, 2018</span></span>

<span data-ttu-id="56085-2138">버전 2.0.30</span><span class="sxs-lookup"><span data-stu-id="56085-2138">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="56085-2139">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2139">Core</span></span>

* <span data-ttu-id="56085-2140">도움말에서 미리 보기로 표시된 확장에 대한 메시지 표시</span><span class="sxs-lookup"><span data-stu-id="56085-2140">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2141">ACS</span></span>

* <span data-ttu-id="56085-2142">Cloud Shell에서 `aks install-cli`에 대한 SSL 인증서 확인 오류 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2142">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2143">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2143">Appservice</span></span>

* <span data-ttu-id="56085-2144">`webapp update`에 HTTPS만 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2144">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="56085-2145">`az webapp identity [assign|show]` 및 `az functionapp identity [assign|show]`에 대한 슬롯 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2145">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="56085-2146">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-2146">Backup</span></span>

* <span data-ttu-id="56085-2147">새 명령 `az backup protection isenabled-for-vm`이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2147">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="56085-2148">이 명령을 사용하여 구독의 자격 증명 모음에 의해 VM을 백업했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2148">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="56085-2149">다음 명령의 `--resource-group` 및 `--vault-name` 매개 변수에 대해 Azure 개체 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2149">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="56085-2150">`backup ... show` 명령의 출력 형식을 허용하도록 `--name` 매개 변수가 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2150">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="56085-2151">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2151">Container</span></span>

* <span data-ttu-id="56085-2152">`container exec` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2152">Added `container exec` command.</span></span> <span data-ttu-id="56085-2153">실행 중인 컨테이너 그룹에 대해 컨테이너에서 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2153">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="56085-2154">컨테이너 그룹 생성 및 업데이트에 관한 테이블 출력 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2154">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2155">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2155">Extension</span></span>

* <span data-ttu-id="56085-2156">확장이 미리 보기에 있는 경우 `extension add`에 대한 메시지가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2156">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="56085-2157">`--show-details`로 전체 확장 데이터를 표시하도록 `extension list-available`이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2157">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="56085-2158">[주요 변경 사항] 기본적으로 단순화된 확장 데이터를 표시하도록 `extension list-available`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2158">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2159">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2159">Interactive</span></span>

* <span data-ttu-id="56085-2160">명령 테이블 로딩이 완료되는 즉시 활성화로 변경 완료</span><span class="sxs-lookup"><span data-stu-id="56085-2160">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="56085-2161">`--style` 매개 변수를 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2161">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="56085-2162">누락된 경우 명령 테이블 덤프 후 대화형 렉서가 인스턴스화됨</span><span class="sxs-lookup"><span data-stu-id="56085-2162">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="56085-2163">완성자 지원 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2163">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="56085-2164">랩</span><span class="sxs-lookup"><span data-stu-id="56085-2164">Lab</span></span>

* <span data-ttu-id="56085-2165">`create environment` 명령을 사용하여 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2165">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2166">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2166">Monitor</span></span>

* <span data-ttu-id="56085-2167">`metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 `--top`, `--orderby` 및 `--namespace`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2167">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="56085-2168">[#4529](https://github.com/Azure/azure-cli/issues/5785) 수정됨: `metrics list` 검색을 위해 공백으로 구분된 메트릭 목록을 허용함</span><span class="sxs-lookup"><span data-stu-id="56085-2168">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="56085-2169">`metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)에 `--namespace` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2169">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="56085-2170">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2170">Network</span></span>

* <span data-ttu-id="56085-2171">프라이빗 DNS 영역에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2171">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2172">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2172">Profile</span></span>

* <span data-ttu-id="56085-2173">`--identity-port` 및 `--msi-port`에 대한 경고가 `login`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2173">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-2174">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-2174">RDBMS</span></span>

* <span data-ttu-id="56085-2175">비즈니스 모델 GA API 버전 2017-12-01 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2175">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2176">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2176">Resource</span></span>

* [호환성이 손상되는 변경]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="56085-2178">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2178">Role</span></span>

* <span data-ttu-id="56085-2179">필수 액세스 구성 및 네이티브 클라이언트에 대한 지원이 `az ad app create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2179">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="56085-2180">개체 확인 시 1000개 미만의 ID를 반환하도록 `rbac` 명령이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2180">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="56085-2181">자격 증명 관리 명령 `ad sp credential [reset|list|delete]` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2181">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="56085-2182">[주요 변경 사항]`az role assignment [list|show]` 출력에서 '속성' 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2182">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="56085-2183">`dataActions` 및 `notDataActions` 권한에 대한 지원이 `role definition`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2183">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2184">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2184">Storage</span></span>

* <span data-ttu-id="56085-2185">크기가 195GB에서 200GB 사이인 파일을 업로드할 때 발생하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2185">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="56085-2186">[#4049](https://github.com/Azure/azure-cli/issues/4049) 수정됨: 조건 매개 변수를 무시하는 BLOB 업로드 추가에 따른 문제</span><span class="sxs-lookup"><span data-stu-id="56085-2186">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2187">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2187">VM</span></span>

* <span data-ttu-id="56085-2188">100개 이상의 인스턴스가 있는 세트의 향후 호환성이 손상되는 변경에 대한 경고가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2188">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="56085-2189">`vm [snapshot|image]`에 영역 복원 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2189">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="56085-2190">향상된 암호화 상태를 보고하도록 디스크 인스턴스 보기 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2190">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="56085-2191">[주요 변경 사항] 더 이상 출력을 반환하지 않도록 `vm extension delete` 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2191">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="56085-2192">2018년 3월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-2192">March 13, 2018</span></span>

<span data-ttu-id="56085-2193">버전 2.0.29</span><span class="sxs-lookup"><span data-stu-id="56085-2193">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2194">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2194">ACR</span></span>

* <span data-ttu-id="56085-2195">`repository delete`에 `--image` 매개 변수에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2195">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="56085-2196">`repository delete` 명령의 `--manifest` 및 `--tag` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2196">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="56085-2197">데이터를 삭제하지 않고 태그를 제거하는 `repository untag` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2197">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2198">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2198">ACS</span></span>

* <span data-ttu-id="56085-2199">기존 커넥터를 업그레이드하는 `aks upgrade-connector` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2199">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="56085-2200">보다 읽기 쉬운 블록 스타일 YAML을 사용하는 `kubectl` 구성 파일 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2200">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="56085-2201">Advisor</span><span class="sxs-lookup"><span data-stu-id="56085-2201">Advisor</span></span>

* <span data-ttu-id="56085-2202">[주요 변경 사항]`advisor configuration get`에서 `advisor configuration list`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2202">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="56085-2203">[주요 변경 사항]`advisor configuration set`에서 `advisor configuration update`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2203">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="56085-2204">[주요 변경 사항]`advisor recommendation generate` 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2204">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="56085-2205">`--refresh` 매개 변수가 `advisor recommendation list`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2205">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="56085-2206">`advisor recommendation show` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2206">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2207">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2207">Appservice</span></span>

* <span data-ttu-id="56085-2208">`[webapp|functionapp] assign-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2208">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="56085-2209">`webapp identity [assign|show]` 및 `functionapp identity [assign|show]` 관리 ID 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2209">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="56085-2210">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="56085-2210">Eventhubs</span></span>

* <span data-ttu-id="56085-2211">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2211">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2212">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2212">Extension</span></span>

* <span data-ttu-id="56085-2213">사용된 배포판이 패키지 원본 파일에 저장된 것과 다른 경우 오류가 발생할 수 있으므로 사용자에게 경고하도록 검사 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2213">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2214">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2214">Interactive</span></span>

* <span data-ttu-id="56085-2215">[#5625](https://github.com/Azure/azure-cli/issues/5625) 수정됨: 여러 세션 간에 기록 유지</span><span class="sxs-lookup"><span data-stu-id="56085-2215">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="56085-2216">[#3016](https://github.com/Azure/azure-cli/issues/3016) 수정됨: 범위에 속하지만 남겨지지 않는 기록</span><span class="sxs-lookup"><span data-stu-id="56085-2216">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="56085-2217">[#5688](https://github.com/Azure/azure-cli/issues/5688) 수정됨: 명령 테이블 로딩에 예외가 발생하는 경우 완료가 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2217">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="56085-2218">장기 실행 작업의 진행률 표시기 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2218">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2219">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2219">Monitor</span></span>

* <span data-ttu-id="56085-2220">`monitor autoscale-settings` 명령 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2220">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="56085-2221">`monitor autoscale` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2221">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="56085-2222">`monitor autoscale profile` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2222">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="56085-2223">`monitor autoscale rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2223">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="56085-2224">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2224">Network</span></span>

* <span data-ttu-id="56085-2225">[주요 변경 사항]`route-filter rule create`에서 `--tags` 매개 변수 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2225">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="56085-2226">다음 명령의 일부 잘못된 기본값 제거:</span><span class="sxs-lookup"><span data-stu-id="56085-2226">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="56085-2227">`network watcher connection-monitor` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2227">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="56085-2228">`network watcher show-topology`에 `--vnet` 및 `--subnet` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2228">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2229">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2229">Profile</span></span>

* <span data-ttu-id="56085-2230">`az login`의 `--msi` 매개 변수 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2230">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="56085-2231">`--msi`을 대체하는 `az login`의 `--identity` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2231">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-2232">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-2232">RDBMS</span></span>

* <span data-ttu-id="56085-2233">[미리 보기] API 2017-12-01-미리 보기를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2233">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="56085-2234">Service Bus</span><span class="sxs-lookup"><span data-stu-id="56085-2234">Service Bus</span></span>

* <span data-ttu-id="56085-2235">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2235">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2236">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2236">Storage</span></span>

* <span data-ttu-id="56085-2237">[#4971](https://github.com/Azure/azure-cli/issues/4971) 수정됨: `storage blob copy`가 이제 다른 Azure 클라우드도 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2237">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="56085-2238">[#5286](https://github.com/Azure/azure-cli/issues/5286) 수정됨: 배치 명령`storage blob [delete-batch|download-batch|upload-batch]`이 더 이상 사전 조건 실패 시 오류를 일으키지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2238">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2239">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2239">VM</span></span>

* <span data-ttu-id="56085-2240">관리되지 않는 데이터 디스크를 추가하고 캐싱을 구성하는 `[vm|vmss] create`에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2240">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="56085-2241">`[vm|vmss] assign-identity` 및 `[vm|vmss] remove-identity` 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2241">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="56085-2242">사용되지 않는 명령을 바꾸는 `vm identity [assign|remove|show]` 및 `vmss identity [assign|remove|show]` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2242">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="56085-2243">`vmss create`의 기본 우선 순위를 None으로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2243">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="56085-2244">2018년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="56085-2244">February 27, 2018</span></span>

<span data-ttu-id="56085-2245">버전 2.0.28</span><span class="sxs-lookup"><span data-stu-id="56085-2245">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="56085-2246">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2246">Core</span></span>

* <span data-ttu-id="56085-2247">[#5184](https://github.com/Azure/azure-cli/issues/5184) 수정됨: Homebrew 설치 문제</span><span class="sxs-lookup"><span data-stu-id="56085-2247">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="56085-2248">사용자 지정 키를 사용하는 확장 원격 분석에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2248">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="56085-2249">`--debug`에 대한 HTTP 로깅 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2249">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2250">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2250">ACS</span></span>

* <span data-ttu-id="56085-2251">기본적으로 `aks install-connector`에 `virtual-kubelet-for-aks` Helm 차트를 사용하도록 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2251">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="56085-2252">문제 해결됨: 서비스 주체에 ACI 컨테이너 그룹 문제를 만들 권한이 불충분함</span><span class="sxs-lookup"><span data-stu-id="56085-2252">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="56085-2253">`aks install-connector`에 `--aci-container-group`, `--location` 및 `--image-tag` 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2253">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="56085-2254">`aks get-versions`에서 사용 중단 공지 제거</span><span class="sxs-lookup"><span data-stu-id="56085-2254">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2255">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2255">Appservice</span></span>

* <span data-ttu-id="56085-2256">새 SDK 버전에 대한 업데이트(azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="56085-2256">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="56085-2257">[#5538](https://github.com/Azure/azure-cli/issues/5538): 잘못된 SKU로 보고된 `Free` 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2257">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="56085-2258">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="56085-2258">Cognitive Services</span></span>

* <span data-ttu-id="56085-2259">새 Cognitive Services 계정을 만들 때 '알림' 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-2259">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-2260">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-2260">Consumption</span></span>

* <span data-ttu-id="56085-2261">가격표 API의 새 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2261">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="56085-2262">기존 사용량 세부 정보 및 예약 세부 정보 형식 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-2262">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="56085-2263">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2263">Container</span></span>

* <span data-ttu-id="56085-2264">ACI에서 암호를 사용하기 위해 `container create`에 `--secrets` 및 `--secrets-mount-path` 인수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2264">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="56085-2265">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2265">Network</span></span>

* <span data-ttu-id="56085-2266">[#5559](https://github.com/Azure/azure-cli/issues/5559) 수정됨: `network vnet-gateway vpn-client generate`에 클라이언트 누락됨</span><span class="sxs-lookup"><span data-stu-id="56085-2266">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2267">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2267">Resource</span></span>

* <span data-ttu-id="56085-2268">실패 시 부분 템플릿 및 오류를 표시하도록 `group deployment export` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2268">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="56085-2269">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2269">Role</span></span>

* <span data-ttu-id="56085-2270">서비스 주체 역할의 감사를 허용하도록 `role assignment list-changelogs` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2270">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2271">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2271">SQL</span></span>

* <span data-ttu-id="56085-2272">생성 및 업데이트 시 데이터베이스 및 탄력적 풀에 대한 영역 중복 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2272">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2273">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2273">Storage</span></span>

* <span data-ttu-id="56085-2274">`storage blob [upload-batch|download-batch]`에 대상-경로/접두사를 지정하도록 설정</span><span class="sxs-lookup"><span data-stu-id="56085-2274">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2275">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2275">VM</span></span>

* <span data-ttu-id="56085-2276">단일 VMSS 인스턴스에서 디스크를 연결/분리하는 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2276">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="56085-2277">2018년 2월 13일</span><span class="sxs-lookup"><span data-stu-id="56085-2277">February 13, 2018</span></span>

<span data-ttu-id="56085-2278">버전 2.0.27</span><span class="sxs-lookup"><span data-stu-id="56085-2278">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="56085-2279">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2279">Core</span></span>

* <span data-ttu-id="56085-2280">MSI 로그인 시 구독 ID 및 이름에 대한 키 인증 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2280">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2281">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2281">ACS</span></span>

* <span data-ttu-id="56085-2282">[주요 변경 사항] 정확성을 위해 `aks get-versions`에서 `aks get-upgrades`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2282">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="56085-2283">`aks create`에 사용 가능한 Kubernetes 버전 표시를 위한 `aks get-versions` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2283">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="56085-2284">서버가 Kubernetes 버전을 선택할 수 있도록 `aks create` 기본값 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2284">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="56085-2285">AKS로 생성되는 서비스 주체를 나타내는 도움말 메시지 업데이트</span><span class="sxs-lookup"><span data-stu-id="56085-2285">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="56085-2286">"Standard\_D1\_v2"에서 "Standard\_DS1\_v2"로 `aks create`의 기본 노드 크기 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2286">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="56085-2287">`az aks browse`의 대시보드 포드를 찾을 때 안정성 향상</span><span class="sxs-lookup"><span data-stu-id="56085-2287">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="56085-2288">Kubernetes 구성 파일을 로드할 때 유니코드 오류 처리를 위한 `aks get-credentials` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2288">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="56085-2289">`$PATH`에서 `kubectl`을(를) 가져올 때 도움이 되도록 `az aks install-cli`에 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2289">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2290">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2290">Appservice</span></span>

* <span data-ttu-id="56085-2291">Null 참조로 인한 `webapp [backup|restore]` 실패 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2291">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="56085-2292">`az configure --defaults appserviceplan=my-asp`을(를) 통한 기본 App Service 계획에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2292">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-2293">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-2293">CDN</span></span>

* <span data-ttu-id="56085-2294">`cdn custom-domain [enable-https|disable-https]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2294">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="56085-2295">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2295">Container</span></span>

* <span data-ttu-id="56085-2296">스트리밍 로그에 대해 `az container logs`에 `--follow` 옵션 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2296">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="56085-2297">로컬 표준 출력 및 오류 스트림을 컨테이너 그룹의 컨테이너에 첨부하는 `container attach` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2297">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-2298">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-2298">CosmosDB</span></span>

* <span data-ttu-id="56085-2299">기능 설정 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2299">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2300">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2300">Extension</span></span>

* <span data-ttu-id="56085-2301">`az extension [add|update]` 명령에 대한 `--pip-proxy` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2301">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="56085-2302">`az extension [add|update]` 명령에 대한 `--pip-extra-index-urls` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2302">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="56085-2303">사용자 의견</span><span class="sxs-lookup"><span data-stu-id="56085-2303">Feedback</span></span>

* <span data-ttu-id="56085-2304">원격 분석 데이터에 대한 확장 정보 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2304">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2305">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2305">Interactive</span></span>

* <span data-ttu-id="56085-2306">Cloud Shell에서 대화형 모드를 사용할 때 사용자에게 로그인 프롬프트가 표시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2306">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="56085-2307">누락된 매개 변수 완성 기능의 재발 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2307">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="56085-2308">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-2308">IoT</span></span>

* <span data-ttu-id="56085-2309">성공 시 `iot dps access policy [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2309">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="56085-2310">성공 시 `iot dps linked-hub [create|update]`가 '찾을 수 없음' 오류를 반환하는 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2310">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="56085-2311">`iot dps access policy [create|update]` 및 `iot dps linked-hub [create|update]`에 대한 `--no-wait` 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2311">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="56085-2312">파티션 수를 지정할 수 있도록 `iot hub create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2312">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2313">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2313">Monitor</span></span>

* <span data-ttu-id="56085-2314">`az monitor log-profiles create` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2314">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="56085-2315">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2315">Network</span></span>

* <span data-ttu-id="56085-2316">다음 명령에 대한 `--tags` 옵션 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2316">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="56085-2317">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2317">Profile</span></span>

* <span data-ttu-id="56085-2318">대화형 모드에서 `az login` 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2318">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2319">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2319">Resource</span></span>

* <span data-ttu-id="56085-2320">`feature show` 다시 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2320">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="56085-2321">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2321">Role</span></span>

* <span data-ttu-id="56085-2322">`--available-to-other-tenants` 인수를 `ad app update`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2322">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2323">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2323">SQL</span></span>

* <span data-ttu-id="56085-2324">`sql server dns-alias` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2324">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="56085-2325">`sql db rename`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2325">Added `sql db rename`</span></span>
* <span data-ttu-id="56085-2326">모든 SQL 명령에 대한 `--ids` 인수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2326">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2327">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2327">Storage</span></span>

* <span data-ttu-id="56085-2328">일시 삭제를 지원하는 `storage blob service-properties delete-policy` 및 `storage blob undelete` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2328">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2329">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2329">VM</span></span>

* <span data-ttu-id="56085-2330">가상 머신 암호화가 완전히 초기화되지 않을 수 있는 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2330">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="56085-2331">MSI 지원에 대한 주체 ID 출력 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2331">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="56085-2332">고정 `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="56085-2332">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="56085-2333">2018년 1월 31일</span><span class="sxs-lookup"><span data-stu-id="56085-2333">January 31, 2018</span></span>

<span data-ttu-id="56085-2334">버전 2.0.26</span><span class="sxs-lookup"><span data-stu-id="56085-2334">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="56085-2335">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2335">Core</span></span>

* <span data-ttu-id="56085-2336">MSI 컨텍스트에서 기본 토큰 검색 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2336">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="56085-2337">Windows cmd.exe에서 LRO 완료 후 폴링 표시기 문자열 제거</span><span class="sxs-lookup"><span data-stu-id="56085-2337">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="56085-2338">구성된 기본값 사용이 INFO 수준 항목으로 변경되었을 때 표시되는 경고가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2338">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="56085-2339">`--verbose`을(를) 사용하여 확인</span><span class="sxs-lookup"><span data-stu-id="56085-2339">Use `--verbose` to see</span></span>
* <span data-ttu-id="56085-2340">대기 명령에 대한 진행률 표시기 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2340">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2341">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2341">ACS</span></span>

* <span data-ttu-id="56085-2342">`--disable-browser` 인수 설명 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2342">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="56085-2343">`--vm-size` 인수에 대한 탭 완성 기능 개선</span><span class="sxs-lookup"><span data-stu-id="56085-2343">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2344">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2344">Appservice</span></span>

* <span data-ttu-id="56085-2345">고정 `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="56085-2345">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="56085-2346">Webapps 및 함수에 대한 `kind` 확인 제거</span><span class="sxs-lookup"><span data-stu-id="56085-2346">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-2347">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-2347">CDN</span></span>

* <span data-ttu-id="56085-2348">`cdn custom-domain create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2348">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-2349">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-2349">CosmosDB</span></span>

* <span data-ttu-id="56085-2350">장애 조치(Failover) 정책에 대한 매개 변수 설명 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2350">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2351">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2351">Interactive</span></span>

* <span data-ttu-id="56085-2352">명령 옵션 완성이 더 이상 표시되지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2352">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="56085-2353">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2353">Network</span></span>

* <span data-ttu-id="56085-2354">`application-gateway create`에 `--cert-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2354">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="56085-2355">`--sku`이(가) 기본값을 잘못 적용하는 `application-gateway update` 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2355">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="56085-2356">`vpn-connection create`에 `--shared-key` 및 `--authorization-key` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2356">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="56085-2357">`asg create`의 클라이언트 누락 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2357">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="56085-2358">`dns zone export`에 내보낸 이름에 대한 `--file-name / -f` 매개변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2358">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="56085-2359">`dns zone export`의 다음 문제 해결:</span><span class="sxs-lookup"><span data-stu-id="56085-2359">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="56085-2360">긴 TXT 레코드가 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2360">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="56085-2361">따옴표 붙은 TXT 레코드가 이스케이프 처리 없이 잘못 내보내지는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2361">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="56085-2362">`dns zone import`에서 특정 레코드를 두 번 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2362">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="56085-2363">`vnet-gateway root-cert` 및 `vnet-gateway revoked-cert` 명령 복원</span><span class="sxs-lookup"><span data-stu-id="56085-2363">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2364">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2364">Profile</span></span>

* <span data-ttu-id="56085-2365">ID가 있는 가상 머신 내에서 작동하도록 `get-access-token` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2365">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2366">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2366">Resource</span></span>

* <span data-ttu-id="56085-2367">템플릿 'type' 필드에 대문자 값이 포함되었을 때 경고가 잘못 표시되는 `deployment [create|validate]` 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2367">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2368">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2368">Storage</span></span>

* <span data-ttu-id="56085-2369">스토리지 V1 계정을 스토리지 V2로 마이그레이션할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2369">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="56085-2370">모든 upload/download 명령에 대한 진행률 보고 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2370">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="56085-2371">`storage account check-name`에서 "-n" 인수 옵션을 방해하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2371">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="56085-2372">`blob [list|show]`에 대한 테이블 출력에 '스냅샷' 열 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2372">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="56085-2373">Ints로 구문 분석되어야 하는 여러 매개 변수의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2373">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2374">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2374">VM</span></span>

* <span data-ttu-id="56085-2375">추가 비용이 있는 이미지에서 가상 머신을 만들 수 있게 허용하는 `vm image accept-terms` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2375">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="56085-2376">서명되지 않은 인증서를 사용해서 프록시로 명령을 실행할 수 있도록 `[vm|vmss create]` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2376">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="56085-2377">[미리 보기] VMSS에 "낮음" 우선 순위 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2377">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="56085-2378">`[vm|vmss] create`에 `--admin-password` 보호 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2378">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="56085-2379">2018년 1월 17일</span><span class="sxs-lookup"><span data-stu-id="56085-2379">January 17, 2018</span></span>

<span data-ttu-id="56085-2380">버전 2.0.25</span><span class="sxs-lookup"><span data-stu-id="56085-2380">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2381">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2381">ACR</span></span>

* <span data-ttu-id="56085-2382">Windows 자격 증명 오류에 acr 로그인 대체 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2382">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="56085-2383">레지스트리 로그를 사용하도록 설정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2383">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2384">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2384">ACS</span></span>

* <span data-ttu-id="56085-2385">`get-credentials` 명령 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2385">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="56085-2386">SPN 역할 요구 사항 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2386">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2387">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2387">Appservice</span></span>

* <span data-ttu-id="56085-2388">`hosting_environment_profile`가 Null인 `config ssl upload`을 사용해 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2388">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="56085-2389">사용자 지정 URL에 대한 지원이 `browse`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2389">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="56085-2390">`log tail`에 대한 슬롯 지원 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2390">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="56085-2391">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-2391">Backup</span></span>

* <span data-ttu-id="56085-2392">`backup item list`의 `--container-name` 옵션이 선택할 수 있도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2392">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="56085-2393">`backup restore restore-disks`에 스토리지 계정 옵션 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2393">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="56085-2394">`backup protection enable-for-vm`의 위치 확인이 대/소문자 구분하지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2394">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="56085-2395">잘못된 컨테이너 이름 때문에 명령이 실패한 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2395">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="56085-2396">기본값으로 ‘상태’ 포함하도록 `backup item list` 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2396">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="56085-2397">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-2397">Batch</span></span>

* <span data-ttu-id="56085-2398">인증 세부정보 반환하도록 `batch login` 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2398">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="56085-2399">클라우드</span><span class="sxs-lookup"><span data-stu-id="56085-2399">Cloud</span></span>

* <span data-ttu-id="56085-2400">클라우드에서 `--profile`을 설정할 때 엔드포인트를 요구하지 않도록 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2400">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-2401">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-2401">Consumption</span></span>

* <span data-ttu-id="56085-2402">새 예약 명령 `consumption reservations summaries`과 `consumption reservations details` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2402">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="56085-2403">Event Grid</span><span class="sxs-lookup"><span data-stu-id="56085-2403">Event Grid</span></span>

* <span data-ttu-id="56085-2404">[주요 변경 사항]`az eventgrid topic event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="56085-2404">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="56085-2405">[주요 변경 사항]`az eventgrid resource event-subscription` 명령이 `eventgrid event-subscription`으로 이동됨</span><span class="sxs-lookup"><span data-stu-id="56085-2405">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="56085-2406">[주요 변경 사항]`eventgrid event-subscription show-endpoint-url` 명령 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2406">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="56085-2407">대신 `eventgrid event-subscription show --include-full-endpoint-url`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="56085-2407">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="56085-2408">명령 `eventgrid topic update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2408">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="56085-2409">명령 `eventgrid event-subscription update` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2409">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="56085-2410">`eventgrid topic` 명령에 대한 `--ids` 매개 변수 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2410">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="56085-2411">토픽 이름에 대한 탭 완성 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2411">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2412">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2412">Interactive</span></span>

* <span data-ttu-id="56085-2413">대화형 모드가 Python 2.x와 작동하지 않는 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2413">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="56085-2414">시작할 때 오류 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2414">Fixed errors on startup</span></span>
* <span data-ttu-id="56085-2415">대화형 모드에서 실행되지 않는 일부 명령 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2415">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="56085-2416">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-2416">IoT</span></span>

* <span data-ttu-id="56085-2417">디바이스 프로비전 서비스에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2417">Added support for device provisioning service</span></span>
* <span data-ttu-id="56085-2418">명령 및 명령 도움말의 사용 중단 메시지 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2418">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="56085-2419">사용자에게 IoT 확장을 알려주는 IoT 검사 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2419">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2420">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2420">Monitor</span></span>

* <span data-ttu-id="56085-2421">다중 진단 설정 지원이 추가됐습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2421">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="56085-2422">`--name` 매개 변수가 이제 `az monitor diagnostic-settings create`를 위해 필요합니다</span><span class="sxs-lookup"><span data-stu-id="56085-2422">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="56085-2423">진단 설정 범주를 가져오기 위해 명령 `monitor diagnostic-settings categories` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2423">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="56085-2424">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2424">Network</span></span>

* <span data-ttu-id="56085-2425">`vnet-gateway update`을 사용해 활성-대기 모드를 변경하려고 할 때의 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2425">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="56085-2426">HTTP2에 대한 지원이 `application-gateway [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2426">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2427">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2427">Profile</span></span>

* <span data-ttu-id="56085-2428">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2428">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="56085-2429">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2429">Role</span></span>

* <span data-ttu-id="56085-2430">그래프 쿼리를 사용하지 않기 위해 `--assignee-object-id` 인수가 `role assignment create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2430">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="56085-2431">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="56085-2431">Service Fabric</span></span>

* <span data-ttu-id="56085-2432">클러스터를 만들 때 유효성 검사 응답에 자세한 오류 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2432">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="56085-2433">여러 명령을 사용하여 누락된 클라이언트 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2433">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2434">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2434">VM</span></span>

* <span data-ttu-id="56085-2435">[미리 보기] `vmss`에 대한 영역 간 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2435">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="56085-2436">[주요 변경 사항] 단일 영역 `vmss` 기본값이 "표준" 부하 분산 장치로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2436">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="56085-2437">[주요 변경 사항] EMSI에 대해 `externalIdentities`을 `userAssignedIdentities`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2437">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="56085-2438">[미리 보기] OS 디스크 교체에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2438">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="56085-2439">다른 구독에서 VM 이미지를 사용하기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2439">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="56085-2440">`--plan-name`, `--plan-product`, `--plan-promotion-code`, `--plan-publisher` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2440">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="56085-2441">`[vm|vmss] create`을 사용하여 오류 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2441">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="56085-2442">`vm image list --all`에 의해 발생하는 과도한 리소스 사용 문제 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2442">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="56085-2443">2017년 12월 19일</span><span class="sxs-lookup"><span data-stu-id="56085-2443">December 19, 2017</span></span>

<span data-ttu-id="56085-2444">버전 2.0.23</span><span class="sxs-lookup"><span data-stu-id="56085-2444">Version 2.0.23</span></span>

* <span data-ttu-id="56085-2445">사용자 할당 ID를 사용하여 로그인에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2445">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="56085-2446">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2446">Container</span></span>

* <span data-ttu-id="56085-2447">컨테이너 로그에 대한 매개 변수의 잘못된 순서 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2447">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="56085-2448">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2448">Network</span></span>

* <span data-ttu-id="56085-2449">`--disable-bgp-route-propagation` 인수를 `route-table [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2449">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="56085-2450">`--ip-tags` 인수를 `public-ip [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2450">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2451">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2451">Storage</span></span>

* <span data-ttu-id="56085-2452">storage V2에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2452">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2453">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2453">VM</span></span>

* <span data-ttu-id="56085-2454">[미리 보기] VM 및 VMSS의 사용자 할당 ID에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2454">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="56085-2455">2017년 12월 5일</span><span class="sxs-lookup"><span data-stu-id="56085-2455">December 5, 2017</span></span>

<span data-ttu-id="56085-2456">버전 2.0.22</span><span class="sxs-lookup"><span data-stu-id="56085-2456">Version 2.0.22</span></span>

* <span data-ttu-id="56085-2457">`az component` 명령이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2457">Removed `az component` commands.</span></span> <span data-ttu-id="56085-2458">대신 `az extension`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="56085-2458">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="56085-2459">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2459">Core</span></span>
* <span data-ttu-id="56085-2460">`AZURE_US_GOV_CLOUD` AAD 권한 엔드포인트가 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2460">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="56085-2461">원격 분석이 지속적으로 다시 전송되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2461">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2462">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2462">ACS</span></span>

* <span data-ttu-id="56085-2463">`aks install-connector` 및 `aks remove-connector` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2463">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="56085-2464">`acs create`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-2464">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="56085-2465">정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2465">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="56085-2466">Advisor</span><span class="sxs-lookup"><span data-stu-id="56085-2466">Advisor</span></span>

* <span data-ttu-id="56085-2467">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2467">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2468">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2468">Appservice</span></span>

* <span data-ttu-id="56085-2469">`webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2469">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="56085-2470">`webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2470">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="56085-2471">`WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2471">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="56085-2472">Consumption</span><span class="sxs-lookup"><span data-stu-id="56085-2472">Consumption</span></span>

* <span data-ttu-id="56085-2473">API 버전 2017-11-30에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2473">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="56085-2474">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2474">Container</span></span>

* <span data-ttu-id="56085-2475">기본 포트 회귀가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2475">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2476">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2476">Monitor</span></span>

* <span data-ttu-id="56085-2477">메트릭 명령에 다차원 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2477">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2478">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2478">Resource</span></span>

* <span data-ttu-id="56085-2479">`--include-response-body` 인수를 `resource show`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2479">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="56085-2480">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2480">Role</span></span>

* <span data-ttu-id="56085-2481">`role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2481">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="56085-2482">덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2482">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="56085-2483">`ad sp create-for-rbac`에 대한 오류 보고가 개선됨</span><span class="sxs-lookup"><span data-stu-id="56085-2483">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2484">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2484">SQL</span></span>

* <span data-ttu-id="56085-2485">`sql db list-usages` 및 `sql db show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2485">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="56085-2486">`sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2486">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2487">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2487">VM</span></span>

* <span data-ttu-id="56085-2488">`az vm list-skus`에 영역 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2488">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="56085-2489">2017년 11월 14일</span><span class="sxs-lookup"><span data-stu-id="56085-2489">November 14, 2017</span></span>

<span data-ttu-id="56085-2490">버전 2.0.21</span><span class="sxs-lookup"><span data-stu-id="56085-2490">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2491">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2491">ACR</span></span>

* <span data-ttu-id="56085-2492">복제 영역에서 웹후크를 만들기 위한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2492">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="56085-2493">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2493">ACS</span></span>

* <span data-ttu-id="56085-2494">AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2494">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="56085-2495">`acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션</span><span class="sxs-lookup"><span data-stu-id="56085-2495">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="56085-2496">AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2496">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="56085-2497">Windows에서 `az aks browse` 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2497">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="56085-2498">Windows에서 `az aks get-credentials` 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2498">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2499">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2499">Appservice</span></span>

* <span data-ttu-id="56085-2500">WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2500">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="56085-2501">`--docker-container-logging` 옵션을 `az webapp log config`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2501">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="56085-2502">`az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2502">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="56085-2503">`deployment user set`에 대한 오류 메시지 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2503">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="56085-2504">Linux 함수 앱을 만들기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2504">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="56085-2505">고정 `list-locations`</span><span class="sxs-lookup"><span data-stu-id="56085-2505">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="56085-2506">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-2506">Batch</span></span>

* <span data-ttu-id="56085-2507">리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2507">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-2508">Batchai</span><span class="sxs-lookup"><span data-stu-id="56085-2508">Batchai</span></span>

* <span data-ttu-id="56085-2509">`file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2509">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="56085-2510">스토리지 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2510">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="56085-2511">`job list-files` 및 `job stream-file` 설명서 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2511">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="56085-2512">`job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2512">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="56085-2513">클라우드</span><span class="sxs-lookup"><span data-stu-id="56085-2513">Cloud</span></span>

* <span data-ttu-id="56085-2514">필요한 엔드포인트가 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2514">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="56085-2515">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2515">Container</span></span>

* <span data-ttu-id="56085-2516">다중 포트를 열기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2516">Added support to open multiple ports</span></span>
* <span data-ttu-id="56085-2517">컨테이너 그룹 다시 시작 정책 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2517">Added container group restart policy</span></span>
* <span data-ttu-id="56085-2518">Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2518">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="56085-2519">업데이트된 도우미 docs</span><span class="sxs-lookup"><span data-stu-id="56085-2519">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="56085-2520">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="56085-2520">Data Lake Analytics</span></span>

* <span data-ttu-id="56085-2521">보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2521">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="56085-2522">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="56085-2522">Data Lake Store</span></span>

* <span data-ttu-id="56085-2523">보다 간결한 정보를 반환하기 위해 `account list` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2523">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2524">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2524">Extension</span></span>

* <span data-ttu-id="56085-2525">공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2525">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="56085-2526">이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2526">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="56085-2527">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-2527">IoT</span></span>

* <span data-ttu-id="56085-2528">인증 기관(CA) 및 인증서 체인에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2528">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2529">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2529">Monitor</span></span>

* <span data-ttu-id="56085-2530">`activity-log alert` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2530">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="56085-2531">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2531">Network</span></span>

* <span data-ttu-id="56085-2532">CAA DNS 레코드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2532">Added support for CAA DNS records</span></span>
* <span data-ttu-id="56085-2533">`traffic-manager profile update`로 엔드포인트를 업데이트할 수 없는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2533">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="56085-2534">VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2534">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="56085-2535">`dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2535">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="56085-2536">예약</span><span class="sxs-lookup"><span data-stu-id="56085-2536">Reservations</span></span>

* <span data-ttu-id="56085-2537">초기 미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2537">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2538">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2538">Resource</span></span>

* <span data-ttu-id="56085-2539">리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2539">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2540">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2540">SQL</span></span>

* <span data-ttu-id="56085-2541">`--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2541">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2542">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2542">Storage</span></span>

* <span data-ttu-id="56085-2543">기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2543">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="56085-2544">비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2544">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="56085-2545">`--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2545">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="56085-2546">glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제</span><span class="sxs-lookup"><span data-stu-id="56085-2546">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="56085-2547">`storage metrics update`로 메트릭을 사용할 때 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2547">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="56085-2548">`storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2548">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="56085-2549">`storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2549">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2550">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2550">VM</span></span>

* <span data-ttu-id="56085-2551">`Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2551">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="56085-2552">청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2552">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="56085-2553">`vm secret `[add|remove|list]\` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2553">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="56085-2554">`vm format-secret`에서 `vm secret format`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2554">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="56085-2555">`--encrypt format` 인수를 `vm encryption enable`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2555">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="56085-2556">2017년 10월 24일</span><span class="sxs-lookup"><span data-stu-id="56085-2556">October 24, 2017</span></span>

<span data-ttu-id="56085-2557">버전 2.0.20</span><span class="sxs-lookup"><span data-stu-id="56085-2557">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="56085-2558">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2558">Core</span></span>

* <span data-ttu-id="56085-2559">`MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함</span><span class="sxs-lookup"><span data-stu-id="56085-2559">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2560">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2560">ACR</span></span>

* <span data-ttu-id="56085-2561">`2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="56085-2561">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="56085-2562">'Bring Your Own Storage' SKU를 클래식으로 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-2562">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="56085-2563">레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함</span><span class="sxs-lookup"><span data-stu-id="56085-2563">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2564">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2564">ACS</span></span>

* <span data-ttu-id="56085-2565">[미리 보기] `az aks` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2565">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="56085-2566">Kubernetes `get-credentials`가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2566">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2567">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2567">Appservice</span></span>

* <span data-ttu-id="56085-2568">다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2568">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="56085-2569">구성 요소</span><span class="sxs-lookup"><span data-stu-id="56085-2569">Component</span></span>

* <span data-ttu-id="56085-2570">모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2570">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2571">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2571">Monitor</span></span>

* <span data-ttu-id="56085-2572">`action-group` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2572">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2573">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2573">Resource</span></span>

* <span data-ttu-id="56085-2574">`group export`의 최신 msrest 종속성과의 비호환성이 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2574">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="56085-2575">기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2575">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2576">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2576">VM</span></span>

* <span data-ttu-id="56085-2577">`--accelerated-networking` 인수를 `vmss create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2577">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="56085-2578">2017년 10월 9일</span><span class="sxs-lookup"><span data-stu-id="56085-2578">October 9, 2017</span></span>

<span data-ttu-id="56085-2579">버전 2.0.19</span><span class="sxs-lookup"><span data-stu-id="56085-2579">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="56085-2580">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2580">Core</span></span>

* <span data-ttu-id="56085-2581">Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2581">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2582">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2582">Appservice</span></span>

* <span data-ttu-id="56085-2583">새 명령 `webapp update`로 일반 업데이트 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2583">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="56085-2584">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-2584">Batch</span></span>

* <span data-ttu-id="56085-2585">일괄 처리 SDK 4.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2585">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="56085-2586">publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2586">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="56085-2587">일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2587">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="56085-2588">구성 요소 모델에서 일괄 처리 지원이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2588">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="56085-2589">Batchai</span><span class="sxs-lookup"><span data-stu-id="56085-2589">Batchai</span></span>

* <span data-ttu-id="56085-2590">일괄 처리 AI 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2590">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-2591">Keyvault</span><span class="sxs-lookup"><span data-stu-id="56085-2591">Keyvault</span></span>

* <span data-ttu-id="56085-2592">Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2592">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="56085-2593">(#4448)</span><span class="sxs-lookup"><span data-stu-id="56085-2593">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="56085-2594">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2594">Network</span></span>

* <span data-ttu-id="56085-2595">빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2595">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="56085-2596">최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2596">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2597">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2597">Resource</span></span>

* <span data-ttu-id="56085-2598">리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2598">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="56085-2599">구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2599">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="56085-2600">그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2600">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="56085-2601">리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2601">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2602">Sql</span><span class="sxs-lookup"><span data-stu-id="56085-2602">Sql</span></span>

* <span data-ttu-id="56085-2603">SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2603">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="56085-2604">삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2604">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="56085-2605">진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2605">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2606">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2606">Storage</span></span>

* <span data-ttu-id="56085-2607">파일 공유 스냅샷에 대한 지원 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2607">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2608">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2608">Vm</span></span>

* <span data-ttu-id="56085-2609">`-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2609">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="56085-2610">[미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2610">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="56085-2611">`vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2611">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="56085-2612">`--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2612">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="56085-2613">Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2613">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="56085-2614">2017년 9월 22일</span><span class="sxs-lookup"><span data-stu-id="56085-2614">September 22, 2017</span></span>

<span data-ttu-id="56085-2615">버전 2.0.18</span><span class="sxs-lookup"><span data-stu-id="56085-2615">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2616">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2616">Resource</span></span>

* <span data-ttu-id="56085-2617">기본 제공 정책 정의를 표시하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2617">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="56085-2618">정책 정의를 만들기 위한 지원 모드 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2618">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="56085-2619">UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2619">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="56085-2620">[주요 변경 사항]`managedapp` 리소스 종류가 `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2620">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="56085-2621">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2621">Network</span></span>

* <span data-ttu-id="56085-2622">가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2622">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="56085-2623">IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2623">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="56085-2624">`asg` 애플리케이션 보안 그룹 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2624">Added `asg` application security group commands</span></span>
* <span data-ttu-id="56085-2625">`--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2625">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="56085-2626">`--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2626">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="56085-2627">`--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2627">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="56085-2628">`network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2628">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2629">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2629">Storage</span></span>

* <span data-ttu-id="56085-2630">SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2630">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="56085-2631">Event Grid</span><span class="sxs-lookup"><span data-stu-id="56085-2631">Eventgrid</span></span>

* <span data-ttu-id="56085-2632">최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK</span><span class="sxs-lookup"><span data-stu-id="56085-2632">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2633">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2633">SQL</span></span>

* <span data-ttu-id="56085-2634">선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2634">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="56085-2635">지정하지 않으면 구독의 모든 sql 서버가 반환됨</span><span class="sxs-lookup"><span data-stu-id="56085-2635">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="56085-2636">`--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2636">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-2637">Keyvault</span><span class="sxs-lookup"><span data-stu-id="56085-2637">Keyvault</span></span>

* <span data-ttu-id="56085-2638">프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2638">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2639">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2639">VM</span></span>

* <span data-ttu-id="56085-2640">가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2640">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="56085-2641">`--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="56085-2641">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="56085-2642">`--asgs` 인수를 `vm create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2642">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="56085-2643">`vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2643">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="56085-2644">[미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2644">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="56085-2645">`vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2645">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2646">ACS</span></span>

* <span data-ttu-id="56085-2647">[미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2647">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2648">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2648">Appservice</span></span>

* <span data-ttu-id="56085-2649">`webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2649">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="56085-2650">Backup</span><span class="sxs-lookup"><span data-stu-id="56085-2650">Backup</span></span>

* <span data-ttu-id="56085-2651">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2651">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="56085-2652">2017년 9월 11일</span><span class="sxs-lookup"><span data-stu-id="56085-2652">September 11, 2017</span></span>

<span data-ttu-id="56085-2653">버전 2.0.17</span><span class="sxs-lookup"><span data-stu-id="56085-2653">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="56085-2654">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2654">Core</span></span>

* <span data-ttu-id="56085-2655">원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2655">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="56085-2656">원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2656">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2657">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2657">Acs</span></span>

* <span data-ttu-id="56085-2658">`acs list-locations` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2658">Added `acs list-locations` command</span></span>
* <span data-ttu-id="56085-2659">예상된 기본값 함께 `ssh-key-file`을 제공함</span><span class="sxs-lookup"><span data-stu-id="56085-2659">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2660">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2660">Appservice</span></span>

* <span data-ttu-id="56085-2661">활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2661">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-2662">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-2662">CDN</span></span>

* <span data-ttu-id="56085-2663">`cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2663">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="56085-2664">내선 번호</span><span class="sxs-lookup"><span data-stu-id="56085-2664">Extension</span></span>

* <span data-ttu-id="56085-2665">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2665">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-2666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="56085-2666">Keyvault</span></span>

* <span data-ttu-id="56085-2667">사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2667">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="56085-2668">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2668">Network</span></span>

* <span data-ttu-id="56085-2669">`vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2669">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="56085-2670">`--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-2670">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="56085-2671">여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2671">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="56085-2672">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2672">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="56085-2673">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2673">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2674">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2674">Resource</span></span>

* <span data-ttu-id="56085-2675">`policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2675">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="56085-2676">`policy assignment create`의 매개 변수 값을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2676">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="56085-2677">모든 매개 변수에 JSON 또는 파일을 전달하도록 허용</span><span class="sxs-lookup"><span data-stu-id="56085-2677">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="56085-2678">증가된 API 버전</span><span class="sxs-lookup"><span data-stu-id="56085-2678">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2679">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2679">SQL</span></span>

* <span data-ttu-id="56085-2680">`sql server vnet-rule` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2680">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2681">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2681">VM</span></span>

* <span data-ttu-id="56085-2682">수정됨: `--scope`이(가) 제공되지 않을 경우 액세스 권한을 할당하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2682">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="56085-2683">수정됨: 포털과 동일한 확장명을 사용함</span><span class="sxs-lookup"><span data-stu-id="56085-2683">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="56085-2684">`[vm|vmss] create` 출력에서 `subscription`이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2684">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="56085-2685">수정됨: `[vm|vmss] create` 스토리지 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2685">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="56085-2686">수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2686">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="56085-2687">2017년 8월 31일</span><span class="sxs-lookup"><span data-stu-id="56085-2687">August 31, 2017</span></span>

<span data-ttu-id="56085-2688">버전 2.0.16</span><span class="sxs-lookup"><span data-stu-id="56085-2688">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-2689">Keyvault</span><span class="sxs-lookup"><span data-stu-id="56085-2689">Keyvault</span></span>

* <span data-ttu-id="56085-2690">`secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2690">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="56085-2691">Sf</span><span class="sxs-lookup"><span data-stu-id="56085-2691">Sf</span></span>

* <span data-ttu-id="56085-2692">Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2692">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2693">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2693">Storage</span></span>

* <span data-ttu-id="56085-2694">스토리지 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2694">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="56085-2695">콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함</span><span class="sxs-lookup"><span data-stu-id="56085-2695">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="56085-2696">2017년 8월 28일</span><span class="sxs-lookup"><span data-stu-id="56085-2696">August 28, 2017</span></span>

<span data-ttu-id="56085-2697">버전 2.0.15</span><span class="sxs-lookup"><span data-stu-id="56085-2697">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="56085-2698">CLI</span><span class="sxs-lookup"><span data-stu-id="56085-2698">CLI</span></span>

* <span data-ttu-id="56085-2699">`--version`에 법적 정보가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2699">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2700">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2700">ACS</span></span>

* <span data-ttu-id="56085-2701">미리 보기 영역 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2701">Corrected preview regions</span></span>
* <span data-ttu-id="56085-2702">`dns_name_prefix`의 기본 형식이 올바르게 지정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2702">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="56085-2703">acs 명령 출력이 최적화됨</span><span class="sxs-lookup"><span data-stu-id="56085-2703">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2704">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2704">Appservice</span></span>

* <span data-ttu-id="56085-2705">[주요 변경 사항]`az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2705">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="56085-2706">`az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2706">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="56085-2707">`az webapp log show`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2707">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="56085-2708">`az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2708">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="56085-2709">수정됨: 슬롯 설정을 올바르게 검색함</span><span class="sxs-lookup"><span data-stu-id="56085-2709">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="56085-2710">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-2710">IoT</span></span>

* <span data-ttu-id="56085-2711">#3934 수정됨: 정책을 새로 만들어도 더 이상 기존 정책이 지워지지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2711">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="56085-2712">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2712">Network</span></span>

* <span data-ttu-id="56085-2713">[주요 변경 사항]`vnet list-private-access-services`에서 `vnet list-endpoint-services`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2713">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="56085-2714">[주요 변경 사항]`vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2714">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="56085-2715">여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2715">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="56085-2716">SKU에 대한 지원이 `lb create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2716">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="56085-2717">SKU에 대한 지원이 `public-ip create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2717">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2718">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2718">Profile</span></span>

* <span data-ttu-id="56085-2719">가상 머신의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2719">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="56085-2720">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="56085-2720">Service Fabric</span></span>

* <span data-ttu-id="56085-2721">미리 보기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2721">Preview release</span></span>
* <span data-ttu-id="56085-2722">명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨</span><span class="sxs-lookup"><span data-stu-id="56085-2722">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="56085-2723">매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2723">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="56085-2724">빈 `registry_cred`에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2724">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2725">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2725">Storage</span></span>

* <span data-ttu-id="56085-2726">설정 Blob 계층이 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2726">Enabled setting blob tier</span></span>
* <span data-ttu-id="56085-2727">서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2727">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="56085-2728">VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2728">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="56085-2729">고객 관리 키에 의한 서비스 암호화가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2729">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="56085-2730">[주요 변경 사항]`az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2730">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="56085-2731">#4220: `az storage account update encryption` - 구문 불일치가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2731">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2732">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2732">VM</span></span>

* <span data-ttu-id="56085-2733">`--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2733">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="56085-2734">`--lb-sku`에 대한 지원이 `vmss create`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2734">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="56085-2735">`[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2735">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="56085-2736">이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2736">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="56085-2737">내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2737">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="56085-2738">`--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2738">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="56085-2739">2017년 8월 15일</span><span class="sxs-lookup"><span data-stu-id="56085-2739">August 15, 2017</span></span>

<span data-ttu-id="56085-2740">버전 2.0.14</span><span class="sxs-lookup"><span data-stu-id="56085-2740">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2741">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2741">ACS</span></span>

* <span data-ttu-id="56085-2742">Kubernetes에 대한 sshMaster0 포트 번호가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2742">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2743">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2743">Appservice</span></span>

* <span data-ttu-id="56085-2744">새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2744">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="56085-2745">Event Grid</span><span class="sxs-lookup"><span data-stu-id="56085-2745">Event Grid</span></span>

* <span data-ttu-id="56085-2746">SDK 종속성이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2746">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="56085-2747">2017년 8월 11일</span><span class="sxs-lookup"><span data-stu-id="56085-2747">August 11, 2017</span></span>

<span data-ttu-id="56085-2748">버전 2.0.13</span><span class="sxs-lookup"><span data-stu-id="56085-2748">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2749">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2749">ACS</span></span>

* <span data-ttu-id="56085-2750">더 많은 미리 보기 지역이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2750">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="56085-2751">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-2751">Batch</span></span>

* <span data-ttu-id="56085-2752">Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2752">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="56085-2753">작업의 태스크 수를 표시하는 새 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2753">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="56085-2754">리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2754">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="56085-2755">배치 계정 엔드포인트에서 이제 선택적 'https://' 접두사를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2755">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="56085-2756">100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2756">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="56085-2757">확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2757">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="56085-2758">구성 요소</span><span class="sxs-lookup"><span data-stu-id="56085-2758">Component</span></span>

* <span data-ttu-id="56085-2759">'az component' 명령에 사용 중단 경고가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2759">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="56085-2760">컨테이너</span><span class="sxs-lookup"><span data-stu-id="56085-2760">Container</span></span>

* <span data-ttu-id="56085-2761">`create`: 환경 변수에서 등호가 허용되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2761">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="56085-2762">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="56085-2762">Data Lake Store</span></span>

* <span data-ttu-id="56085-2763">진행률 컨트롤이 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2763">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="56085-2764">Event Grid</span><span class="sxs-lookup"><span data-stu-id="56085-2764">Event Grid</span></span>

* <span data-ttu-id="56085-2765">초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-2765">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="56085-2766">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2766">Network</span></span>

* <span data-ttu-id="56085-2767">`lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2767">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="56085-2768">`application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2768">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="56085-2769">`application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없던 문제가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2769">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="56085-2770">`az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2770">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2771">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2771">Profile</span></span>

* <span data-ttu-id="56085-2772">`account list`: 서버에서 최신 구독을 동기화하기 위해 `--refresh`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2772">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2773">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2773">Storage</span></span>

* <span data-ttu-id="56085-2774">시스템에 할당된 ID를 통한 스토리지 계정 업데이트가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2774">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2775">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2775">VM</span></span>

* <span data-ttu-id="56085-2776">`availability-set`: 변환 시 장애 도메인 수가 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2776">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="56085-2777">`list-skus` 명령이 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2777">Exposed `list-skus` command</span></span>
* <span data-ttu-id="56085-2778">역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2778">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="56085-2779">데이터 디스크 연결 시 스토리지 SKU를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2779">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="56085-2780">관리 디스크를 사용할 때 기본 OS 디스크 이름 및 스토리지 SKU가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2780">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="56085-2781">2017년 7월 28일</span><span class="sxs-lookup"><span data-stu-id="56085-2781">July 28, 2017</span></span>

<span data-ttu-id="56085-2782">버전 2.0.12</span><span class="sxs-lookup"><span data-stu-id="56085-2782">Version 2.0.12</span></span>

* <span data-ttu-id="56085-2783">컨테이너 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2783">Added container commands</span></span>
* <span data-ttu-id="56085-2784">청구 및 소비 모듈이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2784">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="56085-2785">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2785">Core</span></span>

* <span data-ttu-id="56085-2786">인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨</span><span class="sxs-lookup"><span data-stu-id="56085-2786">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="56085-2787">배포 진행률 예외가 해결됨</span><span class="sxs-lookup"><span data-stu-id="56085-2787">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="56085-2788">현재 클라우드의 ARM 엔드포인트를 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-2788">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="56085-2789">clouds.config 파일의 동시 처리가 향상됨(#3636)</span><span class="sxs-lookup"><span data-stu-id="56085-2789">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="56085-2790">각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침</span><span class="sxs-lookup"><span data-stu-id="56085-2790">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="56085-2791">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)</span><span class="sxs-lookup"><span data-stu-id="56085-2791">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="56085-2792">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="56085-2792">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="56085-2793">jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)</span><span class="sxs-lookup"><span data-stu-id="56085-2793">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="56085-2794">향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)</span><span class="sxs-lookup"><span data-stu-id="56085-2794">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="56085-2795">오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="56085-2795">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="56085-2796">기존의 모든 기록 파일을 최신 폴더로 이동</span><span class="sxs-lookup"><span data-stu-id="56085-2796">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="56085-2797">VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)</span><span class="sxs-lookup"><span data-stu-id="56085-2797">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="56085-2798">명령 경로에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2798">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="56085-2799">특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2799">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="56085-2800">프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2800">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="56085-2801">clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)</span><span class="sxs-lookup"><span data-stu-id="56085-2801">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="56085-2802">ACR</span><span class="sxs-lookup"><span data-stu-id="56085-2802">ACR</span></span>

* <span data-ttu-id="56085-2803">관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2803">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="56085-2804">관리되는 레지스트리에 대한 SKU 업데이트가 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2804">Support SKU update for managed registries</span></span>
* <span data-ttu-id="56085-2805">관리되는 SKU에 관리되는 레지스트리가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2805">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="56085-2806">acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2806">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="56085-2807">acr login 명령에 AAD 인증이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2807">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="56085-2808">Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2808">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2809">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2809">ACS</span></span>

* <span data-ttu-id="56085-2810">API 버전 2017-07-01에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2810">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2811">App Service</span><span class="sxs-lookup"><span data-stu-id="56085-2811">Appservice</span></span>

* <span data-ttu-id="56085-2812">Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2812">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="56085-2813">ACR에서 자격 증명을 검색하도록 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2813">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="56085-2814">`appservice web` 아래의 모든 명령을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2814">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="56085-2815">명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).</span><span class="sxs-lookup"><span data-stu-id="56085-2815">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="56085-2816">macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).</span><span class="sxs-lookup"><span data-stu-id="56085-2816">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="56085-2817">`webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).</span><span class="sxs-lookup"><span data-stu-id="56085-2817">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="56085-2818">정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).</span><span class="sxs-lookup"><span data-stu-id="56085-2818">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="56085-2819">원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).</span><span class="sxs-lookup"><span data-stu-id="56085-2819">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="56085-2820">Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2820">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="56085-2821">대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2821">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="56085-2822">Batch</span><span class="sxs-lookup"><span data-stu-id="56085-2822">Batch</span></span>

* <span data-ttu-id="56085-2823">풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2823">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="56085-2824">`pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2824">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="56085-2825">`pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2825">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="56085-2826">CDN</span><span class="sxs-lookup"><span data-stu-id="56085-2826">CDN</span></span>

* <span data-ttu-id="56085-2827">`--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됨</span><span class="sxs-lookup"><span data-stu-id="56085-2827">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="56085-2828">클라우드</span><span class="sxs-lookup"><span data-stu-id="56085-2828">Cloud</span></span>

* <span data-ttu-id="56085-2829">클라우드 메타데이터 엔드포인트의 API 버전이 YYYY-MM-DD 형식으로 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2829">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="56085-2830">갤러리 엔드포인트가 필요하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-2830">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="56085-2831">ARM 리소스 관리자 엔드포인트를 사용한 클라우드 등록이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2831">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="56085-2832">현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨</span><span class="sxs-lookup"><span data-stu-id="56085-2832">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="56085-2833">`endpoint_vm_image_alias_doc`가 공개됨</span><span class="sxs-lookup"><span data-stu-id="56085-2833">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-2834">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-2834">CosmosDB</span></span>

* <span data-ttu-id="56085-2835">사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2835">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="56085-2836">컬렉션 기본 TTL에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2836">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="56085-2837">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="56085-2837">Data Lake Analytics</span></span>

* <span data-ttu-id="56085-2838">`dla account compute-policy` 제목 아래에 컴퓨팅 정책을 관리하는 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2838">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="56085-2839">`dla job pipeline show`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2839">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="56085-2840">`dla job recurrence list`가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2840">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="56085-2841">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="56085-2841">Data Lake Store</span></span>

* <span data-ttu-id="56085-2842">`dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2842">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="56085-2843">기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2843">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="56085-2844">`dls enable-key-vault` 명령이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2844">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="56085-2845">이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다</span><span class="sxs-lookup"><span data-stu-id="56085-2845">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="56085-2846">대화형</span><span class="sxs-lookup"><span data-stu-id="56085-2846">Interactive</span></span>

* <span data-ttu-id="56085-2847">캐시된 명령을 사용하여 시작 시간이 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2847">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="56085-2848">테스트 검사가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2848">Increased test coverage</span></span>
* <span data-ttu-id="56085-2849">다음 명령에 삽입하는 '?' 제스처가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2849">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="56085-2850">2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)</span><span class="sxs-lookup"><span data-stu-id="56085-2850">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="56085-2851">대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)</span><span class="sxs-lookup"><span data-stu-id="56085-2851">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="56085-2852">유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)</span><span class="sxs-lookup"><span data-stu-id="56085-2852">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="56085-2853">템플릿 배포에 대한 진행률이 보고됨(#3510)</span><span class="sxs-lookup"><span data-stu-id="56085-2853">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="56085-2854">`--progress` 플래그가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2854">Added `--progress` flag</span></span>
* <span data-ttu-id="56085-2855">완료 시 `--debug` 및 `--verbose`가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2855">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="56085-2856">완료 시 `interactive`가 제거됨(#3324)</span><span class="sxs-lookup"><span data-stu-id="56085-2856">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="56085-2857">IoT</span><span class="sxs-lookup"><span data-stu-id="56085-2857">IoT</span></span>

* <span data-ttu-id="56085-2858">정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2858">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="56085-2859">(#3934)</span><span class="sxs-lookup"><span data-stu-id="56085-2859">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="56085-2860">주요 자격 증명 모음</span><span class="sxs-lookup"><span data-stu-id="56085-2860">Key vault</span></span>

* <span data-ttu-id="56085-2861">키 자격 증명 모음 복구 기능에 추가된 명령:</span><span class="sxs-lookup"><span data-stu-id="56085-2861">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="56085-2862">`keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="56085-2862">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="56085-2863">`keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="56085-2863">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="56085-2864">`keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="56085-2864">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="56085-2865">`keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="56085-2865">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="56085-2866">서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)</span><span class="sxs-lookup"><span data-stu-id="56085-2866">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="56085-2867">키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="56085-2867">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="56085-2868">(#3307)</span><span class="sxs-lookup"><span data-stu-id="56085-2868">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="56085-2869">랩</span><span class="sxs-lookup"><span data-stu-id="56085-2869">Lab</span></span>

* <span data-ttu-id="56085-2870">`az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2870">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="56085-2871">`az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2871">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-2872">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-2872">Monitor</span></span>

* <span data-ttu-id="56085-2873">`monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)</span><span class="sxs-lookup"><span data-stu-id="56085-2873">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="56085-2874">`monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2874">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="56085-2875">`monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2875">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="56085-2876">`monitor metric-defintions list`에서 `monitor metrics list-definitions`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2876">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="56085-2877">`monitor alert-rules`에서 `monitor alert`로 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="56085-2877">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="56085-2878">`monitor alert create`에 대한 변경 내용:</span><span class="sxs-lookup"><span data-stu-id="56085-2878">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="56085-2879">`condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2879">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="56085-2880">다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2880">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="56085-2881">`location`은 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2881">`location` no longer required</span></span>
  * <span data-ttu-id="56085-2882">대상에 대한 이름 및 ID 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2882">Add name and ID support for target</span></span>
  * <span data-ttu-id="56085-2883">`--alert-rule-resource-name`이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2883">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="56085-2884">이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2884">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="56085-2885">`description`은 제공된 조건에 따라 기본적으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2885">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="56085-2886">새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2886">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="56085-2887">`monitor metric` 명령에 대해 이름 또는 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2887">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="56085-2888">`monitor alert rule update`에 편의 인수 및 예제가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2888">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="56085-2889">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-2889">Network</span></span>

* <span data-ttu-id="56085-2890">`list-private-access-services` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2890">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="56085-2891">`vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2891">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="56085-2892">`application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2892">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="56085-2893">`--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2893">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="56085-2894">`application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2894">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="56085-2895">`application-gateway redirect-config` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2895">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="56085-2896">`application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="56085-2896">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="56085-2897">`application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="56085-2897">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="56085-2898">`application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="56085-2898">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="56085-2899">`application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="56085-2899">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="56085-2900">`application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="56085-2900">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="56085-2901">`--no-wait`에 대한 지원이 `application-gateway url-path-map rule delete`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2901">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="56085-2902">`application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="56085-2902">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="56085-2903">`application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="56085-2903">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="56085-2904">`--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2904">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="56085-2905">`nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2905">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="56085-2906">`--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --DNS 서버에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2906">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="56085-2907">`local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2907">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="56085-2908">`--dns-servers`에 대한 지원이 `vnet update`에 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2908">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="56085-2909">`express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2909">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="56085-2910">`--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2910">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="56085-2911">`network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2911">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="56085-2912">`network list-usages`에 대한 출력 형식 지정이 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2912">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="56085-2913">하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2913">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="56085-2914">하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2914">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="56085-2915">하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2915">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="56085-2916">하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨</span><span class="sxs-lookup"><span data-stu-id="56085-2916">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="56085-2917">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-2917">Profile</span></span>

* <span data-ttu-id="56085-2918">관리 ID를 사용한 VM 내부 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2918">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="56085-2919">`account show`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2919">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="56085-2920">'--expanded-view'를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="56085-2920">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="56085-2921">원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2921">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="56085-2922">연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2922">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="56085-2923">RDBMS</span><span class="sxs-lookup"><span data-stu-id="56085-2923">RDBMS</span></span>

* <span data-ttu-id="56085-2924">구독을 통해 서버를 나열하도록 지원합니다(#3417).</span><span class="sxs-lookup"><span data-stu-id="56085-2924">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="56085-2925">`% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).</span><span class="sxs-lookup"><span data-stu-id="56085-2925">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="56085-2926">고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).</span><span class="sxs-lookup"><span data-stu-id="56085-2926">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="56085-2927">MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)</span><span class="sxs-lookup"><span data-stu-id="56085-2927">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="56085-2928">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-2928">Resource</span></span>

* <span data-ttu-id="56085-2929">`group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2929">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="56085-2930">`--parameters KEY=VALUE` 구문 분석이 향상됨</span><span class="sxs-lookup"><span data-stu-id="56085-2930">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="56085-2931">`@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2931">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="56085-2932">`resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2932">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="56085-2933">일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).</span><span class="sxs-lookup"><span data-stu-id="56085-2933">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="56085-2934">`lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2934">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="56085-2935">템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).</span><span class="sxs-lookup"><span data-stu-id="56085-2935">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="56085-2936">`KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2936">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="56085-2937">역할</span><span class="sxs-lookup"><span data-stu-id="56085-2937">Role</span></span>

* <span data-ttu-id="56085-2938">`create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2938">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="56085-2939">서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 애플리케이션이 정리됨(#3610)</span><span class="sxs-lookup"><span data-stu-id="56085-2939">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="56085-2940">`app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨</span><span class="sxs-lookup"><span data-stu-id="56085-2940">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="56085-2941">`--expanded-view`를 사용할 때 사용 중단 경고가 표시됨</span><span class="sxs-lookup"><span data-stu-id="56085-2941">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="56085-2942">`create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2942">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="56085-2943">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="56085-2943">Service Fabric</span></span>
* <span data-ttu-id="56085-2944">업로드 시 애플리케이션의 대형 파일을 자르는 문제가 해결되었습니다(#3666).</span><span class="sxs-lookup"><span data-stu-id="56085-2944">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="56085-2945">Service Fabric 명령에 대한 테스트가 추가됨(#3424)</span><span class="sxs-lookup"><span data-stu-id="56085-2945">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="56085-2946">다양한 Service Fabric 명령이 수정됨(#3234)</span><span class="sxs-lookup"><span data-stu-id="56085-2946">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="56085-2947">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-2947">SQL</span></span>

* <span data-ttu-id="56085-2948">중단된 `sql server create` `--identity` 매개 변수가 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2948">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="56085-2949">`sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨</span><span class="sxs-lookup"><span data-stu-id="56085-2949">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="56085-2950">`sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-2950">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="56085-2951">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-2951">Storage</span></span>

* <span data-ttu-id="56085-2952">`storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)</span><span class="sxs-lookup"><span data-stu-id="56085-2952">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="56085-2953">HTTPS 전용 스토리지 계정 만들기 사용</span><span class="sxs-lookup"><span data-stu-id="56085-2953">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="56085-2954">스토리지 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)</span><span class="sxs-lookup"><span data-stu-id="56085-2954">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="56085-2955">CORS add(#3638)(#3362)의 예외 메시지가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2955">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="56085-2956">download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)</span><span class="sxs-lookup"><span data-stu-id="56085-2956">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="56085-2957">Blob download batch dryrun 문제가 해결됨(#3640)(#3592)</span><span class="sxs-lookup"><span data-stu-id="56085-2957">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="56085-2958">VM</span><span class="sxs-lookup"><span data-stu-id="56085-2958">VM</span></span>

* <span data-ttu-id="56085-2959">NSG 구성이 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2959">Support configuring nsg</span></span>
* <span data-ttu-id="56085-2960">DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-2960">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="56085-2961">관리되는 서비스 ID가 지원됨</span><span class="sxs-lookup"><span data-stu-id="56085-2961">Support managed service identities</span></span>
* <span data-ttu-id="56085-2962">기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 수정됨</span><span class="sxs-lookup"><span data-stu-id="56085-2962">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="56085-2963">`vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨</span><span class="sxs-lookup"><span data-stu-id="56085-2963">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="56085-2964">2017년 5월 10일</span><span class="sxs-lookup"><span data-stu-id="56085-2964">May 10, 2017</span></span>

<span data-ttu-id="56085-2965">버전 2.0.6</span><span class="sxs-lookup"><span data-stu-id="56085-2965">Version 2.0.6</span></span>

* <span data-ttu-id="56085-2966">documentdb가 cosmosdb로 바뀜</span><span class="sxs-lookup"><span data-stu-id="56085-2966">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="56085-2967">rdbms(mysql, postgres) 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2967">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="56085-2968">Data Lake Analytics 및 Data Lake Store 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="56085-2968">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="56085-2969">Cognitive Services 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="56085-2969">Include Cognitive Services module</span></span>
* <span data-ttu-id="56085-2970">Service Fabric 모듈 포함</span><span class="sxs-lookup"><span data-stu-id="56085-2970">Include Service Fabric module</span></span>
* <span data-ttu-id="56085-2971">대화형 모듈(az-shell 이름 바꾸기) 포함</span><span class="sxs-lookup"><span data-stu-id="56085-2971">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="56085-2972">CDN 명령에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2972">Add support for CDN commands</span></span>
* <span data-ttu-id="56085-2973">컨테이너 모듈 제거</span><span class="sxs-lookup"><span data-stu-id="56085-2973">Remove Container module</span></span>
* <span data-ttu-id="56085-2974">'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="56085-2974">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="56085-2975">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="56085-2975">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="56085-2976">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-2976">Core</span></span>

* <span data-ttu-id="56085-2977">core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록</span><span class="sxs-lookup"><span data-stu-id="56085-2977">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="56085-2978">perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="56085-2978">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="56085-2979">hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="56085-2979">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="56085-2980">향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="56085-2980">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="56085-2981">‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="56085-2981">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="56085-2982">login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="56085-2982">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="56085-2983">core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="56085-2983">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="56085-2984">core: accessTokens.json의 파일 경로가 env var을 통해 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="56085-2984">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="56085-2985">core: 구성된 기본값이 선택 인수에 적용되도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="56085-2985">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="56085-2986">core: 성능 향상</span><span class="sxs-lookup"><span data-stu-id="56085-2986">core: Improved performance</span></span>
* <span data-ttu-id="56085-2987">core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원</span><span class="sxs-lookup"><span data-stu-id="56085-2987">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="56085-2988">core: 클라우드 구성 - '관리' 엔드포인트가 설정되지 않은 경우 '리소스 관리자' 엔드포인트 사용</span><span class="sxs-lookup"><span data-stu-id="56085-2988">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="56085-2989">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-2989">ACS</span></span>

* <span data-ttu-id="56085-2990">마스터 및 에이전트 수를 문자열이 아닌 정수로 수정</span><span class="sxs-lookup"><span data-stu-id="56085-2990">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="56085-2991">비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출</span><span class="sxs-lookup"><span data-stu-id="56085-2991">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="56085-2992">시험 실행 유효성 검사에 대해 'az acs create --validate' 노출</span><span class="sxs-lookup"><span data-stu-id="56085-2992">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="56085-2993">규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="56085-2993">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-2994">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-2994">AppService</span></span>

* <span data-ttu-id="56085-2995">functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)</span><span class="sxs-lookup"><span data-stu-id="56085-2995">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="56085-2996">"appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가</span><span class="sxs-lookup"><span data-stu-id="56085-2996">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="56085-2997">"az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)</span><span class="sxs-lookup"><span data-stu-id="56085-2997">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="56085-2998">웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출</span><span class="sxs-lookup"><span data-stu-id="56085-2998">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="56085-2999">"webapp list-runtimes" 노출</span><span class="sxs-lookup"><span data-stu-id="56085-2999">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="56085-3000">연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="56085-3000">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="56085-3001">미리 보기를 사용한 슬롯 전환 지원</span><span class="sxs-lookup"><span data-stu-id="56085-3001">support slot swap with preview</span></span>
* <span data-ttu-id="56085-3002">AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="56085-3002">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="56085-3003">인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="56085-3003">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="56085-3004">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="56085-3004">CosmosDB</span></span>

* <span data-ttu-id="56085-3005">documentdb 모듈을 cosmosdb로 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="56085-3005">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="56085-3006">Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-3006">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="56085-3007">데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-3007">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="56085-3008">새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-3008">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="56085-3009">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="56085-3009">Data Lake Analytics</span></span>

* <span data-ttu-id="56085-3010">작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3010">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="56085-3011">새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3011">Add support for new catalog item type: package.</span></span> <span data-ttu-id="56085-3012">`az dla catalog package`를 통해 액세스</span><span class="sxs-lookup"><span data-stu-id="56085-3012">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="56085-3013">데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):</span><span class="sxs-lookup"><span data-stu-id="56085-3013">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="56085-3014">테이블</span><span class="sxs-lookup"><span data-stu-id="56085-3014">Table</span></span>
  * <span data-ttu-id="56085-3015">테이블 반환 함수</span><span class="sxs-lookup"><span data-stu-id="56085-3015">Table valued function</span></span>
  * <span data-ttu-id="56085-3016">보기</span><span class="sxs-lookup"><span data-stu-id="56085-3016">View</span></span>
  * <span data-ttu-id="56085-3017">테이블 통계.</span><span class="sxs-lookup"><span data-stu-id="56085-3017">Table Statistics.</span></span> <span data-ttu-id="56085-3018">테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있음</span><span class="sxs-lookup"><span data-stu-id="56085-3018">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="56085-3019">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="56085-3019">Data Lake Store</span></span>

* <span data-ttu-id="56085-3020">기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 보다 나은 지원 제공</span><span class="sxs-lookup"><span data-stu-id="56085-3020">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="56085-3021">패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="56085-3021">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="56085-3022">액세스 표시에 대한 도움말 누락.</span><span class="sxs-lookup"><span data-stu-id="56085-3022">missed help for access show.</span></span> <span data-ttu-id="56085-3023">추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3023">adding it.</span></span> <span data-ttu-id="56085-3024">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="56085-3024">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="56085-3025">찾기</span><span class="sxs-lookup"><span data-stu-id="56085-3025">Find</span></span>

* <span data-ttu-id="56085-3026">검색 결과 개선 및 검색 인덱스의 버전 관리 허용</span><span class="sxs-lookup"><span data-stu-id="56085-3026">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="56085-3027">KeyVault</span><span class="sxs-lookup"><span data-stu-id="56085-3027">KeyVault</span></span>

* <span data-ttu-id="56085-3028">BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3028">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="56085-3029">BC: --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 `keyvault certificate create`에서 삭제</span><span class="sxs-lookup"><span data-stu-id="56085-3029">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="56085-3030">`keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3030">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="56085-3031">'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3031">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="56085-3032">pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="56085-3032">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="56085-3033">랩</span><span class="sxs-lookup"><span data-stu-id="56085-3033">Lab</span></span>

* <span data-ttu-id="56085-3034">랩 환경에 대한 create, show, delete 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3034">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="56085-3035">랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3035">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="56085-3036">`az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM 필터링</span><span class="sxs-lookup"><span data-stu-id="56085-3036">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="56085-3037">편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냄</span><span class="sxs-lookup"><span data-stu-id="56085-3037">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="56085-3038">랩 내에서 비밀을 관리하는 명령을 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3038">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="56085-3039">모니터</span><span class="sxs-lookup"><span data-stu-id="56085-3039">Monitor</span></span>

* <span data-ttu-id="56085-3040">버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="56085-3040">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="56085-3041">버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="56085-3041">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="56085-3042">네트워크</span><span class="sxs-lookup"><span data-stu-id="56085-3042">Network</span></span>

* <span data-ttu-id="56085-3043">`network watcher test-connectivity` 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3043">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="56085-3044">`network watcher packet-capture create`의 `--filters` 매개 변수 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3044">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="56085-3045">Application Gateway 연결 드레이닝에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3045">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="56085-3046">Application Gateway WAF 규칙 집합 구성에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3046">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="56085-3047">ExpressRoute 경로 필터 및 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3047">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="56085-3048">TrafficManager 지리적 라우팅에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3048">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="56085-3049">VPN 연결 정책 기반 트래픽 선택기에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3049">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="56085-3050">VPN 연결 IPSec 정책에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3050">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="56085-3051">`--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create` 관련 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3051">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="56085-3052">활성-활성 VNet 게이트웨이에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3052">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="56085-3053">`network vpn-connection list/show` 명령의 출력에서 null 값 제거</span><span class="sxs-lookup"><span data-stu-id="56085-3053">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="56085-3054">BC: `vpn-connection create`의 출력에서 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3054">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="56085-3055">'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3055">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="56085-3056">`dns zone import`에서 레코드를 제대로 가져오지 않는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3056">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="56085-3057">`traffic-manager endpoint update`가 작동하지 않는 버그를 수정</span><span class="sxs-lookup"><span data-stu-id="56085-3057">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="56085-3058">'network watcher' 미리 보기 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3058">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="56085-3059">프로필</span><span class="sxs-lookup"><span data-stu-id="56085-3059">Profile</span></span>

* <span data-ttu-id="56085-3060">구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="56085-3060">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="56085-3061">az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="56085-3061">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="56085-3062">Redis</span><span class="sxs-lookup"><span data-stu-id="56085-3062">Redis</span></span>

* <span data-ttu-id="56085-3063">redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3063">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="56085-3064">'update-settings' 명령은 더 이상 사용하지 않음</span><span class="sxs-lookup"><span data-stu-id="56085-3064">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="56085-3065">리소스</span><span class="sxs-lookup"><span data-stu-id="56085-3065">Resource</span></span>

* <span data-ttu-id="56085-3066">managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="56085-3066">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="56085-3067">'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="56085-3067">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="56085-3068">일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="56085-3068">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="56085-3069">리소스 구문 분석 및 API 버전 조회를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3069">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="56085-3070">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="56085-3070">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="56085-3071">az lock update에 대한 문서를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3071">Add docs for az lock update.</span></span> <span data-ttu-id="56085-3072">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="56085-3072">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="56085-3073">존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3073">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="56085-3074">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="56085-3074">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="56085-3075">[Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3075">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="56085-3076">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="56085-3076">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="56085-3077">parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="56085-3077">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="56085-3078">역할</span><span class="sxs-lookup"><span data-stu-id="56085-3078">Role</span></span>

* <span data-ttu-id="56085-3079">create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="56085-3079">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="56085-3080">RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="56085-3080">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="56085-3081">role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="56085-3081">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="56085-3082">create-for-rbac: 사용자 제공 암호가 선택되도록 보장</span><span class="sxs-lookup"><span data-stu-id="56085-3082">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="56085-3083">SQL</span><span class="sxs-lookup"><span data-stu-id="56085-3083">SQL</span></span>

* <span data-ttu-id="56085-3084">az sql server list-usages 및 az sql db list-usages 명령이 추가됨</span><span class="sxs-lookup"><span data-stu-id="56085-3084">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="56085-3085">SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="56085-3085">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="56085-3086">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-3086">Storage</span></span>

* <span data-ttu-id="56085-3087">`storage account create`의 리소스 그룹 위치에 대한 기본 위치</span><span class="sxs-lookup"><span data-stu-id="56085-3087">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="56085-3088">증분 blob 복사에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3088">Add support for incremental blob copy</span></span>
* <span data-ttu-id="56085-3089">큰 블록 blob 업로드에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3089">Add support for large block blob upload</span></span>
* <span data-ttu-id="56085-3090">업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경</span><span class="sxs-lookup"><span data-stu-id="56085-3090">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="56085-3091">VM</span><span class="sxs-lookup"><span data-stu-id="56085-3091">VM</span></span>

* <span data-ttu-id="56085-3092">avail-set: UD&FD 도메인 수를 옵션으로 지정</span><span class="sxs-lookup"><span data-stu-id="56085-3092">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="56085-3093">참고: 소버린 클라우드의 VM 명령 다음을 비롯한 관리 디스크 관련 기능을 피하십시오.</span><span class="sxs-lookup"><span data-stu-id="56085-3093">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="56085-3094">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="56085-3094">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="56085-3095">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="56085-3095">az vm/vmss disk</span></span>
  3. <span data-ttu-id="56085-3096">"az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3096">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="56085-3097">vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선</span><span class="sxs-lookup"><span data-stu-id="56085-3097">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="56085-3098">vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="56085-3098">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="56085-3099">2017년 4월 3일</span><span class="sxs-lookup"><span data-stu-id="56085-3099">April 3, 2017</span></span>

<span data-ttu-id="56085-3100">버전 2.0.2</span><span class="sxs-lookup"><span data-stu-id="56085-3100">Version 2.0.2</span></span>

<span data-ttu-id="56085-3101">이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 릴리스되었습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3101">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="56085-3102">핵심</span><span class="sxs-lookup"><span data-stu-id="56085-3102">Core</span></span>

* <span data-ttu-id="56085-3103">기본 목록에 acr, 랩, 모니터 및 찾기 모듈 추가</span><span class="sxs-lookup"><span data-stu-id="56085-3103">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="56085-3104">로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="56085-3104">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="56085-3105">로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="56085-3105">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="56085-3106">더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="56085-3106">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="56085-3107">코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="56085-3107">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="56085-3108">누락된 템플릿 매개 변수를 요청하는 프롬프트 추가.</span><span class="sxs-lookup"><span data-stu-id="56085-3108">Add prompting for missing template parameters.</span></span> <span data-ttu-id="56085-3109">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="56085-3109">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="56085-3110">기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원</span><span class="sxs-lookup"><span data-stu-id="56085-3110">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="56085-3111">특정 테넌트에 대한 로그인 지원</span><span class="sxs-lookup"><span data-stu-id="56085-3111">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="56085-3112">ACS</span><span class="sxs-lookup"><span data-stu-id="56085-3112">ACS</span></span>

* <span data-ttu-id="56085-3113">[ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="56085-3113">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="56085-3114">ssh 키 암호 프롬프트 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="56085-3114">Add support for ssh key password prompting.</span></span> <span data-ttu-id="56085-3115">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="56085-3115">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="56085-3116">windows 클러스터 지원 추가.</span><span class="sxs-lookup"><span data-stu-id="56085-3116">Add support for windows clusters.</span></span> <span data-ttu-id="56085-3117">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="56085-3117">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="56085-3118">소유자 역할에서 참가자 역할로 전환.</span><span class="sxs-lookup"><span data-stu-id="56085-3118">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="56085-3119">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="56085-3119">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="56085-3120">AppService</span><span class="sxs-lookup"><span data-stu-id="56085-3120">AppService</span></span>

* <span data-ttu-id="56085-3121">appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="56085-3121">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="56085-3122">appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="56085-3122">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="56085-3123">appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="56085-3123">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="56085-3124">AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="56085-3124">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="56085-3125">DataLake</span><span class="sxs-lookup"><span data-stu-id="56085-3125">DataLake</span></span>

* <span data-ttu-id="56085-3126">Data Lake Analytics 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-3126">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="56085-3127">Data Lake Store 모듈의 초기 릴리스</span><span class="sxs-lookup"><span data-stu-id="56085-3127">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="56085-3128">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="56085-3128">DocuemntDB</span></span>

* <span data-ttu-id="56085-3129">DocumentDB: 문자열 목록에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="56085-3129">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="56085-3130">VM</span><span class="sxs-lookup"><span data-stu-id="56085-3130">VM</span></span>

* <span data-ttu-id="56085-3131">[Compute] 가상 머신 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="56085-3131">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="56085-3132">[VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="56085-3132">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="56085-3133">VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="56085-3133">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="56085-3134">wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="56085-3134">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="56085-3135">가상 머신 확장 집합: vm의 인스턴스 보기를 나열하는 \* 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="56085-3135">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="56085-3136">추가 - VM 및 가상 머신 확장 집합의 암호([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="56085-3136">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="56085-3137">특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="56085-3137">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="56085-3138">2017년 2월 27일</span><span class="sxs-lookup"><span data-stu-id="56085-3138">February 27, 2017</span></span>

<span data-ttu-id="56085-3139">버전 2.0.0</span><span class="sxs-lookup"><span data-stu-id="56085-3139">Version 2.0.0</span></span>

<span data-ttu-id="56085-3140">이 Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다. 일반 공급은 다음 명령 모듈에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3140">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="56085-3141">컨테이너 서비스(acs)</span><span class="sxs-lookup"><span data-stu-id="56085-3141">Container Service (acs)</span></span>
- <span data-ttu-id="56085-3142">Compute(Resource Manager, VM, 가상 머신 확장 집합, Managed Disks 포함)</span><span class="sxs-lookup"><span data-stu-id="56085-3142">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="56085-3143">네트워킹</span><span class="sxs-lookup"><span data-stu-id="56085-3143">Networking</span></span>
- <span data-ttu-id="56085-3144">스토리지</span><span class="sxs-lookup"><span data-stu-id="56085-3144">Storage</span></span>

<span data-ttu-id="56085-3145">이러한 명령 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA에서 지원됩니다. Microsoft 지원 부서 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 열 수 있습니다. [azure-cli 태그를 사용하여 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대한 질문을 하거나 [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)에 있는 제품 팀에 문의할 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3145">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="56085-3146">이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3146">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="56085-3147">CLI 버전을 확인하려면 `az --version`을 사용합니다. 출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3147">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="56085-3148">명령 모듈 중 일부에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다. 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3148">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="56085-3149">또한 야간 미리 보기 CLI 빌드가 있습니다. 자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="56085-3149">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="56085-3150">다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="56085-3150">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="56085-3151">[github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고</span><span class="sxs-lookup"><span data-stu-id="56085-3151">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="56085-3152">제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의</span><span class="sxs-lookup"><span data-stu-id="56085-3152">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="56085-3153">`az feedback` 명령을 사용하여 명령줄에서 피드백 제공</span><span class="sxs-lookup"><span data-stu-id="56085-3153">Provide feedback from the command line with the `az feedback` command</span></span>


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
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0 릴리스 정보

## <a name="may-10-2017"></a>2017년 5월 10일

버전 2.0.6

* documentdb가 cosmosdb로 바뀜
* rdbms(mysql, postgres) 추가
* Data Lake Analytics 및 Data Lake Store 모듈을 포함합니다.
* Cognitive Services 모듈을 포함합니다.
* Service Fabric 모듈을 포함합니다.
* 대화형 모듈(az-shell 이름 바꾸기)을 포함합니다.
* CDN 명령에 대한 지원을 추가합니다.
* 컨테이너 모듈을 제거합니다.
* 'az --version'에 대한 바로 가기로 'az -v' 추가([#2926](https://github.com/Azure/azure-cli/issues/2926))
* 패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))

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

### <a name="core"></a>코어

* core: 등록되지 않은 공급자에 의한 예외를 캡처하고 자동으로 등록   
* perf: 프로세스가 종료될 때까지 adal 토큰 캐시를 메모리에 유지([#2603](https://github.com/Azure/azure-cli/issues/2603))
* hex fingerprint -o tsv에 의해 반환된 바이트 수정([#3053](https://github.com/Azure/azure-cli/issues/3053))
* 향상된 Key Vault 인증서 다운로드 및 AAD SP 통합([#3003](https://github.com/Azure/azure-cli/issues/3003))
* ‘az —version’에 Python 위치 추가([#2986](https://github.com/Azure/azure-cli/issues/2986))
* login: 구독이 없을 때 로그인 지원([#2929](https://github.com/Azure/azure-cli/issues/2929))
* core: 서비스 주체를 사용하여 두 번 로그인할 때 오류 수정([#2800](https://github.com/Azure/azure-cli/issues/2800))
* core: env var을 통해 accessTokens.json의 파일 경로를 구성 가능하도록 허용([#2605](https://github.com/Azure/azure-cli/issues/2605))
* core: 구성된 기본값이 선택적 인수에 적용하도록 허용([#2703](https://github.com/Azure/azure-cli/issues/2703))
* core: 향상된 성능
* core: 사용자 지정 CA 인증서 - REQUESTS_CA_BUNDLE 환경 변수 설정 지원
* core: 클라우드 구성 - '관리' 끝점을 설정하지 않은 경우 '리소스 관리자' 끝점 사용

### <a name="acs"></a>ACS

* 마스터 및 에이전트 수를 문자열이 아닌 정수로 수정
* 비동기 작성에 대해 'az acs create --no-wait' 및 'az acs wait' 노출
* 시험 실행 유효성 검사에 대해 'az acs create --validate' 노출
* 규모 명령에 대한 PUT 호출 전에 Windows 프로필 제거([#2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp: 전체 함수 앱 지원 추가(create, show, list, delete, hostname, ssl 등 포함)
* "appservice web source-control config"에 연속 배달 옵션으로 팀 서비스(vsts) 추가
* "az appservice web"을 대신할 "az webapp" 만들기(이전 버전과의 호환성을 위해 "az appservice web"을 두 릴리스에서 유지함)
* 웹앱 만들기 시 배포 및 “런타임 스택”을 구성하기 위한 인수 노출
* "webapp list-runtimes" 노출
* 연결 문자열 구성 지원([#2647](https://github.com/Azure/azure-cli/issues/2647))
* 미리 보기를 사용한 슬롯 전환 지원
* AppService 서비스 명령의 폴란드어 오류([#2948](https://github.com/Azure/azure-cli/issues/2948))
* 인증서 작업에 대해 App Service 계획의 리소스 그룹 사용([#2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* documentdb 모듈 이름을 cosmosdb로 바꿈
* Documentdb 데이터 평면에 API: 데이터베이스 및 컬렉션 관리에 대한 지원이 추가됨
* 데이터베이스 계정에 대해 자동 장애 조치(Failover)를 사용하도록 설정하기 위한 지원이 추가됨
* 새 일관성 정책 ConsistentPrefix에 대한 지원이 추가됨

### <a name="data-lake-analytics"></a>데이터 레이크 분석

* 작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.
* 새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다. `az dla catalog package`를 통해 액세스
* 데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):

  * 테이블
  * 테이블 반환 함수
  * 보기
  * 테이블 통계. 테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.

### <a name="data-lake-store"></a>데이터 레이크 저장소

* 기본 파일 시스템 SDK 버전을 업데이트하여 서버 쪽 제한 시나리오 처리에 대해 보다 나은 지원을 제공합니다.
* 패키지 로드 및 명령 실행의 성능 개선([#2819](https://github.com/Azure/azure-cli/issues/2819))
* 액세스 표시에 대한 도움말 누락. 추가됩니다. ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>찾기

* 검색 결과 개선 및 검색 인덱스의 버전 관리 허용

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` 문자열 또는 이진 파일의 -e를 PEM 또는 DER로 변경하여 옵션을 보다 잘 나타냅니다.
* BC: `keyvault certificate create` 앞에 있는 --expires 및 --not-before 매개 변수는 서비스에서 지원되지 않으므로 제거합니다.
* `keyvault certificate create`에 --validity 매개 변수를 추가하여 --policy의 값을 선택적으로 재정의합니다.
* 'expires' 및 'not_before'가 노출되지만 'validity_in_months'는 노출되지 않는 `keyvault certificate get-default-policy`의 문제를 수정합니다.
* pem 및 pfx 가져오기에 대한 KeyVault 수정([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>랩

* 랩 환경에 대한 create, show, delete 및 list 명령 추가
* 랩에서 ARM 템플릿을 보기 위해 show 및 list 명령 추가
* `az lab vm list`에 --environment 플래그를 추가하여 랩의 환경별로 VM을 필터링합니다.
* 편의성 명령 `az lab formula export-artifacts`를 추가하여 랩 수식 내에 아티팩트 스캐폴드를 내보냅니다.
* 랩 내에서 비밀을 관리하는 명령을 추가합니다.

### <a name="monitor"></a>모니터

* 버그 수정: JSON 문자열을 사용하도록 `az alert-rules create`의 `--actions` 모델링([#3009](https://github.com/Azure/azure-cli/issues/3009))
* 버그 수정 - 진단 설정 만들기가 show 명령의 로그/메트릭을 수락하지 않음([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>네트워크

* `network watcher test-connectivity` 명령을 추가합니다.
* `network watcher packet-capture create`에 대한 `--filters` 매개 변수 지원을 추가합니다.
* Application Gateway 연결 드레이닝에 대한 지원을 추가합니다.
* Application Gateway WAF 규칙 집합 구성에 대한 지원을 추가합니다.
* ExpressRoute 경로 필터 및 규칙에 대한 지원을 추가합니다.
* TrafficManager 지리적 라우팅에 대한 지원을 추가합니다.
* VPN 연결 정책 기반 트래픽 선택기에 대한 지원을 추가합니다.
* VPN 연결 IPSec 정책에 대한 지원을 추가합니다.
* `--no-wait` 또는 `--validate` 매개 변수를 사용할 때 `vpn-connection create`를 사용하여 버그를 수정합니다.
* 활성-활성 VNet 게이트웨이에 대한 지원 추가
* `network vpn-connection list/show` 명령의 출력에서 null 값 제거
* BC: `vpn-connection create`의 출력에서 버그 수정 
* 'vpn-connection create'의 '--key-length' 인수가 제대로 구문 분석되지 않는 버그를 수정합니다.
* 레코드가 제대로 가져와지지 않는 `dns zone import`의 버그를 수정합니다.
* `traffic-manager endpoint update`가 작동하지 않는 버그를 수정합니다.
* 'network watcher' 미리 보기 명령을 추가합니다.

### <a name="profile"></a>프로필

* 구독이 없을 때 로그인 지원([#2560](https://github.com/Azure/azure-cli/issues/2560))
* az account set --subscription에서 짧은 매개 변수 이름 지원 ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* redis cache에 대해 규모를 조정하는 기능도 추가하는 update 명령 추가
* 'update-settings' 명령은 더 이상 사용되지 않습니다.

### <a name="resource"></a>리소스

* managedapp 및 managedapp definition 명령 추가([#2985](https://github.com/Azure/azure-cli/issues/2985))
* 'provider operation' 명령 지원([#2908](https://github.com/Azure/azure-cli/issues/2908))
* 일반 리소스 만들기 지원([#2606](https://github.com/Azure/azure-cli/issues/2606))
* 리소스 구문 분석 및 API 버전 조회를 수정합니다. ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* az lock update에 대한 문서를 추가합니다. ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* 존재하지 않는 그룹의 리소스를 나열하려고 할 때 오류가 발생합니다. ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] VMSS 및 VM 가용성 집합 업데이트 문제를 해결합니다. ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* parent-resource-path가 None인 경우 잠금 만들기 및 삭제 수정([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>역할

* create-for-rbac: SP의 종료 날짜가 인증서의 만료 날짜를 초과하지 않도록 보장([#2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC: 'ad group'에 대한 모든 지원 추가([#2016](https://github.com/Azure/azure-cli/issues/2016))
* role: 역할 정의 업데이트에 대한 문제 수정([#2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac: 사용자 제공 암호가 선택되도록 보장

### <a name="sql"></a>SQL

* az sql server list-usages 및 az sql db list-usages 명령이 추가되었습니다.
* SQL - 리소스 공급자에 직접 연결하는 기능([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>저장소

* 기본 위치를 `storage account create`에 대한 리소스 그룹 위치로 지정합니다.
* 증분 blob 복사에 대한 지원 추가
* 큰 블록 blob 업로드에 대한 지원 추가
* 업로드할 파일이 200GB보다 큰 경우 블록 크기를 100MB로 변경

### <a name="vm"></a>VM

* avail-set: UD&FD 도메인 수를 옵션으로 지정

  note: 독립 클라우드의 VM 명령. 다음을 비롯한 관리되는 디스크 관련 기능을 피하세요.
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. "az vm/vmss create" 내에 "—use-unmanaged-disk"를 사용하여 관리되는 디스크를 피합니다. 다른 명령은 작동합니다.
* vm/vmss: ssh 키 쌍을 생성할 때 경고 텍스트 개선
* vm/vmss: 계획 정보가 필요한 marketplace 이미지에서 만들기 지원([#1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>2017년 4월 3일

버전 2.0.2

이 릴리스에서는 ACR, Batch, KeyVault 및 SQL 구성 요소가 출시되었습니다.

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

### <a name="core"></a>코어

* 기본 목록에 acr, 랩, 모니터 및 찾기 모듈을 추가합니다.
* 로그인: 잘못된 테넌트 건너뛰기([#2634](https://github.com/Azure/azure-cli/pull/2634))
* 로그인: 상태가 "사용"인 구독에 기본 구독 설정([#2575](https://github.com/Azure/azure-cli/pull/2575))
* 더 많은 명령에 wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))
* 코어: 인증서가 있는 서비스 주체를 사용하여 로그인 지원([#2457](https://github.com/Azure/azure-cli/pull/2457))
* 누락된 템플릿 매개 변수를 요청하는 프롬프트 추가. ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* 기본 리소스 그룹, 기본 웹, 기본 vm 등과 같은 공통 인수에 대한 기본값 설정 지원
* 특정 테넌트에 대한 로그인 지원
 
### <a name="acs"></a>ACS

* [ACS] 기본 ACS 클러스터 구성 지원 추가([#2554](https://github.com/Azure/azure-cli/pull/2554))
* ssh 키 암호 프롬프트 지원 추가. ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* windows 클러스터 지원 추가. ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* 소유자 역할에서 참가자 역할로 전환. ([#2321](https://github.com/Azure/azure-cli/pull/2321))
 
### <a name="appservice"></a>AppService

* appservice: DNS A 레코드에 사용된 외부 ip 주소 가져오기 지원([#2627](https://github.com/Azure/azure-cli/pull/2627))
* appservice: 와일드카드 인증서 바인딩 지원([#2625](https://github.com/Azure/azure-cli/pull/2625))
* appservice: 게시 프로필 나열 지원([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService - 구성 후 원본 제어 동기화 트리거([#2326](https://github.com/Azure/azure-cli/pull/2326))
 
### <a name="datalake"></a>DataLake

* Data Lake Analytics 모듈의 초기 릴리스.
* Data Lake Store 모듈의 초기 릴리스.
 
### <a name="docuemntdb"></a>DocuemntDB

* DocumentDB: 연결 문자열 나열에 대한 지원 추가([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] 가상 컴퓨터 확장 집합 만들기에 AppGateway 지원 추가([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] 향상된 디스크 캐싱 지원([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: 포털에서 사용하는 자격 증명 유효성 검사 논리 통합([#2537](https://github.com/Azure/azure-cli/pull/2537))
* wait 명령 및 --no-wait 지원 추가([#2524](https://github.com/Azure/azure-cli/pull/2524))
* 가상 컴퓨터 확장 집합: vm의 인스턴스 보기를 나열하는 * 지원([#2467](https://github.com/Azure/azure-cli/pull/2467))
* VM 및 가상 컴퓨터 확장 집합에 --secrets 추가([#2212}(https://github.com/Azure/azure-cli/pull/2212))
* 특수 VHD로 VM 만들기 허용([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>2017년 2월 27일

버전 2.0.0

Azure CLI 2.0 릴리스는 최초의 "일반 공급" 릴리스입니다.
일반 공급은 다음 명령 모듈에 적용됩니다.
- 컨테이너 서비스(acs)
- Compute(Resource Manager, VM, 가상 컴퓨터 확장 집합, Managed Disks 포함)
- 네트워킹
- 저장소

이러한 명령은 모듈은 프로덕션 환경에서 사용할 수 있으며 표준 Microsoft SLA를 지원합니다.
Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 직접 문제를 개설할 수 있습니다.
[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다.
`az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.

이러한 모듈의 명령은 안정적이므로 이 Azure CLI 버전의 이후 릴리스에서 구문이 변경되지는 않을 것입니다.

CLI 버전을 확인하려면 `az --version`을 사용합니다.
출력은 CLI 자체 버전(이 릴리스에서는 2.0.0), 개별 명령 모듈, 현재 사용 중인 Python 및 GCC CLI의 버전을 나열합니다.

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
> 일부 명령 모듈에는 "b*n*" 또는 "rc*n*" 접미사가 있습니다.
> 이러한 명령 모듈은 아직 미리 보기이며 나중에 일반 공급될 것입니다.

CLI 야간 미리 보기 빌드도 있습니다.
자세한 내용은 [야간 빌드 받기](https://github.com/Azure/azure-cli#nightly-builds) 및 [개발자 설치 및 코드 기여](https://github.com/Azure/azure-cli#developer-setup)에 대한 지침을 참조하세요.

다음과 같은 방법으로 야간 미리 보기 빌드의 문제를 보고할 수 있습니다.
- [github 문제 목록](https://github.com/azure/azure-cli/issues/)에서 문제 보고
- 제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.
- `az feedback` 명령을 사용하여 명령줄에서 피드백 제공.


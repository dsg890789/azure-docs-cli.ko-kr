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
ms.openlocfilehash: e02b84891f4bf60cde12591b8e85987f4b3c9e79
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2017
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0 릴리스 정보

## <a name="december-5-2017"></a>2017년 12월 5일

버전 2.0.22

* `az component` 명령이 제거되었습니다. 대신 `az extension`을 사용하세요.

### <a name="core"></a>코어
* `AZURE_US_GOV_CLOUD` AAD 권한 끝점이 login.microsoftonline.com에서 login.microsoftonline.us로 수정됨
* 원격 분석이 지속적으로 다시 전송되는 문제가 해결됨

### <a name="acs"></a>ACS

* `aks install-connector` 및 `aks remove-connector` 명령이 추가됨
* `acs create`에 대한 오류 보고가 개선됨
* 정규화된 경로 없이 `aks get-credentials -f`가 사용되는 문제가 해결됨

### <a name="advisor"></a>Advisor

* 최초 릴리스

### <a name="appservice"></a>App Service

* `webapp config ssl upload`를 사용한 인증서 이름 생성 문제가 해결됨
* `webapp [list|show]` 및 `functionapp [list|show]`가 올바른 앱을 표시하도록 수정됨
* `WEBSITE_NODE_DEFAULT_VERSION`에 대한 기본값이 추가됨

### <a name="consumption"></a>Consumption

* API 버전 2017-11-30에 대한 지원이 추가됨

### <a name="container"></a>컨테이너

* 기본 포트 회귀가 수정됨

### <a name="monitor"></a>모니터

* 메트릭 명령에 다차원 지원이 추가됨

### <a name="resource"></a>리소스

* `--include-response-body` 인수를 `resource show`에 추가

### <a name="role"></a>역할

* `role assignment list`에 "클래식" 관리자에 대한 기본 할당 표시가 추가됨
* 덮어 쓰지 않고 자격 증명을 추가하기 위한 지원 기능이 `ad sp reset-credentials`에 추가됨
* `ad sp create-for-rbac`에 대한 오류 보고가 개선됨

### <a name="sql"></a>SQL

* `sql db list-usages` 및 `sql db show-usage` 명령이 추가됨
* `sql server conn-policy show` 및 `sql server conn-policy update` 명령이 추가됨

### <a name="vm"></a>VM

* `az vm list-skus`에 영역 정보가 추가됨


## <a name="november-14-2017"></a>2017년 11월 14일

버전 2.0.21

### <a name="acr"></a>ACR

* 복제 영역에서 웹후크를 만들기 위한 지원 추가됨


### <a name="acs"></a>ACS

* AKS에서 "에이전트"의 모든 단어 표현을 "노드"로 변경
* `acs create`에 대한 사용되지 않음 `--orchestrator-release` 옵션
* AKS의 기본 VM 크기를 `Standard_D1_v2`로 변경됨
* Windows에서 `az aks browse` 수정됨
* Windows에서 `az aks get-credentials` 수정됨

### <a name="appservice"></a>App Service

* WebApps 및 함수 앱을 위해 배포 원본 `config-zip` 추가
* `--docker-container-logging` 옵션을 `az webapp log config`에 추가
* `az webapp log config`의 매개 변수`--web-server-logging`에서 `storage` 옵션 제거됨
* `deployment user set`에 대한 오류 메시지 향상됨
* Linux 함수 앱을 만들기 위한 지원 추가
* 고정 `list-locations`

### <a name="batch"></a>Batch

* 리소스 ID가 `--image` 플래그와 함께 사용된 경우 풀 만들기 명령의 버그 수정됨

### <a name="batchai"></a>Batchai

* `file-server create` 명령에서 VM 크기를 제공할 때 `--vm-size`에 대한 짧은 옵션 `-s` 추가
* 저장소 계정 이름 및 키 인수를 `cluster create` 매개 변수에 추가됨
* `job list-files` 및 `job stream-file` 설명서 수정됨
* `job create` 명령에서 클러스터 이름을 제공할 때 `--cluster-name`에 대한 짧은 옵션 `-r` 추가

### <a name="cloud"></a>클라우드

* 필요한 끝점이 누락된 클라우드를 등록하지 못하도록 `cloud [register|update]` 변경

### <a name="container"></a>컨테이너

* 다중 포트를 열기 위한 지원 추가
* 컨테이너 그룹 다시 시작 정책 추가
* Azure 파일 공유를 볼륨으로 마운트하기 위한 지원 추가
* 업데이트된 도우미 docs

### <a name="data-lake-analytics"></a>Data Lake Analytics


* 보다 간결한 정보를 반환하기 위해 `[job|account] list` 변경

### <a name="data-lake-store"></a>Data Lake Store

* 보다 간결한 정보를 반환하기 위해 `account list` 변경

### <a name="extension"></a>내선 번호

* 공식 Microsoft 확장 목록을 나열하기 위해 `extension list-available` 추가
* 이름별로 확장 설치하기 위해 `--name`을 `extension [add|update]`에 추가

### <a name="iot"></a>IoT

* 인증 기관(CA) 및 인증서 체인에 대한 지원 추가

### <a name="monitor"></a>모니터

* `activity-log alert` 명령이 추가됨

### <a name="network"></a>네트워크

* CAA DNS 레코드에 대한 지원 추가
* `traffic-manager profile update`로 끝점을 업데이트할 수 없는 문제 해결
* VNET이 만들어지는 방법에 따라 `vnet update --dns-servers`가 작동하지 않는 문제 해결
* `dns zone import`가 상대 DNS 이름을 잘못 가져오는 문제 해결

### <a name="reservations"></a>예약

* 초기 미리 보기 릴리스

### <a name="resource"></a>리소스

* 리소스 ID에 대한 지원을 `--resource` 매개 변수 및 리소스 수준 잠금 기능에 추가

### <a name="sql"></a>SQL

* `--ignore-missing-vnet-service-endpoint` 매개 변수가 `sql server vnet-rule [create|update]`에 추가됨

### <a name="storage"></a>Storage

* 기본값으로 SKU `Standard_RAGRS`를 사용하기 위해 `storage account create` 변경
* 비 ASCII 문자를 포함하는 파일/Blob 이름을 처리하는 경우 버그 수정됨
* `--source-uri`를 `storage [blob|file] copy start-batch`와 함께 사용하지 못하는 버그 수정
* glob에 명령 추가 및 `storage [blob|file] delete-batch`를 사용하여 여러 개체 삭제
* `storage metrics update`로 메트릭을 사용할 때 문제 해결
* `storage blob upload-batch`를 사용하는 경우 200GB 이상의 파일 사용 시 문제 해결
* `storage account [create|update]`에 의해 `--bypass` 및 `--default-action`이 무시되는 문제 해결

### <a name="vm"></a>VM

* `Basic` 크기 계층을 사용하지 못하게 하는 `vmss create`의 버그 수정
* 청구 정보가 있는 사용자 지정 이미지를 위해 `--plan` 인수를 `[vm|vmss] create`에 추가
* `vm secret `[add|remove|list]` 명령 추가
* 이름이 `vm format-secret`에서 `vm secret format`로 변경됨
* `--encrypt format` 인수를 `vm encryption enable`에 추가

## <a name="october-24-2017"></a>2017년 10월 24일

버전 2.0.20

### <a name="core"></a>코어

* `MGMT_STORAGE` API 버전 `2016-01-01`을 사용하기 위해 `2017-03-09-profile` 업데이트함

### <a name="acr"></a>ACR

* `2017-10-01` API 버전을 가리키도록 리소스 관리를 업데이트함
* 'Bring Your Own Storage' SKU를 클래식으로 변경함
* 레지스트리 SKU를 Basic, Standard 및 Premium으로 이름을 변경함

### <a name="acs"></a>ACS

* [미리 보기] `az aks` 명령이 추가됨
* Kubernetes `get-credentials`가 수정됨

### <a name="appservice"></a>App Service

* 다운로드한 `webapp` 로그가 유효하지 않은 문제가 해결

### <a name="component"></a>구성 요소

* 모든 설치 관리자에 대한 명확한 지원 중단 메시지 및 확인 프롬프트가 추가됨

### <a name="monitor"></a>모니터

* `action-group` 명령이 추가됨

### <a name="resource"></a>리소스

* `group export`의 최신 msrest 종속성과의 비호환성이 수정됨
* 기본 제공 정책 정의 및 정책 집합 정의로 작동하도록 `policy assignment create` 수정

### <a name="vm"></a>VM

* `--accelerated-networking` 인수를 `vmss create`에 추가


## <a name="october-9-2017"></a>2017년 10월 9일

버전 2.0.19

### <a name="core"></a>코어

* Azure Stack에 후행 슬래시로 ADFS 기관 URL의 처리가 추가됨

### <a name="appservice"></a>App Service

* 새 명령 `webapp update`로 일반 업데이트 추가됨

### <a name="batch"></a>Batch

* 일괄 처리 SDK 4.0.0으로 업데이트됨
* publish:offer:sku:version에 추가로 ARM 이미지 참조를 지원하는 VirtualMachineConfiguration의 `--image` 옵션이 업데이트됨
* 일괄 처리 확장 명령을 위해 새 CLI 확장 모델에 대한 지원이 추가됨
* 구성 요소 모델에서 일괄 처리 지원이 제거됨

### <a name="batchai"></a>Batchai

* 일괄 처리 AI 모듈의 초기 릴리스

### <a name="keyvault"></a>Keyvault

* Azure Stack에서 ADFS를 사용 시 Key Vault 인증 문제가 수정되었습니다. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>네트워크

* 빈 주소 풀을 감안하여 `application-gateway address-pool create`의 `--server` 인수가 선택적으로 변경됨
* 최신 기능을 지원하기 위해 `traffic-manager`가 업데이트됨

### <a name="resource"></a>리소스

* 리소스 그룹 이름에 대한 `--resource-group/-g` 옵션 지원이 `group`에 추가됨
* 구독 수준 잠금으로 작동하는 `account lock`에 대한 명령이 추가됨
* 그룹 수준 잠금으로 작동하는 `group lock`에 대한 명령이 추가됨
* 리소스 수준 잠금으로 작동하는 `resource lock`에 대한 명령이 추가됨

### <a name="sql"></a>Sql

* SQL TDE(투명한 데이터 암호화) 및 Bring Your Own Key를 사용하는 TDE에 대한 지원이 추가됨
* 삭제된 데이터베이스를 찾아 복구하는 기능을 허용하는 `db list-deleted` 명령 및 `db restore --deleted-time` 매개 변수가 추가됨
* 진행 중인 작업을 데이터베이스에 나열하고 취소하는 기능을 허용하는 `db op list` 및 `db op cancel` 추가됨

### <a name="storage"></a>Storage

* 파일 공유 스냅숏에 대한 지원 추가됨

### <a name="vm"></a>VM

* `-d` 사용으로 누락된 개인 IP 주소에서 충돌이 발생하는 `vm show`에서 버그 수정됨
* [미리 보기] 롤링 업그레이드에 대한 지원이 `vmss create`에 추가됨
* `vm encryption enable`을 사용하여 암호화 설정 업데이트에 대한 지원이 추가됨
* `--os-disk-size-gb` 매개 변수가 `vm create`에 추가됨
* Windows에 대한 `--license-type` 매개 변수가 `vmss create`에 추가됨


## <a name="september-22-2017"></a>2017년 9월 22일

버전 2.0.18

### <a name="resource"></a>리소스

* 기본 제공 정책 정의를 표시하기 위한 지원 추가
* 정책 정의를 만들기 위한 지원 모드 매개 변수 추가
* UI 정의 및 템플릿에 대한 지원을 `managedapp definition create`에 추가
* [주요 변경 내용] `appliances`에서 `applications`로 그리고 `applianceDefinitions`에서 `applicationDefinitions`로 `managedapp` 리소스 종류 변경

### <a name="network"></a>네트워크

* 가용성 영역에 대한 지원을 `network lb` 및 `network public-ip` 하위 명령에 추가
* IPv6 Microsoft 피어링에 대한 지원을 `express-route`에 추가
* `asg` 응용 프로그램 보안 그룹 명령 추가
* `--application-security-groups` 인수를 `nic [create|ip-config create|ip-config update]`에 추가
* `--source-asgs` 및 `--destination-asgs` 인수를 `nsg rule [create|update]`에 추가
* `--ddos-protection` 및 `--vm-protection` 인수를 `vnet [create|update]`에 추가
* `network [vnet-gateway|vpn-client|show-url]` 명령이 추가됨

### <a name="storage"></a>Storage

* SDK를 업데이트한 후 `storage account network-rule` 명령이 실패하는 경우 문제 해결

### <a name="eventgrid"></a>Event Grid

* 최신 API 버전 "2017-09-15-preview"를 사용하기 위해 업데이트된 Azure Event Grid Python SDK

### <a name="sql"></a>SQL

* 선택할 수 있도록 `sql server list` 인수를 `--resource-group`으로 변경되었습니다. 지정하지 않으면 구독의 모든 sql 서버가 반환됨
* `--no-wait` 매개 변수를 `db [create|copy|restore|update|replica create|create|update]` 및 `dw [create|update]`에 추가

### <a name="keyvault"></a>Keyvault

* 프록시 뒤에서부터 Keyvault 명령에 대한 지원 추가

### <a name="vm"></a>VM

* 가용성 영역에 대한 지원을 `[vm|vmss|disk] create`에 추가
* `--app-gateway ID`와 `vmss create`를 함께 사용하는 경우 오류를 일으키는 문제 해결
* `--asgs` 인수를 `vm create`에 추가
* `vm run-command`를 사용하여 VM에서 명령을 실행하기 위한 지원 추가
* [미리 보기] `vmss encryption`을 사용하여 VMSS 디스크 암호화에 대한 지원 추가
* `vm perform-maintenance`를 사용하여 VM에서 유지 관리를 수행하기 위한 지원 추가

### <a name="acs"></a>ACS

* [미리 보기] `--orchestrator-release` 인수를 ACS 미리 보기 영역에 대한 `acs create`에 추가

### <a name="appservice"></a>App Service

* `webapp auth [update|show]`를 사용하여 인증 설정을 업데이트하고 표시하기 위한 기능 추가

### <a name="backup"></a>Backup

* 미리 보기 릴리스


## <a name="september-11-2017"></a>2017년 9월 11일

버전 2.0.17

### <a name="core"></a>코어

* 원격 분석에서 고유한 상관 관계 ID를 설정하는 명령 모듈 설정됨
* 원격 분석이 진단 모드로 설정된 경우 JSON 덤프 문제 수정됨

### <a name="acs"></a>ACS

* `acs list-locations` 명령이 추가됨
* 예상된 기본값 함께 `ssh-key-file`을 제공함

### <a name="appservice"></a>App Service

* 활성 서비스 계획이 아닌 다른 리소스 그룹에서 웹앱을 만드는 기능 추가됨

### <a name="cdn"></a>CDN

* `cdn custom-domain create`에 대한 'CustomDomain is not interable' 버그 수정됨

### <a name="extension"></a>내선 번호

* 최초 릴리스

### <a name="keyvault"></a>Keyvault

* 사용 권한이 `keyvault set-policy`에서 대/소문자를 구분하는 문제 수정됨

### <a name="network"></a>네트워크

* 이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨
* `--private-access-services` 인수 이름을 `vnet subnet create/update`의 `--service-endpoints`로 변경
* 여러 IP 범위 및 포트 범위에 대한 지원이 `nsg rule create/update`에 추가됨
* SKU에 대한 지원이 `lb create`에 추가됨
* SKU에 대한 지원이 `public-ip create`에 추가됨

### <a name="resource"></a>리소스

* `policy definition create` 및 `policy definition update`에 있는 리소스 정책 매개 변수 정의를 전달하도록 허용
* `policy assignment create`의 매개 변수 값을 전달하도록 허용
* 모든 매개 변수에 JSON 또는 파일을 전달하도록 허용
* 증가된 API 버전

### <a name="sql"></a>SQL

* `sql server vnet-rule` 명령이 추가됨

### <a name="vm"></a>VM

* 수정됨: `--scope`가 제공되지 않으면 액세스 권한을 할당하지 않음
* 수정됨: 포털과 마찬가지로 동일한 확장 명명을 사용함
* `[vm|vmss] create` 출력에서 `subscription`이 제거됨
* 수정됨: `[vm|vmss] create` 저장소 SKU가 이미지를 포함한 데이터 디스크에 적용되지 않음
* 수정됨: `vm format-secret --secrets`가 줄 바꿈으로 구분된 ID를 허용하지 않음

## <a name="august-31-2017"></a>2017년 8월 31일

버전 2.0.16

### <a name="keyvault"></a>Keyvault

* `secret download`로 인코딩한 비밀을 자동으로 확인하려는 경우 버그 수정됨

### <a name="sf"></a>Sf

* Service Fabric CLI(sfctl)에서 모든 명령이 사용되지 않음

### <a name="storage"></a>Storage

* 저장소 계정을 NetworkACLs 기능을 지원하지 않는 지역에 만들지 못하는 문제 수정됨
* 콘텐츠 형식 및 콘텐츠 인코딩을 모두 지정하지 않은 경우 Blob 및 파일을 업로드하는 동안 콘텐츠 형식 및 콘텐츠 인코딩을 결정함

## <a name="august-28-2017"></a>2017년 8월 28일

버전 2.0.15

### <a name="cli"></a>CLI

* `--version`에 법적 정보가 추가되었습니다.

### <a name="acs"></a>ACS

* 미리 보기 지역이 수정되었습니다.
* `dns_name_prefix`의 기본 형식이 올바르게 지정되었습니다.
* acs 명령 출력이 최적화되었습니다.

### <a name="appservice"></a>App Service

* [주요 변경 내용] `az webapp config appsettings [delete|set]` 출력의 불일치가 수정됨
* `az webapp config container set --docker-custom-image-name`에 대해 새로운 `-i` 별칭이 추가됨
* `az webapp log show`가 공개됨
* `az webapp delete`에서 앱 서비스 계획, 통계 또는 DNS 등록을 유지하는 새 인수가 공개됨
* 슬롯 설정을 올바르게 검색하도록 수정됨

### <a name="iot"></a>IoT

* #3934: 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨

### <a name="network"></a>네트워크

* [주요 변경 내용] 이름이 `vnet list-private-access-services`에서 `vnet list-endpoint-services`로 변경됨
* [주요 변경 내용] `vnet subnet [create|update]`에 대한 옵션 이름이 `--private-access-services`에서 `--service-endpoints`로 변경됨
* 여러 IP 및 포트 범위에 대한 지원이 `nsg rule [create|update]`에 추가됨
* SKU에 대한 지원이 `lb create`에 추가됨
* SKU에 대한 지원이 `public-ip create`에 추가됨

### <a name="profile"></a>프로필

* 가상 컴퓨터의 ID를 사용하여 로그인하는 `--msi` 및 `--msi-port`가 공개됨

### <a name="service-fabric"></a>Service Fabric

* 미리 보기 릴리스
* 명령에 대한 레지스트리 사용자/암호 규칙이 간소화됨
* 매개 변수를 전달한 후에도 사용자에게 암호를 묻는 메시지가 수정됨
* 빈 `registry_cred`에 대한 지원이 추가됨

### <a name="storage"></a>Storage

* 설정 Blob 계층이 사용됨
* 서비스 터널링을 지원하는 `--bypass` 및 `--default-action` 인수가 `storage account [create|update]`에 추가됨
* VNET 규칙 및 IP 기반 규칙을 추가하는 명령이 `storage account network-rule`에 추가됨
* 고객 관리 키에 의한 서비스 암호화가 사용됨
* [주요 변경 내용] `az storage account create and az storage account update` 명령에 대한 옵션 이름이 `--encryption`에서 `--encryption-services`로 변경됨
* #4220: `az storage account update encryption` - 구문 불일치가 수정됨

### <a name="vm"></a>VM

* `--instance-id *`를 사용할 때 `vmss get-instance-view`에 대해 잘못된 추가 정보가 표시되는 문제가 해결되었습니다.
* `--lb-sku`에 대한 지원이 `vmss create`에 추가됨
* `[vm|vmss] create`에 대한 관리자 이름 블랙리스트에서 사람의 이름이 제거됨
* 이미지에서 계획 정보를 추출할 수 없는 경우 `[vm|vmss] create`에서 오류를 throw하는 문제가 해결되었습니다.
* 내부 LB가 있는 VMMS 확장 집합을 만들 때 발생하는 크래시가 해결되었습니다.
* `--no-wait` 인수가 `vm availability-set create`와 함께 작동하지 않는 문제가 해결되었습니다.


## <a name="august-15-2017"></a>2017년 8월 15일

버전 2.0.14

### <a name="acs"></a>ACS

* Kubernetes에 대한 sshMaster0 포트 번호가 수정됨

### <a name="appservice"></a>App Service

* 새 Git 기반 Linux 웹앱을 만들 때 발생하는 예외가 해결되었습니다.

### <a name="event-grid"></a>Event Grid

* SDK 종속성이 추가됨

## <a name="august-11-2017"></a>2017년 8월 11일

버전 2.0.13

### <a name="acs"></a>ACS

* 더 많은 미리 보기 지역이 추가됨

### <a name="batch"></a>Batch

* Batch SDK 3.1.0 및 Batch Management SDK 4.1.0으로 업데이트됨
* 작업의 태스크 수를 표시하는 새 명령이 추가됨
* 리소스 파일 SAS URL 처리에서 발견된 버그가 수정됨
* 배치 계정 끝점에서 이제 선택적 'https://' 접두사를 지원합니다.
* 100개 이상의 태스크를 포함한 목록이 작업에 추가되도록 지원합니다.
* 확장 명령 모듈 로드에 대한 디버그 로깅이 추가됨

### <a name="component"></a>구성 요소

* 'az component' 명령에 사용 중단 경고가 추가됨

### <a name="container"></a>컨테이너

* `create`: 환경 변수에서 등호가 허용되지 않는 문제가 해결되었습니다.


### <a name="data-lake-store"></a>Data Lake Store

* 진행률 컨트롤이 사용됨

### <a name="event-grid"></a>Event Grid

* 최초 릴리스

### <a name="network"></a>네트워크

* `lb`: 생략했을 때 특정 자식 리소스 이름이 올바르게 확인되지 않는 문제가 해결되었습니다.
* `application-gateway {subresource} delete`: `--no-wait`를 적용할 수 없는 문제가 해결되었습니다.
* `application-gateway http-settings update`: `--connection-draining-timeout`를 해제할 수 없는 문제가 해결되었습니다.
* `az network vpn-connection ipsec-policy add`에서 예기치 않은 `sa_data_size_kilobyes` 키워드 인수 오류가 발생하는 문제가 해결되었습니다.

### <a name="profile"></a>프로필

* `account list`: 서버에서 최신 구독을 동기화하는 `--refresh`가 추가됨

### <a name="storage"></a>Storage

* 시스템에 할당된 ID를 통한 저장소 계정 업데이트가 사용됨

### <a name="vm"></a>VM

* `availability-set`: 변환 시 오류 도메인 수가 공개됨
* `list-skus` 명령이 공개됨
* 역할 할당을 만들지 않고 ID를 할당하도록 지원합니다.
* 데이터 디스크 연결 시 저장소 SKU를 적용합니다.
* 관리 디스크를 사용할 때 기본 OS 디스크 이름 및 저장소 SKU가 제거됩니다.


## <a name="july-28-2017"></a>2017년 7월 28일

버전 2.0.12

* 컨테이너 명령이 추가됨
* 청구 및 소비 모듈이 추가됨

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

### <a name="core"></a>코어

* 인증서가 있는 서비스 사용자에 대한 SDK 인증 정보가 출력됨
* 배포 진행률 예외가 해결됨
* 현재 클라우드의 ARM 끝점을 사용하여 구독 클라이언트를 만들 수 있음
* clouds.config 파일의 동시 처리가 향상됨(#3636)
* 각 명령 실행에 대한 클라이언트 요청 ID를 새로 고침
* 오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음(#3635)
* 템플릿 배포에 대한 진행률이 보고됨(#3510)
* jmespath 쿼리를 통한 테이블 출력 필드 선택에 대한 지원이 추가됨(#3581)
* 향상된 구문 분석 인수 차단 및 제스처를 사용한 기록 추가 (#3434)
* 오른쪽 SDK 프로필을 사용하여 구독 클라이언트를 만들 수 있음
* 기존의 모든 기록 파일을 최신 폴더로 이동
* VM/VMSS 만들기에 대한 멱등성 문제가 해결됨(#3586)
* 명령 경로에서 더 이상 대/소문자를 구분하지 않음
* 특정 부울 형식 매개 변수에서 더 이상 대/소문자를 구분하지 않음
* 프리미엄 서버(예: Azure Stack)에서 ADFS에 대한 로그인 지원
* clouds.config에 대한 동시 쓰기 문제가 해결됨(#3255)

### <a name="acr"></a>ACR

* 관리되는 레지스트리에 대한 `show-usage` 명령이 추가됨
* 관리되는 레지스트리에 대한 SKU 업데이트가 지원됨
* 관리되는 SKU에 관리되는 레지스트리가 추가됨
* acr webhook 명령 모듈에 관리되는 레지스트리에 대한 웹후크가 추가됨
* acr login 명령에 AAD 인증이 추가됨
* Docker 리포지토리, 매니페스트 및 태그에 대한 delete 명령이 추가됨

### <a name="acs"></a>ACS

* API 버전 2017-07-01에 대한 지원

### <a name="appservice"></a>App Service

* Linux 웹앱을 나열하면 아무 것도 반환하지 않는 버그가 수정되었습니다.
* ACR에서 자격 증명을 검색하도록 지원합니다.
* `appservice web` 아래의 모든 명령을 제거합니다.
* 명령 출력에서 Docker 레지스트리 암호를 마스킹합니다(#3656).
* macOS에서 기본 브라우저가 오류 없이 사용되는지 확인합니다(#3623).
* `webapp log tail` 및 `webapp log download` 지원이 향상되었습니다(#3624).
* 정적 라우팅을 구성하는 `traffic-routing` 명령이 공개되었습니다(#3566).
* 원본 제어 구성에 안정성 수정이 추가되었습니다(#3245).
* Windows 웹앱에 대한 `webapp config update`에서 지원되지 않는 `--node-version` 인수가 제거되었습니다. 대신 `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`을 사용합니다.

### <a name="batch"></a>Batch

* 풀에서 우선 순위가 낮은 VM을 지원하는 Batch SDK 3.0.0으로 업데이트됨
* `pool create`에 대한 옵션 이름이 `--target-dedicated`에서 `--target-dedicated-nodes`로 변경됨
* `pool create`에 대한 옵션으로 `--target-low-priority-nodes` 및 `--application-licenses`가 추가됨

### <a name="cdn"></a>CDN

* `--profile-name`에서 지정된 프로필이 존재하지 않을 때 `cdn endpoint list`에 대한 더 나은 오류 메시지가 제공됩니다.

### <a name="cloud"></a>클라우드

* 클라우드 메타데이터 끝점의 API 버전이 YYYY-MM-DD 형식으로 변경됨
* 갤러리 끝점이 필요하지 않음
* ARM 리소스 관리자 끝점을 사용한 클라우드 등록이 지원됨
* 현재 클라우드를 선택하는 동안에 `cloud set`에서 프로필을 선택하는 옵션이 제공됨
* `endpoint_vm_image_alias_doc`가 공개됨

### <a name="cosmosdb"></a>CosmosDB

* 사용자 지정 파티션 키를 사용하여 컬렉션을 만들 수 있도록 수정되었습니다.
* 컬렉션 기본 TTL에 대한 지원이 추가되었습니다.

### <a name="data-lake-analytics"></a>Data Lake Analytics


* `dla account compute-policy` 제목 아래에 계산 정책을 관리하는 명령이 추가됨
* `dla job pipeline show`가 추가됨
* `dla job recurrence list`가 추가됨

### <a name="data-lake-store"></a>Data Lake Store

* `dls account update`에 사용자 관리 키 자격 증명 모음 키 회전에 대한 지원이 추가되었습니다.
* 기본 Data Lake Store 파일 시스템 SDK 버전을 업데이트하여 성능 문제가 해결되었습니다.
* `dls enable-key-vault` 명령이 추가되었습니다. 이 명령은 Data Lake Store 계정의 데이터를 암호화하기 위해 사용자가 제공한 Key Vault를 사용하도록 설정하려고 시도합니다

### <a name="interactive"></a>대화형

* 캐시된 명령을 사용하여 시작 시간이 향상됨
* 테스트 검사가 향상됨
* 다음 명령에 삽입하는 '?' 제스처가 향상됨
* 2017-03-09-profile-preview 프로필을 사용하여 대화형 오류가 수정됨(#3587)
* 대화형 모드에 대한 매개 변수로 `--version`이 허용됨(#3645)
* 유효성 검사 완료 시 오류를 throw하는 대화형 모드가 중지됨(#3570)
* 템플릿 배포에 대한 진행률이 보고됨(#3510)
* `--progress` 플래그가 추가됨
* 완료 시 `--debug` 및 `--verbose`가 제거됨
* 완료 시 `interactive`가 제거됨(#3324)

### <a name="iot"></a>IoT

* 정책을 만들 때 기존 정책을 더 이상 지우지 않도록 수정됨 (#3934)

### <a name="key-vault"></a>주요 자격 증명 모음

* 키 자격 증명 모음 복구 기능에 추가된 명령:
  * `keyvault` 하위 명령: `purge`, `recover`, `keyvault list-deleted`
  * `keyvault secret` 하위 명령: `backup`, `restore`, `purge`, `recover`, `list-deleted`
  * `keyvault certificate` 하위 명령: `purge`, `recover`, `list-deleted`
  * `keyvault key` 하위 명령: `purge`, `recover`, `list-deleted`
* 서비스 사용자 키 자격 증명 모음 통합이 추가됨(#3133)
* 키 자격 증명 모음 데이터 평면이 0.3.2로 업데이트됨 (#3307)

### <a name="lab"></a>랩

* `az lab vm claim`을 통한 랩의 모든 VM 요청 작업에 대한 지원이 추가됨
* `az lab vm list` 및 `az lab vm show`에 대한 테이블 출력 포맷터가 추가됨

### <a name="monitor"></a>모니터

* `monitor autoscale-settings get-parameters-template` 명령으로 템플릿 파일이 수정됨(#3349)
* 이름이 `monitor alert-rule-incidents list`에서 `monitor alert list-incidents`로 변경됨
* 이름이 `monitor alert-rule-incidents show`에서 `monitor alert show-incident`로 변경됨
* 이름이 `monitor metric-defintions list`에서 `monitor metrics list-definitions`로 변경됨
* 이름이 `monitor alert-rules`에서 `monitor alert`로 변경됨
* `monitor alert create`에 대한 변경 내용:
  * `condition` 및 `action` 하위 명령에는 JSON이 더 이상 허용되지 않습니다.
  * 다양한 매개 변수를 추가하여 규칙 작성 프로세스가 간소화되었습니다.
  * `location`은 더 이상 필수가 아닙니다.
  * 대상에 대한 이름 및 ID 지원이 추가되었습니다.
  * `--alert-rule-resource-name`이 제거되었습니다.
  * 이름이 `is-enabled`에서 `enabled`로 변경되었으며, 더 이상 필수가 아닙니다.
  * `description`은 제공된 조건에 따라 기본적으로 설정됩니다.
  *  새 형식을 명확히 하는 데 도움이 되는 예제가 추가되었습니다.
* `monitor metric` 명령에 대해 이름 또는 ID가 지원됨
* `monitor alert rule update`에 편의 인수 및 예제가 추가됨

### <a name="network"></a>네트워크

* `list-private-access-services` 명령이 추가됨
* `vnet subnet create` 및 `vnet subnet update`에 `--private-access-services` 인수가 추가됨
* `application-gateway redirect-config create`가 실패하는 문제가 해결되었습니다.
* `--no-wait`가 포함된 `application-gateway redirect-config update`가 작동하지 않는 문제가 해결되었습니다.
* `application-gateway address-pool create` 및 `application-gateway address-pool update`에 `--servers` 인수를 사용하는 버그가 수정되었습니다.
* `application-gateway redirect-config` 명령이 추가됨
* `application-gateway ssl-policy`에 추가된 명령: `list-options`, `predefined list`, `predefined show`
* `application-gateway ssl-policy set`에 추가된 인수: `--name`, `--cipher-suites`, `--min-protocol-version`
* `application-gateway http-settings create` 및 `application-gateway http-settings update`에 추가된 인수: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* `application-gateway url-path-map create` 및 `application-gateway url-path-map update`에 추가된 인수: `--default-redirect-config`, `--redirect-config`
* `application-gateway url-path-map rule create`에 추가된 인수: `--redirect-config`
* `application-gateway url-path-map rule delete`에 추가된 지원: `--no-wait`
* `application-gateway probe create` 및 `application-gateway probe update`에 추가된 인수: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* `application-gateway rule create` 및 `application-gateway rule update`에 추가된 인수: `--redirect-config`
* `--accelerated-networking`에 대한 지원이 `nic create` 및 `nic update`에 추가됨
* `nic create`에서 `--internal-dns-name-suffix` 인수가 제거됨
* `--dns-servers`에 대한 지원이 `nic update` 및 `nic create`에 추가됨: --dns-servers에 대한 지원 추가
* `local-gateway create`에서 `--local-address-prefixes`를 무시하는 버그가 수정되었습니다.
* `--dns-servers`에 대한 지원이 `vnet update`에 추가됨
* `express-route peering create`를 사용하여 경로를 필터링하지 않고 피어링을 만드는 버그가 수정되었습니다.
* `--provider` 및 `--bandwidth` 인수가 `express-route update`에서 작동하지 않는 버그가 수정되었습니다.
* `network watcher show-topology` 기본값 논리가 있는 버그가 수정되었습니다.
* `network list-usages`에 대한 출력 형식 지정이 향상됨
* 하나만 있는 경우 `application-gateway http-listener create`에 대해 기본 프런트 엔드 IP가 사용됨
* 하나만 있는 경우 `application-gateway rule create`에 대해 기본 주소 풀, HTTP 설정 및 HTTP 수신기가 사용됨
* 하나만 있는 경우 `lb rule create`에 대해 기본 프런트 엔드 IP 및 백 엔드 풀이 사용됨
* 하나만 있는 경우 `lb inbound-nat-rule create`에 대해 기본 프런트 엔드 IP가 사용됨

### <a name="profile"></a>프로필

* 관리 ID를 사용한 VM 내부 로그인이 지원됨
* `account show`에 대한 SDK 인증 파일 형식 출력이 지원됨
* '--expanded-view'를 사용할 때 사용 중단 경고가 표시됨
* 원시 AAD 토큰을 제공하는 `get-access-token` 명령이 추가됨
* 연결된 구독이 없는 사용자 계정을 사용한 로그인이 지원됨

### <a name="rdbms"></a>RDBMS

* 구독을 통해 서버를 나열하도록 지원합니다(#3417).
* `% server_type` 누락으로 인해 처리되지 않는 `%s`가 해결되었습니다(#3393).
* 고정 문서 원본 맵이 수정되고 CI 확인 작업이 추가되었습니다(#3361).
* MySQL 및 PostgreSQL 도움말이 수정되었습니다(#3369)

### <a name="resource"></a>리소스

* `group deployment create`의 누락된 매개 변수에 대한 프롬프트가 향상됨
* `--parameters KEY=VALUE` 구문 분석이 향상됨
* `@<file>` 구문을 사용하여 `group deployment create` 매개 변수 파일을 더 이상 인식하지 못하는 문제가 해결되었습니다.
* `resource` 및 `managedapp` 명령에 대해 `--ids` 인수가 지원됩니다.
* 일부 구문 분석 및 오류 메시지가 수정되었습니다(#3584).
* `lock` 명령에 대한 `--resource-type` 구문 분석에서 `<resource-namespace>`과 `<resource-type>`을 허용하도록 수정되었습니다.
* 템플릿 링크 템플릿에 대한 매개 변수 검사가 추가되었습니다(#3629).
* `KEY=VALUE` 구문을 사용하여 배포 매개 변수를 지정하도록 지원하는 기능이 추가되었습니다.

### <a name="role"></a>역할

* `create-for-rbac`에 대한 SDK 인증 파일 형식 출력이 지원됨
* 서비스 사용자를 삭제할 때 역할 할당 및 관련 AAD 응용 프로그램이 정리됨(#3610)
* `app create` 인수 `--start-date` 및 `--end-date` 설명에 시간 형식이 포함됨
* `--expanded-view`를 사용할 때 사용 중단 경고가 표시됨
* `create-for-rbac` 및 `reset-credentials` 명령에 키 자격 증명 모음 통합이 추가됨

### <a name="service-fabric"></a>Service Fabric
* 업로드 시 응용 프로그램의 대형 파일을 자르는 문제가 해결되었습니다(#3666).
* Service Fabric 명령에 대한 테스트가 추가됨(#3424)
* 다양한 Service Fabric 명령이 수정됨(#3234)

### <a name="sql"></a>SQL

* 중단된 `sql server create` `--identity` 매개 변수가 제거됨
* `sql server create` 및 `sql server update` 명령 출력에서 암호 값이 제거됨
* `sql db list-editions` 및 `sql elastic-pool list-editions` 명령이 추가됨

### <a name="storage"></a>Storage

* `storage blob list`, `storage container list` 및 `storage share list` 명령에서 `--marker` 옵션이 제거됨(#3745)
* HTTPS 전용 저장소 계정 만들기 사용
* 저장소 메트릭, 로깅 및 CORS 명령이 업데이트됨(#3495)
* CORS add(#3638)(#3362)의 예외 메시지가 수정됨
* download batch 명령 dryrun(시험 실행) 모드에서 생성기가 목록으로 변환됨(#3592)
* Blob download batch dryrun 문제가 해결됨(#3640)(#3592)

### <a name="vm"></a>VM

* NSG 구성이 지원됨
* DNS 서버가 올바르게 구성되지 않는 버그가 수정되었습니다.
* 관리되는 서비스 ID가 지원됨
* 기존 부하 분산 장치가 있는 `cmss create`에 `--backend-pool-name`이 필요했던 문제가 해결되었습니다.
* `vm image create` lun을 사용하여 만든 데이터 디스크가 0으로 시작됨


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

### <a name="data-lake-analytics"></a>Data Lake Analytics


* 작업 목록의 결과 및 상태에 대한 필터링 시 오류가 throw되는 버그를 수정합니다.
* 새 카탈로그 항목 형식: 패키지에 대한 지원을 추가합니다. `az dla catalog package`를 통해 액세스
* 데이터베이스 내에서 다음 카탈로그 항목을 나열할 수 있음(스키마 사양 필요 없음):

  * 테이블
  * 테이블 반환 함수
  * 보기
  * 테이블 통계. 테이블 이름을 지정하지 않고 스키마와 함께 나열될 수도 있습니다.

### <a name="data-lake-store"></a>Data Lake Store

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
[azure-cli 태그를 사용하는 StackOverflow](http://stackoverflow.com/questions/tagged/azure-cli)에 대해 질문하거나 제품 팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))으로 문의하실 수 있습니다. `az feedback` 명령을 사용하여 명령줄에서 피드백을 제공할 수 있습니다.

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


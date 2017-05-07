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
ms.openlocfilehash: 56190b653ab9765017fffd1699056de7eae2db77
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
translationtype: HT
---
# <a name="azure-cli-20-release-notes"></a>Azure CLI 2.0 릴리스 정보

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
Microsoft 지원 또는 [github 문제 목록](https://github.com/azure/azure-cli/issues)에서 직접 문제를 개설할 수 있습니다.
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
- [github 문제 목록](https://github.com/azure/azure-cli/issues)에서 문제 보고
- 제품팀([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com))에 문의.
- `az feedback` 명령을 사용하여 명령줄에서 피드백 제공.


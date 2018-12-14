---
title: Azure CLI에 대해 사용 가능한 확장
description: Azure CLI에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/07/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 21e1b208f3f022f7c0a9d9f521ba25e23bca3f8b
ms.sourcegitcommit: 3da80a57b6bd64d909c89a7d1ac6e830085313fe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2018
ms.locfileid: "53070254"
---
# <a name="available-extensions-for-the-azure-cli"></a>Azure CLI에 대해 사용 가능한 확장

이 문서는 Microsoft에서 지원하는 Azure CLI에 사용할 수 있는 전체 확장 목록입니다.

확장 목록도 CLI로부터 가져올 수 있습니다. 가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.

```azurecli-interactive
az extension list-available --output table
```

| 이름 | 버전 | 요약 | 미리 보기 |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | SAP용 Azure 고급 모니터링 확장 관리 |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.1.0 | 예정된 AKS 기능에 대한 미리 보기 제공 | yes |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | 명령 별칭 지원 | yes |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.5.1 | Azure Batch 서비스와 함께 사용하기 위한 추가 명령 |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.6.1 | Azure IoT Hub, IoT Edge 및 IoT 디바이스 프로비전 서비스에 대한 데이터 플레인 명령 계층 제공 |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.1 | Azure Firewall 리소스를 관리합니다. | yes |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | 네이티브 botservice cli 명령 모듈 문제에 대한 버그가 수정되었습니다. | yes |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces는 팀에게 신속하고 반복적인 Kubernetes 개발 환경을 제공합니다. | yes |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.6.0 | Database Migration Service의 새로운 시나리오에 대한 지원. | yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | DNS 영역을 위한 Azure CLI Extension |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Azure EventGrid 2018-09-15 미리 보기 기능에 대한 지원 | yes |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | 미리 보기 기능을 사용하여 Expressroute를 관리합니다. | yes |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | ExpressRoute 간 연결을 사용하여 고객의 ExpressRoute 회로를 관리 합니다. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | CLI 정보에 대한 지능형 쿼리. | yes |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.1 | 네트워킹 Front Doors를 관리합니다. | yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.9 | 지역 간 관리 vm 이미지 복사 기능에 대한 지원 |  |
| [대화형](https://github.com/Azure/azure-cli) | 0.4.1 | Microsoft Azure 명령줄 대화형 셸 | yes |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Azure Key Vault 미리보기 명령어 | yes |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Azure Log Analytics 쿼리 기능을 지원합니다. | yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 관리 그룹을 위한 Azure CLI Extension |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | 관리 파트너 미리 보기 지원 |  |
| [메시](https://github.com/Azure/azure-cli-extensions) | 0.10.2 | Microsoft Azure Service Fabric Mesh - 공개 미리 보기에 대한 지원 | yes |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Azure MySQL 및 Azure PostgreSQL 리소스 내 가상 네트워크 규칙에 대한 지원 |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Resource Graph로 Azure 리소스 쿼리에 대한 지원 | yes |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.1.6 | SAP HanaOnAzure 인스턴스와 함께 사용하기 위한 추가 명령 |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | signalr 관리 미리 보기를 지원합니다. | yes |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.7 | 예정된 저장소 기능에 대한 미리 보기를 제공합니다. | yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | 구독 관리 미리 보기를 지원합니다. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | 가상 네트워크 관리 탭(VTAP) | yes |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | 가상 WAN, 허브, VPN 게이트웨이 및 VPN 사이트를 관리합니다. | yes |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.16 | Azure AppService에 대한 추가 명령입니다. | yes |
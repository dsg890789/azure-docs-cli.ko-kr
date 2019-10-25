---
title: Azure CLI에 대해 사용 가능한 확장
description: Azure CLI에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/22/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: e32ef6b1623c4fb64c31111e4b237fd8997f5d5f
ms.sourcegitcommit: 269eb3589059c145c3fef0b723a72b5a25feb71c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/23/2019
ms.locfileid: "72783673"
---
# <a name="available-extensions-for-the-azure-cli"></a>Azure CLI에 대해 사용 가능한 확장

이 문서는 Microsoft에서 지원하는 Azure CLI에 사용할 수 있는 전체 확장 목록입니다.

확장 목록도 CLI로부터 가져올 수 있습니다. 가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.

```azurecli-interactive
az extension list-available --output table
```

| Name | 버전 | 요약 | 미리 보기 |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | SAP용 Azure 고급 모니터링 확장 관리 |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.17 | 예정된 AKS 기능에 대한 미리 보기 제공 | 예 |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | 명령 별칭 지원 | 예 |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | 예정된 앱 구성에 대한 미리 보기를 제공합니다. | 예 |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.1 | Application Insights 구성 요소 관리와 그러한 구성 요소에서 메트릭, 이벤트, 로그의 쿼리를 지원합니다. | 예 |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Azure Batch 서비스와 함께 사용하기 위한 추가 명령 |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.3 | Azure IoT Hub, IoT Edge 및 IoT 디바이스 프로비전 서비스에 대한 데이터 플레인 명령 계층 제공 |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.69 | Microsoft Azure 명령줄 도구 AzureML 명령 모듈 |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.13.0 | Azure DevOps를 관리하는 도구입니다. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.3 | Azure Firewall 리소스를 관리합니다. | 예 |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Azure Database 워크플로를 간소화하는 추가 명령입니다. | 예 |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.3 | Dev Spaces는 팀에게 신속하고 반복적인 Kubernetes 개발 환경을 제공합니다. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces는 팀에게 신속하고 반복적인 Kubernetes 개발 환경을 제공합니다. | 예 |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Database Migration Service의 새로운 시나리오에 대한 지원. | 예 |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | DNS 영역을 위한 Azure CLI Extension |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Microsoft Azure 명령줄 도구 EventGrid 명령 모듈 | 예 |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | 미리 보기 기능을 사용하여 Expressroute를 관리합니다. | 예 |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | ExpressRoute 간 연결을 사용하여 고객의 ExpressRoute 회로를 관리 합니다. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | CLI 정보에 대한 지능형 쿼리. | 예 |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.1 | 네트워킹 Front Doors를 관리합니다. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Microsoft Azure 명령줄 도구 Hack 확장 | 예 |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Microsoft Azure 명령줄 도구 HealthCareApis 확장 |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | 지역 간 관리 vm 이미지 복사 기능에 대한 지원 |  |
| [대화형](https://github.com/Azure/azure-cli) | 0.4.3 | Microsoft Azure 명령줄 대화형 셸 | 예 |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Azure Key Vault 미리보기 명령어 | 예 |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Azure Log Analytics 쿼리 기능을 지원합니다. | 예 |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 관리 그룹을 위한 Azure CLI Extension |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | 관리 파트너 미리 보기 지원 |  |
| [메시](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Microsoft Azure Service Fabric Mesh - 공개 미리 보기에 대한 지원 | 예 |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Mixed Reality Azure CLI 확장. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | 예정된 ANF(Azure NetApp Files) 기능에 대한 미리보기를 제공합니다. | 예 |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | 프라이빗 DNS 영역을 관리하는 명령입니다. | 예 |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Resource Graph로 Azure 리소스 쿼리에 대한 지원 |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | SAP HanaOnAzure 인스턴스와 함께 사용하기 위한 추가 명령 |  |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.8 | 예정된 스토리지 기능에 대한 미리 보기를 제공합니다. | 예 |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | 구독 관리 미리 보기를 지원합니다. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | 가상 네트워크 관리 탭(VTAP) | 예 |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | 가상 WAN, 허브, VPN 게이트웨이 및 VPN 사이트를 관리합니다. | 예 |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.2 | VM을 수정하기 위한 자동 복구 명령입니다. |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.1.0 | Azure VMware 솔루션을 관리합니다. | 예 |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Azure AppService에 대한 추가 명령입니다. | 예 |
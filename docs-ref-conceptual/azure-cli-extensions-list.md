---
title: Azure CLI 2.0에 대해 사용 가능한 확장
description: Azure CLI 2.0에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 07/30/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 92d2ac36d0176469f8f5a77e7a27d0b11ab6d947
ms.sourcegitcommit: 70bb8b115f7b9079ca1fdb65c7f5582b060a466f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/31/2018
ms.locfileid: "39356610"
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Azure CLI 2.0에 대해 사용 가능한 확장

이 문서는 Microsoft에서 제공하고 지원하는 Azure CLI 2.0에 사용할 수 있는 전체 확장 목록입니다.

확장 목록도 CLI로부터 직접 가져올 수 있습니다. 가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.

```azurecli
az extension list-available --output table
```

| Name | 버전 | 요약 | 미리 보기 |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | SAP용 Azure 고급 모니터링 확장 관리 |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | 명령 별칭 지원 | yes |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.4.1 | Azure Batch 서비스와 함께 사용하기 위한 추가 명령 |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.5.1 | Azure IoT Hub, IoT Edge 및 IoT 장치 프로비전 서비스에 대한 데이터 플레인 명령 계층 제공 |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.0.3 | Azure Bot Service 2017-12-01 미리 보기 기능 지원 | yes |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces는 팀에게 신속하고 반복적인 Kubernetes 개발 환경을 제공합니다. | yes |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | DNS 영역을 위한 Azure CLI Extension |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.1 | Azure EventGrid 2018-05-01 미리 보기 기능에 대한 지원 | yes |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.7 | 지역 간 관리 vm 이미지 복사 기능에 대한 지원 |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Azure Key Vault 미리보기 명령어 | yes |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.2 | Azure Log Analytics 쿼리 기능을 지원합니다. | yes |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 관리 그룹을 위한 Azure CLI Extension |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | 관리 파트너 미리 보기 지원 |  |
| [메시](https://github.com/Azure/azure-cli-extensions) | 0.9.1 | Microsoft Azure Service Fabric Mesh - 공개 미리 보기에 대한 지원 | yes |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Azure MySQL 및 Azure PostgreSQL 리소스 내 가상 네트워크 규칙에 대한 지원 |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | signalr 관리 미리 보기를 지원합니다. | yes |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.1.3 | 예정된 저장소 기능에 대한 미리 보기를 제공합니다. | yes |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | 구독 관리 미리 보기를 지원합니다. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | 앱 서비스 리소스를 관리하는 Azure CLI Extension | yes |

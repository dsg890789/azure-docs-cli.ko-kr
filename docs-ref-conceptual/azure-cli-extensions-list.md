---
title: Azure CLI 2.0에 대해 사용 가능한 확장
description: Azure CLI 2.0에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5a71a5809aaaa26a4b67193c1a9ff70a6b8dec05
ms.sourcegitcommit: 1d18f667af28b59f5524a3499a4b7dc12af5163d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/09/2018
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
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.1 | 명령 별칭 지원 | 예 |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.2.1 | Azure Batch 서비스와 함께 사용하기 위한 추가 명령 |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.4 | Azure IoT Hub, IoT Edge 및 IoT 장치 프로비전 서비스에 대한 데이터 플레인 명령 계층 제공 |  |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Azure Bot Service 2017-12-01 미리 보기 기능 지원 | 예 |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | DNS 영역을 위한 Azure CLI Extension |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Azure EventGrid 2018-05-01 미리 보기 기능에 대한 지원 | 예 |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.6 | 지역 간 관리 vm 이미지 복사 기능에 대한 지원 |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Azure Key Vault 미리보기 명령어 | 예 |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 관리 그룹을 위한 Azure CLI Extension |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | 관리 파트너 미리 보기 지원 |  |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Azure MySQL 및 Azure PostgreSQL에 대한 지원을 제공하는 Azure CLI Extension입니다. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | signalr 관리 미리 보기를 지원합니다. | 예 |
| [storage-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 예정된 저장소 기능에 대한 미리 보기를 제공합니다. | 예 |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | 구독 관리 미리 보기를 지원합니다. |  |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.6 | 앱 서비스 리소스를 관리하는 Azure CLI Extension | 예 |

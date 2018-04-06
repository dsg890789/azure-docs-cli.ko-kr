---
title: Azure CLI 2.0에 대해 사용 가능한 확장
description: Azure CLI 2.0에 대해 공식적으로 지원되는 확장의 전체 목록입니다.
author: derekbekoe
ms.author: debekoe
manager: routlaw
ms.date: 04/02/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e7cf22d1611c224e1d7af351210e12fe0124fad0
ms.sourcegitcommit: 26e0816dad17cc3584d1724493feecf5f5faa1f5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/04/2018
---
# <a name="available-extensions-for-the-azure-cli-20"></a>Azure CLI 2.0에 대해 사용 가능한 확장

이 문서는 Microsoft에서 제공하고 지원하는 Azure CLI 2.0에 사용할 수 있는 전체 확장 목록입니다.

확장 목록도 CLI로부터 직접 가져올 수 있습니다. 가져오려면 [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available)을 실행합니다.

```azurecli
az extension list-available --output table
```

| Name | 버전 | 요약 | 미리 보기 |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | SAP용 Azure 고급 모니터링 확장을 관리합니다. |  |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.3.0 | 명령 별칭을 지원합니다. | 예 |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 2.1.0 | 추가 미리 보기 Azure Batch 명령입니다. |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.4.1 | Azure IoT Hub, IoT Edge 및 IoT 장치 프로비전 서비스에 대한 데이터 플레인 명령 계층을 제공합니다. |  |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Azure 사설 DNS 영역 공개 미리 보기를 지원합니다. |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | 영역 간에 이미지를 복사합니다. |  |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | 관리 그룹 미리 보기를 지원합니다. | 예 |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | 관리 파트너 미리 보기를 지원합니다. | 예 |
| [rdbms](https://github.com/Azure/azure-cli-extensions) | 0.0.5 | Azure MySQL 및 Azure PostgreSQL을 지원합니다. |  |
| [subscription](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | 구독 정의 미리 보기를 지원합니다. | 예 |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | appservice 리소스를 만들고 배포합니다. | 예 |

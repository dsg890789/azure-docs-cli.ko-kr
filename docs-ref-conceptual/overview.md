---
title: Azure CLI 2.0
description: "Azure CLI 2.0의 개요입니다."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 36a08835b9c4f6e71c5ddadbce8ba946c52a1e9b
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2017
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0은 Azure 리소스를 관리하기 위한 Azure의 새로운 명령줄 환경입니다.
[Azure Cloud Shell](/azure/cloud-shell/overview)을 실행하는 브라우저에서 사용하거나 macOS, Linux 및 Windows에서 [설치](install-azure-cli.md)하고 명령줄에서 실행할 수 있습니다.

Azure CLI 2.0은 명령줄에서 Azure 리소스를 관리하는 작업 및 Azure Resource Manager에 대해 작동하는 자동화 스크립트 작성 작업에 최적화되었습니다. Azure CLI 2.0을 사용하면 간단하게 다음 명령을 입력하여 Azure 내에서 VM을 만들 수 있습니다.

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

[Cloud Shell](/azure/cloud-shell/overview)을 사용하여 CLI 브라우저에서 실행하거나 macOS, Linux 또는 Windows에서 [설치](install-azure-cli.md)합니다.
[시작](get-started-with-azure-cli.md) 문서를 읽고 CLI 사용을 시작합니다.
최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.

다음 샘플을 통해 Azure CLI 2.0으로 일반 시나리오를 수행하는 방법을 배울 수 있습니다.
- [Linux 가상 컴퓨터](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Windows 가상 컴퓨터](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL 데이터베이스](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

각 Azure CLI 2.0 명령을 사용하는 방법이 설명된 자세한 [참고 자료](/cli/azure/)도 제공됩니다.

지금 Azure CLI 2.0을 [시작](get-started-with-azure-cli.md)하세요.


> [!NOTE]
> 이전 버전의 CLI(Azure CLI)를 사용하는 경우 계속 사용해도 됩니다.
> 두 CLI를 모두 사용하는 경우 `azure`는 기존 CLI(Azure CLI)이고 `az`는 새 CLI(Azure CLI 2.0)라는 사실을 기억하세요. 
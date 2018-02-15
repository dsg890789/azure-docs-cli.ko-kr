---
title: "Windows용 Azure CLI 설치"
description: "Windows에 Azure CLI 2.0을 설치하는 방법"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3e732ea7fae118ddb1564bed28d54d15bab4f7f0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Windows에 Azure CLI 2.0 설치

MSI를 통해 Azure CLI 이진을 Windows에 설치하면 Windows 명령 프롬프트(CMD) 또는 PowerShell을 통해 CLI에 대한 액세스 권한을 제공 합니다.
WSL(Linux용 Windows 하위 시스템)을 실행하는 경우 Linux 배포에 사용할 수 있는 패키지가 있습니다. 지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.

## <a name="install-or-update"></a>설치 또는 업데이트

MSI 배포판은 Windows에서 `az` 명령을 설치, 업데이트 및 제거하는 데 사용됩니다.

> [!div class="nextstepaction"]
> [MSI 설치 관리자 다운로드](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.

이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다. PowerShell은 CMD에서 사용할 수 없는 일부 탭 완성 기능을 제공합니다.

## <a name="uninstall"></a>제거

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

MSI를 다시 실행 하 고 "제거" 옵션을 선택하여 제거할 수 있습니다.

> [!div class="nextstepaction"]
> [MSI 설치 관리자 다운로드](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

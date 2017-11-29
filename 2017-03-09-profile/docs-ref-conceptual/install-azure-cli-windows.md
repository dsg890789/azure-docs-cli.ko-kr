---
title: "Windows용 Azure CLI 설치"
description: "Windows에 Azure CLI 2.0을 설치하는 방법"
keywords: "Azure CLI,Azure CLI 설치,azure 설치 windows, azure cli windows, azure windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 96a123575226f281accf125cb5bb29ee7d14ef2a
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Windows에 Azure CLI 2.0 설치

Windows에서, Windows 명령 프롬프트 또는 PowerShell을 통해 사용할 수 있는 MSI로 네이티브 이진 파일을 설치할 수 있습니다. WSL(Linux용 Windows 하위 시스템)을 실행하는 경우 실행 중인 배포에 사용할 수 있는 패키지가 있습니다. 지원되는 패키지 관리자 목록 또는 WSL에서 수동으로 설치하는 방법은 [주 설치 페이지](install-azure-cli.md)를 참조하세요.

## <a name="install-or-update-with-msi"></a>MSI를 사용하여 설치 또는 업데이트

MSI 배포판은 Windows에서 `az` 명령을 설치, 업데이트 및 제거하는 데 사용됩니다. [MSI 설치 관리자를 다운로드](https://aka.ms/InstallAzureCliWindows)한 후 실행하여 설치 또는 업데이트할 수 있습니다.

설치 관리자가 컴퓨터를 변경해도 되는지 물어보면 "예" 상자를 클릭합니다.

이제 Windows 명령 프롬프트 또는 PowerShell에서 `az` 명령으로 Azure CLI를 실행할 수 있습니다.

## <a name="uninstall-with-msi"></a>MSI를 사용하여 제거

Azure CLI를 제거하려는 경우 유감스럽게 생각합니다. 제거하기 전에 `az feedback` 명령을 사용하여 제거하시는 이유와 CLI 환경 개선을 위한 조건을 남겨주시기 바랍니다. 버그 없고 사용자에게 친숙한 Azure CLI를 만드는 것이 목적입니다. 또한 [github 문제를 제출](https://github.com/Azure/azure-cli/issues)할 수 있습니다.

MSI를 다시 실행 하 고 "제거" 옵션을 선택하여 제거할 수 있습니다. MSI 설치 관리자가 없는 경우 [MSI 설치 관리자를 다운로드](https://aka.ms/InstallAzureCliWindows)할 수 있습니다.

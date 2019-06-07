---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516257"
---
<span data-ttu-id="03e14-101">프록시로 인해 외부 리소스에 연결할 수 없는 경우 셸에서 `HTTP_PROXY` 및 `HTTPS_PROXY` 변수를 올바르게 설정했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="03e14-102">이러한 프록시에 사용할 호스트와 포트를 확인하려면 시스템 관리자에게 문의해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="03e14-103">이러한 값은 설치 프로세스에서 사용되는 값을 포함하여 많은 Linux 프로그램에서 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="03e14-104">이러한 값을 설정하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="03e14-105">프록시를 지원하는 경우 CLI를 사용하여 이러한 셸 변수를 Azure 서비스에 연결하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="03e14-106">기본 인증을 사용하지 않는 경우 `.bashrc` 파일에서 이러한 변수를 내보내는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="03e14-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="03e14-107">항상 회사의 보안 정책과 시스템 관리자의 요구 사항을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="03e14-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>

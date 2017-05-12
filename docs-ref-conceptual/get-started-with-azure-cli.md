---
title: "Azure CLI 2.0 시작"
description: "Linux, Mac 또는 Windows에서 Azure CLI 2.0을 시작합니다."
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
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 0f8e494ffdd73c666b8361488db0966af01d6876
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/11/2017
---
# <a name="get-started-with-azure-cli-20"></a>Azure CLI 2.0 시작

Azure CLI 2.0은 Azure 리소스를 관리하기 위한 Azure의 새로운 명령줄 환경입니다.
macOS, Linux 및 Windows에서 사용할 수 있습니다. 

Azure CLI 2.0은 명령줄에서 Azure 리소스를 관리하는 작업 및 Azure Resource Manager에 대해 작동하는 자동화 스크립트 작성 작업에 최적화되었습니다.
이 문서에서는 Azure CLI 2.0을 시작하는 방법 및 핵심 개념을 설명합니다.

최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.

## <a name="install-azure-cli"></a>Azure CLI 설치

첫 번째 단계는 최신 버전의 Azure CLI를 설치하는 것입니다.

1. 사용하는 플랫폼에 [Azure CLI 2.0을 설치](install-azure-cli.md)합니다.

2. 설치가 완료되었는지 확인하려면 명령줄에서 `az --version` 명령을 실행합니다. 

Azure CLI 및 컴퓨터에 설치된 기타 종속 라이브러리의 버전 번호가 표시됩니다.  
  
오류가 발생하는 경우 CLI를 설치하는 과정에서 문제가 발생했을 가능성이 있습니다. [Azure CLI 2.0 설치 문서](install-azure-cli.md#troubleshooting)의 "설치 문제 해결" 섹션에서 지침을 검토하거나 해당 페이지 맨 아래의 토론에 도움을 요청하는 글을 올리세요.

## <a name="log-in-to-azure"></a>Azure에 로그인

Azure CLI 2.0을 설치했으니, 다음 단계로 넘어가서 Azure 계정과 안전하게 연결해야 합니다. `az login` 명령을 사용합니다.

1. 명령줄에서 다음 명령을 실행합니다.

   ```azurecli-interactive
   az login
   ```
   
   이 명령은 다음 단계에서 사용할 코드를 출력합니다. 

2. 웹 브라우저를 사용하여 [https://aka.ms/devicelogin](https://aka.ms/devicelogin) 페이지를 열고 코드를 입력합니다.
  
3. 프롬프트가 나타나면 Azure 자격 증명을 사용하여 로그인합니다.

이제 계정에 제공되는 Azure 리소스 및 서비스에서 Azure CLI 2.0으로 명령을 실행할 수 있습니다.

## <a name="create-a-resource-group"></a>리소스 그룹 만들기

모든 설정이 완료되었으니, 이제부터 Azure CLI를 사용하여 Azure 내에 리소스를 만들어 보겠습니다.

먼저 리소스 그룹을 만듭니다.  Azure의 리소스 그룹은 논리적으로 그룹화하려는 여러 리소스를 관리하는 방법을 제공합니다.  예를 들어 응용 프로그램 또는 프로젝트에 대한 리소스 그룹을 만들고 그 안에 가상 컴퓨터, 데이터베이스 및 CDN 서비스를 추가할 수 있습니다.

Azure의 *westus2* 지역에 "MyResourceGroup"이라는 이름의 리소스 그룹을 만듭니다.  이렇게 하려면 다음 명령을 입력합니다.

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

리소스 그룹이 만들어지면 `az group create` 명령이 새로 생성된 리소스의 여러 속성을 출력합니다.

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a>Linux 가상 컴퓨터 만들기

리소스 그룹이 생겼으니, 그 안에 Linux VM을 만들어 보겠습니다.

10GB 및 20GB 저장소 디스크 두 개가 연결된 인기 있는 UbuntuTLS 이미지와 다음 명령을 사용하여 Linux VM을 만들 수 있습니다.

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

앞에서 말한 명령을 실행하면 Azure CLI 2.0이 ~/.ssh 디렉터리 아래에 저장된 SSH 키 쌍을 찾습니다.  여기에 저장된 SSH 키 쌍이 없으면 --generate-ssh-keys 매개 변수를 전달하여 Azure CLI가 자동으로 생성하게 할 수 있습니다.

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --generate-ssh-keys
```

VM이 완전히 생성되어 액세스 및 사용 준비를 마치면 `az vm create` 명령이 출력을 반환합니다. 출력에는 공용 IP 주소를 포함하여 새로 만든 VM의 여러 속성이 포함됩니다.

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

VM을 만들었으니, **SSH**를 사용하여 앞에서 만든 VM의 공용 IP 주소로 새 Linux VM에 로그온할 수 있습니다.

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a>Windows Server 가상 컴퓨터 만들기

이제 `az vm create` 명령을 사용하여 Windows Server 2016 Datacenter 기반 VM을 만들고, Linux VM에 사용한 것과 동일한 "MyResourceGroup" 리소스 그룹에 추가하겠습니다.  Linux VM 예제와 마찬가지로 `--data-disk-sizes-gb` 매개 변수를 사용하여 두 개의 저장소 디스크를 연결하겠습니다.

Azure에서는 예측하기 어려운 사용자 이름/암호를 사용해야 합니다. 사용 가능한 문자와 사용자 이름 및 암호의 최소 길이에 대한 구체적인 규칙이 있습니다.  

> [!NOTE]
> 이 명령을 실행하면 사용자 이름 및 암호를 입력하라는 메시지가 표시됩니다.

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

VM이 완전히 생성되어 액세스 및 사용 준비를 마치면 `az vm create` 명령이 결과를 출력합니다.

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

이제 원격 데스크톱 및 VM(`az vm create`의 출력에 반환된)의 공용 IP 주소를 사용하여 새로 만든 Windows Server VM에 로그온합니다.  
Windows 기반 시스템을 사용하는 경우 명령줄에서 `mstsc` 명령을 사용하여 다음과 같은 일을 할 수 있습니다.

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

로그인할 VM을 만들 때 사용한 것과 동일한 사용자 이름/암호 조합을 제공합니다.

## <a name="creating-other-resources-in-azure"></a>Azure에서 다른 리소스 만들기

지금까지 리소스 그룹, Linux VM 및 Windows Server VM을 만드는 방법을 살펴보았습니다. 여러 다른 유형의 Azure 리소스도 만들 수 있습니다.  

모든 새 리소스는 일관적인 `az <resource type name> create` 명명 패턴을 사용하여 생성됩니다.  예를 들어 Azure 네트워크 부하 분산 장치를 만든 후 새로 만든 VM과 연결하려면 다음 만들기 명령을 사용합니다.

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

다음 만들기 명령을 사용하여 인프라에 대한 새 개인 가상 네트워크(일반적으로 Azure 내에서는 "VNet"이라고 함)를 만들 수도 있습니다.

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

Azure 및 Azure CLI가 강력한 이유는 클라우드 기반 인프라를 가져오는 데 사용할 수 있을 뿐 아니라 관리형 플랫폼 서비스를 만드는 데도 사용할 수 있기 때문입니다.  관리형 플랫폼 서비스를 인프라와 결합하면 더욱 강력한 솔루션을 구축할 수 있습니다.

예를 들어 Azure CLI를 사용하여 Azure AppService를 만들 수 있습니다.  Azure AppService는 인프라에 대한 걱정 없이 웹앱을 호스트하는 훌륭한 방법을 제공하는 관리형 플랫폼 서비스입니다.  Azure AppService를 만든 후에는 다음 만들기 명령을 사용하여 AppService 내에서 두 개의 새 Azure Web Apps를 만들 수 있습니다.

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

`az <resource type name> create` 패턴의 기본을 이해하고 나면 무엇이든 쉽게 만들 수 있습니다. 다음은 몇 가지 인기 있는 Azure 리소스 유형과 해당 유형을 만드는 해당 Azure CLI 만들기 명령입니다.

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

앞서 언급한 각 명령에 전달할 수 있는 추가 리소스별 매개 변수 및 사용자가 만들 수 있는 리소스 유형에 대한 자세한 내용은 [참조 설명서](/azure/doc-ref-autogen)를 참조하세요. 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>유용한 팁: --no-wait를 사용하여 만들기 작업 최적화

기본적으로 Azure CLI 2.0을 사용하여 리소스를 만들 때 `az <resource type name> create` 명령은 리소스가 생성되고 사용 준비가 완료될 때까지 기다립니다.  예를 들어 VM을 만들 때, `az vm create` 명령은 기본적으로 VM이 생성되고 사용자가 그 VM에 SSH 또는 RDP 작업을 수행할 수 있을 때까지 결과를 반환하지 않습니다.

이 접근 방식을 사용하는 이유는 종속성이 있는 여러 단계를 포함하고 있는(그리고 계속하려면 이전 작업을 성공적으로 완료해야 하는) 자동화 스크립트를 좀 더 쉽게 작성할 수 있기 때문입니다.

리소스가 생성될 때까지 기다리지 않고도 계속 진행할 수 있다면 `no-wait` 옵션을 사용하여 백그라운드에서 만들기 작업을 시작할 수 있습니다. 다른 명령에 CLI를 계속 사용할 수 있습니다.

예를 들어 다음 `az vm create` 명령을 사용하면 VM 배포가 시작된 후 훨씬 빠르게(그리고 VM이 완전히 부팅되기 전에) 더 많은 결과를 반환합니다.

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

`--no-wait` 접근 방식을 사용하면 자동화 스크립트의 성능을 최적화하는 데 많은 도움이 됩니다.

## <a name="listing-resources-and-formatting-output"></a>리소스 나열 및 출력 서식 지정

Azure CLI 내에서 `list` 명령을 사용하여 Azure에서 실행되는 리소스를 찾아 나열할 수 있습니다. 

만들기 명령과 마찬가지로, 모든 리소스 유형에서 동일한 일반적인 `az <resource type name> list` 명명 패턴을 사용하는 Azure CLI 2.0을 사용하여 리소스를 나열할 수 있습니다.  리소스 목록을 보고 싶은 대로 필터링하고 정렬할 수 있는 다양한 출력 형식 및 쿼리 옵션이 제공됩니다.

예를 들어 `az vm list` 명령은 갖고 있는 모든 VM 목록을 표시합니다.   

```azurecli-interactive
az vm list 
```
반환되는 값은 기본적으로 JSON 형식입니다(간단하게 표시하기 위해 출력의 일부만 표시).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...   
]
```

원한다면 `--output` 옵션을 사용하여 출력 형식을 수정할 수 있습니다.  `az vm list` 명령을 실행하여 앞에서 만든 Linux 및 Windows Server VM을 모두 표시하고, 읽기 쉬운 *테이블* 형식 옵션을 사용하여 VM의 가장 일반적인 속성을 함께 표시할 수 있습니다.

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

*tsv* 출력 옵션을 사용하여 텍스트 기반의 탭으로 구분된 형식을 헤더 없이 가져올 수 있습니다.  이 형식은 grep 같은 다른 텍스트 기반 도구로 출력을 전달하려는 경우에 유용합니다. 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
리소스를 나열하고 출력 형식을 지정하는 추가적인 방법에 대한 자세한 내용은 [출력 형식](format-output-azure-cli.md) 문서를 참조하세요.

## <a name="querying-resources-and-shaping-outputs"></a>리소스 쿼리 및 출력 셰이핑

특정 조건을 충족하는 리소스만 쿼리하려는 경우가 종종 있습니다.  

`list` 명령은 간편하게 리소스 그룹 이름으로 리소스를 필터링할 수 있는 기본 지원을 제공합니다.  예를 들어 `--ResourceGroup` 또는 `-g` 매개 변수를 `list` 명령에 전달하여 특정 리소스 그룹 내에 있는 리소스만 검색할 수 있습니다.


```azurecli
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

보다 강력한 쿼리 지원을 원하는 경우 `--query` 매개 변수를 사용하여 *모든* `az` 명령의 결과에 대해 JMESPath 쿼리를 실행하면 됩니다.  JMESPath 쿼리는 반환된 결과의 필터링뿐 아니라 셰이핑에도 사용할 수 있습니다.

예를 들어 다음 명령을 실행하여 "My"라는 문자가 포함된 리소스 그룹 내의 모든 VM 리소스를 쿼리할 수 있습니다.

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

그런 다음 출력을 더욱 구체화하는 JMESPath 쿼리의 셰이핑 기능을 사용하여 다른 값을 출력할 수도 있습니다.  예를 들어 다음 명령은 OS가 Linux 기반인지 아니면 Windows 기반인지 확인하기 위해 VM에서 사용하는 OS 디스크 종류를 검색합니다.

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

Azure CLI의 JMESPath 지원은 강력합니다.  [쿼리](query-azure-cli.md) 문서에서 사용 방법에 대해 자세히 알아보세요.

## <a name="deleting-resources"></a>리소스 삭제

Azure CLI 내에서 `delete` 명령을 사용하여 더 이상 필요 없는 리소스를 삭제할 수 있습니다. `delete` 명령은 `create` 명령과 마찬가지로 모든 종류의 리소스에 사용할 수 있습니다.

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

기본적으로 CLI는 삭제 확인을 요청합니다.  자동화된 스크립트를 위해 이 프롬프트를 표시하지 않을 수 있습니다.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

`delete` 명령을 사용하여 여러 리소스를 한꺼번에 삭제할 수도 있습니다. 예를 들어 다음 명령은 우리가 이 시작 자습서의 모든 샘플에 사용한 "MyResourceGroup" 리소스 그룹에 있는 모든 리소스를 삭제합니다.

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>샘플 받기

Azure CLI 사용 방법을 자세히 알아보려면 [Linux VM](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VM](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [웹앱](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) 및 [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)에 대한 가장 일반적인 스크립트를 확인하세요.

## <a name="read-the-api-reference-docs"></a>API 참조 문서 읽기

[API 참조](/cli/azure)

## <a name="get-help"></a>도움말 보기

Azure CLI는 명령줄에서 실행할 수 있는 웹 문서를 찾아주는 도움말 문서가 기본적으로 포함되어 있습니다.

```azurecli-interactive
az [command-group [command]] -h
```

예를 들어 VM에 사용할 수 있는 명령 및 하위 그룹을 보려면 다음을 사용합니다.

```azurecli-interactive
az vm -h
```

VM을 만드는 명령과 관련된 도움말을 보려면 다음을 사용합니다.

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Azure CLI 1.0에서 전환

Azure CLI 1.0(azure.js) 사용 방법을 이미 알고 있는 분들은 명령이 약간 다른 부분을 알아볼 수 있을 것입니다.
작업을 실행하는 명령이 약간 다른 경우가 가끔 있습니다.
Azure CLI 1.0에서 Azure CLI 2.0으로의 전환을 도와드리기 위해 이 [명령 매핑](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst)을 시작했습니다.

## <a name="send-us-your-feedback"></a>사용자 의견을 보냅니다.

```azurecli-interactive
az feedback
```

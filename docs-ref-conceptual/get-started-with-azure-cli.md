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
ms.openlocfilehash: 274336acbf09a21d45b6ef3868f5f7f21757831b
ms.sourcegitcommit: 21c42ed07c9f7679e4860013ac5647cf31213f4e
ms.contentlocale: ko-KR
ms.lasthandoff: 05/22/2017
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="00219-104">Azure CLI 2.0 시작</span><span class="sxs-lookup"><span data-stu-id="00219-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="00219-105">Azure CLI 2.0은 Azure 리소스를 관리하기 위한 Azure의 새로운 명령줄 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-105">The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.</span></span>
<span data-ttu-id="00219-106">[Azure Cloud Shell](/azure/cloud-shell/overview)을 실행하는 브라우저에서 사용하거나 macOS, Linux 및 Windows에서 [설치](install-azure-cli.md)하고 명령줄에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="00219-107">Azure CLI 2.0은 명령줄에서 Azure 리소스를 관리하는 작업 및 Azure Resource Manager에 대해 작동하는 자동화 스크립트 작성 작업에 최적화되었습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span>
<span data-ttu-id="00219-108">이 문서에서는 Azure CLI 2.0을 시작하는 방법 및 핵심 개념을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-108">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

<span data-ttu-id="00219-109">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="00219-109">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

## <a name="connect"></a><span data-ttu-id="00219-110">연결</span><span class="sxs-lookup"><span data-stu-id="00219-110">Connect</span></span>

<span data-ttu-id="00219-111">가장 간단하게 시작하는 방법은 [Cloud Shell을 실행](/azure.cloud-shell/quickstart)하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-111">The simplest way to get started is to [launch  Cloud Shell](/azure.cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="00219-112">Azure Portal의 위쪽 탐색 모음에서 Cloud Shell을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-112">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![셸 아이콘](media/get-started-with-azure-cli/shell-icon.png)

2. <span data-ttu-id="00219-114">사용하려는 구독을 선택하고 저장소 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="00219-114">Choose the subscription you want to use and create a storage account.</span></span>

   ![저장소 계정 만들기](media/get-started-with-azure-cli/storage-prompt.png)

<span data-ttu-id="00219-116">CLI를 [설치](install-azure-cli.md)하고 명령줄에서 로컬로 실행할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-116">You can also [install](install-azure-cli.md) the CLI and run it locally form the command line.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="00219-117">리소스 그룹 만들기</span><span class="sxs-lookup"><span data-stu-id="00219-117">Create a Resource Group</span></span>

<span data-ttu-id="00219-118">모든 설정이 완료되었으니, 이제부터 Azure CLI를 사용하여 Azure 내에 리소스를 만들어 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-118">Now that we've got everything set up, let's use the Azure CLI to create resources within Azure.</span></span>

<span data-ttu-id="00219-119">먼저 리소스 그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="00219-119">First, create a Resource Group.</span></span>  <span data-ttu-id="00219-120">Azure의 리소스 그룹은 논리적으로 그룹화하려는 여러 리소스를 관리하는 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-120">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group.</span></span>  <span data-ttu-id="00219-121">예를 들어 응용 프로그램 또는 프로젝트에 대한 리소스 그룹을 만들고 그 안에 가상 컴퓨터, 데이터베이스 및 CDN 서비스를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-121">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="00219-122">Azure의 *westus2* 지역에 "MyResourceGroup"이라는 이름의 리소스 그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="00219-122">Let's create a resource group named "MyResourceGroup" in the *westus2* region of Azure.</span></span>  <span data-ttu-id="00219-123">이렇게 하려면 다음 명령을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-123">To do so type the following command:</span></span>

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

<span data-ttu-id="00219-124">리소스 그룹이 만들어지면 `az group create` 명령이 새로 생성된 리소스의 여러 속성을 출력합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-124">Once the resource group has been created, the `az group create` command outputs several properties of the newly created resource:</span></span>

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

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="00219-125">Linux 가상 컴퓨터 만들기</span><span class="sxs-lookup"><span data-stu-id="00219-125">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="00219-126">리소스 그룹이 생겼으니, 그 안에 Linux VM을 만들어 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-126">Now that we have our resource group, let's create a Linux VM within it.</span></span>

<span data-ttu-id="00219-127">10GB 및 20GB 저장소 디스크 두 개가 연결된 인기 있는 UbuntuTLS 이미지와 다음 명령을 사용하여 Linux VM을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-127">You can create a Linux VM using the popular UbuntuTLS image, with two attached storage disks of 10 GB and 20 GB, with the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

<span data-ttu-id="00219-128">앞에서 말한 명령을 실행하면 Azure CLI 2.0이 ~/.ssh 디렉터리 아래에 저장된 SSH 키 쌍을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-128">When you run the preceding command, the Azure CLI 2.0 looks for an SSH key pair stored under your ~/.ssh directory.</span></span>  <span data-ttu-id="00219-129">여기에 저장된 SSH 키 쌍이 없으면 --generate-ssh-keys 매개 변수를 전달하여 Azure CLI가 자동으로 생성하게 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-129">If you don't already have an SSH key pair stored there, you can ask the Azure CLI to automatically create one for you by passing the --generate-ssh-keys parameter:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --generate-ssh-keys
```

<span data-ttu-id="00219-130">VM이 완전히 생성되어 액세스 및 사용 준비를 마치면 `az vm create` 명령이 출력을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-130">The `az vm create` command returns output once the VM has been fully created and is ready to be accessed and used.</span></span> <span data-ttu-id="00219-131">출력에는 공용 IP 주소를 포함하여 새로 만든 VM의 여러 속성이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-131">The output includes several properties of the newly created VM including its public IP address:</span></span>

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

<span data-ttu-id="00219-132">VM을 만들었으니, **SSH**를 사용하여 앞에서 만든 VM의 공용 IP 주소로 새 Linux VM에 로그온할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-132">Now that the VM has been created, you can log on to your new Linux VM using **SSH** with the public IP address of the VM you created:</span></span>

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

## <a name="create-a-windows-server-virtual-machine"></a><span data-ttu-id="00219-133">Windows Server 가상 컴퓨터 만들기</span><span class="sxs-lookup"><span data-stu-id="00219-133">Create a Windows Server Virtual Machine</span></span>

<span data-ttu-id="00219-134">이제 `az vm create` 명령을 사용하여 Windows Server 2016 Datacenter 기반 VM을 만들고, Linux VM에 사용한 것과 동일한 "MyResourceGroup" 리소스 그룹에 추가하겠습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-134">Let's now create a Windows Server 2016 Datacenter-based VM using the `az vm create` command and add it to the same "MyResourceGroup" resource group that we used for our Linux VM.</span></span>  <span data-ttu-id="00219-135">Linux VM 예제와 마찬가지로 `--data-disk-sizes-gb` 매개 변수를 사용하여 두 개의 저장소 디스크를 연결하겠습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-135">Like the Linux VM example, we'll also attach two storage disks using the `--data-disk-sizes-gb` parameter.</span></span>

<span data-ttu-id="00219-136">Azure에서는 예측하기 어려운 사용자 이름/암호를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-136">Azure requires that you avoid using easily guessed usernames/passwords.</span></span> <span data-ttu-id="00219-137">사용 가능한 문자와 사용자 이름 및 암호의 최소 길이에 대한 구체적인 규칙이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-137">There are specific rules for what characters can be used as well as the minimum length of both username and password.</span></span>  

> [!NOTE]
> <span data-ttu-id="00219-138">이 명령을 실행하면 사용자 이름 및 암호를 입력하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-138">You will be prompted to enter your username and password when running this command.</span></span>

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

<span data-ttu-id="00219-139">VM이 완전히 생성되어 액세스 및 사용 준비를 마치면 `az vm create` 명령이 결과를 출력합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-139">The `az vm create` command output results once the VM has been fully created and is ready to be accessed and used.</span></span>

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

<span data-ttu-id="00219-140">이제 원격 데스크톱 및 VM(`az vm create`의 출력에 반환된)의 공용 IP 주소를 사용하여 새로 만든 Windows Server VM에 로그온합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-140">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM (which is returned in the output from `az vm create`).</span></span>  
<span data-ttu-id="00219-141">Windows 기반 시스템을 사용하는 경우 명령줄에서 `mstsc` 명령을 사용하여 다음과 같은 일을 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-141">If you are on a Windows-based system, you can do this from the command line using the `mstsc` command:</span></span>

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="00219-142">로그인할 VM을 만들 때 사용한 것과 동일한 사용자 이름/암호 조합을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-142">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="00219-143">Azure에서 다른 리소스 만들기</span><span class="sxs-lookup"><span data-stu-id="00219-143">Creating other resources in Azure</span></span>

<span data-ttu-id="00219-144">지금까지 리소스 그룹, Linux VM 및 Windows Server VM을 만드는 방법을 살펴보았습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-144">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="00219-145">여러 다른 유형의 Azure 리소스도 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-145">You can create many other types of Azure resources as well.</span></span>  

<span data-ttu-id="00219-146">모든 새 리소스는 일관적인 `az <resource type name> create` 명명 패턴을 사용하여 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-146">All new resources are created using a consistent `az <resource type name> create` naming pattern.</span></span>  <span data-ttu-id="00219-147">예를 들어 Azure 네트워크 부하 분산 장치를 만든 후 새로 만든 VM과 연결하려면 다음 만들기 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-147">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

<span data-ttu-id="00219-148">다음 만들기 명령을 사용하여 인프라에 대한 새 개인 가상 네트워크(일반적으로 Azure 내에서는 "VNet"이라고 함)를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-148">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following create command:</span></span>

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

<span data-ttu-id="00219-149">Azure 및 Azure CLI가 강력한 이유는 클라우드 기반 인프라를 가져오는 데 사용할 수 있을 뿐 아니라 관리형 플랫폼 서비스를 만드는 데도 사용할 수 있기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-149">What makes Azure and the Azure CLI powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span>  <span data-ttu-id="00219-150">관리형 플랫폼 서비스를 인프라와 결합하면 더욱 강력한 솔루션을 구축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-150">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="00219-151">예를 들어 Azure CLI를 사용하여 Azure AppService를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-151">For example, you can use the Azure CLI to create an Azure AppService.</span></span>  <span data-ttu-id="00219-152">Azure AppService는 인프라에 대한 걱정 없이 웹앱을 호스트하는 훌륭한 방법을 제공하는 관리형 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-152">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span>  <span data-ttu-id="00219-153">Azure AppService를 만든 후에는 다음 만들기 명령을 사용하여 AppService 내에서 두 개의 새 Azure Web Apps를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-153">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following create commands:</span></span>

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

<span data-ttu-id="00219-154">`az <resource type name> create` 패턴의 기본을 이해하고 나면 무엇이든 쉽게 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-154">Once you understand the basics of the `az <resource type name> create` pattern, it becomes easy to create anything.</span></span> <span data-ttu-id="00219-155">다음은 몇 가지 인기 있는 Azure 리소스 유형과 해당 유형을 만드는 해당 Azure CLI 만들기 명령입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-155">Following are some popular Azure resource types and the corresponding Azure CLI create commands to create them:</span></span>

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

<span data-ttu-id="00219-156">앞서 언급한 각 명령에 전달할 수 있는 추가 리소스별 매개 변수 및 사용자가 만들 수 있는 리소스 유형에 대한 자세한 내용은 [참조 설명서](/cli/azure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="00219-156">Visit the [Reference documentation](/cli/azure) to learn more about the additional resource-specific parameters that you can pass to each of the preceding commands and the resource types you can create.</span></span> 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a><span data-ttu-id="00219-157">유용한 팁: --no-wait를 사용하여 만들기 작업 최적화</span><span class="sxs-lookup"><span data-stu-id="00219-157">Useful tip: Optimizing create operations using --no-wait</span></span>

<span data-ttu-id="00219-158">기본적으로 Azure CLI 2.0을 사용하여 리소스를 만들 때 `az <resource type name> create` 명령은 리소스가 생성되고 사용 준비가 완료될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="00219-158">By default when you create resources using the Azure CLI 2.0, the `az <resource type name> create` command waits until the resource has been created and is ready for you to use.</span></span>  <span data-ttu-id="00219-159">예를 들어 VM을 만들 때, `az vm create` 명령은 기본적으로 VM이 생성되고 사용자가 그 VM에 SSH 또는 RDP 작업을 수행할 수 있을 때까지 결과를 반환하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-159">For example, if you create a VM, the `az vm create` command will, by default, not return until the VM is created and is ready for you to SSH or RDP into it.</span></span>

<span data-ttu-id="00219-160">이 접근 방식을 사용하는 이유는 종속성이 있는 여러 단계를 포함하고 있는(그리고 계속하려면 이전 작업을 성공적으로 완료해야 하는) 자동화 스크립트를 좀 더 쉽게 작성할 수 있기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-160">We use this approach because it makes it easier to write automation scripts that contain multiple steps with dependencies (and need a prior task to have completed successfully before continuing).</span></span>

<span data-ttu-id="00219-161">리소스가 생성될 때까지 기다리지 않고도 계속 진행할 수 있다면 `no-wait` 옵션을 사용하여 백그라운드에서 만들기 작업을 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-161">If you do not need to wait on creation of a resource before continuing, you can use the `no-wait` option to start a create action in the background.</span></span> <span data-ttu-id="00219-162">다른 명령에 CLI를 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-162">You can continue using the CLI for other commands.</span></span>

<span data-ttu-id="00219-163">예를 들어 다음 `az vm create` 명령을 사용하면 VM 배포가 시작된 후 훨씬 빠르게(그리고 VM이 완전히 부팅되기 전에) 더 많은 결과를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-163">For example, the following usage of the `az vm create` starts a VM deployment and then return much more quickly (and before the VM has fully booted):</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

<span data-ttu-id="00219-164">`--no-wait` 접근 방식을 사용하면 자동화 스크립트의 성능을 최적화하는 데 많은 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-164">Using the `--no-wait` approach can help you optimize the performance of your automation scripts considerably.</span></span>

## <a name="listing-resources-and-formatting-output"></a><span data-ttu-id="00219-165">리소스 나열 및 출력 서식 지정</span><span class="sxs-lookup"><span data-stu-id="00219-165">Listing resources and formatting output</span></span>

<span data-ttu-id="00219-166">Azure CLI 내에서 `list` 명령을 사용하여 Azure에서 실행되는 리소스를 찾아 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-166">You can use the `list` command within the Azure CLI to find and list the resources running in Azure.</span></span> 

<span data-ttu-id="00219-167">만들기 명령과 마찬가지로, 모든 리소스 유형에서 동일한 일반적인 `az <resource type name> list` 명명 패턴을 사용하는 Azure CLI 2.0을 사용하여 리소스를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-167">Like with the create command, you can list resources using the Azure CLI 2.0 using a common `az <resource type name> list` naming pattern that is consistent across all resource types.</span></span>  <span data-ttu-id="00219-168">리소스 목록을 보고 싶은 대로 필터링하고 정렬할 수 있는 다양한 출력 형식 및 쿼리 옵션이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-168">There are various output formats and query options available to filter and sort the list of resources in the way you prefer to see them.</span></span>

<span data-ttu-id="00219-169">예를 들어 `az vm list` 명령은 갖고 있는 모든 VM 목록을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-169">For example, `az vm list` shows the list of all VMs you have.</span></span>   

```azurecli-interactive
az vm list 
```
<span data-ttu-id="00219-170">반환되는 값은 기본적으로 JSON 형식입니다(간단하게 표시하기 위해 출력의 일부만 표시).</span><span class="sxs-lookup"><span data-stu-id="00219-170">The values returned are by default in JSON (only showing partial output for sake of brevity).</span></span>

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

<span data-ttu-id="00219-171">원한다면 `--output` 옵션을 사용하여 출력 형식을 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-171">You can optionally modify the output format using the `--output` option.</span></span>  <span data-ttu-id="00219-172">`az vm list` 명령을 실행하여 앞에서 만든 Linux 및 Windows Server VM을 모두 표시하고, 읽기 쉬운 *테이블* 형식 옵션을 사용하여 VM의 가장 일반적인 속성을 함께 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-172">Run the `az vm list` command to see both the Linux and Windows Server VMs created earlier, along with the most common properties of a VM, using the easy to read *table* format option:</span></span>

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="00219-173">*tsv* 출력 옵션을 사용하여 텍스트 기반의 탭으로 구분된 형식을 헤더 없이 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-173">The *tsv* output option can be used to get a text-based, tab-separated format without any headers.</span></span>  <span data-ttu-id="00219-174">이 형식은 grep 같은 다른 텍스트 기반 도구로 출력을 전달하려는 경우에 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-174">This format is useful when you want to pipe the output into another text-based tool like grep.</span></span> 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
<span data-ttu-id="00219-175">리소스를 나열하고 출력 형식을 지정하는 추가적인 방법에 대한 자세한 내용은 [출력 형식](format-output-azure-cli.md) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="00219-175">Visit the [output formats](format-output-azure-cli.md) article to learn more about the additional ways to list resources and format the output.</span></span>

## <a name="querying-resources-and-shaping-outputs"></a><span data-ttu-id="00219-176">리소스 쿼리 및 출력 셰이핑</span><span class="sxs-lookup"><span data-stu-id="00219-176">Querying resources and shaping outputs</span></span>

<span data-ttu-id="00219-177">특정 조건을 충족하는 리소스만 쿼리하려는 경우가 종종 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-177">Often you want to be able to query for only those resources that meet a specific condition.</span></span>  

<span data-ttu-id="00219-178">`list` 명령은 간편하게 리소스 그룹 이름으로 리소스를 필터링할 수 있는 기본 지원을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-178">The `list` command has built-in support that makes it easy to filter resources by Resource Group name.</span></span>  <span data-ttu-id="00219-179">예를 들어 `--ResourceGroup` 또는 `-g` 매개 변수를 `list` 명령에 전달하여 특정 리소스 그룹 내에 있는 리소스만 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-179">For example, you can pass either a `--ResourceGroup` or `-g` parameter to a `list` command to only retrieve those resources within a specific resource group:</span></span>


```azurecli
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="00219-180">보다 강력한 쿼리 지원을 원하는 경우 `--query` 매개 변수를 사용하여 *모든* `az` 명령의 결과에 대해 JMESPath 쿼리를 실행하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00219-180">For even more powerful querying support, you can use the `--query` parameter to execute a JMESPath query on the results of *any* `az` command.</span></span>  <span data-ttu-id="00219-181">JMESPath 쿼리는 반환된 결과의 필터링뿐 아니라 셰이핑에도 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-181">JMESPath queries can be used both to filter as well as shape the output of any returned result.</span></span>

<span data-ttu-id="00219-182">예를 들어 다음 명령을 실행하여 "My"라는 문자가 포함된 리소스 그룹 내의 모든 VM 리소스를 쿼리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-182">For example, execute the following command to query for any VM resource within any resource group that contains the letters "My":</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="00219-183">그런 다음 출력을 더욱 구체화하는 JMESPath 쿼리의 셰이핑 기능을 사용하여 다른 값을 출력할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-183">We could then choose to further refine the output by using the shaping capability of JMESPath queries to output different values as well.</span></span>  <span data-ttu-id="00219-184">예를 들어 다음 명령은 OS가 Linux 기반인지 아니면 Windows 기반인지 확인하기 위해 VM에서 사용하는 OS 디스크 종류를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-184">For example, the following command retrieves the type of OS disk the VM is using to determine whether the OS is Linux or Windows based:</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

<span data-ttu-id="00219-185">Azure CLI의 JMESPath 지원은 강력합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-185">The JMESPath support in Azure CLI is powerful.</span></span>  <span data-ttu-id="00219-186">[쿼리](query-azure-cli.md) 문서에서 사용 방법에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="00219-186">Learn more about how to use it in our [query](query-azure-cli.md) article.</span></span>

## <a name="deleting-resources"></a><span data-ttu-id="00219-187">리소스 삭제</span><span class="sxs-lookup"><span data-stu-id="00219-187">Deleting resources</span></span>

<span data-ttu-id="00219-188">Azure CLI 내에서 `delete` 명령을 사용하여 더 이상 필요 없는 리소스를 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-188">You can use the `delete` command within Azure CLI to delete the resources you no longer need.</span></span> <span data-ttu-id="00219-189">`delete` 명령은 `create` 명령과 마찬가지로 모든 종류의 리소스에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-189">You can use the `delete` command with any resource just like you can with the `create` command.</span></span>

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

<span data-ttu-id="00219-190">기본적으로 CLI는 삭제 확인을 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-190">By default the CLI prompts to confirm deletion.</span></span>  <span data-ttu-id="00219-191">자동화된 스크립트를 위해 이 프롬프트를 표시하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-191">You can suppress this prompt for automated scripts.</span></span>

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

<span data-ttu-id="00219-192">`delete` 명령을 사용하여 여러 리소스를 한꺼번에 삭제할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-192">You can also use the `delete` command to delete many resources at a time.</span></span> <span data-ttu-id="00219-193">예를 들어 다음 명령은 우리가 이 시작 자습서의 모든 샘플에 사용한 "MyResourceGroup" 리소스 그룹에 있는 모든 리소스를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-193">For example, the following command deletes all the resources in the "MyResourceGroup" resource group that we've used for all the samples in this Get Started tutorial.</span></span>

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a><span data-ttu-id="00219-194">샘플 받기</span><span class="sxs-lookup"><span data-stu-id="00219-194">Get samples</span></span>

<span data-ttu-id="00219-195">Azure CLI 사용 방법을 자세히 알아보려면 [Linux VM](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VM](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [웹앱](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) 및 [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)에 대한 가장 일반적인 스크립트를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="00219-195">To learn more about ways to use the Azure CLI, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), and [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span></span>

## <a name="read-the-api-reference-docs"></a><span data-ttu-id="00219-196">API 참조 문서 읽기</span><span class="sxs-lookup"><span data-stu-id="00219-196">Read the API reference docs</span></span>

[<span data-ttu-id="00219-197">API 참조</span><span class="sxs-lookup"><span data-stu-id="00219-197">API reference</span></span>](/cli/azure)

## <a name="get-help"></a><span data-ttu-id="00219-198">도움말 보기</span><span class="sxs-lookup"><span data-stu-id="00219-198">Get help</span></span>

<span data-ttu-id="00219-199">Azure CLI는 명령줄에서 실행할 수 있는 웹 문서를 찾아주는 도움말 문서가 기본적으로 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-199">The Azure CLI has built-in help documentation, which matches our web documentation that you can run from the command line:</span></span>

```azurecli-interactive
az [command-group [command]] -h
```

<span data-ttu-id="00219-200">예를 들어 VM에 사용할 수 있는 명령 및 하위 그룹을 보려면 다음을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-200">For example, to see what commands and subgroups are available for VMs, use:</span></span>

```azurecli-interactive
az vm -h
```

<span data-ttu-id="00219-201">VM을 만드는 명령과 관련된 도움말을 보려면 다음을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="00219-201">To get help with the command to create a VM, use:</span></span>

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a><span data-ttu-id="00219-202">Azure CLI 1.0에서 전환</span><span class="sxs-lookup"><span data-stu-id="00219-202">Switch from Azure CLI 1.0</span></span>

<span data-ttu-id="00219-203">Azure CLI 1.0(azure.js) 사용 방법을 이미 알고 있는 분들은 명령이 약간 다른 부분을 알아볼 수 있을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="00219-203">If you already know how to use Azure CLI 1.0 (azure.js), you'll notice places where the commands aren't quite the same.</span></span>
<span data-ttu-id="00219-204">작업을 실행하는 명령이 약간 다른 경우가 가끔 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-204">Sometimes the commands to perform a task are significantly different.</span></span>
<span data-ttu-id="00219-205">Azure CLI 1.0에서 Azure CLI 2.0으로의 전환을 도와드리기 위해 이 [명령 매핑](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst)을 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="00219-205">To help you make the switch from Azure CLI 1.0 to Azure CLI 2.0, we've started this [command mapping](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span></span>

## <a name="send-us-your-feedback"></a><span data-ttu-id="00219-206">사용자 의견을 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="00219-206">Send us your feedback</span></span>

```azurecli-interactive
az feedback
```

---
title: Azure CLI를 사용한 쿼리 명령 결과
description: Azure CLI 명령의 출력에 대해 JMESPath 쿼리를 수행하는 방법을 학습합니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: e878c467f71423cc8c9caa1f8cfe270d0019c48b
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194862"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="ff9b4-103">Azure CLI 명령 출력 쿼리</span><span class="sxs-lookup"><span data-stu-id="ff9b4-103">Query Azure CLI command output</span></span>

<span data-ttu-id="ff9b4-104">Azure CLI는 `--query` 인수를 사용하여 명령의 결과에 대해 [JMESPath 쿼리](http://jmespath.org)를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="ff9b4-105">JMESPath는 JSON의 쿼리 언어이며, CLI 출력의 데이터를 선택하고 수정하는 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="ff9b4-106">다른 표시 형식 전에 이러한 쿼리를 JSON 출력에서 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="ff9b4-107">`--query` 인수는 Azure CLI의 모든 명령에서 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="ff9b4-108">이 문서에서는 일련의 간단한 예제를 사용하여 JMESPath의 기능을 사용하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="ff9b4-109">사전 및 CLI 결과 목록</span><span class="sxs-lookup"><span data-stu-id="ff9b4-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="ff9b4-110">JSON이 아닌 출력 형식을 사용하는 경우에도 CLI 명령 결과는 먼저 쿼리용 JSON으로 처리됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="ff9b4-111">CLI 결과는 JSON 배열 또는 사전입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="ff9b4-112">배열은 인덱싱할 수 있는 개체의 시퀀스이며 사전은 키를 사용하여 액세스되는 정렬되지 않은 개체입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="ff9b4-113">둘 이상의 개체를 반환할 _수 있는_ 명령은 배열을 반환하고 _항상_ 단일 개체_만_ 반환하는 명령은 사전을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="ff9b4-114">사전에 속성 가져오기</span><span class="sxs-lookup"><span data-stu-id="ff9b4-114">Get properties in a dictionary</span></span>

<span data-ttu-id="ff9b4-115">사전 결과로 작업하면 키만으로 최상위 레벨에서 속성에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="ff9b4-116">`.`(__subexpression__) 문자를 사용하여 중첩된 사전의 속성을 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="ff9b4-117">쿼리를 도입하기 전에 `az vm show` 명령의 수정되지 않은 출력을 살펴보기:</span><span class="sxs-lookup"><span data-stu-id="ff9b4-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="ff9b4-118">명령은 사전을 출력합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-118">The command will output a dictionary.</span></span> <span data-ttu-id="ff9b4-119">일부 콘텐츠는 생략 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="ff9b4-120">다음 명령은 쿼리를 추가하여 VM에 연결할 수 있는 SSH 공개 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

<span data-ttu-id="ff9b4-121">둘 이상의 속성을 가져오려면 대괄호 `[ ]`(__다중 선택 목록__)에 쉼표로 구분된 목록으로 언어 식을 입력하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-121">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="ff9b4-122">VM 이름, 관리 사용자 및 SSH 키를 모두 한 번에 가져 오려면 다음 명령을 사용하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-122">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="ff9b4-123">이러한 값은 쿼리에서 제공된 순서로 결과 배열에 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-123">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="ff9b4-124">결과가 배열이므로 결과와 연결된 키가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-124">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="get-a-single-value"></a><span data-ttu-id="ff9b4-125">단일 값 가져오기</span><span class="sxs-lookup"><span data-stu-id="ff9b4-125">Get a single value</span></span>

<span data-ttu-id="ff9b4-126">일반적으로 Azure 리소스 ID, 리소스 이름, 사용자 이름 또는 암호와 같은 CLI 명령에서는 _하나_의 값만 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-126">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="ff9b4-127">이 경우 값을 로컬 환경 변수에 저장하려는 경우도 많습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-127">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="ff9b4-128">단일 속성을 가져오려면 먼저 쿼리에서 하나의 속성만 가져오도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-128">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="ff9b4-129">관리 사용자 이름만 가져오도록 마지막 예제를 다음과 같이 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-129">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="ff9b4-130">여기서는 유효한 단일 값처럼 보이지만 `"` 문자가 출력의 일부로 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-130">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="ff9b4-131">이 문자는 개체가 JSON 문자열임을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-131">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="ff9b4-132">이 값을 명령의 출력으로 환경 변수에 직접 할당하면 셸에서 따옴표가 해석되지 __않을__ 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-132">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="ff9b4-133">이는 거의 확실히 원하는 작업이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-133">This is almost certainly not what you want.</span></span> <span data-ttu-id="ff9b4-134">이 경우 반환된 값을 형식 정보와 함께 포함하지 않는 출력 형식을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-134">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="ff9b4-135">이 용도를 위해 CLI에서 제공하는 최상의 출력 옵션은 `tsv`(탭으로 구분된 값)입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-135">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="ff9b4-136">특히 단일 값(사전이나 목록이 아닌)인 값만 검색할 때 `tsv` 출력이 인용되지 않도록 보장됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-136">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="ff9b4-137">`tsv` 출력 형식에 대한 자세한 내용은 [출력 형식 - TSV 출력 형식](format-output-azure-cli.md#tsv-output-format)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-137">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="ff9b4-138">쿼리에서 속성 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="ff9b4-138">Rename properties in a query</span></span>

<span data-ttu-id="ff9b4-139">여러 값을 쿼리할 때 배열 대신 사전을 가져오려면 `{ }`(__다중 선택 해시__) 연산자를 사용하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-139">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="ff9b4-140">다중 선택 해시 양식은 `{displayName:JMESPathExpression, ...}`입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-140">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="ff9b4-141">`displayName`은 출력에 표시되는 문자열이며 `JMESPathExpression`은 평가할 JMESPath 식입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-141">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="ff9b4-142">다중 선택 목록을 해시로 변경하여 마지막 섹션에서 예제를 수정하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-142">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="ff9b4-143">배열에 속성 가져오기</span><span class="sxs-lookup"><span data-stu-id="ff9b4-143">Get properties in an array</span></span>

<span data-ttu-id="ff9b4-144">배열 자체에 대한 속성은 없지만 인덱싱할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-144">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="ff9b4-145">이 기능은 마지막 예제에서 `publicKeys[0]` 표현식과 함께 표시되며 `publicKeys` 배열의 첫 번째 요소를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-145">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="ff9b4-146">CLI 출력이 명령되었는지 보장할 수 없으므로 명령에 대해 확신하거나 어떤 요소를 얻을지 신경 쓰지 않는 한 색인을 사용하지 마십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-146">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="ff9b4-147">배열의 요소 속성에 액세스하려면 _평면화_ 및 _필터링_ 중 하나를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-147">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="ff9b4-148">이 섹션에서는 배열을 평면화하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-148">This section covers how to flatten an array.</span></span>

<span data-ttu-id="ff9b4-149">배열을 평면화는 `[]` JMESPath 연산자를 사용 하여 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-149">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="ff9b4-150">`[]` 연산자 다음의 모든 표현식은 현재 배열의 각 요소에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-150">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="ff9b4-151">쿼리 시작 부분에 `[]`이 나타나면 CLI 명령 결과가 평면화됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-151">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="ff9b4-152">`az vm list`의 결과는 이 기능을 사용하여 검사할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-152">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="ff9b4-153">리소스 그룹의 각 VM에 대한 이름, OS 및 관리자 이름을 가져오려면:</span><span class="sxs-lookup"><span data-stu-id="ff9b4-153">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="ff9b4-154">`--output table` 출력 양식과 결합하면 열 이름이 다중 선택 해시의 `displayKey` 값과 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-154">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="ff9b4-155">특정 키는 필터링되고 테이블 보기에 인쇄되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-155">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="ff9b4-156">이러한 키는 `id`, `type` 및 `etag`입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-156">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="ff9b4-157">이러한 값을 보려면 multiselect 해시 키 이름을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-157">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="ff9b4-158">명령으로 반환된 최상위 결과뿐만 아니라 모든 배열을 평면화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-158">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="ff9b4-159">마지막 섹션에서는 `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` 식이 로그인에 대한 SSH 공개 키를 가져오기 위해 사용되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-159">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="ff9b4-160">_모든_ SSH 공개 키를 얻으려면 식을 대신 `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`로 작성하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-160">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="ff9b4-161">이 쿼리 식은 `osProfile.linuxConfiguration.ssh.publicKeys` 배열을 평면화한 다음 각 요소에서 `keyData` 식을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-161">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="ff9b4-162">배열 필터링</span><span class="sxs-lookup"><span data-stu-id="ff9b4-162">Filter arrays</span></span>

<span data-ttu-id="ff9b4-163">배열에서 데이터를 가져오는 데 사용되는 다른 작업은 _필터링_입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-163">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="ff9b4-164">필터링은 `[?...]` JMESPath 연산자를 사용하여 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-164">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="ff9b4-165">이 연산자는 내용에 맞게 조건자를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-165">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="ff9b4-166">조건자는 `true` 또는 `false`로 평가할 수 있는 문입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-166">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="ff9b4-167">조건자가 `true`로 평가되는 표현식은 출력에 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-167">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="ff9b4-168">JMESPath는 표준 비교 및 논리 연산자를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-168">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="ff9b4-169">`<`, `<=`, `>`, `>=`, `==`, `!=`을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-169">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="ff9b4-170">JMESPath은 또한 논리 and(`&&`), or(`||`), not(`!`)을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-170">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="ff9b4-171">괄호 안에 식은 그룹화하여 더 복잡한 조건자 식이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-171">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="ff9b4-172">조건자 및 논리 조작에 대한 전체 세부 정보는 [JMESPath 사양](http://jmespath.org/specification.html)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-172">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="ff9b4-173">마지막 섹션에서는 리소스 그룹의 모든 VM의 전체 목록을 가져오기 위해 배열을 평면화했습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-173">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="ff9b4-174">필터를 사용하여, 이 출력은 Linux VM으로만 제한할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-174">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="ff9b4-175">JMESPath에서 문자열은 항상 작은 따옴표(`'`)로 둘러싸입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-175">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="ff9b4-176">필터 조건자에 있는 문자열의 일부로 큰 따옴표를 사용하는 경우 빈 출력을 얻게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-176">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="ff9b4-177">JMESPath에는 또한 필터링에 도움이 될 수 있는 기본 제공 함수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-177">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="ff9b4-178">이러한 함수 중 하나는 `contains(string, substring)`로서, 문자열에 부분 문자열에 포함되어 있는지를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-178">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="ff9b4-179">표현식은 함수를 호출하기 전에 평가되므로 첫 번째 인수가 전체 JMESPath 표현식이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-179">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="ff9b4-180">다음 예제에서는 SSD 스토리지를 사용하여 해당 OS 디스크에 대한 모든 VM을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-180">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="ff9b4-181">이 쿼리는 약간 깁니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-181">This query is a little long.</span></span> <span data-ttu-id="ff9b4-182">`storageProfile.osDisk.managedDisk.storageAccountType` 키는 두 번 언급되며 출력에서 키가 다시 입력됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-182">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="ff9b4-183">이를 줄이는 한 가지 방법은 데이터를 평면화 하고 선택한 후 필터링을 적용하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-183">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="ff9b4-184">대형 배열의 경우, 데이터를 선택하기 전에 필터를 적용하는 것이 더 빠를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-184">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="ff9b4-185">전체 함수 목록은 [JMESPath 스펙 - 내장 함수](http://jmespath.org/specification.html#built-in-functions)를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-185">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="ff9b4-186">출력 변경</span><span class="sxs-lookup"><span data-stu-id="ff9b4-186">Change output</span></span>

<span data-ttu-id="ff9b4-187">JMESPath 함수는 쿼리 결과 대해 작동하는, 다른 목적을 가질 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-187">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="ff9b4-188">부울이 아닌 값을 반환하는 모든 함수는 식의 결과를 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-188">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="ff9b4-189">예를 들어, `sort_by(array, &sort_expression)`를 사용하여 속성 값으로 데이터를 정렬할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-189">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="ff9b4-190">JMESPath는 특수 연산자(`&`)를 사용하여, 함수의 일부로 나중 평가되어야 하는 식에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-190">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="ff9b4-191">다음 예제에서는 OS 디스크 크기에 따라 VM 목록을 정렬하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-191">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="ff9b4-192">전체 함수 목록은 [JMESPath 스펙 - 내장 함수](http://jmespath.org/specification.html#built-in-functions)를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-192">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="ff9b4-193">대화형으로 쿼리를 사용하여 실험</span><span class="sxs-lookup"><span data-stu-id="ff9b4-193">Experiment with queries interactively</span></span>

<span data-ttu-id="ff9b4-194">JMESPath 실험을 시작하기 위해 [JMESPath-터미널](https://github.com/jmespath/jmespath.terminal) Python 패키지는 쿼리 작업을 할 수 있는 대화형 환경을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-194">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="ff9b4-195">데이터는 입력으로 파이프되고 쿼리는 편집기에서 작성 및 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="ff9b4-195">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

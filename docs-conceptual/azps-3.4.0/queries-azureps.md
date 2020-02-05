---
title: Azure PowerShell コマンドレットの出力に対してクエリを実行する
description: Azure のリソースに対してクエリを実行し、その結果の書式を設定する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/10/2019
ms.openlocfilehash: 9141f5640467722608cb7748f425ce3942668fb8
ms.sourcegitcommit: 9181f20c2c5eaa271150de9e25b9cb30ba5e6cb0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "77002777"
---
# <a name="query-output-of-azure-powershell"></a><span data-ttu-id="9d7e2-103">Azure PowerShell の出力に対してクエリを実行する</span><span class="sxs-lookup"><span data-stu-id="9d7e2-103">Query output of Azure PowerShell</span></span> 

<span data-ttu-id="9d7e2-104">各 Azure PowerShell コマンドレットの結果は、Azure PowerShell オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-104">The results of each Azure PowerShell cmdlet are an Azure PowerShell object.</span></span> <span data-ttu-id="9d7e2-105">明示的に `Get-` 操作ではないコマンドレットであっても、検査可能な値を返し、作成または変更されたリソースに関する情報を提供する場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-105">Even cmdlets that aren't explicitly `Get-` operations might return a value that can be inspected, to give information about a resource that was created or modified.</span></span> <span data-ttu-id="9d7e2-106">ほとんどのコマンドレットは単一オブジェクトを返す一方、反復処理される必要のある配列を返すコマンドもあります。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-106">While most cmdlets return a single object, some return an array that should be iterated through.</span></span>

<span data-ttu-id="9d7e2-107">ほぼすべての場合において、[Select-Object](/powershell/module/Microsoft.PowerShell.Utility/Select-Object) コマンドレット (省略形: `select`) を使って Azure PowerShell からの出力に対してクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-107">In almost all cases, you query output from Azure PowerShell with the [Select-Object](/powershell/module/Microsoft.PowerShell.Utility/Select-Object) cmdlet, often abbreviated to `select`.</span></span> <span data-ttu-id="9d7e2-108">出力は [Where-Object](/powershell/module/Microsoft.PowerShell.Core/Where-Object) またはそのエイリアス `where` を使用してフィルターできます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-108">Output can be filtered with [Where-Object](/powershell/module/Microsoft.PowerShell.Core/Where-Object), or its alias `where`.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="9d7e2-109">単純なプロパティを選択する</span><span class="sxs-lookup"><span data-stu-id="9d7e2-109">Select simple properties</span></span>

<span data-ttu-id="9d7e2-110">既定の表形式では、Azure PowerShell コマンドレットにより、使用可能なすべてのプロパティは表示されません。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-110">In the default table format, Azure PowerShell cmdlets don't display all of their available properties.</span></span> <span data-ttu-id="9d7e2-111">完全なプロパティを取得するには、[Format-List](/powershell/module/microsoft.powershell.utility/format-list) コマンドレットを使用するか、出力を `Select-Object *` にパイプ処理します。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-111">You can get the full properties by using the [Format-List](/powershell/module/microsoft.powershell.utility/format-list) cmdlet, or by piping output to `Select-Object *`:</span></span>

```azurepowershell-interactive
Get-AzVM -Name TestVM -ResourceGroupName TestGroup | Select-Object *
```

```output
ResourceGroupName        : TESTGROUP
Id                       : /subscriptions/711d8ed1-b888-4c52-8ab9-66f07b87eb6b/resourceGroups/TESTGROUP/providers/Micro
                           soft.Compute/virtualMachines/TestVM
VmId                     : 711d8ed1-b888-4c52-8ab9-66f07b87eb6b
Name                     : TestVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : westus2
LicenseType              :
Tags                     : {}
AvailabilitySetReference :
DiagnosticsProfile       :
Extensions               : {}
HardwareProfile          : Microsoft.Azure.Management.Compute.Models.HardwareProfile
InstanceView             :
NetworkProfile           : Microsoft.Azure.Management.Compute.Models.NetworkProfile
OSProfile                : Microsoft.Azure.Management.Compute.Models.OSProfile
Plan                     :
ProvisioningState        : Succeeded
StorageProfile           : Microsoft.Azure.Management.Compute.Models.StorageProfile
DisplayHint              : Compact
Identity                 :
Zones                    : {}
FullyQualifiedDomainName :
AdditionalCapabilities   :
RequestId                : 711d8ed1-b888-4c52-8ab9-66f07b87eb6b
StatusCode               : OK
```

<span data-ttu-id="9d7e2-112">関心のあるプロパティの名前がわかったら、これらのプロパティ名を `Select-Object` と共に使用して、それらを直接取得できます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-112">Once you know the names of the properties that you're interested in, you can use those property names with `Select-Object` to get them directly:</span></span>

```azurepowershell-interactive
Get-AzVM -Name TestVM -ResourceGroupName TestGroup | Select-Object Name,VmId,ProvisioningState
```

```output
Name   VmId                                 ProvisioningState
----   ----                                 -----------------
TestVM 711d8ed1-b888-4c52-8ab9-66f07b87eb6b Succeeded
```

<span data-ttu-id="9d7e2-113">`Select-Object` を使用して取得した出力は、常に、要求された情報を表示するように書式設定されます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-113">Output from using `Select-Object` is always formatted to display the requested information.</span></span> <span data-ttu-id="9d7e2-114">クエリ実行コマンドレットの結果の一部として書式設定を使用する方法については、「[Azure PowerShell コマンドレット出力の書式設定](formatting-output.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-114">To learn about using formatting as part of querying cmdlet results, see [Format Azure PowerShell cmdlet output](formatting-output.md).</span></span>

## <a name="select-nested-properties"></a><span data-ttu-id="9d7e2-115">入れ子になったプロパティの選択</span><span class="sxs-lookup"><span data-stu-id="9d7e2-115">Select nested properties</span></span>

<span data-ttu-id="9d7e2-116">Azure PowerShell コマンドレットの出力の一部のプロパティでは、入れ子になったオブジェクトが使用されます (`Get-AzVM` 出力の `StorageProfile` プロパティなど)。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-116">Some properties in Azure PowerShell cmdlet output use nested objects, like the `StorageProfile` property of `Get-AzVM` output.</span></span> <span data-ttu-id="9d7e2-117">入れ子になったプロパティから値を取得するには、`Select-Object` のディクショナリの引数の一部として検査する値に表示名と完全なパスを提供します。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-117">To get a value from a nested property, provide a display name and the full path to the value you want to inspect as part of a dictionary argument to `Select-Object`:</span></span>

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Select-Object Name,@{Name="OSType"; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name     OSType
----     ------
TestVM    Linux
TestVM2   Linux
WinVM   Windows
```

<span data-ttu-id="9d7e2-118">各ディクショナリの引数により、オブジェクトから 1 つのプロパティが選択されます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-118">Each dictionary argument selects one property from the object.</span></span> <span data-ttu-id="9d7e2-119">抽出するプロパティは、式の一部である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-119">The property to extract must be part of an expression.</span></span>

## <a name="filter-results"></a><span data-ttu-id="9d7e2-120">結果のフィルター処理</span><span class="sxs-lookup"><span data-stu-id="9d7e2-120">Filter results</span></span> 

<span data-ttu-id="9d7e2-121">`Where-Object` コマンドレットを使うと、入れ子になったプロパティなど、プロパティの値に基づいて結果をフィルター選択することができます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-121">The `Where-Object` cmdlet allows you to filter the result based on any property value, including nested properties.</span></span> <span data-ttu-id="9d7e2-122">次の例は、`Where-Object` を使用してリソース グループの Linux VM を見つける方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-122">The next example shows how to use `Where-Object` to find the Linux VMs in a resource group.</span></span>

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Where-Object {$_.StorageProfile.OSDisk.OSType -eq "Linux"}
```

```output
ResourceGroupName    Name Location          VmSize OsType        NIC ProvisioningState Zone
-----------------    ---- --------          ------ ------        --- ----------------- ----
TestGroup          TestVM  westus2 Standard_D2s_v3  Linux  testvm299         Succeeded
TestGroup         TestVM2  westus2 Standard_D2s_v3  Linux testvm2669         Succeeded
```

<span data-ttu-id="9d7e2-123">`Select-Object` と `Where-Object` の結果を互いにパイプ処理できます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-123">You can pipe the results of `Select-Object` and `Where-Object` to each other.</span></span> <span data-ttu-id="9d7e2-124">パフォーマンス上の理由から、`Where-Object` 操作を `Select-Object` の前に常に配置することが推奨されます。</span><span class="sxs-lookup"><span data-stu-id="9d7e2-124">For performance purposes, it's always recommended to put the `Where-Object` operation before `Select-Object`:</span></span>

```azurepowershell-interactive
Get-AzVM -ResourceGroupName TestGroup | `
    Where-Object {$_.StorageProfile.OsDisk.OsType -eq "Linux"} | `
    Select-Object Name,VmID,ProvisioningState
```

```output
Name    VmId                                 ProvisioningState
----    ----                                 -----------------
TestVM  711d8ed1-b888-4c52-8ab9-66f07b87eb6  Succeeded
TestVM2 cbcee769-dd78-45e3-a14d-2ad11c647d0  Succeeded
```
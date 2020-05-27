---
title: Azure PowerShell コマンドレットの出力に対してクエリを実行する
description: Azure のリソースに対してクエリを実行し、その結果の書式を設定する方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/10/2019
ms.openlocfilehash: ebd108a2c13bdb376213d054fb72188e6205a565
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "83624312"
---
# <a name="query-output-of-azure-powershell"></a>Azure PowerShell の出力に対してクエリを実行する 

各 Azure PowerShell コマンドレットの結果は、Azure PowerShell オブジェクトです。 明示的に `Get-` 操作ではないコマンドレットであっても、検査可能な値を返し、作成または変更されたリソースに関する情報を提供する場合があります。 ほとんどのコマンドレットは単一オブジェクトを返す一方、反復処理される必要のある配列を返すコマンドもあります。

ほぼすべての場合において、[Select-Object](/powershell/module/Microsoft.PowerShell.Utility/Select-Object) コマンドレット (省略形: `select`) を使って Azure PowerShell からの出力に対してクエリを実行します。 出力は [Where-Object](/powershell/module/Microsoft.PowerShell.Core/Where-Object) またはそのエイリアス `where` を使用してフィルターできます。

## <a name="select-simple-properties"></a>単純なプロパティを選択する

既定の表形式では、Azure PowerShell コマンドレットにより、使用可能なすべてのプロパティは表示されません。 完全なプロパティを取得するには、[Format-List](/powershell/module/microsoft.powershell.utility/format-list) コマンドレットを使用するか、出力を `Select-Object *` にパイプ処理します。

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

関心のあるプロパティの名前がわかったら、これらのプロパティ名を `Select-Object` と共に使用して、それらを直接取得できます。

```azurepowershell-interactive
Get-AzVM -Name TestVM -ResourceGroupName TestGroup | Select-Object Name,VmId,ProvisioningState
```

```output
Name   VmId                                 ProvisioningState
----   ----                                 -----------------
TestVM 711d8ed1-b888-4c52-8ab9-66f07b87eb6b Succeeded
```

`Select-Object` を使用して取得した出力は、常に、要求された情報を表示するように書式設定されます。 クエリ実行コマンドレットの結果の一部として書式設定を使用する方法については、「[Azure PowerShell コマンドレット出力の書式設定](formatting-output.md)」をご覧ください。

## <a name="select-nested-properties"></a>入れ子になったプロパティの選択

Azure PowerShell コマンドレットの出力の一部のプロパティでは、入れ子になったオブジェクトが使用されます (`Get-AzVM` 出力の `StorageProfile` プロパティなど)。 入れ子になったプロパティから値を取得するには、`Select-Object` のディクショナリの引数の一部として検査する値に表示名と完全なパスを提供します。

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

各ディクショナリの引数により、オブジェクトから 1 つのプロパティが選択されます。 抽出するプロパティは、式の一部である必要があります。

## <a name="filter-results"></a>結果のフィルター処理 

`Where-Object` コマンドレットを使うと、入れ子になったプロパティなど、プロパティの値に基づいて結果をフィルター選択することができます。 次の例は、`Where-Object` を使用してリソース グループの Linux VM を見つける方法を示しています。

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

`Select-Object` と `Where-Object` の結果を互いにパイプ処理できます。 パフォーマンス上の理由から、`Where-Object` 操作を `Select-Object` の前に常に配置することが推奨されます。

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

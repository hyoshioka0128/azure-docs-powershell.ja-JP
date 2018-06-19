---
title: Azure PowerShell コマンドレット出力の書式設定
description: Azure PowerShell コマンドレット出力の書式を設定する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/07/2018
ms.openlocfilehash: 833c82903305f99be5ad43f707e22644bb568abe
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323052"
---
# <a name="format-azurepowershell-cmdlet-output"></a>Azure PowerShell コマンドレット出力の書式設定

Azure PowerShell コマンドレットにはそれぞれ、出力結果が読みやすいように既定の書式があらかじめ定義されています。  次の PowerShell コマンドレットを使って、必要に応じて出力の書式を調整したり、コマンドレットの出力形式を変換したりすることもできます。

| 書式設定      | Conversion       |
|-----------------|------------------|
| [Format-Custom](/powershell/module/microsoft.powershell.utility/format-custom) | [ConvertTo-Csv](/powershell/module/microsoft.powershell.utility/convertto-csv)  |
| [Format-List](/powershell/module/microsoft.powershell.utility/format-list)   | [ConvertTo-Html](/powershell/module/microsoft.powershell.utility/convertto-html) |
| [Format-Table](/powershell/module/microsoft.powershell.utility/format-table)  | [ConvertTo-Json](/powershell/module/microsoft.powershell.utility/convertto-json) |
| [Format-Wide](/powershell/module/microsoft.powershell.utility/format-wide)   | [ConvertTo-Xml](/powershell/module/microsoft.powershell.utility/convertto-xml)  |

## <a name="format-examples"></a>書式設定の例

この例では、既定のサブスクリプションに含まれる一連の Azure VM を取得しています。  `Get-AzureRmVM` コマンドの既定の出力は表形式です。

```azurepowershell-interactive
Get-AzureRmVM
```

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

取得する列を制限する必要がある場合は、`Format-Table` コマンドレットを使ってください。 以下の例は、先ほどと同じ一連の仮想マシンを取得するものです。ただし今回は、VM の名前とリソース グループ、VM の場所に出力内容を限定しています。  データのサイズに応じて列のサイズを変更するには、`-Autosize` パラメーターを使います。

```azurepowershell-interactive
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

リスト形式で出力することもできます。 `Format-List` コマンドレットを使った表示例を次に示します。

```azurepowershell-interactive
Get-AzureRmVM | Format-List Name,VmId,Location,ResourceGroupName
```

```output
Name              : MyUnbuntu1610
VmId              : 33422f9b-e339-4704-bad8-dbe094585496
Location          : westeurope
ResourceGroupName : MYWESTEURG

Name              : MyWin2016VM
VmId              : 4650c755-fc2b-4fc7-a5bc-298d5c00808f
Location          : westeurope
ResourceGroupName : MYWESTEURG
```

## <a name="convert-to-other-data-types"></a>他のデータ型への変換

PowerShell では、コマンド出力を複数のデータ形式に変換することもできます。 次の例では、`Select-Object` コマンドレットを使って、サブスクリプションに含まれる仮想マシンの属性を取得し、その出力を、データベースやスプレッドシートにインポートしやすいように CSV に変換します。

```azurepowershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```output
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

出力を JSON 形式に変換することもできます。  次の例は、先ほどと同じ VM のリストを作成するものですが、出力形式は JSON に変更しています。

```azurepowershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Json
```

```output
[
    {
        "ResourceGroupName":  "MYWESTEURG",
        "Id":  "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTEURG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610",
        "VmId":  "33422f9b-e339-4704-bad8-dbe094585496",
        "Name":  "MyUnbuntu1610",
        "Location":  "westeurope",
        "ProvisioningState":  "Succeeded"
    },
    {
        "ResourceGroupName":  "MYWESTEURG",
        "Id":  "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTEURG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM",
        "VmId":  "4650c755-fc2b-4fc7-a5bc-298d5c00808f",
        "Name":  "MyWin2016VM",
        "Location":  "westeurope",
        "ProvisioningState":  "Succeeded"
    }
]
```

---
title: Azure PowerShell コマンドレット出力の書式設定
description: Azure PowerShell コマンドレット出力の書式を設定する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 390285bcf483e75b7a2b77d345ccb108669f66e5
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153488"
---
# <a name="format-azurepowershell-cmdlet-output"></a><span data-ttu-id="155da-103">Azure PowerShell コマンドレット出力の書式設定</span><span class="sxs-lookup"><span data-stu-id="155da-103">Format AzurePowerShell cmdlet output</span></span>

<span data-ttu-id="155da-104">Azure PowerShell コマンドレットにはそれぞれ、出力結果が読みやすいように既定の書式があらかじめ定義されています。</span><span class="sxs-lookup"><span data-stu-id="155da-104">By default each Azure PowerShell cmdlet has predefined formatting of output making it easy to read.</span></span>  <span data-ttu-id="155da-105">次の PowerShell コマンドレットを使って、必要に応じて出力の書式を調整したり、コマンドレットの出力形式を変換したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="155da-105">PowerShell also provides the flexibility to adjust the output or convert the cmdlet output to a different format with the following cmdlets:</span></span>

| <span data-ttu-id="155da-106">書式設定</span><span class="sxs-lookup"><span data-stu-id="155da-106">Formatting</span></span>      | <span data-ttu-id="155da-107">Conversion</span><span class="sxs-lookup"><span data-stu-id="155da-107">Conversion</span></span>       |
|-----------------|------------------|
| [<span data-ttu-id="155da-108">Format-Custom</span><span class="sxs-lookup"><span data-stu-id="155da-108">Format-Custom</span></span>](/powershell/module/microsoft.powershell.utility/format-custom) | [<span data-ttu-id="155da-109">ConvertTo-Csv</span><span class="sxs-lookup"><span data-stu-id="155da-109">ConvertTo-Csv</span></span>](/powershell/module/microsoft.powershell.utility/convertto-csv)  |
| [<span data-ttu-id="155da-110">Format-List</span><span class="sxs-lookup"><span data-stu-id="155da-110">Format-List</span></span>](/powershell/module/microsoft.powershell.utility/format-list)   | [<span data-ttu-id="155da-111">ConvertTo-Html</span><span class="sxs-lookup"><span data-stu-id="155da-111">ConvertTo-Html</span></span>](/powershell/module/microsoft.powershell.utility/convertto-html) |
| [<span data-ttu-id="155da-112">Format-Table</span><span class="sxs-lookup"><span data-stu-id="155da-112">Format-Table</span></span>](/powershell/module/microsoft.powershell.utility/format-table)  | [<span data-ttu-id="155da-113">ConvertTo-Json</span><span class="sxs-lookup"><span data-stu-id="155da-113">ConvertTo-Json</span></span>](/powershell/module/microsoft.powershell.utility/convertto-json) |
| [<span data-ttu-id="155da-114">Format-Wide</span><span class="sxs-lookup"><span data-stu-id="155da-114">Format-Wide</span></span>](/powershell/module/microsoft.powershell.utility/format-wide)   | [<span data-ttu-id="155da-115">ConvertTo-Xml</span><span class="sxs-lookup"><span data-stu-id="155da-115">ConvertTo-Xml</span></span>](/powershell/module/microsoft.powershell.utility/convertto-xml)  |

## <a name="format-examples"></a><span data-ttu-id="155da-116">書式設定の例</span><span class="sxs-lookup"><span data-stu-id="155da-116">Format examples</span></span>

<span data-ttu-id="155da-117">この例では、既定のサブスクリプションに含まれる一連の Azure VM を取得しています。</span><span class="sxs-lookup"><span data-stu-id="155da-117">In this example, we get a list of Azure VMs in our default subscription.</span></span>  <span data-ttu-id="155da-118">`Get-AzureRmVM` コマンドの既定の出力は表形式です。</span><span class="sxs-lookup"><span data-stu-id="155da-118">The `Get-AzureRmVM` command defaults output into a table format.</span></span>

```azurepowershell-interactive
Get-AzureRmVM
```

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="155da-119">取得する列を制限する必要がある場合は、`Format-Table` コマンドレットを使ってください。</span><span class="sxs-lookup"><span data-stu-id="155da-119">If you would like to limit the columns returned you can use the `Format-Table` cmdlet.</span></span> <span data-ttu-id="155da-120">以下の例は、先ほどと同じ一連の仮想マシンを取得するものです。ただし今回は、VM の名前とリソース グループ、VM の場所に出力内容を限定しています。</span><span class="sxs-lookup"><span data-stu-id="155da-120">In the following example, we get the same list of virtual machines but restrict the output to just the name of the VM, the resource group, and the location of the VM.</span></span>  <span data-ttu-id="155da-121">データのサイズに応じて列のサイズを変更するには、`-Autosize` パラメーターを使います。</span><span class="sxs-lookup"><span data-stu-id="155da-121">The `-Autosize` parameter sizes the columns according to the size of the data.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

<span data-ttu-id="155da-122">リスト形式で出力することもできます。</span><span class="sxs-lookup"><span data-stu-id="155da-122">Output can also be formatted into a list.</span></span> <span data-ttu-id="155da-123">`Format-List` コマンドレットを使った表示例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="155da-123">The following example shows this using the`Format-List` cmdlet.</span></span>

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

## <a name="convert-to-other-data-types"></a><span data-ttu-id="155da-124">他のデータ型への変換</span><span class="sxs-lookup"><span data-stu-id="155da-124">Convert to other data types</span></span>

<span data-ttu-id="155da-125">PowerShell では、コマンド出力を複数のデータ形式に変換することもできます。</span><span class="sxs-lookup"><span data-stu-id="155da-125">PowerShell also allows taking command output and converting it into multiple data formats.</span></span> <span data-ttu-id="155da-126">次の例では、`Select-Object` コマンドレットを使って、サブスクリプションに含まれる仮想マシンの属性を取得し、その出力を、データベースやスプレッドシートにインポートしやすいように CSV に変換します。</span><span class="sxs-lookup"><span data-stu-id="155da-126">In the following example, the `Select-Object` cmdlet is used to get attributes of the virtual machines in our subscription and convert the output to CSV format for easy import into a database or spreadsheet.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```output
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

<span data-ttu-id="155da-127">出力を JSON 形式に変換することもできます。</span><span class="sxs-lookup"><span data-stu-id="155da-127">Output can also be converted into the JSON format.</span></span>  <span data-ttu-id="155da-128">次の例は、先ほどと同じ VM のリストを作成するものですが、出力形式は JSON に変更しています。</span><span class="sxs-lookup"><span data-stu-id="155da-128">The following example creates the same list of VMs but changes the output format to JSON.</span></span>

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

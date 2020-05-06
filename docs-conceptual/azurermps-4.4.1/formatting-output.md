---
title: クエリの結果の書式設定 | Microsoft Docs
description: Azure のリソースに対してクエリを実行し、その結果の書式を設定する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 7f6cf61eef9c5549dfe78d2d801ab1278db40c17
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "67863563"
---
# <a name="formatting-query-results"></a><span data-ttu-id="7c0c4-103">クエリの結果の書式設定</span><span class="sxs-lookup"><span data-stu-id="7c0c4-103">Formatting query results</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="7c0c4-104">PowerShell コマンドレットにはそれぞれ、出力結果が読みやすいように既定の書式があらかじめ定義されています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-104">By default each PowerShell cmdlet has predefined formatting of output making it easy to read.</span></span>  <span data-ttu-id="7c0c4-105">次の PowerShell コマンドレットを使って、必要に応じて出力の書式を調整したり、コマンドレットの出力形式を変換したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-105">PowerShell also provides the flexibility to adjust the output or convert the cmdlet output to a different format with the following cmdlets:</span></span>

| <span data-ttu-id="7c0c4-106">書式設定</span><span class="sxs-lookup"><span data-stu-id="7c0c4-106">Formatting</span></span>      | <span data-ttu-id="7c0c4-107">変換</span><span class="sxs-lookup"><span data-stu-id="7c0c4-107">Conversion</span></span>       |
|-----------------|------------------|
| `Format-Custom` | `ConvertTo-Csv`  |
| `Format-List`   | `ConvertTo-Html` |
| `Format-Table`  | `ConvertTo-Json` |
| `Format-Wide`   | `ConvertTo-Xml`  |

## <a name="formatting-examples"></a><span data-ttu-id="7c0c4-108">書式設定の例</span><span class="sxs-lookup"><span data-stu-id="7c0c4-108">Formatting examples</span></span>

<span data-ttu-id="7c0c4-109">この例では、既定のサブスクリプションに含まれる一連の Azure VM を取得しています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-109">In this example we get a list of Azure VMs in our default subscription.</span></span>  <span data-ttu-id="7c0c4-110">Get-AzureRmVM コマンドの既定の出力は表形式です。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-110">The Get-AzureRmVM command defaults output into a table format.</span></span>

```powershell-interactive
Get-AzureRmVM
```

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="7c0c4-111">取得する列を制限する必要がある場合は、`Format-Table` コマンドレットを使ってください。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-111">If you would like to limit the columns returned you can use the `Format-Table` cmdlet.</span></span> <span data-ttu-id="7c0c4-112">以下の例は、先ほどと同じ一連の仮想マシンを取得するものです。ただし今回は、VM の名前とリソース グループ、VM の場所に出力内容を限定しています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-112">In the following example we get the same list of virtual machines but restrict the output to just the name of the VM, the resource group, and the location of the VM.</span></span>  <span data-ttu-id="7c0c4-113">データのサイズに応じて列のサイズを変更するには、`-Autosize` パラメーターを使います。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-113">The `-Autosize` parameter sizes the columns according to the size of the data.</span></span>

```powershell-interactive
Get-AzureRmVM | Format-Table Name,ResourceGroupName,Location -AutoSize
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

<span data-ttu-id="7c0c4-114">必要であれば、リスト形式で情報を表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-114">If you would prefer you can view information in a list format.</span></span> <span data-ttu-id="7c0c4-115">`Format-List` コマンドレットを使った表示例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-115">The following example shows this using the`Format-List` cmdlet.</span></span>

```powershell-interactive
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

## <a name="converting-to-other-data-types"></a><span data-ttu-id="7c0c4-116">他のデータ形式への変換</span><span class="sxs-lookup"><span data-stu-id="7c0c4-116">Converting to other data types</span></span>

<span data-ttu-id="7c0c4-117">さまざまなニーズに応えるために、PowerShell には複数の出力形式が用意されています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-117">PowerShell also offers multiple output format you can use to meet your needs.</span></span>  <span data-ttu-id="7c0c4-118">次の例では、サブスクリプションに含まれる仮想マシンの属性を `Select-Object` コマンドレットで取得し、データベースやスプレッドシートにインポートしやすいように、その出力形式を CSV に変換しています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-118">In the following example we use the `Select-Object` cmdlet to get attributes of the virtual machines in our subscription and convert the output to CSV format for easy import into a database or spreadsheet.</span></span>

```powershell-interactive
Get-AzureRmVM | Select-Object ResourceGroupName,Id,VmId,Name,Location,ProvisioningState | ConvertTo-Csv -NoTypeInformation
```

```output
"ResourceGroupName","Id","VmId","Name","Location","ProvisioningState"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyUnbuntu1610","33422f9b-e339-4704-bad8-dbe094585496","MyUnbuntu1610","westeurope","Succeeded"
"MYWESTUERG","/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MYWESTUERG/providers/Microsoft.Compute/virtualMachines/MyWin2016VM","4650c755-fc2b-4fc7-a5bc-298d5c00808f","MyWin2016VM","westeurope","Succeeded"
```

<span data-ttu-id="7c0c4-119">出力形式を JSON に変換することもできます。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-119">You can also convert the output into JSON format.</span></span>  <span data-ttu-id="7c0c4-120">次の例は、先ほどと同じ VM のリストを作成するものですが、出力形式は JSON に変更しています。</span><span class="sxs-lookup"><span data-stu-id="7c0c4-120">The following example creates the same list of VMs but changes the output format to JSON.</span></span>

```powershell-interactive
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

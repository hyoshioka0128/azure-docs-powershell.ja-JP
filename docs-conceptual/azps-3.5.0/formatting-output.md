---
title: Azure PowerShell コマンドレット出力の書式設定
description: Azure PowerShell コマンドレット出力の書式を設定する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/07/2019
ms.openlocfilehash: e5c9a9df830f6d866d171107472ff94166442be9
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477303"
---
# <a name="format-azure-powershell-cmdlet-output"></a><span data-ttu-id="76384-103">Azure PowerShell コマンドレット出力の書式設定</span><span class="sxs-lookup"><span data-stu-id="76384-103">Format Azure PowerShell cmdlet output</span></span>

<span data-ttu-id="76384-104">既定では、いずれの Azure PowerShell コマンドレットでも、読みやすいように出力が書式設定されます。</span><span class="sxs-lookup"><span data-stu-id="76384-104">By default each Azure PowerShell cmdlet formats output to be easy to read.</span></span> <span data-ttu-id="76384-105">PowerShell では、次のコマンドレットの 1 つにパイプ処理することでコマンドレット出力を変換または書式設定できます。</span><span class="sxs-lookup"><span data-stu-id="76384-105">PowerShell allows you to convert or format cmdlet output by piping to one of the following cmdlets:</span></span>

| <span data-ttu-id="76384-106">書式設定</span><span class="sxs-lookup"><span data-stu-id="76384-106">Formatting</span></span>      | <span data-ttu-id="76384-107">変換</span><span class="sxs-lookup"><span data-stu-id="76384-107">Conversion</span></span>       |
|-----------------|------------------|
| [<span data-ttu-id="76384-108">Format-Custom</span><span class="sxs-lookup"><span data-stu-id="76384-108">Format-Custom</span></span>](/powershell/module/microsoft.powershell.utility/format-custom) | [<span data-ttu-id="76384-109">ConvertTo-Csv</span><span class="sxs-lookup"><span data-stu-id="76384-109">ConvertTo-Csv</span></span>](/powershell/module/microsoft.powershell.utility/convertto-csv)  |
| [<span data-ttu-id="76384-110">Format-List</span><span class="sxs-lookup"><span data-stu-id="76384-110">Format-List</span></span>](/powershell/module/microsoft.powershell.utility/format-list)   | [<span data-ttu-id="76384-111">ConvertTo-Html</span><span class="sxs-lookup"><span data-stu-id="76384-111">ConvertTo-Html</span></span>](/powershell/module/microsoft.powershell.utility/convertto-html) |
| [<span data-ttu-id="76384-112">Format-Table</span><span class="sxs-lookup"><span data-stu-id="76384-112">Format-Table</span></span>](/powershell/module/microsoft.powershell.utility/format-table)  | [<span data-ttu-id="76384-113">ConvertTo-Json</span><span class="sxs-lookup"><span data-stu-id="76384-113">ConvertTo-Json</span></span>](/powershell/module/microsoft.powershell.utility/convertto-json) |
| [<span data-ttu-id="76384-114">Format-Wide</span><span class="sxs-lookup"><span data-stu-id="76384-114">Format-Wide</span></span>](/powershell/module/microsoft.powershell.utility/format-wide)   | [<span data-ttu-id="76384-115">ConvertTo-Xml</span><span class="sxs-lookup"><span data-stu-id="76384-115">ConvertTo-Xml</span></span>](/powershell/module/microsoft.powershell.utility/convertto-xml)  |

<span data-ttu-id="76384-116">PowerShell ターミナルに表示するために使用されるのが書式設定で、他のスクリプトまたはプログラムで使用するためのデータ生成に使用されるのが変換です。</span><span class="sxs-lookup"><span data-stu-id="76384-116">Formatting is used for display in a PowerShell terminal, and conversion is used for generating data to be consumed by other scripts or programs.</span></span>

## <a name="table-output-format"></a><span data-ttu-id="76384-117">テーブル出力形式</span><span class="sxs-lookup"><span data-stu-id="76384-117">Table output format</span></span>

<span data-ttu-id="76384-118">Azure PowerShell コマンドレットの出力形式は既定で表形式となります。</span><span class="sxs-lookup"><span data-stu-id="76384-118">By default, Azure PowerShell cmdlets output in the table format.</span></span> <span data-ttu-id="76384-119">この形式の場合、要求したリソースの情報が一部表示されません。</span><span class="sxs-lookup"><span data-stu-id="76384-119">This format doesn't display all information of the requested resource:</span></span>

```powershell-interactive
Get-AzVM
```

```output
ResourceGroupName           Name Location          VmSize  OsType               NIC ProvisioningState Zone
-----------------           ---- --------          ------  ------               --- ----------------- ----
QueryExample      ExampleLinuxVM  westus2        Basic_A0   Linux examplelinuxvm916         Succeeded
QueryExample         RHELExample  westus2  Standard_D2_v3   Linux    rhelexample469         Succeeded
QueryExample        WinExampleVM  westus2 Standard_DS1_v2 Windows   winexamplevm268         Succeeded
```

<span data-ttu-id="76384-120">`Format-Table` によって表示されるデータの量は、PowerShell セッションのウィンドウ幅によって決められることがあります。</span><span class="sxs-lookup"><span data-stu-id="76384-120">The amount of data displayed by `Format-Table` can be affected by the width of your PowerShell session window.</span></span> <span data-ttu-id="76384-121">特定のプロパティに出力を制限したり、プロパティを並べ替えたりする目的で、プロパティ名を引数として `Format-Table` に指定できます。</span><span class="sxs-lookup"><span data-stu-id="76384-121">To restrict the output to specific properties and order them, property names can be provided as arguments to `Format-Table`:</span></span>

```powershell-interactive
Get-AzVM -ResourceGroupName QueryExample | Format-Table Name,ResourceGroupName,Location
```

```output
Name           ResourceGroupName Location
----           ----------------- --------
ExampleLinuxVM QueryExample      westus2
RHELExample    QueryExample      westus2
WinExampleVM   QueryExample      westus2
```

## <a name="list-output-format"></a><span data-ttu-id="76384-122">一覧出力の形式</span><span class="sxs-lookup"><span data-stu-id="76384-122">List output format</span></span>

<span data-ttu-id="76384-123">一覧で出力する形式では、2 列が生成され、プロパティ名に値が続きます。</span><span class="sxs-lookup"><span data-stu-id="76384-123">List output format produces two columns, property names followed by the value.</span></span> <span data-ttu-id="76384-124">複雑なオブジェクトの場合、オブジェクトの種類が代わりに表示されます。</span><span class="sxs-lookup"><span data-stu-id="76384-124">For complex objects, the type of the object is displayed instead.</span></span>

```powershell-interactive
Get-AzVM | Format-List
```

<span data-ttu-id="76384-125">次の出力では、一部のフィールドが削除されています。</span><span class="sxs-lookup"><span data-stu-id="76384-125">The following output has some fields removed.</span></span>

```output
ResourceGroupName        : QueryExample
Id                       : /subscriptions/.../resourceGroups/QueryExample/providers/Microsoft.Compute/virtualMachines/ExampleLinuxVM
VmId                     : ...
Name                     : ExampleLinuxVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : westus2
...
HardwareProfile          : Microsoft.Azure.Management.Compute.Models.HardwareProfile
InstanceView             :
NetworkProfile           : Microsoft.Azure.Management.Compute.Models.NetworkProfile
OSProfile                : Microsoft.Azure.Management.Compute.Models.OSProfile
...
StatusCode               : OK

ResourceGroupName        : QueryExample
Id                       : /subscriptions/.../resourceGroups/QueryExample/providers/Microsoft.Compute/virtualMachines/RHELExample
VmId                     : ...
Name                     : RHELExample
Type                     : Microsoft.Compute/virtualMachines
Location                 : westus2
...
```

<span data-ttu-id="76384-126">`Format-Table` と同様に、出力を並べ替えたり、制限したりする目的でプロパティ名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="76384-126">Like `Format-Table`, property names can be provided to order and restrict the output:</span></span>

```powershell-interactive
Get-AzVM | Format-List ResourceGroupName,Name,Location
```

```output
ResourceGroupName : QueryExample
Name              : ExampleLinuxVM
Location          : westus2

ResourceGroupName : QueryExample
Name              : RHELExample
Location          : westus2

ResourceGroupName : QueryExample
Name              : WinExampleVM
Location          : westus2
```

## <a name="wide-output-format"></a><span data-ttu-id="76384-127">ワイド出力の形式</span><span class="sxs-lookup"><span data-stu-id="76384-127">Wide output format</span></span>

<span data-ttu-id="76384-128">形式がワイド出力の場合、クエリごとにプロパティが 1 つだけ生成されます。</span><span class="sxs-lookup"><span data-stu-id="76384-128">Wide output format produces only one property name per query.</span></span> <span data-ttu-id="76384-129">表示されるプロパティは、引数としてプロパティを指定することで制御できます。</span><span class="sxs-lookup"><span data-stu-id="76384-129">Which property is displayed can be controlled by giving a property as an argument.</span></span>

```powershell-interactive
Get-AzVM | Format-Wide
```

```output
ExampleLinuxVM                                  RHELExample
WinExampleVM
```

```powershell-interactive
Get-AzVM | Format-Wide ResourceGroupName
```

```output
QueryExample                                    QueryExample
QueryExample
```

## <a name="custom-output-format"></a><span data-ttu-id="76384-130">カスタム出力の形式</span><span class="sxs-lookup"><span data-stu-id="76384-130">Custom output format</span></span>

<span data-ttu-id="76384-131">出力の種類が `Custom-Format` の場合、カスタム オブジェクトの書式設定向けとなります。</span><span class="sxs-lookup"><span data-stu-id="76384-131">The `Custom-Format` output type is meant for formatting custom objects.</span></span> <span data-ttu-id="76384-132">引数がない場合、`Format-List` と同様に動作しますが、カスタム クラスのプロパティ名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="76384-132">Without any arguments, it behaves like `Format-List` but displays the property names of custom classes.</span></span>

```powershell-interactive
Get-AzVM | Format-Custom
```

<span data-ttu-id="76384-133">次の出力では、一部のフィールドが削除されています。</span><span class="sxs-lookup"><span data-stu-id="76384-133">The following output has some fields removed.</span></span>

```output
ResourceGroupName : QueryExample
Id                : /subscriptions/.../resourceGroups/QueryExample/providers/Microsoft.Compute/virtualMachines/ExampleLinuxVM
VmId              : ...
Name              : ExampleLinuxVM
Type              : Microsoft.Compute/virtualMachines
Location          : westus2
Tags              : {}
HardwareProfile   : {VmSize}
NetworkProfile    : {NetworkInterfaces}
OSProfile         : {ComputerName, AdminUsername, LinuxConfiguration, Secrets,
AllowExtensionOperations}
ProvisioningState : Succeeded
StorageProfile    : {ImageReference, OsDisk, DataDisks}
...
```

<span data-ttu-id="76384-134">引数としてプロパティ名を `Custom-Format` に指定すると、値として設定されているカスタム オブジェクトのプロパティ/値のペアが表示されます。</span><span class="sxs-lookup"><span data-stu-id="76384-134">Giving property names as arguments to `Custom-Format` displays the property/value pairs for custom objects set as values:</span></span>

```powershell-interactive
Get-AzVM | Format-Custom Name,ResourceGroupName,Location,OSProfile
```

<span data-ttu-id="76384-135">次の出力では、一部のフィールドが削除されています。</span><span class="sxs-lookup"><span data-stu-id="76384-135">The following output has some fields removed.</span></span>

```output
class PSVirtualMachineList
{
  Name = ExampleLinuxVM
  ResourceGroupName = QueryExample
  Location = westus2
  OSProfile =
    class OSProfile
    {
      ComputerName = ExampleLinuxVM
      AdminUsername = ...
      AdminPassword =
      CustomData =
      WindowsConfiguration =
      LinuxConfiguration =
        class LinuxConfiguration
        {
          DisablePasswordAuthentication = False
          Ssh =
          ProvisionVMAgent = True
        }
      Secrets =
        [
        ]

      AllowExtensionOperations = True
    }
}

...

class PSVirtualMachineList
{
  Name = WinExampleVM
  ResourceGroupName = QueryExample
  Location = westus2
  OSProfile =
    class OSProfile
    {
      ComputerName = WinExampleVM
      AdminUsername = ...
      AdminPassword =
      CustomData =
      WindowsConfiguration =
        class WindowsConfiguration
        {
          ProvisionVMAgent = True
          EnableAutomaticUpdates = True
          TimeZone =
          AdditionalUnattendContent =
          WinRM =
        }
      LinuxConfiguration =
      Secrets =
        [
        ]

      AllowExtensionOperations = True
    }
}
```

## <a name="conversion-to-other-data-formats"></a><span data-ttu-id="76384-136">他のデータ形式に変換する</span><span class="sxs-lookup"><span data-stu-id="76384-136">Conversion to other data formats</span></span>

<span data-ttu-id="76384-137">`ConvertTo-*` 群のコマンドレットの場合、Azure PowerShell コマンドレットの結果が機械で読める形式に変換できます。</span><span class="sxs-lookup"><span data-stu-id="76384-137">The `ConvertTo-*` family of cmdlets allows for converting the results of Azure PowerShell cmdlets to machine-readable formats.</span></span> <span data-ttu-id="76384-138">Azure PowerShell の結果から一部のプロパティのみを取得するには、変換の前にパイプで `Select-Object` コマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="76384-138">To get only some properties from the Azure PowerShell results, use the `Select-Object` command in a pipe before performing the conversion.</span></span> <span data-ttu-id="76384-139">次の例では、各変換によってさまざまな種類の出力が生成されます。</span><span class="sxs-lookup"><span data-stu-id="76384-139">The following examples demonstrate the different kinds of output that each conversion produces.</span></span>

### <a name="conversion-to-csv"></a><span data-ttu-id="76384-140">CSV に変換</span><span class="sxs-lookup"><span data-stu-id="76384-140">Conversion to CSV</span></span>

```azurepowershell-interactive
Get-AzVM | ConvertTo-CSV
```

```output
#TYPE Microsoft.Azure.Commands.Compute.Models.PSVirtualMachineList
"ResourceGroupName","Id","VmId","Name","Type","Location","LicenseType","Tags","AvailabilitySetReference","DiagnosticsProfile","Extensions","HardwareProfile","InstanceView","NetworkProfile","OSProfile","Plan","ProvisioningState","StorageProfile","DisplayHint","Identity","Zones","FullyQualifiedDomainName","AdditionalCapabilities","RequestId","StatusCode"
"QUERYEXAMPLE","/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/ExampleLinuxVM","...","ExampleLinuxVM","Microsoft.Compute/virtualMachines","westus2",,"System.Collections.Generic.Dictionary`2[System.String,System.String]",,,"System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]","Microsoft.Azure.Management.Compute.Models.HardwareProfile",,"Microsoft.Azure.Management.Compute.Models.NetworkProfile","Microsoft.Azure.Management.Compute.Models.OSProfile",,"Succeeded","Microsoft.Azure.Management.Compute.Models.StorageProfile","Compact",,"System.Collections.Generic.List`1[System.String]",,,"...","OK"
"QUERYEXAMPLE","/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/RHELExample","...","RHELExample","Microsoft.Compute/virtualMachines","westus2",,"System.Collections.Generic.Dictionary`2[System.String,System.String]",,,"System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]","Microsoft.Azure.Management.Compute.Models.HardwareProfile",,"Microsoft.Azure.Management.Compute.Models.NetworkProfile","Microsoft.Azure.Management.Compute.Models.OSProfile",,"Succeeded","Microsoft.Azure.Management.Compute.Models.StorageProfile","Compact",,"System.Collections.Generic.List`1[System.String]",,,"...","OK"
"QUERYEXAMPLE","/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/WinExampleVM","...","WinExampleVM","Microsoft.Compute/virtualMachines","westus2",,"System.Collections.Generic.Dictionary`2[System.String,System.String]",,,"System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]","Microsoft.Azure.Management.Compute.Models.HardwareProfile",,"Microsoft.Azure.Management.Compute.Models.NetworkProfile","Microsoft.Azure.Management.Compute.Models.OSProfile",,"Succeeded","Microsoft.Azure.Management.Compute.Models.StorageProfile","Compact",,"System.Collections.Generic.List`1[System.String]",,,"...","OK"
```

### <a name="conversion-to-json"></a><span data-ttu-id="76384-141">JSON に変換</span><span class="sxs-lookup"><span data-stu-id="76384-141">Conversion to JSON</span></span>

<span data-ttu-id="76384-142">JSON 出力の場合、既定では一部のプロパティが展開されません。</span><span class="sxs-lookup"><span data-stu-id="76384-142">JSON output doesn't expand all properties by default.</span></span> <span data-ttu-id="76384-143">展開されるプロパティの深さを変更するには、`-Depth` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="76384-143">To change the depth of properties expanded, use the `-Depth` argument.</span></span> <span data-ttu-id="76384-144">既定では、展開の深さは `2` です。</span><span class="sxs-lookup"><span data-stu-id="76384-144">By default, the expansion depth is `2`.</span></span>

```azurepowershell-interactive
Get-AzVM|ConvertTo-JSON
```

<span data-ttu-id="76384-145">次の出力では、一部のフィールドが削除されています。</span><span class="sxs-lookup"><span data-stu-id="76384-145">The following output has some fields removed.</span></span>

```output
[
    {
        "ResourceGroupName":  "QUERYEXAMPLE",
        "Id":  "/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/ExampleLinuxVM",
        "VmId":  "...",
        "Name":  "ExampleLinuxVM",
        "Type":  "Microsoft.Compute/virtualMachines",
        "Location":  "westus2",
        ...
        "OSProfile":  {
                          "ComputerName":  "ExampleLinuxVM",
                          "AdminUsername":  "...",
                          "AdminPassword":  null,
                          "CustomData":  null,
                          "WindowsConfiguration":  null,
                          "LinuxConfiguration":  "Microsoft.Azure.Management.Compute.Models.LinuxConfiguration",
                          "Secrets":  "",
                          "AllowExtensionOperations":  true
                      },
        "Plan":  null,
        "ProvisioningState":  "Succeeded",
        "StorageProfile":  {
                               "ImageReference":  "Microsoft.Azure.Management.Compute.Models.ImageReference",
                               "OsDisk":  "Microsoft.Azure.Management.Compute.Models.OSDisk",
                               "DataDisks":  ""
                           },
        "DisplayHint":  0,
        "Identity":  null,
        "Zones":  [

                  ],
        "FullyQualifiedDomainName":  null,
        "AdditionalCapabilities":  null,
        "RequestId":  "...",
        "StatusCode":  200
    },
    ...
]
```

### <a name="conversion-to-xml"></a><span data-ttu-id="76384-146">XML に変換</span><span class="sxs-lookup"><span data-stu-id="76384-146">Conversion to XML</span></span>

<span data-ttu-id="76384-147">`ConvertTo-XML` コマンドレットでは、Azure PowerShell 応答オブジェクトが純粋な XML オブジェクトに変換されます。この XML オブジェクトは PowerShell 内で他の XML オブジェクトと同様に処理できます。</span><span class="sxs-lookup"><span data-stu-id="76384-147">The `ConvertTo-XML` cmdlet converts the Azure PowerShell response object into a pure XML object, which can be handled like any other XML object within PowerShell.</span></span> 

```azurepowershell-interactive
Get-AzVM | ConvertTo-XML
```

```output
xml                            Objects
---                            -------
version="1.0" encoding="utf-8" Objects
```

### <a name="conversion-to-html"></a><span data-ttu-id="76384-148">HTML に変換</span><span class="sxs-lookup"><span data-stu-id="76384-148">Conversion to HTML</span></span>

<span data-ttu-id="76384-149">オブジェクトを HTML に変換すると、HTML テーブルとしてレンダリングされる出力が生成されます。</span><span class="sxs-lookup"><span data-stu-id="76384-149">Converting an object to HTML produces output that will be rendered as an HTML table.</span></span> <span data-ttu-id="76384-150">HTML のレンダリングは、幅情報を含まないテーブルをレンダリングするためのブラウザー動作に依存します。</span><span class="sxs-lookup"><span data-stu-id="76384-150">Rendering of the HTML will depend on your browser behavior for rendering tables which contain no width information.</span></span>
<span data-ttu-id="76384-151">カスタム クラス オブジェクトは展開されません。</span><span class="sxs-lookup"><span data-stu-id="76384-151">No custom class objects are expanded.</span></span>

```azurepowershell-interactive
Get-AzVM | ConvertTo-HTML
```

```output
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>HTML TABLE</title>
</head><body>
<table>
<colgroup><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/><col/></colgroup>
<tr><th>ResourceGroupName</th><th>Id</th><th>VmId</th><th>Name</th><th>Type</th><th>Location</th><th>LicenseType</th><th>Tags</th><th>AvailabilitySetReference</th><th>DiagnosticsProfile</th><th>Extensions</th><th>HardwareProfile</th><th>InstanceView</th><th>NetworkProfile</th><th>OSProfile</th><th>Plan</th><th>ProvisioningState</th><th>StorageProfile</th><th>DisplayHint</th><th>Identity</th><th>Zones</th><th>FullyQualifiedDomainName</th><th>AdditionalCapabilities</th><th>RequestId</th><th>StatusCode</th></tr>
<tr><td>QUERYEXAMPLE</td><td>/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/ExampleLinuxVM</td><td>...</td><td>ExampleLinuxVM</td><td>Microsoft.Compute/virtualMachines</td><td>westus2</td><td></td><td>System.Collections.Generic.Dictionary`2[System.String,System.String]</td><td></td><td></td><td>System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]</td><td>Microsoft.Azure.Management.Compute.Models.HardwareProfile</td><td></td><td>Microsoft.Azure.Management.Compute.Models.NetworkProfile</td><td>Microsoft.Azure.Management.Compute.Models.OSProfile</td><td></td><td>Succeeded</td><td>Microsoft.Azure.Management.Compute.Models.StorageProfile</td><td>Compact</td><td></td><td>System.Collections.Generic.List`1[System.String]</td><td></td><td></td><td>...</td><td>OK</td></tr>
<tr><td>QUERYEXAMPLE</td><td>/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/RHELExample</td><td>...</td><td>RHELExample</td><td>Microsoft.Compute/virtualMachines</td><td>westus2</td><td></td><td>System.Collections.Generic.Dictionary`2[System.String,System.String]</td><td></td><td></td><td>System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]</td><td>Microsoft.Azure.Management.Compute.Models.HardwareProfile</td><td></td><td>Microsoft.Azure.Management.Compute.Models.NetworkProfile</td><td>Microsoft.Azure.Management.Compute.Models.OSProfile</td><td></td><td>Succeeded</td><td>Microsoft.Azure.Management.Compute.Models.StorageProfile</td><td>Compact</td><td></td><td>System.Collections.Generic.List`1[System.String]</td><td></td><td></td><td>...</td><td>OK</td></tr>
<tr><td>QUERYEXAMPLE</td><td>/subscriptions/.../resourceGroups/QUERYEXAMPLE/providers/Microsoft.Compute/virtualMachines/WinExampleVM</td><td>...</td><td>WinExampleVM</td><td>Microsoft.Compute/virtualMachines</td><td>westus2</td><td></td><td>System.Collections.Generic.Dictionary`2[System.String,System.String]</td><td></td><td></td><td>System.Collections.Generic.List`1[Microsoft.Azure.Management.Compute.Models.VirtualMachineExtension]</td><td>Microsoft.Azure.Management.Compute.Models.HardwareProfile</td><td></td><td>Microsoft.Azure.Management.Compute.Models.NetworkProfile</td><td>Microsoft.Azure.Management.Compute.Models.OSProfile</td><td></td><td>Succeeded</td><td>Microsoft.Azure.Management.Compute.Models.StorageProfile</td><td>Compact</td><td></td><td>System.Collections.Generic.List`1[System.String]</td><td></td><td></td><td>...</td><td>OK</td></tr>
</table>
</body></html>
```

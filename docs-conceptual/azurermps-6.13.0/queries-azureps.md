---
title: Azure PowerShell コマンドレットの出力に対してクエリを実行する
description: Azure のリソースに対してクエリを実行し、その結果の書式を設定する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 6bd1bea43303e9f5a2b46d63a3ac51b4c4031b9f
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217985"
---
# <a name="query-output-of-azure-powershell-cmdlets"></a><span data-ttu-id="46e80-103">Azure PowerShell コマンドレットの出力に対してクエリを実行する</span><span class="sxs-lookup"><span data-stu-id="46e80-103">Query output of Azure PowerShell cmdlets</span></span>

<span data-ttu-id="46e80-104">PowerShell におけるクエリは、組み込みのコマンドレットを使って実行できます。</span><span class="sxs-lookup"><span data-stu-id="46e80-104">Querying in PowerShell can be completed by using built-in cmdlets.</span></span> <span data-ttu-id="46e80-105">PowerShell のコマンドレット名は、**_<動詞>-<名詞>_** の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="46e80-105">In PowerShell, cmdlet names take the form of **_Verb-Noun_**.</span></span> <span data-ttu-id="46e80-106">**_Get_** という動詞が使われているコマンドレットがクエリのコマンドレットです。</span><span class="sxs-lookup"><span data-stu-id="46e80-106">The cmdlets using the verb **_Get_** are the query cmdlets.</span></span> <span data-ttu-id="46e80-107">コマンドレットの名詞の部分には、動詞の作用が及ぶ Azure リソースの種類が入ります。</span><span class="sxs-lookup"><span data-stu-id="46e80-107">The cmdlet nouns are the types of Azure resources that are acted upon by the cmdlet verbs.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="46e80-108">単純なプロパティを選択する</span><span class="sxs-lookup"><span data-stu-id="46e80-108">Select simple properties</span></span>

<span data-ttu-id="46e80-109">Azure PowerShell では、コマンドレットごとに既定の書式が定義されています。</span><span class="sxs-lookup"><span data-stu-id="46e80-109">Azure PowerShell has default formatting defined for each cmdlet.</span></span> <span data-ttu-id="46e80-110">各リソース タイプのきわめて一般的なプロパティについては、自動的に表形式または一覧形式で表示されます。</span><span class="sxs-lookup"><span data-stu-id="46e80-110">The most common properties for each resource type are displayed in a table or list format automatically.</span></span> <span data-ttu-id="46e80-111">出力の書式設定について詳しくは、「[クエリの結果の書式設定](formatting-output.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="46e80-111">For more information about formatting output, see [Formatting query results](formatting-output.md).</span></span>

<span data-ttu-id="46e80-112">ご利用のアカウントに存在する一連の VM を照会するには、`Get-AzureRmVM` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="46e80-112">Use the `Get-AzureRmVM` cmdlet to query for a list of VMs in your account.</span></span>

```azurepowershell-interactive
Get-AzureRmVM
```

<span data-ttu-id="46e80-113">既定の出力は、自動的に表形式となります。</span><span class="sxs-lookup"><span data-stu-id="46e80-113">The default output is automatically formatted as a table.</span></span>

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

<span data-ttu-id="46e80-114">特定のプロパティが必要であれば、`Select-Object` コマンドレットを使ってそれらを選択することができます。</span><span class="sxs-lookup"><span data-stu-id="46e80-114">The `Select-Object` cmdlet can be used to select the specific properties that are interesting to you.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Select Name,ResourceGroupName,Location
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="46e80-115">入れ子になった複雑なプロパティを選択する</span><span class="sxs-lookup"><span data-stu-id="46e80-115">Select complex nested properties</span></span>

<span data-ttu-id="46e80-116">必要なプロパティが、JSON 出力で入れ子になっている場合は、そのプロパティへの完全パスを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e80-116">If the property you want is nested in the JSON output, you need to supply the full path to the property.</span></span> <span data-ttu-id="46e80-117">`Get-AzureRmVM` コマンドレットの出力から VM 名と OS の種類を選択する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46e80-117">The following example shows how to select the VM Name and the OS type from the `Get-AzureRmVM` cmdlet.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-results-with-the-where-object-cmdlet"></a><span data-ttu-id="46e80-118">Where-Object コマンドレットを使って結果をフィルター処理する</span><span class="sxs-lookup"><span data-stu-id="46e80-118">Filter results with the Where-Object cmdlet</span></span>

<span data-ttu-id="46e80-119">`Where-Object` コマンドレットを使うと、プロパティの値に基づいて結果をフィルター選択することができます。</span><span class="sxs-lookup"><span data-stu-id="46e80-119">The `Where-Object` cmdlet allows you to filter the result based on any property value.</span></span> <span data-ttu-id="46e80-120">次の例では、名前に "RGD" という文字列が含まれる VM だけをフィルターで選択しています。</span><span class="sxs-lookup"><span data-stu-id="46e80-120">In the following example, the filter selects only VMs that have the text "RGD" in their name.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```output
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

<span data-ttu-id="46e80-121">次の例では、vmSize が 'Standard_DS1_V2' と等しい VM が結果として返されます。</span><span class="sxs-lookup"><span data-stu-id="46e80-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1_V2'.</span></span>

```azurepowershell-interactive
Get-AzureRmVM | Where vmSize -eq Standard_DS1_V2
```

```output
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```
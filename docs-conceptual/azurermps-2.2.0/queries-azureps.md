---
title: Azure リソースに対するクエリと結果の書式設定 | Microsoft Docs
description: Azure のリソースに対してクエリを実行し、その結果の書式を設定する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 1584c8166078b7d7d24ce8748307fde0f565b662
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853476"
---
# <a name="querying-for-azure-resources"></a>Azure リソースに対するクエリ

PowerShell におけるクエリは、組み込みのコマンドレットを使って実行できます。 PowerShell のコマンドレット名は、**_<動詞>-<名詞>_** の形式になっています。 **_Get_** という動詞が使われているコマンドレットがクエリのコマンドレットです。 コマンドレットの名詞の部分には、動詞の作用が及ぶ Azure リソースの種類が入ります。


## <a name="selecting-simple-properties"></a>単純なプロパティの選択

Azure PowerShell では、コマンドレットごとに既定の書式が定義されています。 各リソース タイプのきわめて一般的なプロパティについては、自動的に表形式または一覧形式で表示されます。 出力の書式設定について詳しくは、「[クエリの結果の書式設定](formatting-output.md)」をご覧ください。

ご利用のアカウントに存在する一連の VM を照会するには、`Get-AzureRmVM` コマンドレットを使います。

```powershell
Get-AzureRmVM
```

既定の出力は、自動的に表形式となります。

```
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

特定のプロパティが必要であれば、`Select-Object` コマンドレットを使ってそれらを選択することができます。

```powershell
Get-AzureRmVM | Select Name,ResourceGroupName,Location
```

```
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="selecting-complex-nested-properties"></a>入れ子になった複雑なプロパティを選択する

選択の対象となるプロパティが、JSON 出力の中で深く入れ子になっている場合は、その入れ子になっているプロパティの完全パスを指定する必要があります。 `Get-AzureRmVM` コマンドレットの出力から VM 名と OS の種類を選択する例を次に示します。

```powershell
Get-AzureRmVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-result-using-the-where-object-cmdlet"></a>Where-Object コマンドレットを使って結果をフィルター選択する

`Where-Object` コマンドレットを使うと、プロパティの値に基づいて結果をフィルター選択することができます。 次の例では、名前に "RGD" という文字列が含まれる VM だけをフィルターで選択しています。

```powershell
Get-AzureRmVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

次の例では、vmSize が 'Standard_DS1_V2' と等しい VM が結果として返されます。

```powershell
Get-AzureRmVM | Where vmSize -eq Standard_DS1_V2
```

```
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

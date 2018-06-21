---
title: PowerShell ジョブを使用したコマンドレットの並列実行
description: -AsJob パラメーターを使用してコマンドレットを並列して実行する方法。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/11/2017
ms.openlocfilehash: dfc1efa752c9c9fa42ad5904adacd83c2dc333b8
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2018
ms.locfileid: "33911937"
---
# <a name="running-cmdlets-in-parallel-using-powershell-jobs"></a>PowerShell ジョブを使用したコマンドレットの並列実行

PowerShell は、[PowerShell ジョブ](/powershell/module/microsoft.powershell.core/about/about_jobs)による非同期アクションをサポートしています。
Azure PowerShell は、Azure に対するネットワーク呼び出し (および、呼び出し待機) に大きく依存します。 開発者として、スクリプトで Azure への非ブロッキング呼び出しを複数実行しようとしていること、また、現在のセッションをブロックせずに REPL で Azure リソースを作成しなければならないことはよくあるでしょう。 こうしたニーズに対処するために、Azure PowerShell ではファースト クラス [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) がサポートされます。

## <a name="context-persistence-and-psjobs"></a>コンテキストの永続化と PSJob

PSJob は個別のプロセスで実行されます。つまり、Azure 接続に関する情報は、作成するジョブと適切に共有されている必要があります。 `Connect-AzureRmAccount` で Azure アカウントを PowerShell セッションに接続するとき、コンテキストをジョブに渡すことができます。

```powershell
$creds = Get-Credential
$job = Start-Job { param($context,$vmadmin) New-AzureRmVM -Name MyVm -AzureRmContext $context -Credential $vmadmin} -Arguments (Get-AzureRmContext),$creds
```

ただし、コンテキストが `Enable-AzureRmContextAutosave` で自動的に保存されるように選択した場合、そのコンテキストは、作成するすべてのジョブと自動的に共有されます。

```powershell
Enable-AzureRmContextAutosave
$creds = Get-Credential
$job = Start-Job { param($vmadmin) New-AzureRmVM -Name MyVm -Credential $vmadmin} -Arguments $creds
```

## <a name="automatic-jobs-with--asjob"></a>自動ジョブと `-AsJob`

必要に応じて、Azure PowerShell は実行時間の長い一部のコマンドレットで `-AsJob` スイッチを提供します。
`-AsJob` スイッチにより、PSJob の作成がさらに簡単になります。

```powershell
$creds = Get-Credential
$job = New-AzureRmVM -Name MyVm -Credential $creds -AsJob
```

ジョブと進行状況は、`Get-Job` および `Get-AzureRmVM` を使用していつでも確認できます。

```powershell
Get-Job $job
Get-AzureRmVM MyVm
```

```Output
Id Name                                       PSJobTypeName         State   HasMoreData Location  Command
-- ----                                       -------------         -----   ----------- --------  -------
1  Long Running Operation for 'New-AzureRmVM' AzureLongRunningJob`1 Running True        localhost New-AzureRmVM

ResourceGroupName    Name Location          VmSize  OsType     NIC ProvisioningState Zone
-----------------    ---- --------          ------  ------     --- ----------------- ----
MyVm                 MyVm   eastus Standard_DS1_v2 Windows    MyVm          Creating
```

その後、完了時に、ジョブの結果を取得するには、`Receive-Job` を使用します。

> [!NOTE]
> `Receive-Job` は、`-AsJob` フラグが存在しないように、コマンドレットから結果を返します。
> たとえば、`Do-Action -AsJob` の `Receive-Job` 結果の種類は、`Do-Action` の結果と同じです。

```powershell
$vm = Receive-Job $job
$vm
```

```Output
ResourceGroupName        : MyVm
Id                       : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyVm/providers/Microsoft.Compute/virtualMachines/MyVm
VmId                     : dff1f79e-a8f7-4664-ab72-0ec28b9fbb5b
Name                     : MyVm
Type                     : Microsoft.Compute/virtualMachines
Location                 : eastus
Tags                     : {}
HardwareProfile          : {VmSize}
NetworkProfile           : {NetworkInterfaces}
OSProfile                : {ComputerName, AdminUsername, WindowsConfiguration, Secrets}
ProvisioningState        : Succeeded
StorageProfile           : {ImageReference, OsDisk, DataDisks}
FullyQualifiedDomainName : myvmmyvm.eastus.cloudapp.azure.com
```

## <a name="example-scenarios"></a>シナリオ例

複数の VM を一度に作成します。

```powershell
$creds = Get-Credential
# Create 10 jobs.
for($k = 0; $k -lt 10; $k++) {
    New-AzureRmVm -Name MyVm$k  -Credential $creds -AsJob
}

# Get all jobs and wait on them.
Get-Job | Wait-Job
"All jobs completed"
Get-AzureRmVM
```

この例では、`Wait-Job` コマンドレットは、ジョブの実行中にスクリプトを一時停止します。 スクリプトは、すべてのジョブが完了した後に実行を続けます。 これにより、並列実行される複数のジョブを作成し、完了するのを待ってから、続行することができます。

```Output
Id     Name            PSJobTypeName   State         HasMoreData     Location             Command
--     ----            -------------   -----         -----------     --------             -------
2      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
3      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
4      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
5      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
6      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
7      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
8      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
9      Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
10     Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
11     Long Running... AzureLongRun... Running       True            localhost            New-AzureRmVM
2      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
3      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
4      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
5      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
6      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
7      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
8      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
9      Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
10     Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
11     Long Running... AzureLongRun... Completed     True            localhost            New-AzureRmVM
All Jobs completed.

ResourceGroupName        Name   Location          VmSize  OsType           NIC ProvisioningState Zone
-----------------        ----   --------          ------  ------           --- ----------------- ----
MYVM                     MyVm     eastus Standard_DS1_v2 Windows          MyVm         Succeeded
MYVM0                   MyVm0     eastus Standard_DS1_v2 Windows         MyVm0         Succeeded
MYVM1                   MyVm1     eastus Standard_DS1_v2 Windows         MyVm1         Succeeded
MYVM2                   MyVm2     eastus Standard_DS1_v2 Windows         MyVm2         Succeeded
MYVM3                   MyVm3     eastus Standard_DS1_v2 Windows         MyVm3         Succeeded
MYVM4                   MyVm4     eastus Standard_DS1_v2 Windows         MyVm4         Succeeded
MYVM5                   MyVm5     eastus Standard_DS1_v2 Windows         MyVm5         Succeeded
MYVM6                   MyVm6     eastus Standard_DS1_v2 Windows         MyVm6         Succeeded
MYVM7                   MyVm7     eastus Standard_DS1_v2 Windows         MyVm7         Succeeded
MYVM8                   MyVm8     eastus Standard_DS1_v2 Windows         MyVm8         Succeeded
MYVM9                   MyVm9     eastus Standard_DS1_v2 Windows         MyVm9         Succeeded
```

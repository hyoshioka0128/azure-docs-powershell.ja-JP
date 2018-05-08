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
ms.sourcegitcommit: 5f0013981fcea1d689649b9a2b2ffe84ae842e56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2018
---
# <a name="running-cmdlets-in-parallel-using-powershell-jobs"></a><span data-ttu-id="e3126-103">PowerShell ジョブを使用したコマンドレットの並列実行</span><span class="sxs-lookup"><span data-stu-id="e3126-103">Running cmdlets in parallel using PowerShell jobs</span></span>

<span data-ttu-id="e3126-104">PowerShell は、[PowerShell ジョブ](/powershell/module/microsoft.powershell.core/about/about_jobs)による非同期アクションをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e3126-104">PowerShell supports asynchronous action with [PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>
<span data-ttu-id="e3126-105">Azure PowerShell は、Azure に対するネットワーク呼び出し (および、呼び出し待機) に大きく依存します。</span><span class="sxs-lookup"><span data-stu-id="e3126-105">Azure PowerShell is heavily dependent on making, and waiting for, network calls to Azure.</span></span> <span data-ttu-id="e3126-106">開発者として、スクリプトで Azure への非ブロッキング呼び出しを複数実行しようとしていること、また、現在のセッションをブロックせずに REPL で Azure リソースを作成しなければならないことはよくあるでしょう。</span><span class="sxs-lookup"><span data-stu-id="e3126-106">As a developer, you may often find yourself looking to make multiple non-blocking calls to Azure in a script, or you may find that you want to create Azure resources in the REPL without blocking the current session.</span></span> <span data-ttu-id="e3126-107">こうしたニーズに対処するために、Azure PowerShell ではファースト クラス [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="e3126-107">To address these needs, Azure PowerShell provides first-class [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) support.</span></span>

## <a name="context-persistence-and-psjobs"></a><span data-ttu-id="e3126-108">コンテキストの永続化と PSJob</span><span class="sxs-lookup"><span data-stu-id="e3126-108">Context Persistence and PSJobs</span></span>

<span data-ttu-id="e3126-109">PSJob は個別のプロセスで実行されます。つまり、Azure 接続に関する情報は、作成するジョブと適切に共有されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3126-109">PSJobs are run in separate processes, which means that information about your Azure connection must be properly shared with the jobs you create.</span></span> <span data-ttu-id="e3126-110">`Connect-AzureRmAccount` で Azure アカウントを PowerShell セッションに接続するとき、コンテキストをジョブに渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="e3126-110">Upon connecting your Azure account to your PowerShell session with `Connect-AzureRmAccount`, you can pass the context to a job.</span></span>

```powershell
$creds = Get-Credential
$job = Start-Job { param($context,$vmadmin) New-AzureRmVM -Name MyVm -AzureRmContext $context -Credential $vmadmin} -Arguments (Get-AzureRmContext),$creds
```

<span data-ttu-id="e3126-111">ただし、コンテキストが `Enable-AzureRmContextAutosave` で自動的に保存されるように選択した場合、そのコンテキストは、作成するすべてのジョブと自動的に共有されます。</span><span class="sxs-lookup"><span data-stu-id="e3126-111">However, if you have chosen to have your context automatically saved with `Enable-AzureRmContextAutosave`, the context is automatically shared with any jobs you create.</span></span>

```powershell
Enable-AzureRmContextAutosave
$creds = Get-Credential
$job = Start-Job { param($vmadmin) New-AzureRmVM -Name MyVm -Credential $vmadmin} -Arguments $creds
```

## <a name="automatic-jobs-with--asjob"></a><span data-ttu-id="e3126-112">自動ジョブと `-AsJob`</span><span class="sxs-lookup"><span data-stu-id="e3126-112">Automatic Jobs with `-AsJob`</span></span>

<span data-ttu-id="e3126-113">必要に応じて、Azure PowerShell は実行時間の長い一部のコマンドレットで `-AsJob` スイッチを提供します。</span><span class="sxs-lookup"><span data-stu-id="e3126-113">As a convenience, Azure PowerShell also provides an `-AsJob` switch on some long-running cmdlets.</span></span>
<span data-ttu-id="e3126-114">`-AsJob` スイッチにより、PSJob の作成がさらに簡単になります。</span><span class="sxs-lookup"><span data-stu-id="e3126-114">The `-AsJob` switch makes creating PSJobs even easier.</span></span>

```powershell
$creds = Get-Credential
$job = New-AzureRmVM -Name MyVm -Credential $creds -AsJob
```

<span data-ttu-id="e3126-115">ジョブと進行状況は、`Get-Job` および `Get-AzureRmVM` を使用していつでも確認できます。</span><span class="sxs-lookup"><span data-stu-id="e3126-115">You can inspect the job and progress at any time with `Get-Job` and `Get-AzureRmVM`.</span></span>

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

<span data-ttu-id="e3126-116">その後、完了時に、ジョブの結果を取得するには、`Receive-Job` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3126-116">Subsequently, upon completion, you can obtain the result of the job with `Receive-Job`.</span></span>

> [!NOTE]
> <span data-ttu-id="e3126-117">`Receive-Job` は、`-AsJob` フラグが存在しないように、コマンドレットから結果を返します。</span><span class="sxs-lookup"><span data-stu-id="e3126-117">`Receive-Job` returns the result from the cmdlet as if the `-AsJob` flag were not present.</span></span>
> <span data-ttu-id="e3126-118">たとえば、`Do-Action -AsJob` の `Receive-Job` 結果の種類は、`Do-Action` の結果と同じです。</span><span class="sxs-lookup"><span data-stu-id="e3126-118">For example, the `Receive-Job` result of `Do-Action -AsJob` is of the same type as the result of `Do-Action`.</span></span>

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

## <a name="example-scenarios"></a><span data-ttu-id="e3126-119">シナリオ例</span><span class="sxs-lookup"><span data-stu-id="e3126-119">Example Scenarios</span></span>

<span data-ttu-id="e3126-120">複数の VM を一度に作成します。</span><span class="sxs-lookup"><span data-stu-id="e3126-120">Create multiple VMs at once.</span></span>

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

<span data-ttu-id="e3126-121">この例では、`Wait-Job` コマンドレットは、ジョブの実行中にスクリプトを一時停止します。</span><span class="sxs-lookup"><span data-stu-id="e3126-121">In this example, the `Wait-Job` cmdlet causes the script to pause while jobs run.</span></span> <span data-ttu-id="e3126-122">スクリプトは、すべてのジョブが完了した後に実行を続けます。</span><span class="sxs-lookup"><span data-stu-id="e3126-122">The script continues executing once all of the jobs have completed.</span></span> <span data-ttu-id="e3126-123">これにより、並列実行される複数のジョブを作成し、完了するのを待ってから、続行することができます。</span><span class="sxs-lookup"><span data-stu-id="e3126-123">This allows you to create several jobs running in parallel then wait for completion before continuing.</span></span>

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

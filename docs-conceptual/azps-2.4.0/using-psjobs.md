---
title: PowerShell ジョブを使用したコマンドレットを並列実行する
description: -AsJob パラメーターを使用してコマンドレットを並列して実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 825a07e01194a07b747712a62384c7f162e63d7d
ms.sourcegitcommit: a4e527d3deba004007cfa22fa536e8255dd23b37
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "67516489"
---
# <a name="running-cmdlets-in-parallel-using-powershell-jobs"></a><span data-ttu-id="0e620-103">PowerShell ジョブを使用したコマンドレットの並列実行</span><span class="sxs-lookup"><span data-stu-id="0e620-103">Running cmdlets in parallel using PowerShell jobs</span></span>

<span data-ttu-id="0e620-104">PowerShell は、[PowerShell ジョブ](/powershell/module/microsoft.powershell.core/about/about_jobs)による非同期アクションをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="0e620-104">PowerShell supports asynchronous action with [PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>
<span data-ttu-id="0e620-105">Azure PowerShell は、Azure に対するネットワーク呼び出し (および、呼び出し待機) に大きく依存します。</span><span class="sxs-lookup"><span data-stu-id="0e620-105">Azure PowerShell is heavily dependent on making, and waiting for, network calls to Azure.</span></span> <span data-ttu-id="0e620-106">非ブロッキング呼び出しを実行しなければならないことはよくあるでしょう。</span><span class="sxs-lookup"><span data-stu-id="0e620-106">You may often find yourself needing to make non-blocking calls.</span></span> <span data-ttu-id="0e620-107">このニーズに対処するために、Azure PowerShell ではファースト クラス [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="0e620-107">To address this need, Azure PowerShell provides first-class [PSJob](/powershell/module/microsoft.powershell.core/about/about_jobs) support.</span></span>

## <a name="context-persistence-and-psjobs"></a><span data-ttu-id="0e620-108">コンテキストの永続化と PSJob</span><span class="sxs-lookup"><span data-stu-id="0e620-108">Context Persistence and PSJobs</span></span>

<span data-ttu-id="0e620-109">PSJob は個別のプロセスで実行されるため、ご自身の Azure 接続は、これらの PSJob と共有されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e620-109">Since PSJobs are run as separate processes, your Azure connection must be shared with them.</span></span> <span data-ttu-id="0e620-110">コンテキストは、`Connect-AzAccount` でご自身の Azure アカウントにサインインしてから、ジョブに渡してください。</span><span class="sxs-lookup"><span data-stu-id="0e620-110">After signing in to your Azure account with `Connect-AzAccount`, pass the context to a job.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = Start-Job { param($context,$vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList (Get-AzContext),$creds
```

<span data-ttu-id="0e620-111">ただし、コンテキストが `Enable-AzContextAutosave` で自動的に保存されるように選択した場合、そのコンテキストは、作成するすべてのジョブと自動的に共有されます。</span><span class="sxs-lookup"><span data-stu-id="0e620-111">However, if you have chosen to have your context automatically saved with `Enable-AzContextAutosave`, the context is automatically shared with any jobs you create.</span></span>

```azurepowershell-interactive
Enable-AzContextAutosave
$creds = Get-Credential
$job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin} -ArgumentList $creds
```

## <a name="automatic-jobs-with--asjob"></a><span data-ttu-id="0e620-112">自動ジョブと `-AsJob`</span><span class="sxs-lookup"><span data-stu-id="0e620-112">Automatic Jobs with `-AsJob`</span></span>

<span data-ttu-id="0e620-113">必要に応じて、Azure PowerShell は実行時間の長い一部のコマンドレットで `-AsJob` スイッチを提供します。</span><span class="sxs-lookup"><span data-stu-id="0e620-113">As a convenience, Azure PowerShell also provides an `-AsJob` switch on some long-running cmdlets.</span></span>
<span data-ttu-id="0e620-114">`-AsJob` スイッチにより、PSJob の作成がさらに簡単になります。</span><span class="sxs-lookup"><span data-stu-id="0e620-114">The `-AsJob` switch makes creating PSJobs even easier.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$job = New-AzVM -Name MyVm -Credential $creds -AsJob
```

<span data-ttu-id="0e620-115">ジョブと進行状況は、`Get-Job` および `Get-AzVM` を使用していつでも確認できます。</span><span class="sxs-lookup"><span data-stu-id="0e620-115">You can inspect the job and progress at any time with `Get-Job` and `Get-AzVM`.</span></span>

```azurepowershell-interactive
Get-Job $job
Get-AzVM MyVm
```

```output
Id Name                                       PSJobTypeName         State   HasMoreData Location  Command
-- ----                                       -------------         -----   ----------- --------  -------
1  Long Running Operation for 'New-AzVM' AzureLongRunningJob`1 Running True        localhost New-AzVM

ResourceGroupName    Name Location          VmSize  OsType     NIC ProvisioningState Zone
-----------------    ---- --------          ------  ------     --- ----------------- ----
MyVm                 MyVm   eastus Standard_DS1_v2 Windows    MyVm          Creating
```

<span data-ttu-id="0e620-116">ジョブが完了したら、`Receive-Job` を使用してジョブの結果を取得します。</span><span class="sxs-lookup"><span data-stu-id="0e620-116">When the job completes, get the result of the job with `Receive-Job`.</span></span>

> [!NOTE]
> <span data-ttu-id="0e620-117">`Receive-Job` は、`-AsJob` フラグが存在しないように、コマンドレットから結果を返します。</span><span class="sxs-lookup"><span data-stu-id="0e620-117">`Receive-Job` returns the result from the cmdlet as if the `-AsJob` flag were not present.</span></span>
> <span data-ttu-id="0e620-118">たとえば、`Do-Action -AsJob` の `Receive-Job` 結果の種類は、`Do-Action` の結果と同じです。</span><span class="sxs-lookup"><span data-stu-id="0e620-118">For example, the `Receive-Job` result of `Do-Action -AsJob` is of the same type as the result of `Do-Action`.</span></span>

```azurepowershell-interactive
$vm = Receive-Job $job
$vm
```

```output
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

## <a name="example-scenarios"></a><span data-ttu-id="0e620-119">シナリオ例</span><span class="sxs-lookup"><span data-stu-id="0e620-119">Example Scenarios</span></span>

<span data-ttu-id="0e620-120">複数の VM を一度に作成します。</span><span class="sxs-lookup"><span data-stu-id="0e620-120">Create several VMs at once:</span></span>

```azurepowershell-interactive
$creds = Get-Credential
# Create 10 jobs.
for($k = 0; $k -lt 10; $k++) {
    New-AzVm -Name MyVm$k  -Credential $creds -AsJob
}

# Get all jobs and wait on them.
Get-Job | Wait-Job
"All jobs completed"
Get-AzVM
```

<span data-ttu-id="0e620-121">この例では、`Wait-Job` コマンドレットは、ジョブの実行中にスクリプトを一時停止します。</span><span class="sxs-lookup"><span data-stu-id="0e620-121">In this example, the `Wait-Job` cmdlet causes the script to pause while jobs run.</span></span> <span data-ttu-id="0e620-122">スクリプトは、すべてのジョブが完了した後に実行を続けます。</span><span class="sxs-lookup"><span data-stu-id="0e620-122">The script continues executing once all of the jobs have completed.</span></span> <span data-ttu-id="0e620-123">複数のジョブが並列で実行され、スクリプトはその完了後に続行されます。</span><span class="sxs-lookup"><span data-stu-id="0e620-123">Several jobs run in parallel then the script waits for completion before continuing.</span></span>

```output
Id     Name            PSJobTypeName   State         HasMoreData     Location             Command
--     ----            -------------   -----         -----------     --------             -------
2      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
3      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
4      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
5      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
6      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
7      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
8      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
9      Long Running... AzureLongRun... Running       True            localhost            New-AzVM
10     Long Running... AzureLongRun... Running       True            localhost            New-AzVM
11     Long Running... AzureLongRun... Running       True            localhost            New-AzVM
2      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
3      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
4      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
5      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
6      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
7      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
8      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
9      Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
10     Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
11     Long Running... AzureLongRun... Completed     True            localhost            New-AzVM
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

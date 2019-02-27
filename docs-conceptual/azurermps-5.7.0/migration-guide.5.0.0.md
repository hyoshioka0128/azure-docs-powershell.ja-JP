---
title: Microsoft Azure PowerShell 5.0.0 の重大な変更
description: この移行ガイドには、バージョン 5 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: b4cbeb1b523664fb49c4640eaafd56e3b843ebaa
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56144558"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a><span data-ttu-id="af287-103">Microsoft Azure PowerShell 5.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-103">Breaking changes for Microsoft Azure PowerShell 5.0.0</span></span>

<span data-ttu-id="af287-104">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="af287-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="af287-105">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="af287-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="af287-106">詳細なコンテキストについては、各変更に関する pull request を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af287-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="af287-107">目次</span><span class="sxs-lookup"><span data-stu-id="af287-107">Table of Contents</span></span>

- [<span data-ttu-id="af287-108">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-108">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
- [<span data-ttu-id="af287-109">Batch コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-109">Breaking changes to Batch cmdlets</span></span>](#breaking-changes-to-batch-cmdlets)
- [<span data-ttu-id="af287-110">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-110">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="af287-111">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-111">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="af287-112">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-112">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="af287-113">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-113">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="af287-114">Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-114">Breaking changes to Resources cmdlets</span></span>](#breaking-changes-to-resources-cmdlets)
- [<span data-ttu-id="af287-115">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-115">Breaking Changes to ServiceBus Cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="af287-116">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-116">Breaking changes to ApiManagement cmdlets</span></span>

### <a name="new-azurermapimanagementbackendproxy"></a><span data-ttu-id="af287-117">**New-AzureRmApiManagementBackendProxy**</span><span class="sxs-lookup"><span data-stu-id="af287-117">**New-AzureRmApiManagementBackendProxy**</span></span>
- <span data-ttu-id="af287-118">"UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-118">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell-interactive
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a><span data-ttu-id="af287-119">**New-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="af287-119">**New-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="af287-120">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-120">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a><span data-ttu-id="af287-121">**Set-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="af287-121">**Set-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="af287-122">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-122">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a><span data-ttu-id="af287-123">Batch コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-123">Breaking changes to Batch cmdlets</span></span>

### <a name="new-azurebatchcertificate"></a><span data-ttu-id="af287-124">**New-AzureBatchCertificate**</span><span class="sxs-lookup"><span data-stu-id="af287-124">**New-AzureBatchCertificate**</span></span>
- <span data-ttu-id="af287-125">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-125">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a><span data-ttu-id="af287-126">**New-AzureBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="af287-126">**New-AzureBatchComputeNodeUser**</span></span>
- <span data-ttu-id="af287-127">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-127">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a><span data-ttu-id="af287-128">**Set-AzureRmBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="af287-128">**Set-AzureRmBatchComputeNodeUser**</span></span>
- <span data-ttu-id="af287-129">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-129">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell-interactive
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a><span data-ttu-id="af287-130">**New-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="af287-130">**New-AzureBatchTask**</span></span>
 - <span data-ttu-id="af287-131">`RunElevated` スイッチが削除され、`UserIdentity` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af287-131">Removed the `RunElevated` switch and replaced it with `UserIdentity`.</span></span>

```powershell-interactive
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

<span data-ttu-id="af287-132">これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="af287-132">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="psmultiinstancesettings"></a><span data-ttu-id="af287-133">**PSMultiInstanceSettings**</span><span class="sxs-lookup"><span data-stu-id="af287-133">**PSMultiInstanceSettings**</span></span>

- <span data-ttu-id="af287-134">`PSMultiInstanceSettings` コンストラクターが `numberOfInstances` 必須パラメーターを受け取らなくなりました。代わりに、`coordinationCommandLine` 必須パラメーターを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="af287-134">`PSMultiInstanceSettings` constructor no longer takes a required `numberOfInstances` parameter, instead it takes a required `coordinationCommandLine` parameter.</span></span>

```powershell-interactive
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a><span data-ttu-id="af287-135">**Get-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="af287-135">**Get-AzureBatchTask**</span></span>
 - <span data-ttu-id="af287-136">`PSCloudTask` の `RunElevated` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-136">Removed the `RunElevated` property on `PSCloudTask`.</span></span> <span data-ttu-id="af287-137">`RunElevated` に代わって `UserIdentity` プロパティが追加されました。</span><span class="sxs-lookup"><span data-stu-id="af287-137">The `UserIdentity` property has been added to replace `RunElevated`.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

<span data-ttu-id="af287-138">これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="af287-138">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="multiple-types"></a><span data-ttu-id="af287-139">**複数の型**</span><span class="sxs-lookup"><span data-stu-id="af287-139">**Multiple types**</span></span>

- <span data-ttu-id="af287-140">`PSExitConditions` の `SchedulingError` プロパティの名前が `PreProcessingError` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af287-140">Renamed the `SchedulingError` property on `PSExitConditions` to `PreProcessingError`.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a><span data-ttu-id="af287-141">**複数の型**</span><span class="sxs-lookup"><span data-stu-id="af287-141">**Multiple types**</span></span>

- <span data-ttu-id="af287-142">`PSJobPreparationTaskExecutionInformation`、`PSJobReleaseTaskExecutionInformation`、`PSStartTaskInformation`、`PSSubtaskInformation`、`PSTaskExecutionInformation` の `SchedulingError` プロパティの名前が `FailureInformation` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af287-142">Renamed the `SchedulingError` property on `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation`, and `PSTaskExecutionInformation` to `FailureInformation`.</span></span>
  - <span data-ttu-id="af287-143">タスク エラーが発生すると、常に `FailureInformation` が返されます。</span><span class="sxs-lookup"><span data-stu-id="af287-143">`FailureInformation` is returned any time there is a task failure.</span></span> <span data-ttu-id="af287-144">これには、以前のすべてのスケジュール エラー ケースとゼロ以外のタスク終了コード、および新しい出力ファイル機能からのファイル アップロード エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="af287-144">This includes all previous scheduling error cases, as well as nonzero task exit codes, and file upload failures from the new output files feature.</span></span>
  - <span data-ttu-id="af287-145">これは以前と同様に構造化されているので、この型を使用するときにコードの変更は不要です。</span><span class="sxs-lookup"><span data-stu-id="af287-145">This is structured the same as before, so no code change is needed when using this type.</span></span>

```powershell-interactive
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

<span data-ttu-id="af287-146">これは、次のものにも影響を及ぼします。Get-AzureBatchPool、Get-AzureBatchSubtask、Get-AzureBatchJobPreparationAndReleaseTaskStatus</span><span class="sxs-lookup"><span data-stu-id="af287-146">This additionally impacts: Get-AzureBatchPool, Get-AzureBatchSubtask, and Get-AzureBatchJobPreparationAndReleaseTaskStatus</span></span>

### <a name="new-azurebatchpool"></a><span data-ttu-id="af287-147">**New-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="af287-147">**New-AzureBatchPool**</span></span>
 - <span data-ttu-id="af287-148">`TargetDedicated` が削除され、`TargetDedicatedComputeNodes` および `TargetLowPriorityComputeNodes` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af287-148">Removed `TargetDedicated` and replaced it with `TargetDedicatedComputeNodes` and `TargetLowPriorityComputeNodes`.</span></span>
 - <span data-ttu-id="af287-149">`TargetDedicatedComputeNodes` には、エイリアス `TargetDedicated` があります。</span><span class="sxs-lookup"><span data-stu-id="af287-149">`TargetDedicatedComputeNodes` has an alias `TargetDedicated`.</span></span>

```powershell-interactive
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

<span data-ttu-id="af287-150">これは、次のものにも影響を及ぼします。Start-AzureBatchPoolResize</span><span class="sxs-lookup"><span data-stu-id="af287-150">This also impacts: Start-AzureBatchPoolResize</span></span>

### <a name="get-azurebatchpool"></a><span data-ttu-id="af287-151">**Get-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="af287-151">**Get-AzureBatchPool**</span></span>
 - <span data-ttu-id="af287-152">`PSCloudPool` の `TargetDedicated` プロパティおよび `CurrentDedicated` プロパティの名前が、`TargetDedicatedComputeNodes`、`CurrentDedicatedComputeNodes` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="af287-152">Renamed the `TargetDedicated` and `CurrentDedicated` properties on `PSCloudPool` to `TargetDedicatedComputeNodes` and `CurrentDedicatedComputeNodes`.</span></span>

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a><span data-ttu-id="af287-153">**PSCloudPool 型**</span><span class="sxs-lookup"><span data-stu-id="af287-153">**Type PSCloudPool**</span></span>

- <span data-ttu-id="af287-154">`PSCloudPool` の `ResizeError` の名前が `ResizeErrors` に変更され、コレクションになりました。</span><span class="sxs-lookup"><span data-stu-id="af287-154">Renamed `ResizeError` to `ResizeErrors` on `PSCloudPool`, and it is now a collection.</span></span>

```powershell-interactive
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a><span data-ttu-id="af287-155">**New-AzureBatchJob**</span><span class="sxs-lookup"><span data-stu-id="af287-155">**New-AzureBatchJob**</span></span>
- <span data-ttu-id="af287-156">`PSPoolSpecification` の `TargetDedicated` プロパティの名前が `TargetDedicatedComputeNodes` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af287-156">Renamed the `TargetDedicated` property on `PSPoolSpecification` to `TargetDedicatedComputeNodes`.</span></span>

```powershell-interactive
# Old
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicated = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo

# New
$poolInfo = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolInformation
$poolInfo.AutoPoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification = New-Object Microsoft.Azure.Commands.Batch.Models.PSPoolSpecification
$poolInfo.AutoPoolSpecification.PoolSpecification.TargetDedicatedComputeNodes = 5
New-AzureBatchJob [other parameters] -PoolInformation $poolInfo
```

### <a name="get-azurebatchnodefile"></a><span data-ttu-id="af287-157">**Get-AzureBatchNodeFile**</span><span class="sxs-lookup"><span data-stu-id="af287-157">**Get-AzureBatchNodeFile**</span></span>
 - <span data-ttu-id="af287-158">`Name` が削除され、`Path` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af287-158">Removed `Name` and replaced it with `Path`.</span></span>
 - <span data-ttu-id="af287-159">`Path` には、エイリアス `Name` があります。</span><span class="sxs-lookup"><span data-stu-id="af287-159">`Path` has an alias `Name`.</span></span>

```powershell-interactive
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

<span data-ttu-id="af287-160">これは、次のものにも影響を及ぼします。Get-AzureBatchNodeFileContent、Remove-AzureBatchNodeFile</span><span class="sxs-lookup"><span data-stu-id="af287-160">This also impacts: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span></span>

### <a name="type-psnodefile"></a><span data-ttu-id="af287-161">**PSNodeFile** 型</span><span class="sxs-lookup"><span data-stu-id="af287-161">Type **PSNodeFile**</span></span>

 - <span data-ttu-id="af287-162">`PSNodeFile` の `Name` プロパティの名前が `Path` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af287-162">Renamed the `Name` property on `PSNodeFile` to `Path`.</span></span>

```powershell-interactive
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a><span data-ttu-id="af287-163">**Get-AzureBatchSubtask**</span><span class="sxs-lookup"><span data-stu-id="af287-163">**Get-AzureBatchSubtask**</span></span>
- <span data-ttu-id="af287-164">`PSSubtaskInformation` の `PreviousState` プロパティと `State` プロパティが `TaskState` 型ではなくなり、`SubtaskState` 型になりました。</span><span class="sxs-lookup"><span data-stu-id="af287-164">The `PreviousState` and `State` properties of `PSSubtaskInformation` are no longer of type `TaskState`, instead they are of type `SubtaskState`.</span></span>
  - <span data-ttu-id="af287-165">`TaskState` とは異なり、`SubtaskState` はサブタスクを `Active` 状態にすることができないため、この型には `Active` 値はありません。</span><span class="sxs-lookup"><span data-stu-id="af287-165">Unlike `TaskState`, `SubtaskState` has no `Active` value, since it is not possible for subtasks to be in an `Active` state.</span></span>

```powershell-interactive
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="af287-166">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-166">Breaking changes to Compute cmdlets</span></span>

### <a name="set-azurermvmaccessextension"></a><span data-ttu-id="af287-167">**Set-AzureRmVMAccessExtension**</span><span class="sxs-lookup"><span data-stu-id="af287-167">**Set-AzureRmVMAccessExtension**</span></span>
- <span data-ttu-id="af287-168">"UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-168">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell-interactive
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="af287-169">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-169">Breaking changes to EventHub cmdlets</span></span>

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="af287-170">**New-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-170">**New-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-171">"New-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-171">The 'New-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-172">"New-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-172">Please use the 'New-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="af287-173">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-173">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-174">"Get-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-174">The 'Get-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-175">"Get-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-175">Please use the 'Get-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="af287-176">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-176">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-177">"Set-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-177">The 'Set-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-178">"Set-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-178">Please use the 'Set-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="af287-179">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-179">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-180">"Remove-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-180">The 'Remove-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-181">"Remove-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-181">Please use the 'Remove-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespacekey"></a><span data-ttu-id="af287-182">**New-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="af287-182">**New-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="af287-183">"New-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-183">The 'New-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-184">"New-AzureRmEventHubKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-184">Please use the 'New-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespacekey"></a><span data-ttu-id="af287-185">**Get-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="af287-185">**Get-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="af287-186">"Get-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-186">The 'Get-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-187">"Get-AzureRmEventHubKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-187">Please use the 'Get-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="af287-188">**New-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="af287-188">**New-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="af287-189">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-189">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="af287-190">**Get-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="af287-190">**Get-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="af287-191">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-191">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a><span data-ttu-id="af287-192">**Set-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="af287-192">**Set-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="af287-193">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-193">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a><span data-ttu-id="af287-194">**New-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="af287-194">**New-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="af287-195">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-195">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a><span data-ttu-id="af287-196">**Set-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="af287-196">**Set-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="af287-197">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-197">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a><span data-ttu-id="af287-198">**Get-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="af287-198">**Get-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="af287-199">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="af287-199">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell-interactive
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="af287-200">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-200">Breaking changes to Insights cmdlets</span></span>

### <a name="add-azurermlogalertrule"></a><span data-ttu-id="af287-201">**Add-AzureRMLogAlertRule**</span><span class="sxs-lookup"><span data-stu-id="af287-201">**Add-AzureRMLogAlertRule**</span></span>
- <span data-ttu-id="af287-202">**Add-AzureRMLogAlertRule** コマンドレットは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="af287-202">The **Add-AzureRMLogAlertRule** cmdlet has been deprecated</span></span>
- <span data-ttu-id="af287-203">10 月 1 日以降、この機能はアクティビティ ログ アラートに移行するため、このコマンドレットを使用しても効果はなくなります。</span><span class="sxs-lookup"><span data-stu-id="af287-203">After October 1st using this cmdlet will no longer have any effect as this functionality is being transitioned to Activity Log Alerts.</span></span> <span data-ttu-id="af287-204">詳細については、 https://aka.ms/migratemealerts を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af287-204">Please see https://aka.ms/migratemealerts for more information.</span></span>

### <a name="get-azurermusage"></a><span data-ttu-id="af287-205">**Get-AzureRMUsage**</span><span class="sxs-lookup"><span data-stu-id="af287-205">**Get-AzureRMUsage**</span></span>
- <span data-ttu-id="af287-206">**Get-AzureRMUsage** コマンドレットは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="af287-206">The **Get-AzureRMUsage** cmdlet has been deprecated</span></span>

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a><span data-ttu-id="af287-207">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span><span class="sxs-lookup"><span data-stu-id="af287-207">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span></span>
- <span data-ttu-id="af287-208">出力の変更:(これらのコマンドレットから返される) EventData オブジェクトの EventChannels フィールドは、定数値 (Admin,Operation) を返すようになったため、非推奨となります。</span><span class="sxs-lookup"><span data-stu-id="af287-208">Output change: The field EventChannels from the EventData object (returned by these cmdlets) is being deprecated since it now returns a constant value (Admin,Operation.)</span></span>

### <a name="get-azurermalertrule"></a><span data-ttu-id="af287-209">**Get-AzureRmAlertRule**</span><span class="sxs-lookup"><span data-stu-id="af287-209">**Get-AzureRmAlertRule**</span></span>
- <span data-ttu-id="af287-210">出力の変更:ユーザー エクスペリエンスを向上させるために、このコマンドレットの出力はフラット化されます (プロパティ フィールドが排除されます)。</span><span class="sxs-lookup"><span data-stu-id="af287-210">Output change: The output of this cmdlet will be flattened, i.e. elimination of the properties field, to improve the user experience.</span></span>

```powershell-interactive
# Old
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground Red "Error updating alert rule"
    Write-Host $rules[0].Id
    Write-Host $rules[0].Properties.IsEnabled
    Write-Host $rules[0].Properties.Condition
}

# New
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -Foreground red "Error updating alert rule"
    Write-Host $rules[0].Id

    # Properties will remain for a while
    Write-Host $rules[0].Properties.IsEnabled
      
    # But the properties will be at the top level too. Later Properties will be removed
    Write-Host $rules[0].IsEnabled
    Write-Host $rules[0].Condition
}
```

### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="af287-211">**Get-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="af287-211">**Get-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="af287-212">出力の変更:AutoscaleSettingResourceName フィールドは Name フィールドと常に等しいため、非推奨となります。</span><span class="sxs-lookup"><span data-stu-id="af287-212">Output change: The AutoscaleSettingResourceName field will be deprecated since it always equals the Name field.</span></span>

```powershell-interactive
# Old
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
if ($s1.AutoscaleSettingResourceName -ne $s1.Name)
{
    Write-Host "There is something wrong with the name"
}

# New
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
    
# there won't be a AutoscaleSettingResourceName
Write-Host $s1.Name    
```

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a><span data-ttu-id="af287-213">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="af287-213">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span></span>
- <span data-ttu-id="af287-214">出力の変更:要求 ID と状態コードを含む単一のオブジェクトを返すために出力の型が変更されます。</span><span class="sxs-lookup"><span data-stu-id="af287-214">Output change: The type of the output will change to return a single object containing the request Id and the status code.</span></span>

```powershell-interactive
# Old
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
if ($s1 -ne $null)
{
    $r = $s1[0].RequestId
    $s = $s1[0].StatusCode
}

# New
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name $ruleName
$r = $s1.RequestId
$s = $s1.StatusCode
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="af287-215">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-215">Breaking changes to Network cmdlets</span></span>

### <a name="add-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="af287-216">**Add-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="af287-216">**Add-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="af287-217">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-217">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="af287-218">**New-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="af287-218">**New-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="af287-219">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-219">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="af287-220">**Set-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="af287-220">**Set-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="af287-221">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-221">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a><span data-ttu-id="af287-222">Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-222">Breaking changes to Resources cmdlets</span></span>

### <a name="new-azurermadappcredential"></a><span data-ttu-id="af287-223">**New-AzureRmADAppCredential**</span><span class="sxs-lookup"><span data-stu-id="af287-223">**New-AzureRmADAppCredential**</span></span>
- <span data-ttu-id="af287-224">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-224">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a><span data-ttu-id="af287-225">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="af287-225">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="af287-226">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-226">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a><span data-ttu-id="af287-227">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="af287-227">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="af287-228">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-228">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a><span data-ttu-id="af287-229">**New-AzureRmADSpCredential**</span><span class="sxs-lookup"><span data-stu-id="af287-229">**New-AzureRmADSpCredential**</span></span>
- <span data-ttu-id="af287-230">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-230">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a><span data-ttu-id="af287-231">**New-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="af287-231">**New-AzureRmADUser**</span></span>
- <span data-ttu-id="af287-232">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-232">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a><span data-ttu-id="af287-233">**Set-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="af287-233">**Set-AzureRmADUser**</span></span>
- <span data-ttu-id="af287-234">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="af287-234">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell-interactive
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="af287-235">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="af287-235">Breaking changes to ServiceBus cmdlets</span></span>

### <a name="get-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="af287-236">**Get-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-236">**Get-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="af287-237">"Get-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-237">The 'Get-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-238">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-238">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>    

### <a name="get-azurermservicebustopickey"></a><span data-ttu-id="af287-239">**Get-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="af287-239">**Get-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="af287-240">"Get-AzureRmServiceBusTopicKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-240">The 'Get-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-241">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-241">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="af287-242">**New-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-242">**New-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="af287-243">"New-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-243">The 'New-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-244">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-244">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebustopickey"></a><span data-ttu-id="af287-245">**New-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="af287-245">**New-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="af287-246">"New-AzureRmServiceBusTopicKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-246">The 'New-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-247">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-247">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="af287-248">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-248">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="af287-249">"Remove-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-249">The 'Remove-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-250">"Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-250">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="af287-251">**Set-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-251">**Set-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="af287-252">"Set-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-252">The 'Set-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-253">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-253">Please use the 'Set-AzureRmServiceBusAuthorizationRule'cmdlet.</span></span>

### <a name="new-azurermservicebusnamespacekey"></a><span data-ttu-id="af287-254">**New-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="af287-254">**New-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="af287-255">"New-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-255">The 'New-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-256">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-256">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="get-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="af287-257">**Get-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-257">**Get-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="af287-258">"Get-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-258">The 'Get-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-259">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-259">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusqueuekey"></a><span data-ttu-id="af287-260">**Get-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="af287-260">**Get-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="af287-261">"Get-AzureRmServiceBusQueueKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-261">The 'Get-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-262">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-262">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="af287-263">**New-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-263">**New-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="af287-264">"New-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-264">The 'New-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-265">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-265">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebusqueuekey"></a><span data-ttu-id="af287-266">**New-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="af287-266">**New-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="af287-267">"New-AzureRmServiceBusQueueKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-267">The 'New-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-268">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-268">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="af287-269">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-269">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="af287-270">"Remove-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-270">The 'Remove-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-271">"GRemove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-271">Please use the 'GRemove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="af287-272">**Set-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-272">**Set-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="af287-273">"Set-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-273">The 'Set-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-274">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-274">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="af287-275">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-275">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-276">"Get-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-276">The 'Get-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-277">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-277">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespacekey"></a><span data-ttu-id="af287-278">**Get-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="af287-278">**Get-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="af287-279">"Get-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-279">The 'Get-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="af287-280">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-280">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="af287-281">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-281">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-282">"New-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-282">The 'New-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-283">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-283">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="af287-284">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-284">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-285">"Remove-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-285">The 'Remove-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-286">"Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-286">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="af287-287">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="af287-287">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="af287-288">"Set-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-288">The 'Set-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="af287-289">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="af287-289">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="type-namespaceattributes"></a><span data-ttu-id="af287-290">**NamespaceAttributes 型**</span><span class="sxs-lookup"><span data-stu-id="af287-290">**Type NamespaceAttributes**</span></span>
- <span data-ttu-id="af287-291">次のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af287-291">The following properties have been removed</span></span>
    - <span data-ttu-id="af287-292">Enabled</span><span class="sxs-lookup"><span data-stu-id="af287-292">Enabled</span></span>
    - <span data-ttu-id="af287-293">Status</span><span class="sxs-lookup"><span data-stu-id="af287-293">Status</span></span>
   
```powershell-interactive
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a><span data-ttu-id="af287-294">**QueueAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="af287-294">**Type QueueAttribute**</span></span>
- <span data-ttu-id="af287-295">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="af287-295">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="af287-296">EnableBatchedOperations</span><span class="sxs-lookup"><span data-stu-id="af287-296">EnableBatchedOperations</span></span>
    - <span data-ttu-id="af287-297">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="af287-297">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="af287-298">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="af287-298">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="af287-299">SupportOrdering</span><span class="sxs-lookup"><span data-stu-id="af287-299">SupportOrdering</span></span>

```powershell-interactive
# Old
# The $queue has EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties
$queue = Get-AzureRmServiceBusQueue <parameters>
$queue.EntityAvailabilityStatus
$queue.EnableBatchedOperations
$queue.IsAnonymousAccessible
$queue.SupportOrdering  

# New
# The call remains the same, but the returned values Queue object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$queue = Get-AzureRmServiceBusQueue <parameters>
```
   
### <a name="type-topicattribute"></a><span data-ttu-id="af287-300">**TopicAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="af287-300">**Type TopicAttribute**</span></span>
- <span data-ttu-id="af287-301">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="af287-301">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="af287-302">Location</span><span class="sxs-lookup"><span data-stu-id="af287-302">Location</span></span>
    - <span data-ttu-id="af287-303">IsExpress</span><span class="sxs-lookup"><span data-stu-id="af287-303">IsExpress</span></span>
    - <span data-ttu-id="af287-304">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="af287-304">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="af287-305">FilteringMessagesBeforePublishing</span><span class="sxs-lookup"><span data-stu-id="af287-305">FilteringMessagesBeforePublishing</span></span>
    - <span data-ttu-id="af287-306">EnableSubscriptionPartitioning</span><span class="sxs-lookup"><span data-stu-id="af287-306">EnableSubscriptionPartitioning</span></span>
    - <span data-ttu-id="af287-307">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="af287-307">EntityAvailabilityStatus</span></span>

```powershell-interactive
# Old
# The $topic has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$topic = Get-AzureRmServiceBusTopic <parameters>
$topic.EntityAvailabilityStatus
$topic.EnableSubscriptionPartitioning
$topic.IsAnonymousAccessible
$topic.IsExpress
$topic.FilteringMessagesBeforePublishing
$topic.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$topic = Get-AzureRmServiceBusTopic <parameters>
```
   
### <a name="type-subscriptionattribute"></a><span data-ttu-id="af287-308">**SubscriptionAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="af287-308">**Type SubscriptionAttribute**</span></span>
- <span data-ttu-id="af287-309">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="af287-309">The following properties are marked as obsolete</span></span>
    - <span data-ttu-id="af287-310">DeadLetteringOnFilterEvaluationExceptions</span><span class="sxs-lookup"><span data-stu-id="af287-310">DeadLetteringOnFilterEvaluationExceptions</span></span>
    - <span data-ttu-id="af287-311">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="af287-311">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="af287-312">IsReadOnly</span><span class="sxs-lookup"><span data-stu-id="af287-312">IsReadOnly</span></span>
    - <span data-ttu-id="af287-313">Location</span><span class="sxs-lookup"><span data-stu-id="af287-313">Location</span></span>
   
```powershell-interactive
# Old
# The $subscription has EntityAvailabilityStatus, EnableSubscriptionPartitioning, IsAnonymousAccessible, IsExpress, Location and FilteringMessagesBeforePublishing properties
$subscription = Get-AzureRmServiceBussubscription <parameters>
$subscription.EntityAvailabilityStatus
$subscription.EnableSubscriptionPartitioning
$subscription.IsAnonymousAccessible
$subscription.IsExpress
$subscription.FilteringMessagesBeforePublishing
$subscription.Location

# New
# The call remains the same, but the returned values Topic object will not have the EntityAvailabilityStatus, EnableBatchedOperations, IsAnonymousAccessible and SupportOrdering properties    
$subscription = Get-AzureRmServiceBussubscription <parameters>
```
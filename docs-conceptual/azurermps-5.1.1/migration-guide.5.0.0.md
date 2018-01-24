# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a><span data-ttu-id="48bf3-101">Microsoft Azure PowerShell 5.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-101">Breaking changes for Microsoft Azure PowerShell 5.0.0</span></span>

<span data-ttu-id="48bf3-102">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="48bf3-103">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="48bf3-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="48bf3-104">詳細なコンテキストについては、各変更に関するプル要求を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="48bf3-105">目次</span><span class="sxs-lookup"><span data-stu-id="48bf3-105">Table of Contents</span></span>

- [<span data-ttu-id="48bf3-106">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-106">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
- [<span data-ttu-id="48bf3-107">Batch コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-107">Breaking changes to Batch cmdlets</span></span>](#breaking-changes-to-batch-cmdlets)
- [<span data-ttu-id="48bf3-108">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-108">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="48bf3-109">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-109">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="48bf3-110">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-110">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="48bf3-111">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-111">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="48bf3-112">Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-112">Breaking changes to Resources cmdlets</span></span>](#breaking-changes-to-resources-cmdlets)
- [<span data-ttu-id="48bf3-113">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-113">Breaking Changes to ServiceBus Cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="48bf3-114">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-114">Breaking changes to ApiManagement cmdlets</span></span>

### <a name="new-azurermapimanagementbackendproxy"></a><span data-ttu-id="48bf3-115">**New-AzureRmApiManagementBackendProxy**</span><span class="sxs-lookup"><span data-stu-id="48bf3-115">**New-AzureRmApiManagementBackendProxy**</span></span>
- <span data-ttu-id="48bf3-116">"UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-116">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a><span data-ttu-id="48bf3-117">**New-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-117">**New-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="48bf3-118">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-118">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a><span data-ttu-id="48bf3-119">**Set-AzureRmApiManagementUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-119">**Set-AzureRmApiManagementUser**</span></span>
- <span data-ttu-id="48bf3-120">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-120">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a><span data-ttu-id="48bf3-121">Batch コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-121">Breaking changes to Batch cmdlets</span></span>

### <a name="new-azurebatchcertificate"></a><span data-ttu-id="48bf3-122">**New-AzureBatchCertificate**</span><span class="sxs-lookup"><span data-stu-id="48bf3-122">**New-AzureBatchCertificate**</span></span>
- <span data-ttu-id="48bf3-123">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-123">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a><span data-ttu-id="48bf3-124">**New-AzureBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-124">**New-AzureBatchComputeNodeUser**</span></span>
- <span data-ttu-id="48bf3-125">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-125">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a><span data-ttu-id="48bf3-126">**Set-AzureRmBatchComputeNodeUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-126">**Set-AzureRmBatchComputeNodeUser**</span></span>
- <span data-ttu-id="48bf3-127">`Password` パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-127">Parameter `Password` being replaced in favor of a Secure string</span></span>

```powershell
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a><span data-ttu-id="48bf3-128">**New-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="48bf3-128">**New-AzureBatchTask**</span></span>
 - <span data-ttu-id="48bf3-129">`RunElevated` スイッチが削除され、`UserIdentity` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-129">Removed the `RunElevated` switch and replaced it with `UserIdentity`.</span></span>

```powershell
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

<span data-ttu-id="48bf3-130">これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="48bf3-130">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="psmultiinstancesettings"></a><span data-ttu-id="48bf3-131">**PSMultiInstanceSettings**</span><span class="sxs-lookup"><span data-stu-id="48bf3-131">**PSMultiInstanceSettings**</span></span>

- <span data-ttu-id="48bf3-132">`PSMultiInstanceSettings` コンストラクターが `numberOfInstances` 必須パラメーターを受け取らなくなりました。代わりに、`coordinationCommandLine` 必須パラメーターを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-132">`PSMultiInstanceSettings` constructor no longer takes a required `numberOfInstances` parameter, instead it takes a required `coordinationCommandLine` parameter.</span></span>

```powershell
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a><span data-ttu-id="48bf3-133">**Get-AzureBatchTask**</span><span class="sxs-lookup"><span data-stu-id="48bf3-133">**Get-AzureBatchTask**</span></span>
 - <span data-ttu-id="48bf3-134">`PSCloudTask` の `RunElevated` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-134">Removed the `RunElevated` property on `PSCloudTask`.</span></span> <span data-ttu-id="48bf3-135">`RunElevated` に代わって `UserIdentity` プロパティが追加されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-135">The `UserIdentity` property has been added to replace `RunElevated`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

<span data-ttu-id="48bf3-136">これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="48bf3-136">This additionally impacts the `RunElevated` property on `PSCloudTask`, `PSStartTask`, `PSJobManagerTask`, `PSJobPreparationTask`, and `PSJobReleaseTask`.</span></span>

### <a name="multiple-types"></a><span data-ttu-id="48bf3-137">**複数の型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-137">**Multiple types**</span></span>

- <span data-ttu-id="48bf3-138">`PSExitConditions` の `SchedulingError` プロパティの名前が `PreProcessingError` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-138">Renamed the `SchedulingError` property on `PSExitConditions` to `PreProcessingError`.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a><span data-ttu-id="48bf3-139">**複数の型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-139">**Multiple types**</span></span>

- <span data-ttu-id="48bf3-140">`PSJobPreparationTaskExecutionInformation`、`PSJobReleaseTaskExecutionInformation`、`PSStartTaskInformation`、`PSSubtaskInformation`、`PSTaskExecutionInformation` の `SchedulingError` プロパティの名前が `FailureInformation` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-140">Renamed the `SchedulingError` property on `PSJobPreparationTaskExecutionInformation`, `PSJobReleaseTaskExecutionInformation`, `PSStartTaskInformation`, `PSSubtaskInformation`, and `PSTaskExecutionInformation` to `FailureInformation`.</span></span>
  - <span data-ttu-id="48bf3-141">タスク エラーが発生すると、常に `FailureInformation` が返されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-141">`FailureInformation` is returned any time there is a task failure.</span></span> <span data-ttu-id="48bf3-142">これには、以前のすべてのスケジュール エラー ケースとゼロ以外のタスク終了コード、および新しい出力ファイル機能からのファイル アップロード エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-142">This includes all previous scheduling error cases, as well as nonzero task exit codes, and file upload failures from the new output files feature.</span></span>
  - <span data-ttu-id="48bf3-143">これは以前と同様に構造化されているので、この型を使用するときにコードの変更は不要です。</span><span class="sxs-lookup"><span data-stu-id="48bf3-143">This is structured the same as before, so no code change is needed when using this type.</span></span>

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

<span data-ttu-id="48bf3-144">これは、Get-AzureBatchPool、Get-AzureBatchSubtask、Get-AzureBatchJobPreparationAndReleaseTaskStatus にも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="48bf3-144">This additionally impacts: Get-AzureBatchPool, Get-AzureBatchSubtask, and Get-AzureBatchJobPreparationAndReleaseTaskStatus</span></span>

### <a name="new-azurebatchpool"></a><span data-ttu-id="48bf3-145">**New-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="48bf3-145">**New-AzureBatchPool**</span></span>
 - <span data-ttu-id="48bf3-146">`TargetDedicated` が削除され、`TargetDedicatedComputeNodes` および `TargetLowPriorityComputeNodes` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-146">Removed `TargetDedicated` and replaced it with `TargetDedicatedComputeNodes` and `TargetLowPriorityComputeNodes`.</span></span>
 - <span data-ttu-id="48bf3-147">`TargetDedicatedComputeNodes` には、エイリアス `TargetDedicated` があります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-147">`TargetDedicatedComputeNodes` has an alias `TargetDedicated`.</span></span>

```powershell
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

<span data-ttu-id="48bf3-148">これは、Start-AzureBatchPoolResize にも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="48bf3-148">This also impacts: Start-AzureBatchPoolResize</span></span>

### <a name="get-azurebatchpool"></a><span data-ttu-id="48bf3-149">**Get-AzureBatchPool**</span><span class="sxs-lookup"><span data-stu-id="48bf3-149">**Get-AzureBatchPool**</span></span>
 - <span data-ttu-id="48bf3-150">`PSCloudPool` の `TargetDedicated` プロパティおよび `CurrentDedicated` プロパティの名前が、`TargetDedicatedComputeNodes`、`CurrentDedicatedComputeNodes` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-150">Renamed the `TargetDedicated` and `CurrentDedicated` properties on `PSCloudPool` to `TargetDedicatedComputeNodes` and `CurrentDedicatedComputeNodes`.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicated
$pool.CurrentDedicated

# New
$pool = Get-AzureBatchPool [parameters]
$pool.TargetDedicatedComputeNodes
$pool.CurrentDedicatedComputeNodes
```

### <a name="type-pscloudpool"></a><span data-ttu-id="48bf3-151">**PSCloudPool 型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-151">**Type PSCloudPool**</span></span>

- <span data-ttu-id="48bf3-152">`PSCloudPool` の `ResizeError` の名前が `ResizeErrors` に変更され、コレクションになりました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-152">Renamed `ResizeError` to `ResizeErrors` on `PSCloudPool`, and it is now a collection.</span></span>

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a><span data-ttu-id="48bf3-153">**New-AzureBatchJob**</span><span class="sxs-lookup"><span data-stu-id="48bf3-153">**New-AzureBatchJob**</span></span>
- <span data-ttu-id="48bf3-154">`PSPoolSpecification` の `TargetDedicated` プロパティの名前が `TargetDedicatedComputeNodes` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-154">Renamed the `TargetDedicated` property on `PSPoolSpecification` to `TargetDedicatedComputeNodes`.</span></span>

```powershell
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

### <a name="get-azurebatchnodefile"></a><span data-ttu-id="48bf3-155">**Get-AzureBatchNodeFile**</span><span class="sxs-lookup"><span data-stu-id="48bf3-155">**Get-AzureBatchNodeFile**</span></span>
 - <span data-ttu-id="48bf3-156">`Name` が削除され、`Path` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-156">Removed `Name` and replaced it with `Path`.</span></span>
 - <span data-ttu-id="48bf3-157">`Path` には、エイリアス `Name` があります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-157">`Path` has an alias `Name`.</span></span>

```powershell
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

<span data-ttu-id="48bf3-158">これは、Get-AzureBatchNodeFileContent と Remove-AzureBatchNodeFile にも影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="48bf3-158">This also impacts: Get-AzureBatchNodeFileContent, Remove-AzureBatchNodeFile</span></span>

### <a name="type-psnodefile"></a><span data-ttu-id="48bf3-159">**PSNodeFile** 型</span><span class="sxs-lookup"><span data-stu-id="48bf3-159">Type **PSNodeFile**</span></span>

 - <span data-ttu-id="48bf3-160">`PSNodeFile` の `Name` プロパティの名前が `Path` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-160">Renamed the `Name` property on `PSNodeFile` to `Path`.</span></span>

```powershell
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a><span data-ttu-id="48bf3-161">**Get-AzureBatchSubtask**</span><span class="sxs-lookup"><span data-stu-id="48bf3-161">**Get-AzureBatchSubtask**</span></span>
- <span data-ttu-id="48bf3-162">`PSSubtaskInformation` の `PreviousState` プロパティと `State` プロパティが `TaskState` 型ではなくなり、`SubtaskState` 型になりました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-162">The `PreviousState` and `State` properties of `PSSubtaskInformation` are no longer of type `TaskState`, instead they are of type `SubtaskState`.</span></span>
  - <span data-ttu-id="48bf3-163">`TaskState` とは異なり、`SubtaskState` はサブタスクを `Active` 状態にすることができないため、この型には `Active` 値はありません。</span><span class="sxs-lookup"><span data-stu-id="48bf3-163">Unlike `TaskState`, `SubtaskState` has no `Active` value, since it is not possible for subtasks to be in an `Active` state.</span></span>

```powershell
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="48bf3-164">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-164">Breaking changes to Compute cmdlets</span></span>

### <a name="set-azurermvmaccessextension"></a><span data-ttu-id="48bf3-165">**Set-AzureRmVMAccessExtension**</span><span class="sxs-lookup"><span data-stu-id="48bf3-165">**Set-AzureRmVMAccessExtension**</span></span>
- <span data-ttu-id="48bf3-166">"UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-166">Parameters "UserName" and "Password" are being replaced in favor of a PSCredential</span></span>

```powershell
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="48bf3-167">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-167">Breaking changes to EventHub cmdlets</span></span>

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-168">**New-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-169">"New-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-169">The 'New-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-170">"New-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-170">Please use the 'New-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-171">**Get-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-172">"Get-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-172">The 'Get-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-173">"Get-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-173">Please use the 'Get-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-174">**Set-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-175">"Set-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-175">The 'Set-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-176">"Set-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-176">Please use the 'Set-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-177">**Remove-AzureRmEventHubNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-178">"Remove-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-178">The 'Remove-AzureRmEventHubNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-179">"Remove-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-179">Please use the 'Remove-AzureRmEventHubAuthorizationRule' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespacekey"></a><span data-ttu-id="48bf3-180">**New-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-180">**New-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="48bf3-181">"New-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-181">The 'New-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-182">"New-AzureRmEventHubKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-182">Please use the 'New-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="get-azurermeventhubnamespacekey"></a><span data-ttu-id="48bf3-183">**Get-AzureRmEventHubNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-183">**Get-AzureRmEventHubNamespaceKey**</span></span>
- <span data-ttu-id="48bf3-184">"Get-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-184">The 'Get-AzureRmEventHubNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-185">"Get-AzureRmEventHubKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-185">Please use the 'Get-AzureRmEventHubKey' cmdlet</span></span>
    
### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="48bf3-186">**New-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="48bf3-186">**New-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="48bf3-187">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-187">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property  
$namespace = New-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="48bf3-188">**Get-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="48bf3-188">**Get-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="48bf3-189">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-189">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Get-AzureRmEventHubNamespace <parameters>
```
    
### <a name="set-azurermeventhubnamespace"></a><span data-ttu-id="48bf3-190">**Set-AzureRmEventHubNamespace**</span><span class="sxs-lookup"><span data-stu-id="48bf3-190">**Set-AzureRmEventHubNamespace**</span></span>
- <span data-ttu-id="48bf3-191">NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-191">The property 'Status' and 'Enabled' from the NamespceAttributes will be removed.</span></span> 

```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Set-AzureRmEventHubNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Status and Enabled property    
$namespace = Set-AzureRmEventHubNamespace <parameters>
``` 
  
### <a name="new-azurermeventhubconsumergroup"></a><span data-ttu-id="48bf3-192">**New-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="48bf3-192">**New-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="48bf3-193">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-193">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a><span data-ttu-id="48bf3-194">**Set-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="48bf3-194">**Set-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="48bf3-195">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-195">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a><span data-ttu-id="48bf3-196">**Get-AzureRmEventHubConsumerGroup**</span><span class="sxs-lookup"><span data-stu-id="48bf3-196">**Get-AzureRmEventHubConsumerGroup**</span></span>
- <span data-ttu-id="48bf3-197">ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-197">The property 'EventHubPath' from the ConsumerGroupAttributes will be removed.</span></span>

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="48bf3-198">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-198">Breaking changes to Insights cmdlets</span></span>

### <a name="add-azurermlogalertrule"></a><span data-ttu-id="48bf3-199">**Add-AzureRMLogAlertRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-199">**Add-AzureRMLogAlertRule**</span></span>
- <span data-ttu-id="48bf3-200">**Add-AzureRMLogAlertRule** コマンドレットは使用されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-200">The **Add-AzureRMLogAlertRule** cmdlet has been deprecated</span></span>
- <span data-ttu-id="48bf3-201">10 月 1 日以降、この機能はアクティビティ ログ アラートに移行するため、このコマンドレットを使用しても効果はなくなります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-201">After October 1st using this cmdlet will no longer have any effect as this functionality is being transitioned to Activity Log Alerts.</span></span> <span data-ttu-id="48bf3-202">詳細については、https://aka.ms/migratemealerts を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-202">Please see https://aka.ms/migratemealerts for more information.</span></span>

### <a name="get-azurermusage"></a><span data-ttu-id="48bf3-203">**Get-AzureRMUsage**</span><span class="sxs-lookup"><span data-stu-id="48bf3-203">**Get-AzureRMUsage**</span></span>
- <span data-ttu-id="48bf3-204">**Get-AzureRMUsage** コマンドレットは使用されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-204">The **Get-AzureRMUsage** cmdlet has been deprecated</span></span>

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a><span data-ttu-id="48bf3-205">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span><span class="sxs-lookup"><span data-stu-id="48bf3-205">**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**</span></span>
- <span data-ttu-id="48bf3-206">出力の変更: (これらのコマンドレットから返される) EventData オブジェクトの EventChannels フィールドは、定数値 (Admin,Operation) を返すようになったため、使用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-206">Output change: The field EventChannels from the EventData object (returned by these cmdlets) is being deprecated since it now returns a constant value (Admin,Operation.)</span></span>

### <a name="get-azurermalertrule"></a><span data-ttu-id="48bf3-207">**Get-AzureRmAlertRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-207">**Get-AzureRmAlertRule**</span></span>
- <span data-ttu-id="48bf3-208">出力の変更: ユーザー エクスペリエンスを向上させるために、このコマンドレットの出力はフラット化されます (プロパティ フィールドが排除されます)。</span><span class="sxs-lookup"><span data-stu-id="48bf3-208">Output change: The output of this cmdlet will be flattened, i.e. elimination of the properties field, to improve the user experience.</span></span>

```powershell
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

### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="48bf3-209">**Get-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="48bf3-209">**Get-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="48bf3-210">出力の変更: AutoscaleSettingResourceName フィールドは Name フィールドと常に等しいため、使用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="48bf3-210">Output change: The AutoscaleSettingResourceName field will be deprecated since it always equals the Name field.</span></span>

```powershell
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

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a><span data-ttu-id="48bf3-211">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="48bf3-211">**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**</span></span>
- <span data-ttu-id="48bf3-212">出力の変更: 要求 ID と状態コードを含む単一のオブジェクトを返すために出力の型が変更されます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-212">Output change: The type of the output will change to return a single object containing the request Id and the status code.</span></span>

```powershell
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

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="48bf3-213">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-213">Breaking changes to Network cmdlets</span></span>

### <a name="add-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="48bf3-214">**Add-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="48bf3-214">**Add-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="48bf3-215">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-215">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="48bf3-216">**New-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="48bf3-216">**New-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="48bf3-217">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-217">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a><span data-ttu-id="48bf3-218">**Set-AzureRmApplicationGatewaySslCertificate**</span><span class="sxs-lookup"><span data-stu-id="48bf3-218">**Set-AzureRmApplicationGatewaySslCertificate**</span></span>
- <span data-ttu-id="48bf3-219">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-219">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a><span data-ttu-id="48bf3-220">Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-220">Breaking changes to Resources cmdlets</span></span>

### <a name="new-azurermadappcredential"></a><span data-ttu-id="48bf3-221">**New-AzureRmADAppCredential**</span><span class="sxs-lookup"><span data-stu-id="48bf3-221">**New-AzureRmADAppCredential**</span></span>
- <span data-ttu-id="48bf3-222">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-222">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a><span data-ttu-id="48bf3-223">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="48bf3-223">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="48bf3-224">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-224">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a><span data-ttu-id="48bf3-225">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="48bf3-225">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="48bf3-226">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-226">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a><span data-ttu-id="48bf3-227">**New-AzureRmADSpCredential**</span><span class="sxs-lookup"><span data-stu-id="48bf3-227">**New-AzureRmADSpCredential**</span></span>
- <span data-ttu-id="48bf3-228">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-228">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a><span data-ttu-id="48bf3-229">**New-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-229">**New-AzureRmADUser**</span></span>
- <span data-ttu-id="48bf3-230">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-230">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a><span data-ttu-id="48bf3-231">**Set-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="48bf3-231">**Set-AzureRmADUser**</span></span>
- <span data-ttu-id="48bf3-232">"Password" パラメーターが SecureString に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="48bf3-232">Parameter "Password" being replaced in favor of a SecureString</span></span>

```powershell
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="48bf3-233">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="48bf3-233">Breaking changes to ServiceBus cmdlets</span></span>

### <a name="get-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="48bf3-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-234">**Get-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-235">"Get-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-235">The 'Get-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-236">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-236">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>    

### <a name="get-azurermservicebustopickey"></a><span data-ttu-id="48bf3-237">**Get-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-237">**Get-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="48bf3-238">"Get-AzureRmServiceBusTopicKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-238">The 'Get-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-239">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-239">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="48bf3-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-240">**New-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-241">"New-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-241">The 'New-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-242">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-242">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebustopickey"></a><span data-ttu-id="48bf3-243">**New-AzureRmServiceBusTopicKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-243">**New-AzureRmServiceBusTopicKey**</span></span>
- <span data-ttu-id="48bf3-244">"New-AzureRmServiceBusTopicKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-244">The 'New-AzureRmServiceBusTopicKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-245">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-245">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="48bf3-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-246">**Remove-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-247">"Remove-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-247">The 'Remove-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-248">"Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-248">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebustopicauthorizationrule"></a><span data-ttu-id="48bf3-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-249">**Set-AzureRmServiceBusTopicAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-250">"Set-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-250">The 'Set-AzureRmServiceBusTopicAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-251">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-251">Please use the 'Set-AzureRmServiceBusAuthorizationRule'cmdlet.</span></span>

### <a name="new-azurermservicebusnamespacekey"></a><span data-ttu-id="48bf3-252">**New-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-252">**New-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="48bf3-253">"New-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-253">The 'New-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-254">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-254">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="get-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="48bf3-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-255">**Get-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-256">"Get-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-256">The 'Get-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-257">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-257">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusqueuekey"></a><span data-ttu-id="48bf3-258">**Get-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-258">**Get-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="48bf3-259">"Get-AzureRmServiceBusQueueKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-259">The 'Get-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-260">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-260">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="48bf3-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-261">**New-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-262">"New-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-262">The 'New-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-263">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-263">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="new-azurermservicebusqueuekey"></a><span data-ttu-id="48bf3-264">**New-AzureRmServiceBusQueueKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-264">**New-AzureRmServiceBusQueueKey**</span></span>
- <span data-ttu-id="48bf3-265">"New-AzureRmServiceBusQueueKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-265">The 'New-AzureRmServiceBusQueueKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-266">"New-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-266">Please use the 'New-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="remove-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="48bf3-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-267">**Remove-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-268">"Remove-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-268">The 'Remove-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-269">"GRemove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-269">Please use the 'GRemove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusqueueauthorizationrule"></a><span data-ttu-id="48bf3-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-270">**Set-AzureRmServiceBusQueueAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-271">"Set-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-271">The 'Set-AzureRmServiceBusQueueAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-272">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-272">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-273">**Get-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-274">"Get-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-274">The 'Get-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-275">"Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-275">Please use the 'Get-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="get-azurermservicebusnamespacekey"></a><span data-ttu-id="48bf3-276">**Get-AzureRmServiceBusNamespaceKey**</span><span class="sxs-lookup"><span data-stu-id="48bf3-276">**Get-AzureRmServiceBusNamespaceKey**</span></span>
- <span data-ttu-id="48bf3-277">"Get-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-277">The 'Get-AzureRmServiceBusNamespaceKey' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-278">"Get-AzureRmServiceBusKey" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-278">Please use the 'Get-AzureRmServiceBusKey' cmdlet.</span></span>

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-279">**New-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-280">"New-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-280">The 'New-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-281">"New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-281">Please use the 'New-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-282">**Remove-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-283">"Remove-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-283">The 'Remove-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-284">"Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-284">Please use the 'Remove-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a><span data-ttu-id="48bf3-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span><span class="sxs-lookup"><span data-stu-id="48bf3-285">**Set-AzureRmServiceBusNamespaceAuthorizationRule**</span></span>
- <span data-ttu-id="48bf3-286">"Set-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-286">The 'Set-AzureRmServiceBusNamespaceAuthorizationRule' cmdlet has been removed.</span></span> <span data-ttu-id="48bf3-287">"Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。</span><span class="sxs-lookup"><span data-stu-id="48bf3-287">Please use the 'Set-AzureRmServiceBusAuthorizationRule' cmdlet.</span></span>

### <a name="type-namespaceattributes"></a><span data-ttu-id="48bf3-288">**NamespaceAttributes 型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-288">**Type NamespaceAttributes**</span></span>
- <span data-ttu-id="48bf3-289">次のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="48bf3-289">The following properties have been removed</span></span>
    - <span data-ttu-id="48bf3-290">有効</span><span class="sxs-lookup"><span data-stu-id="48bf3-290">Enabled</span></span>
    - <span data-ttu-id="48bf3-291">状態</span><span class="sxs-lookup"><span data-stu-id="48bf3-291">Status</span></span>
   
```powershell
# Old
# The $namespace has Status and Enabled property 
$namespace = Get-AzureRmServiceBusNamespace <parameters>
$namespace.Status
$namespace.Enabled

# New
# The call remains the same, but the returned values NameSpace object will not have the Enabled and Status properties    
$namespace = Get-AzureRmServiceBusNamespace <parameters>
```

### <a name="type-queueattribute"></a><span data-ttu-id="48bf3-292">**QueueAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-292">**Type QueueAttribute**</span></span>
- <span data-ttu-id="48bf3-293">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="48bf3-293">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="48bf3-294">EnableBatchedOperations</span><span class="sxs-lookup"><span data-stu-id="48bf3-294">EnableBatchedOperations</span></span>
    - <span data-ttu-id="48bf3-295">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="48bf3-295">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="48bf3-296">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="48bf3-296">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="48bf3-297">SupportOrdering</span><span class="sxs-lookup"><span data-stu-id="48bf3-297">SupportOrdering</span></span>

```powershell
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
   
### <a name="type-topicattribute"></a><span data-ttu-id="48bf3-298">**TopicAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-298">**Type TopicAttribute**</span></span>
- <span data-ttu-id="48bf3-299">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="48bf3-299">The following properties are marked as obsolete:</span></span>
    - <span data-ttu-id="48bf3-300">場所</span><span class="sxs-lookup"><span data-stu-id="48bf3-300">Location</span></span>
    - <span data-ttu-id="48bf3-301">IsExpress</span><span class="sxs-lookup"><span data-stu-id="48bf3-301">IsExpress</span></span>
    - <span data-ttu-id="48bf3-302">IsAnonymousAccessible</span><span class="sxs-lookup"><span data-stu-id="48bf3-302">IsAnonymousAccessible</span></span>
    - <span data-ttu-id="48bf3-303">FilteringMessagesBeforePublishing</span><span class="sxs-lookup"><span data-stu-id="48bf3-303">FilteringMessagesBeforePublishing</span></span>
    - <span data-ttu-id="48bf3-304">EnableSubscriptionPartitioning</span><span class="sxs-lookup"><span data-stu-id="48bf3-304">EnableSubscriptionPartitioning</span></span>
    - <span data-ttu-id="48bf3-305">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="48bf3-305">EntityAvailabilityStatus</span></span>

```powershell
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
   
### <a name="type-subscriptionattribute"></a><span data-ttu-id="48bf3-306">**SubscriptionAttribute 型**</span><span class="sxs-lookup"><span data-stu-id="48bf3-306">**Type SubscriptionAttribute**</span></span>
- <span data-ttu-id="48bf3-307">次のプロパティは古い形式としてマークされています。</span><span class="sxs-lookup"><span data-stu-id="48bf3-307">The following properties are marked as obsolete</span></span>
    - <span data-ttu-id="48bf3-308">DeadLetteringOnFilterEvaluationExceptions</span><span class="sxs-lookup"><span data-stu-id="48bf3-308">DeadLetteringOnFilterEvaluationExceptions</span></span>
    - <span data-ttu-id="48bf3-309">EntityAvailabilityStatus</span><span class="sxs-lookup"><span data-stu-id="48bf3-309">EntityAvailabilityStatus</span></span>
    - <span data-ttu-id="48bf3-310">IsReadOnly</span><span class="sxs-lookup"><span data-stu-id="48bf3-310">IsReadOnly</span></span>
    - <span data-ttu-id="48bf3-311">場所</span><span class="sxs-lookup"><span data-stu-id="48bf3-311">Location</span></span>
   
```powershell
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
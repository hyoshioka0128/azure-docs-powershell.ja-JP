# <a name="breaking-changes-for-microsoft-azure-powershell-500"></a>Microsoft Azure PowerShell 5.0.0 の重大な変更

このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。 各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。 詳細なコンテキストについては、各変更に関する pull request を参照してください。

## <a name="table-of-contents"></a>目次

- [ApiManagement コマンドレットの重大な変更](#breaking-changes-to-apimanagement-cmdlets)
- [Batch コマンドレットの重大な変更](#breaking-changes-to-batch-cmdlets)
- [Compute コマンドレットの重大な変更](#breaking-changes-to-compute-cmdlets)
- [EventHub コマンドレットの重大な変更](#breaking-changes-to-eventhub-cmdlets)
- [Insights コマンドレットの重大な変更](#breaking-changes-to-insights-cmdlets)
- [Network コマンドレットの重大な変更](#breaking-changes-to-network-cmdlets)
- [Resources コマンドレットの重大な変更](#breaking-changes-to-resources-cmdlets)
- [ServiceBus コマンドレットの重大な変更](#breaking-changes-to-servicebus-cmdlets)

## <a name="breaking-changes-to-apimanagement-cmdlets"></a>ApiManagement コマンドレットの重大な変更

### <a name="new-azurermapimanagementbackendproxy"></a>**New-AzureRmApiManagementBackendProxy**
- "UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。

```powershell
# Old
New-AzureRmApiManagementBackendProxy [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
New-AzureRmApiManagementBackendProxy [other required parameters] -Credential $PSCredentialVariable
```

### <a name="new-azurermapimanagementuser"></a>**New-AzureRmApiManagementUser**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapimanagementuser"></a>**Set-AzureRmApiManagementUser**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
Set-AzureRmApiManagementUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApiManagementUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-batch-cmdlets"></a>Batch コマンドレットの重大な変更

### <a name="new-azurebatchcertificate"></a>**New-AzureBatchCertificate**
- `Password` パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureBatchCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureBatchCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchcomputenodeuser"></a>**New-AzureBatchComputeNodeUser**
- `Password` パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
New-AzureBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermbatchcomputenodeuser"></a>**Set-AzureRmBatchComputeNodeUser**
- `Password` パラメーターが SecureString に置き換えられます。

```powershell
# Old
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmBatchComputeNodeUser [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurebatchtask"></a>**New-AzureBatchTask**
 - `RunElevated` スイッチが削除され、`UserIdentity` に置き換えられました。

```powershell
# Old
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -RunElevated $TRUE

# New
$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
New-AzureBatchTask -Id $taskId1 -JobId $jobId -CommandLine "cmd /c echo hello" -UserIdentity $userIdentity
```

これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。

### <a name="psmultiinstancesettings"></a>**PSMultiInstanceSettings**

- `PSMultiInstanceSettings` コンストラクターが `numberOfInstances` 必須パラメーターを受け取らなくなりました。代わりに、`coordinationCommandLine` 必須パラメーターを受け取ります。

```powershell
# Old
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @(2)
$settings.CoordinationCommandLine = "cmd /c echo hello"
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings

# New
$settings = New-Object Microsoft.Azure.Commands.Batch.Models.PSMultiInstanceSettings -ArgumentList @("cmd /c echo hello", 2)
New-AzureBatchTask [other parameters] -MultiInstanceSettings $settings
```

### <a name="get-azurebatchtask"></a>**Get-AzureBatchTask**
 - `PSCloudTask` の `RunElevated` プロパティが削除されました。 `RunElevated` に代わって `UserIdentity` プロパティが追加されました。

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.RunElevated

# New
$task = Get-AzureBatchTask [parameters]
$task.UserIdentity.AutoUser.ElevationLevel
```

これは、`PSCloudTask`、`PSStartTask`、`PSJobManagerTask`、`PSJobPreparationTask`、`PSJobReleaseTask` の `RunElevated` プロパティにも影響を及ぼします。

### <a name="multiple-types"></a>**複数の型**

- `PSExitConditions` の `SchedulingError` プロパティの名前が `PreProcessingError` に変更されました。

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExitConditions.PreProcessingError
```

### <a name="multiple-types"></a>**複数の型**

- `PSJobPreparationTaskExecutionInformation`、`PSJobReleaseTaskExecutionInformation`、`PSStartTaskInformation`、`PSSubtaskInformation`、`PSTaskExecutionInformation` の `SchedulingError` プロパティの名前が `FailureInformation` に変更されました。
  - タスク エラーが発生すると、常に `FailureInformation` が返されます。 これには、以前のすべてのスケジュール エラー ケースとゼロ以外のタスク終了コード、および新しい出力ファイル機能からのファイル アップロード エラーが含まれます。
  - これは以前と同様に構造化されているので、この型を使用するときにコードの変更は不要です。

```powershell
# Old
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.SchedulingError

# New
$task = Get-AzureBatchTask [parameters]
$task.ExecutionInformation.FailureInformation
```

これは、Get-AzureBatchPool、Get-AzureBatchSubtask、Get-AzureBatchJobPreparationAndReleaseTaskStatus にも影響を及ぼします。

### <a name="new-azurebatchpool"></a>**New-AzureBatchPool**
 - `TargetDedicated` が削除され、`TargetDedicatedComputeNodes` および `TargetLowPriorityComputeNodes` に置き換えられました。
 - `TargetDedicatedComputeNodes` には、エイリアス `TargetDedicated` があります。

```powershell
# Old
New-AzureBatchPool [other parameters] [-TargetDedicated <Int32>]

# New
New-AzureBatchPool [other parameters] [-TargetDedicatedComputeNodes <Int32>] [-TargetLowPriorityComputeNodes <Int32>]
```

これは、Start-AzureBatchPoolResize にも影響を及ぼします。

### <a name="get-azurebatchpool"></a>**Get-AzureBatchPool**
 - `PSCloudPool` の `TargetDedicated` プロパティおよび `CurrentDedicated` プロパティの名前が、`TargetDedicatedComputeNodes`、`CurrentDedicatedComputeNodes` にそれぞれ変更されました。

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

### <a name="type-pscloudpool"></a>**PSCloudPool 型**

- `PSCloudPool` の `ResizeError` の名前が `ResizeErrors` に変更され、コレクションになりました。

```powershell
# Old
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeError

# New
$pool = Get-AzureBatchPool [parameters]
$pool.ResizeErrors[0]
```

### <a name="new-azurebatchjob"></a>**New-AzureBatchJob**
- `PSPoolSpecification` の `TargetDedicated` プロパティの名前が `TargetDedicatedComputeNodes` に変更されました。

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

### <a name="get-azurebatchnodefile"></a>**Get-AzureBatchNodeFile**
 - `Name` が削除され、`Path` に置き換えられました。
 - `Path` には、エイリアス `Name` があります。

```powershell
# Old
Get-AzureBatchNodeFile [other parameters] [[-Name] <String>]

# New
Get-AzureBatchNodeFile [other parameters] [[-Path] <String>]
```

これは、Get-AzureBatchNodeFileContent と Remove-AzureBatchNodeFile にも影響を及ぼします。

### <a name="type-psnodefile"></a>**PSNodeFile** 型

 - `PSNodeFile` の `Name` プロパティの名前が `Path` に変更されました。

```powershell
# Old
$file = Get-AzureBatchNodeFile [parameters]
$file.Name

# New
$file = Get-AzureBatchNodeFile [parameters]
$file.Path
```

### <a name="get-azurebatchsubtask"></a>**Get-AzureBatchSubtask**
- `PSSubtaskInformation` の `PreviousState` プロパティと `State` プロパティが `TaskState` 型ではなくなり、`SubtaskState` 型になりました。
  - `TaskState` とは異なり、`SubtaskState` はサブタスクを `Active` 状態にすることができないため、この型には `Active` 値はありません。

```powershell
# Old
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.TaskState.Running) { }

# New
$subtask = Get-AzureBatchSubtask [parameters]
if ($subtask.State -eq Microsoft.Azure.Batch.Common.SubtaskState.Running) { }
```

## <a name="breaking-changes-to-compute-cmdlets"></a>Compute コマンドレットの重大な変更

### <a name="set-azurermvmaccessextension"></a>**Set-AzureRmVMAccessExtension**
- "UserName" パラメーターと "Password" パラメーターが PSCredential に置き換えられます。

```powershell
# Old
Set-AzureRmVMAccessExtension [other required parameters] -UserName "plain-text string" -Password "plain-text string"

# New
Set-AzureRmVMAccessExtension [other required parameters] -Credential $PSCredential
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a>EventHub コマンドレットの重大な変更

### <a name="new-azurermeventhubnamespaceauthorizationrule"></a>**New-AzureRmEventHubNamespaceAuthorizationRule**
- "New-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。 "New-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。
    
### <a name="get-azurermeventhubnamespaceauthorizationrule"></a>**Get-AzureRmEventHubNamespaceAuthorizationRule**
- "Get-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。 "Get-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。
    
### <a name="set-azurermeventhubnamespaceauthorizationrule"></a>**Set-AzureRmEventHubNamespaceAuthorizationRule**
- "Set-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。 "Set-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。
    
### <a name="remove-azurermeventhubnamespaceauthorizationrule"></a>**Remove-AzureRmEventHubNamespaceAuthorizationRule**
- "Remove-AzureRmEventHubNamespaceAuthorizationRule" コマンドレットが削除されました。 "Remove-AzureRmEventHubAuthorizationRule" コマンドレットを使用してください。
    
### <a name="new-azurermeventhubnamespacekey"></a>**New-AzureRmEventHubNamespaceKey**
- "New-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。 "New-AzureRmEventHubKey" コマンドレットを使用してください。
    
### <a name="get-azurermeventhubnamespacekey"></a>**Get-AzureRmEventHubNamespaceKey**
- "Get-AzureRmEventHubNamespaceKey" コマンドレットが削除されました。 "Get-AzureRmEventHubKey" コマンドレットを使用してください。
    
### <a name="new-azurermeventhubnamespace"></a>**New-AzureRmEventHubNamespace**
- NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。 

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
    
### <a name="get-azurermeventhubnamespace"></a>**Get-AzureRmEventHubNamespace**
- NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。 

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
    
### <a name="set-azurermeventhubnamespace"></a>**Set-AzureRmEventHubNamespace**
- NamespceAttributes の "Status" プロパティと "Enabled" プロパティが削除されます。 

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
  
### <a name="new-azurermeventhubconsumergroup"></a>**New-AzureRmEventHubConsumerGroup**
- ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = New-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="set-azurermeventhubconsumergroup"></a>**Set-AzureRmEventHubConsumerGroup**
- ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Set-AzureRmEventHubConsumerGroup <parameters>
```
    
### <a name="get-azurermeventhubconsumergroup"></a>**Get-AzureRmEventHubConsumerGroup**
- ConsumerGroupAttributes の "EventHubPath" プロパティが削除されます。

```powershell
# Old
# The $consumergroup has EventHubPath property 
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
$consumergroup.EventHubPath

# New
# The call remains the same, but the returned values ConsumerGroup object will not have the EventHubPath property    
$consumergroup = Get-AzureRmEventHubConsumerGroup <parameters>
```

## <a name="breaking-changes-to-insights-cmdlets"></a>Insights コマンドレットの重大な変更

### <a name="add-azurermlogalertrule"></a>**Add-AzureRMLogAlertRule**
- 
  **Add-AzureRMLogAlertRule** コマンドレットは非推奨となりました。
- 10 月 1 日以降、この機能はアクティビティ ログ アラートに移行するため、このコマンドレットを使用しても効果はなくなります。 詳細については、 https://aka.ms/migratemealerts を参照してください。

### <a name="get-azurermusage"></a>**Get-AzureRMUsage**
- 
  **Get-AzureRMUsage** コマンドレットは非推奨となりました。

### <a name="get-azurermalerthistory--get-azurermautoscalehistory--get-azurermlogs"></a>**Get-AzureRmAlertHistory** / **Get-AzureRmAutoscaleHistory** / **Get-AzureRmLogs**
- 出力の変更: (これらのコマンドレットから返される) EventData オブジェクトの EventChannels フィールドは、定数値 (Admin,Operation) を返すようになったため、非推奨となります。

### <a name="get-azurermalertrule"></a>**Get-AzureRmAlertRule**
- 出力の変更: ユーザー エクスペリエンスを向上させるために、このコマンドレットの出力はフラット化されます (プロパティ フィールドが排除されます)。

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

### <a name="get-azurermautoscalesetting"></a>**Get-AzureRmAutoscaleSetting**
- 出力の変更: AutoscaleSettingResourceName フィールドは Name フィールドと常に等しいため、非推奨となります。

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

### <a name="remove-azurermalertrule--remove-azurermlogprofile"></a>**Remove-AzureRmAlertRule** / **Remove-AzureRmLogProfile**
- 出力の変更: 要求 ID と状態コードを含む単一のオブジェクトを返すために出力の型が変更されます。

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

## <a name="breaking-changes-to-network-cmdlets"></a>Network コマンドレットの重大な変更

### <a name="add-azurermapplicationgatewaysslcertificate"></a>**Add-AzureRmApplicationGatewaySslCertificate**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Add-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermapplicationgatewaysslcertificate"></a>**New-AzureRmApplicationGatewaySslCertificate**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
New-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermapplicationgatewaysslcertificate"></a>**Set-AzureRmApplicationGatewaySslCertificate**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password "plain-text string"

# New
Set-AzureRmApplicationGatewaySslCertificate [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-resources-cmdlets"></a>Resources コマンドレットの重大な変更

### <a name="new-azurermadappcredential"></a>**New-AzureRmADAppCredential**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmADAppCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADAppCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadapplication"></a>**New-AzureRmADApplication**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmADApplication [other required parameters] -Password "plain-text string"

# New
New-AzureRmADApplication [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadserviceprincipal"></a>**New-AzureRmADServicePrincipal**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmADServicePrincipal [other required parameters] -Password "plain-text string"

# New
New-AzureRmADServicePrincipal [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermadspcredential"></a>**New-AzureRmADSpCredential**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmADSpCredential [other required parameters] -Password "plain-text string"

# New
New-AzureRmADSpCredential [other required parameters] -Password $SecureStringVariable
```

### <a name="new-azurermaduser"></a>**New-AzureRmADUser**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
New-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
New-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

### <a name="set-azurermaduser"></a>**Set-AzureRmADUser**
- "Password" パラメーターが SecureString に置き換えられます。

```powershell
# Old
Set-AzureRmADUser [other required parameters] -Password "plain-text string"

# New
Set-AzureRmADUser [other required parameters] -Password $SecureStringVariable
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a>ServiceBus コマンドレットの重大な変更

### <a name="get-azurermservicebustopicauthorizationrule"></a>**Get-AzureRmServiceBusTopicAuthorizationRule**
- "Get-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。 "Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。    

### <a name="get-azurermservicebustopickey"></a>**Get-AzureRmServiceBusTopicKey**
- "Get-AzureRmServiceBusTopicKey" コマンドレットが削除されました。 "Get-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="new-azurermservicebustopicauthorizationrule"></a>**New-AzureRmServiceBusTopicAuthorizationRule**
- "New-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。 "New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="new-azurermservicebustopickey"></a>**New-AzureRmServiceBusTopicKey**
- "New-AzureRmServiceBusTopicKey" コマンドレットが削除されました。 "New-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="remove-azurermservicebustopicauthorizationrule"></a>**Remove-AzureRmServiceBusTopicAuthorizationRule**
- "Remove-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。 "Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="set-azurermservicebustopicauthorizationrule"></a>**Set-AzureRmServiceBusTopicAuthorizationRule**
- "Set-AzureRmServiceBusTopicAuthorizationRule" コマンドレットが削除されました。 "Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="new-azurermservicebusnamespacekey"></a>**New-AzureRmServiceBusNamespaceKey**
- "New-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。 "New-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="get-azurermservicebusqueueauthorizationrule"></a>**Get-AzureRmServiceBusQueueAuthorizationRule**
- "Get-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。 "Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="get-azurermservicebusqueuekey"></a>**Get-AzureRmServiceBusQueueKey**
- "Get-AzureRmServiceBusQueueKey" コマンドレットが削除されました。 "Get-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="new-azurermservicebusqueueauthorizationrule"></a>**New-AzureRmServiceBusQueueAuthorizationRule**
- "New-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。 "New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="new-azurermservicebusqueuekey"></a>**New-AzureRmServiceBusQueueKey**
- "New-AzureRmServiceBusQueueKey" コマンドレットが削除されました。 "New-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="remove-azurermservicebusqueueauthorizationrule"></a>**Remove-AzureRmServiceBusQueueAuthorizationRule**
- "Remove-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。 "GRemove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="set-azurermservicebusqueueauthorizationrule"></a>**Set-AzureRmServiceBusQueueAuthorizationRule**
- "Set-AzureRmServiceBusQueueAuthorizationRule" コマンドレットが削除されました。 "Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="get-azurermservicebusnamespaceauthorizationrule"></a>**Get-AzureRmServiceBusNamespaceAuthorizationRule**
- "Get-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。 "Get-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="get-azurermservicebusnamespacekey"></a>**Get-AzureRmServiceBusNamespaceKey**
- "Get-AzureRmServiceBusNamespaceKey" コマンドレットが削除されました。 "Get-AzureRmServiceBusKey" コマンドレットを使用してください。

### <a name="new-azurermservicebusnamespaceauthorizationrule"></a>**New-AzureRmServiceBusNamespaceAuthorizationRule**
- "New-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。 "New-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="remove-azurermservicebusnamespaceauthorizationrule"></a>**Remove-AzureRmServiceBusNamespaceAuthorizationRule**
- "Remove-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。 "Remove-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="set-azurermservicebusnamespaceauthorizationrule"></a>**Set-AzureRmServiceBusNamespaceAuthorizationRule**
- "Set-AzureRmServiceBusNamespaceAuthorizationRule" コマンドレットが削除されました。 "Set-AzureRmServiceBusAuthorizationRule" コマンドレットを使用してください。

### <a name="type-namespaceattributes"></a>**NamespaceAttributes 型**
- 次のプロパティが削除されました。
    - 有効
    - 状態
   
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

### <a name="type-queueattribute"></a>**QueueAttribute 型**
- 次のプロパティは古い形式としてマークされています。
    - EnableBatchedOperations
    - EntityAvailabilityStatus
    - IsAnonymousAccessible
    - SupportOrdering

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
   
### <a name="type-topicattribute"></a>**TopicAttribute 型**
- 次のプロパティは古い形式としてマークされています。
    - 場所
    - IsExpress
    - IsAnonymousAccessible
    - FilteringMessagesBeforePublishing
    - EnableSubscriptionPartitioning
    - EntityAvailabilityStatus

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
   
### <a name="type-subscriptionattribute"></a>**SubscriptionAttribute 型**
- 次のプロパティは古い形式としてマークされています。
    - DeadLetteringOnFilterEvaluationExceptions
    - EntityAvailabilityStatus
    - IsReadOnly
    - 場所
   
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
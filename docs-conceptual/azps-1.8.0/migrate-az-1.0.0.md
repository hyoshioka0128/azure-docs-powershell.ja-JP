---
title: AzureRM から Azure PowerShell Az 1.0.0 へのすべての変更
description: この移行ガイドには、Az バージョン 1 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2019
ms.openlocfilehash: ea7593cf2b753b210ff2955b7bd450030ad83596
ms.sourcegitcommit: f9445d1525eac8c165637e1a80fbc92b1ab005c2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/16/2019
ms.locfileid: "75035831"
---
# <a name="breaking-changes-for-az-100"></a>Az 1.0.0 の破壊的変更

このドキュメントでは、AzureRM 6.x と新しい Az モジュール、バージョン 1.x 以降の間の変更について詳しく説明します。 目次は、スクリプトに影響する可能性のあるモジュール固有の変更など、完全な移行パスのすべての段階で役立ちます。

AzureRM から Az への移行の開始に関する一般的なアドバイスについては、[AzureRM から Az への移行の開始](migrate-from-azurerm-to-az.md)に関するページを参照してください。

## <a name="table-of-contents"></a>目次

- [重大な変更 - 全般](#general-breaking-changes)
  - [コマンドレットの名詞プレフィックスの変更](#cmdlet-noun-prefix-changes)
  - [モジュール名の変更](#module-name-changes)
  - [削除されたモジュール](#removed-modules)
  - [Windows PowerShell 5.1 と .NET 4.7.2](#windows-powershell-51-and-net-472)
  - [PSCredential を使用したユーザー ログインの一時的な削除](#temporary-removal-of-user-login-using-pscredential)
  - [Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用](#default-device-code-login-instead-of-web-browser-prompt)
- [モジュールの破壊的変更](#module-breaking-changes)
  - [Az.ApiManagement (以前の AzureRM.ApiManagement)](#azapimanagement-previously-azurermapimanagement)
  - [Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [Az.CognitiveServices (以前の AzureRM.CognitiveServices)](#azcognitiveservices-previously-azurermcognitiveservices)
  - [Az.Compute (以前の AzureRM.Compute)](#azcompute-previously-azurermcompute)
  - [Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [Az.DataLakeStore (以前の AzureRM.DataLakeStore)](#azdatalakestore-previously-azurermdatalakestore)
  - [Az.KeyVault (以前の AzureRM.KeyVault)](#azkeyvault-previously-azurermkeyvault)
  - [Az.Media (以前の AzureRM.Media)](#azmedia-previously-azurermmedia)
  - [Az.Monitor (以前の AzureRM.Insights)](#azmonitor-previously-azurerminsights)
  - [Az.Network (以前の AzureRM.Network)](#aznetwork-previously-azurermnetwork)
  - [Az.OperationalInsights (以前の AzureRM.OperationalInsights)](#azoperationalinsights-previously-azurermoperationalinsights)
  - [Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [Az.Resources (以前の AzureRM.Resources)](#azresources-previously-azurermresources)
  - [Az.ServiceFabric (以前の AzureRM.ServiceFabric)](#azservicefabric-previously-azurermservicefabric)
  - [Az.Sql (以前の AzureRM.Sql)](#azsql-previously-azurermsql)
  - [Az.Storage (以前の Azure.Storage and AzureRM.Storage)](#azstorage-previously-azurestorage-and-azurermstorage)
  - [Az.Websites (以前の AzureRM.Websites)](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a>重大な変更 - 全般

このセクションでは、Az モジュールの再設計の一部である、一般的な重大な変更について説明します。

### <a name="cmdlet-noun-prefix-changes"></a>コマンドレットの名詞プレフィックスの変更

AzureRM モジュールでは、コマンドレットの名詞プレフィックスとして `AzureRM` または `Azure` が使用されていました。  Az ではコマンドレット名が簡略化され、正規化されています。そのため、すべてのコマンドレットでコマンドレット名詞プレフィックスとして "Az" が使用されます。 例:

```azurepowershell-interactive
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

次のように変更されました。

```azurepowershell-interactive
Get-AzVM
Get-AzKeyVaultSecret
```

これらの新しいコマンドレット名に簡単に移行できるように、Az では [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) と [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias) の 2 つの新しいコマンドレットが導入されています。  `Enable-AzureRmAlias` では、新しい Az コマンドレット名に対応する、AzureRM の古いコマンドレット名のエイリアスが作成されます。 `Enable-AzureRmAlias` で `-Scope` 引数を使用すると、エイリアスを有効にする場所を選択することができます。

たとえば、AzureRM の次のスクリプトがあるとします。

```azurepowershell-interactive
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

`Enable-AzureRmAlias` を使用すると、最小限の変更で実行できます。

```azurepowershell-interactive
#Requires -Modules Az.Storage
Enable-AzureRmAlias -Scope Process
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

`Enable-AzureRmAlias -Scope CurrentUser` を実行すると、現在のユーザーが開くすべての PowerShell セッションでエイリアスが有効になるため、このコマンドレットの実行後は、次のようなスクリプトを変更する必要はありません。

```azurepowershell-interactive
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

エイリアス コマンドレットの使用方法の詳細については、[Enable-AzureRmAlias リファレンス](/powershell/module/az.accounts/enable-azurermalias)を参照してください。

エイリアスを無効にする準備ができたら、`Disable-AzureRmAlias` により作成されたエイリアスが削除されます。 詳細については、[Disable-AzureRmAlias リファレンス](/powershell/module/az.accounts/disable-azurermalias)を参照してください。

> [!IMPORTANT]
> エイリアスを無効にする場合は、必ず、エイリアスが有効になっている_すべて_のスコープに対して無効にしてください。

### <a name="module-name-changes"></a>モジュール名の変更

次のモジュールを除き、モジュール名が `AzureRM.*` から `Az.*` に変更されました。

| AzureRM モジュール | Az モジュール |
|----------------|-----------|
| Azure.Storage | Az.Storage |
| Azure.AnalysisServices | Az.AnalysisServices |
| AzureRM.Profile | Az.Accounts |
| AzureRM.Insights | Az.Monitor |
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |
| AzureRM.Tags | Az.Resources |
| AzureRM.MachineLearningCompute | Az.MachineLearning |
| AzureRM.UsageAggregates | Az.Billing |
| AzureRM.Consumption | Az.Billing |

モジュール名が変更されたので、`#Requires` または `Import-Module` を使用して特定のモジュールを読み込むスクリプトは、新しいモジュールを代わりに使用するように変更する必要があります。 コマンドレットのサフィックスが変更されていないモジュールの場合、これは、モジュール名が変更されていても操作スペースを示すサフィックスは_変更されていない_ことを意味します。

#### <a name="migrating-requires-and-import-module-statements"></a>#Requires ステートメントと Import-Module ステートメントの移行

`#Requires` または `Import-Module` を使用して AzureRM モジュールへの依存関係を宣言しているスクリプトは、新しいモジュール名を使用するように更新する必要があります。 例:

```azurepowershell-interactive
#Requires -Module AzureRM.Compute
```

次のように変更する必要があります。

```azurepowershell-interactive
#Requires -Module Az.Compute
```

`Import-Module` の場合:

```azurepowershell-interactive
Import-Module -Name AzureRM.Compute
```

次のように変更する必要があります。

```azurepowershell-interactive
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a>完全修飾コマンドレットの呼び出しの移行

次のように、モジュール修飾コマンドレットの呼び出しを使用するスクリプトは、

```azurepowershell-interactive
AzureRM.Compute\Get-AzureRmVM
```

新しいモジュール名とコマンドレット名を使用するように変更する必要があります。

```azurepowershell-interactive
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a>モジュール マニフェスト依存関係の移行

モジュール マニフェスト (.psd1) ファイルを使用して AzureRM モジュールへの依存関係を表すモジュールは、`RequiredModules` セクションのモジュール名を更新する必要があります。

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

次のように変更する必要があります。

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a>削除されたモジュール

次のモジュールが削除されました。

- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

これらのサービス用のツールは積極的にサポートされなくなりました。  都合がつき次第、代替サービスに移行することをお勧めします。

### <a name="windows-powershell-51-and-net-472"></a>Windows PowerShell 5.1 と .NET 4.7.2

Windows 用の PowerShell 5.1 で Az を使用するには、.NET Framework 4.7.2 をインストールする必要があります。 PowerShell Core 6.x 以降を使用する場合、.NET Fremework は不要です。

### <a name="temporary-removal-of-user-login-using-pscredential"></a>PSCredential を使用したユーザー ログインの一時的な削除

.NET Standard の認証フローの変更により、PSCredential を使用したユーザー ログインが一時的に削除されます。 この機能は、Windows 用の PowerShell 5.1 の 2019/1/15 リリースで再導入されます。 詳細については、[こちらの GitHub の問題](https://github.com/Azure/azure-powershell/issues/7430)をご覧ください。

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a>Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用

.NET Standard の認証フローの変更により、対話型ログイン時の既定のログイン フローとしてデバイス ログインが使用されます。 Web ブラウザー ベースのログインは、Windows 用の PowerShell 5.1 の 2019/1/15 リリースで既定のログインとして再導入されます。 その時点で、ユーザーは Switch パラメーターを使用してデバイス ログインを選択できるようになります。

## <a name="module-breaking-changes"></a>モジュールの破壊的変更

このセクションでは、個々のモジュールとコマンドレットの特定の重大な変更について説明します。

### <a name="azapimanagement-previously-azurermapimanagement"></a>Az.ApiManagement (以前の AzureRM.ApiManagement)

- 次のコマンドレットが削除されました。
  - New-AzureRmApiManagementHostnameConfiguration
  - Set-AzureRmApiManagementHostnames
  - Update-AzureRmApiManagementDeployment
  - Import-AzureRmApiManagementHostnameCertificate
  - 代わりに、**Set-AzApiManagement** コマンドレットを使用してこれらのプロパティを設定します
- 次のプロパティが削除されました。
  - `PsApiManagementContext` から、`PsApiManagementHostnameConfiguration` 型の `PortalHostnameConfiguration`、`ProxyHostnameConfiguration`、`ManagementHostnameConfiguration`、`ScmHostnameConfiguration` の各プロパティが削除されました。 代わりに、`PsApiManagementCustomHostNameConfiguration` 型の `PortalCustomHostnameConfiguration`、`ProxyCustomHostnameConfiguration`、`ManagementCustomHostnameConfiguration`、`ScmCustomHostnameConfiguration` を使用します。
  - PsApiManagementContext から `StaticIPs` プロパティが削除されました。 このプロパティは、`PublicIPAddresses` と `PrivateIPAddresses` に分割されました。
  - New-AzureApiManagementVirtualNetwork コマンドレットから、必須の `Location` プロパティが削除されました。

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a>Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)

- `Get-AzConsumptionUsageDetail` コマンドレットから、`InvoiceName` パラメーターが削除されました。  スクリプトでは、請求書に他の ID パラメーターを使用する必要があります。

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a>Az.CognitiveServices (以前の AzureRM.CognitiveServices)

- `Get-AzCognitiveServicesAccountSkus` コマンドレットから、`GetSkusWithAccountParamSetName` パラメーター セットが削除されました。  ResourceGroupName とアカウント名を使用するのではなく、アカウントの種類と場所で SKU を取得する必要があります。

### <a name="azcompute-previously-azurermcompute"></a>Az.Compute (以前の AzureRM.Compute)

- `PSVirtualMachine` および `PSVirtualMachineScaleSet` オブジェクトの `Identity` プロパティから `IdentityIds` が削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。
- `PSVirtualMachineScaleSetVM` オブジェクトの `InstanceView` プロパティの型が、`VirtualMachineInstanceView` から `VirtualMachineScaleSetVMInstanceView` に変更されました。
- `UpgradePolicy` プロパティから、`AutoOSUpgradePolicy` および `AutomaticOSUpgrade` プロパティが削除されました。
- `PSSnapshotUpdate` オブジェクトの `Sku` プロパティの型が、`DiskSku` から `SnapshotSku` に変更されました。
- `Add-AzVMDataDisk` コマンドレットから、`VmScaleSetVMParameterSet` が削除されました。スケールセット VM にデータ ディスクを個別に追加することはできなくなりました。

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a>Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)

- `New-AzDataFactoryEncryptValue` コマンドレットで `GatewayName` パラメーターが必須になりました。
- `New-AzDataFactoryGatewayKey` コマンドレットが削除されました。
- `Get-AzDataFactoryV2ActivityRun` コマンドレットから、`LinkedServiceName` パラメーターが削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a>Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)

- 非推奨の `New-AzDataLakeAnalyticsCatalogSecret`、`Remove-AzDataLakeAnalyticsCatalogSecret`、`Set-AzDataLakeAnalyticsCatalogSecret` の各コマンドレットが削除されました。

### <a name="azdatalakestore-previously-azurermdatalakestore"></a>Az.DataLakeStore (以前の AzureRM.DataLakeStore)

- 次のコマンドレットの `Encoding` パラメーターの型が、`FileSystemCmdletProviderEncoding` から `System.Text.Encoding` に変更されました。 この変更により、エンコード値 `String` と `Oem` が削除されます。 以前からの他のエンコード値はすべて残ります。
  - New-AzureRmDataLakeStoreItem
  - Add-AzureRmDataLakeStoreItemContent
  - Get-AzureRmDataLakeStoreItemContent
- `New-AzDataLakeStoreAccount` および `Set-AzDataLakeStoreAccount` コマンドレットから、非推奨の `Tags` プロパティのエイリアスが削除されました。

  次のコマンドレットを使用するスクリプトは
  ```azurepowershell-interactive
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  次のように変更する必要があります。
  ```azurepowershell-interactive
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- `PSDataLakeStoreAccountBasic` オブジェクトから、非推奨の `Identity`、`EncryptionState`、`EncryptionProvisioningState`、`EncryptionConfig`、`FirewallState`、`FirewallRules`、`VirtualNetworkRules`、`TrustedIdProviderState`、`TrustedIdProviders`、`DefaultGroup`、`NewTier`、`CurrentTier`、`FirewallAllowAzureIps` の各プロパティが削除されました。  `Get-AzDataLakeStoreAccount` から返された `PSDatalakeStoreAccount` を使用するスクリプトでは、これらのプロパティを参照しないでください。

### <a name="azkeyvault-previously-azurermkeyvault"></a>Az.KeyVault (以前の AzureRM.KeyVault)

- `PSKeyVaultKeyAttributes`、`PSKeyVaultKeyIdentityItem`、`PSKeyVaultSecretAttributes` の各オブジェクトから、`PurgeDisabled` プロパティが削除されました。スクリプトでは、```PurgeDisabled``` プロパティを参照して処理を決定することはできなくなりました。

### <a name="azmedia-previously-azurermmedia"></a>Az.Media (以前の AzureRM.Media)

- `New-AzMediaService` コマンドレットから、非推奨の `Tags` プロパティのエイリアスが削除されました。次のコマンドレットを使用するスクリプトは
  ```azurepowershell-interactive
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  次のように変更する必要があります。
  ```azurepowershell-interactive
  New-AzMediaService -Tag @{TagName="TagValue"}
  ```

### <a name="azmonitor-previously-azurerminsights"></a>Az.Monitor (以前の AzureRM.Insights)

- 単数形のパラメーター名を優先して、`Set-AzDiagnosticSetting` コマンドレットから複数形のパラメーター名 `Categories` と `Timegrains` が削除されました。次のコマンドレットを使用するスクリプトは
  ```azurepowershell-interactive
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  次のように変更する必要があります。
  ```azurepowershell-interactive
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```

### <a name="aznetwork-previously-azurermnetwork"></a>Az.Network (以前の AzureRM.Network)

- `Get-AzServiceEndpointPolicyDefinition` コマンドレットから、非推奨の `ResourceId` パラメーターが削除されました。
- `PSVirtualNetwork` オブジェクトから、非推奨の `EnableVmProtection` プロパティが削除されました。
- 非推奨の `Set-AzVirtualNetworkGatewayVpnClientConfig` コマンドレットが削除されました。

スクリプトでは、これらのフィールドの値に基づいて処理を決定することはできなくなりました。

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a>Az.OperationalInsights (以前の AzureRM.OperationalInsights)

- `Get-AzOperationalInsightsDataSource` の既定のパラメーター セットが削除され、`ByWorkspaceNameByKind` が既定のパラメーター セットになりました。

  次のコマンドレットを使用してデータ ソースのリストを表示するスクリプトは
  ```azurepowershell-interactive
  Get-AzureRmOperationalInsightsDataSource
  ```

  種類 (Kind) を指定するように変更する必要があります。
  ```azurepowershell-interactive
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a>Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)

- `New/Set-AzRecoveryServicesAsrPolicy` コマンドレットから、`Encryption` パラメーターが削除されました。
- `Restore-AzRecoveryServicesBackupItem` コマンドレットでのマネージド ディスクの復元に `TargetStorageAccountName` パラメーターが必須になりました。
- `Restore-AzRecoveryServicesBackupItem` コマンドレットの `StorageAccountName` および `StorageAccountResourceGroupName` パラメーターが削除されました。
- `Get-AzRecoveryServicesBackupContainer` コマンドレットの `Name` パラメーターが削除されました。

### <a name="azresources-previously-azurermresources"></a>Az.Resources (以前の AzureRM.Resources)

- `New/Set-AzPolicyAssignment` コマンドレットから、`Sku` パラメーターが削除されました。
- `New-AzADServicePrincipal` および `New-AzADSpCredential` コマンドレットから、`Password` パラメーターが削除されました。パスワードは自動的に生成されます。次のようにパスワードを指定しているスクリプトは

  ```azurepowershell-interactive
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  出力からパスワードを取得するように変更する必要があります。

  ```azurepowershell-interactive
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a>Az.ServiceFabric (以前の AzureRM.ServiceFabric)

- コマンドレットの次の戻り値の型が変更されました。
  - `ApplicationHealthPolicy` 型の `ServiceTypeHealthPolicies` プロパティが削除されました。
  - `ClusterUpgradeDeltaHealthPolicy` 型の `ApplicationHealthPolicies` プロパティが削除されました。
  - `ClusterUpgradePolicy` 型の `OverrideUserUpgradePolicy` プロパティが削除されました。
  - これらの変更は、次のコマンドレットに影響します。
    - Add-AzServiceFabricClientCertificate
    - Add-AzServiceFabricClusterCertificate
    - Add-AzServiceFabricNode
    - Add-AzServiceFabricNodeType
    - Get-AzServiceFabricCluster
    - Remove-AzServiceFabricClientCertificate
    - Remove-AzServiceFabricClusterCertificate
    - Remove-AzServiceFabricNode
    - Remove-AzServiceFabricNodeType
    - Remove-AzServiceFabricSetting
    - Set-AzServiceFabricSetting
    - Set-AzServiceFabricUpgradeType
    - Update-AzServiceFabricDurability
    - Update-AzServiceFabricReliability

### <a name="azsql-previously-azurermsql"></a>Az.Sql (以前の AzureRM.Sql)

- `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` コマンドレットから、`State` および `ResourceId` パラメーターが削除されました。
- 非推奨の `Get/Set-AzSqlServerBackupLongTermRetentionVault`、`Get/Start/Stop-AzSqlServerUpgrade`、`Get/Set-AzSqlDatabaseAuditingPolicy`、`Get/Set-AzSqlServerAuditingPolicy`、`Remove-AzSqlDatabaseAuditing`、`Remove-AzSqlServerAuditing` の各コマンドレットが削除されました。
- `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` コマンドレットから、非推奨の `Current` パラメーターが削除されました。
- `Get-AzSqlServerServiceObjective` コマンドレットから、非推奨の `DatabaseName` パラメーターが削除されました。
- `Set-AzSqlDatabaseDataMaskingPolicy` コマンドレットから、非推奨の `PrivilegedLogin` パラメーターが削除されました。

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a>Az.Storage (以前の Azure.Storage and AzureRM.Storage)

- ストレージ アカウント名のみを使用した Oauth ストレージ コンテキストの作成をサポートするために、既定のパラメーター セットが `OAuthParameterSet` に変更されました。
  - 例: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`
- `Get-AzStorageUsage` コマンドレットで `Location` パラメーターが必須になりました。
- Storage API のメソッドで、同期 API 呼び出しの代わりに、タスク ベースの非同期パターン (TAP) が使用されるようになりました。 次の例は、新しい非同期コマンドを示しています。

#### <a name="blob-snapshot"></a>BLOB スナップショット

AzureRM:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

Az:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="share-snapshot"></a>スナップショットの共有

AzureRM:

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```

Az:

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="undelete-soft-deleted-blob"></a>論理的に削除された BLOB の削除の取り消し

AzureRM:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```

Az:

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="set-blob-tier"></a>BLOB 層の設定

AzureRM:

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

Az:

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a>Az.Websites (以前の AzureRM.Websites)

- `PSAppServicePlan`、`PSCertificate`、`PSCloningInfo`、`PSSite` の各オブジェクトから非推奨のプロパティが削除されました。

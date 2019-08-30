---
ms.openlocfilehash: f89d13d6bbedaea29b62287942d8c7a509abe32b
ms.sourcegitcommit: abca342d8687ca638679c049792d0cef6045837d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "70052636"
---
## <a name="260---august-2019"></a><span data-ttu-id="8ede5-101">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-101">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="8ede5-102">全般</span><span class="sxs-lookup"><span data-stu-id="8ede5-102">General</span></span>
* <span data-ttu-id="8ede5-103">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-103">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ede5-104">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-104">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-105">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="8ede5-105">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="8ede5-106">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8ede5-106">Az.Aks</span></span>
* <span data-ttu-id="8ede5-107">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-107">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="8ede5-108">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="8ede5-108">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ede5-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ede5-109">Az.ApiManagement</span></span>
* <span data-ttu-id="8ede5-110">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="8ede5-110">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="8ede5-111">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="8ede5-111">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="8ede5-112">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-112">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="8ede5-113">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="8ede5-113">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="8ede5-114">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-114">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ede5-115">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ede5-115">Az.Batch</span></span>
* <span data-ttu-id="8ede5-116">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-116">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ede5-117">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ede5-117">Az.Cdn</span></span>
* <span data-ttu-id="8ede5-118">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-118">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-119">Az.Compute</span></span>
* <span data-ttu-id="8ede5-120">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-120">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="8ede5-121">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-121">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="8ede5-122">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-122">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="8ede5-123">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-123">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="8ede5-124">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="8ede5-124">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="8ede5-125">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="8ede5-125">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="8ede5-126">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-126">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="8ede5-127">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-127">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-128">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-128">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-129">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-129">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="8ede5-130">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-130">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="8ede5-131">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-131">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="8ede5-132">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-132">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-133">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-133">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-134">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-134">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ede5-135">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-135">Az.EventHub</span></span>
* <span data-ttu-id="8ede5-136">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="8ede5-136">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="8ede5-137">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="8ede5-137">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="8ede5-138">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-138">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="8ede5-139">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="8ede5-139">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="8ede5-140">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8ede5-140">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8ede5-141">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-141">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ede5-142">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-142">Az.Monitor</span></span>
* <span data-ttu-id="8ede5-143">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-143">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-144">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-144">Az.Network</span></span>
* <span data-ttu-id="8ede5-145">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-145">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="8ede5-146">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-146">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="8ede5-147">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-147">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="8ede5-148">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-148">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="8ede5-149">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-149">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="8ede5-150">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-150">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="8ede5-151">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-151">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-152">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-152">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-153">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-153">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="8ede5-154">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-154">Added example</span></span>
    - <span data-ttu-id="8ede5-155">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-155">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="8ede5-156">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-156">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="8ede5-157">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-157">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-158">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-158">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-159">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-159">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-160">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-160">Az.Resources</span></span>
* <span data-ttu-id="8ede5-161">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-161">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="8ede5-162">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-162">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="8ede5-163">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="8ede5-163">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="8ede5-164">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-164">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-165">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-165">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-166">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="8ede5-166">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="8ede5-167">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="8ede5-167">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="8ede5-168">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-168">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="8ede5-169">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-169">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-170">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-170">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="8ede5-171">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="8ede5-171">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="8ede5-172">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="8ede5-172">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="8ede5-173">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-173">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="8ede5-174">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="8ede5-174">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="8ede5-175">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-175">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-176">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-176">Az.Sql</span></span>
* <span data-ttu-id="8ede5-177">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-177">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-178">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-178">Az.Storage</span></span>
* <span data-ttu-id="8ede5-179">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-179">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="8ede5-180">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ede5-180">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="8ede5-181">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ede5-181">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="8ede5-182">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ede5-182">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="8ede5-183">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ede5-183">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="8ede5-184">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ede5-184">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-185">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-185">Az.Websites</span></span>
* <span data-ttu-id="8ede5-186">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-186">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="8ede5-187">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-187">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-188">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-188">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-189">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-189">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8ede5-190">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-190">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8ede5-191">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-191">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="8ede5-192">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-192">Az.Automation</span></span>
* <span data-ttu-id="8ede5-193">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-193">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-194">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-194">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-195">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-195">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-196">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-196">Az.Compute</span></span>
* <span data-ttu-id="8ede5-197">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-197">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8ede5-198">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8ede5-198">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8ede5-199">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-199">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="8ede5-200">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="8ede5-200">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-201">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-202">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-202">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="8ede5-203">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-203">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ede5-204">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-204">Az.EventHub</span></span>
* <span data-ttu-id="8ede5-205">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8ede5-205">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8ede5-206">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-206">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ede5-207">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-207">Az.KeyVault</span></span>
* <span data-ttu-id="8ede5-208">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-208">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ede5-209">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ede5-209">Az.LogicApp</span></span>
* <span data-ttu-id="8ede5-210">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-210">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="8ede5-211">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-211">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="8ede5-212">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-212">Az.ManagedServices</span></span>
* <span data-ttu-id="8ede5-213">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-213">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-214">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-214">Az.Network</span></span>
* <span data-ttu-id="8ede5-215">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-215">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="8ede5-216">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-216">New cmdlets</span></span>
        - <span data-ttu-id="8ede5-217">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ede5-217">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ede5-218">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ede5-218">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ede5-219">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-219">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ede5-220">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-220">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ede5-221">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-221">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ede5-222">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-222">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ede5-223">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="8ede5-223">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="8ede5-224">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ede5-224">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="8ede5-225">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="8ede5-225">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="8ede5-226">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-226">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="8ede5-227">このサブネット内のプライベート エンドポイントでネットワーク ポリシーの適用を有効または無効にすることを示す省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-227">Added optional parameter -PrivateEndpointNetworkPoliciesFlag to indicate that enable or disable apply network policies on pivate endpoint in this subnet.</span></span>
        - <span data-ttu-id="8ede5-228">このサブネット内のプライベート リンク サービスでネットワーク ポリシーの適用を有効または無効にすることを示す省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-228">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag to indicate that enable or disable apply network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="8ede5-229">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="8ede5-229">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="8ede5-230">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-230">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="8ede5-231">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-231">Updated cmdlets</span></span>
        - <span data-ttu-id="8ede5-232">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-232">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ede5-233">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-233">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ede5-234">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-234">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8ede5-235">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-235">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8ede5-236">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-236">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="8ede5-237">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ede5-237">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ede5-238">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-238">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8ede5-239">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-239">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8ede5-240">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-240">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="8ede5-241">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-241">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="8ede5-242">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-242">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="8ede5-243">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-243">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-244">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-244">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-245">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-245">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="8ede5-246">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-246">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-247">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-248">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-248">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8ede5-249">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-249">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="8ede5-250">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-250">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="8ede5-251">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-251">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8ede5-252">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-252">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="8ede5-253">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-253">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8ede5-254">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-254">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="8ede5-255">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-255">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8ede5-256">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-256">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="8ede5-257">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-257">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-258">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-258">Az.Resources</span></span>
- <span data-ttu-id="8ede5-259">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-259">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="8ede5-260">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-260">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-261">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-261">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-262">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8ede5-262">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8ede5-263">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-263">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-264">Az.Sql</span></span>
* <span data-ttu-id="8ede5-265">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-265">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="8ede5-266">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-266">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="8ede5-267">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-267">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-268">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-268">Az.Storage</span></span>
* <span data-ttu-id="8ede5-269">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-269">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ede5-270">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ede5-270">Az.StorageSync</span></span>
* <span data-ttu-id="8ede5-271">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-271">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="8ede5-272">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-272">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-273">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-273">Az.Websites</span></span>
* <span data-ttu-id="8ede5-274">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-274">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="8ede5-275">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-275">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="8ede5-276">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-276">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="8ede5-277">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-277">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-278">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-278">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-279">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-279">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8ede5-280">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-280">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8ede5-281">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-281">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8ede5-282">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8ede5-282">Az.Advisor</span></span>
* <span data-ttu-id="8ede5-283">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-283">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8ede5-284">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-284">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ede5-285">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ede5-285">Az.ApiManagement</span></span>
* <span data-ttu-id="8ede5-286">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8ede5-286">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8ede5-287">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8ede5-287">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8ede5-288">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-288">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8ede5-289">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-289">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8ede5-290">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-290">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8ede5-291">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8ede5-291">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8ede5-292">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-292">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-293">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-293">Az.Automation</span></span>
* <span data-ttu-id="8ede5-294">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-294">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-295">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-295">Az.Compute</span></span>
* <span data-ttu-id="8ede5-296">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-296">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-297">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-297">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-298">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-298">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ede5-299">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ede5-299">Az.EventGrid</span></span>
* <span data-ttu-id="8ede5-300">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-300">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ede5-301">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-301">Az.IotHub</span></span>
* <span data-ttu-id="8ede5-302">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-302">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-303">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-303">Az.Network</span></span>
* <span data-ttu-id="8ede5-304">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-304">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8ede5-305">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-305">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ede5-306">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-306">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ede5-307">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-307">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8ede5-308">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8ede5-308">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-309">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-309">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-310">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-310">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-311">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-311">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-312">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-312">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-313">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-313">Az.Resources</span></span>
    - <span data-ttu-id="8ede5-314">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-314">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8ede5-315">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-315">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8ede5-316">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-316">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8ede5-317">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-317">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-318">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-318">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-319">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="8ede5-319">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-320">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-320">Az.Sql</span></span>
* <span data-ttu-id="8ede5-321">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-321">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8ede5-322">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-322">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8ede5-323">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-323">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ede5-324">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-324">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ede5-325">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-325">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ede5-326">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-326">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8ede5-327">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-327">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8ede5-328">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ede5-328">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8ede5-329">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-329">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-330">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-330">Az.Storage</span></span>
* <span data-ttu-id="8ede5-331">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-331">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8ede5-332">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ede5-332">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8ede5-333">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-333">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8ede5-334">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="8ede5-334">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8ede5-335">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-335">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8ede5-336">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-336">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8ede5-337">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-337">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8ede5-338">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-338">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8ede5-339">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ede5-339">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8ede5-340">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ede5-340">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ede5-341">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ede5-341">Az.StorageSync</span></span>
* <span data-ttu-id="8ede5-342">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-342">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8ede5-343">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-343">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-344">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-344">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-345">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-345">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8ede5-346">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8ede5-346">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8ede5-347">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-347">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8ede5-348">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8ede5-348">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8ede5-349">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8ede5-349">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-350">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-350">Az.Compute</span></span>
* <span data-ttu-id="8ede5-351">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-351">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8ede5-352">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-352">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8ede5-353">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8ede5-353">Az.Dns</span></span>
* <span data-ttu-id="8ede5-354">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-354">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ede5-355">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ede5-355">Az.EventGrid</span></span>
* <span data-ttu-id="8ede5-356">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-356">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8ede5-357">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ede5-357">New cmdlets:</span></span>
    - <span data-ttu-id="8ede5-358">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ede5-358">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ede5-359">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-359">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ede5-360">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ede5-360">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ede5-361">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-361">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8ede5-362">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ede5-362">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ede5-363">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-363">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ede5-364">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8ede5-364">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8ede5-365">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-365">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ede5-366">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8ede5-366">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8ede5-367">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-367">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8ede5-368">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8ede5-368">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8ede5-369">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-369">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8ede5-370">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8ede5-370">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8ede5-371">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-371">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="8ede5-372">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8ede5-372">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8ede5-373">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-373">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8ede5-374">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ede5-374">Updated cmdlets:</span></span>
    - <span data-ttu-id="8ede5-375">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8ede5-375">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8ede5-376">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-376">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8ede5-377">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-377">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8ede5-378">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="8ede5-378">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8ede5-379">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ede5-379">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8ede5-380">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="8ede5-380">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8ede5-381">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ede5-381">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8ede5-382">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-382">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8ede5-383">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="8ede5-383">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="8ede5-384">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8ede5-384">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8ede5-385">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-385">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8ede5-386">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8ede5-386">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8ede5-387">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-387">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8ede5-388">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-388">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ede5-389">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ede5-389">Az.FrontDoor</span></span>
* <span data-ttu-id="8ede5-390">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8ede5-390">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8ede5-391">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-391">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8ede5-392">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8ede5-392">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8ede5-393">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-393">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-394">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-394">Az.Network</span></span>
* <span data-ttu-id="8ede5-395">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-395">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8ede5-396">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-396">New cmdlets</span></span>
        - <span data-ttu-id="8ede5-397">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8ede5-397">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8ede5-398">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-398">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8ede5-399">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-399">New cmdlets</span></span> 
        - <span data-ttu-id="8ede5-400">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8ede5-400">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8ede5-401">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-401">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8ede5-402">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-402">New cmdlets</span></span> 
        - <span data-ttu-id="8ede5-403">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ede5-403">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="8ede5-404">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ede5-404">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ede5-405">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ede5-405">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ede5-406">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-406">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8ede5-407">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-407">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8ede5-408">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-408">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8ede5-409">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-409">New cmdlets</span></span>
        - <span data-ttu-id="8ede5-410">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ede5-410">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ede5-411">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ede5-411">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ede5-412">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ede5-412">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ede5-413">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8ede5-413">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8ede5-414">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="8ede5-414">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8ede5-415">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-415">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8ede5-416">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-416">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8ede5-417">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-417">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8ede5-418">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-418">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8ede5-419">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-419">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8ede5-420">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-420">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8ede5-421">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-421">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8ede5-422">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-422">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8ede5-423">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-423">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8ede5-424">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-424">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8ede5-425">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-425">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8ede5-426">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-426">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8ede5-427">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-427">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8ede5-428">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="8ede5-428">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8ede5-429">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-429">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8ede5-430">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-430">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8ede5-431">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="8ede5-431">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8ede5-432">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-432">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="8ede5-433">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-433">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="8ede5-434">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-434">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8ede5-435">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-435">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8ede5-436">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-436">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-437">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-437">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-438">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-438">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-439">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-439">Az.Resources</span></span>
* <span data-ttu-id="8ede5-440">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ede5-440">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8ede5-441">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-441">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8ede5-442">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-442">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8ede5-443">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-443">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ede5-444">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-444">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-445">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-445">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-446">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-446">Az.Sql</span></span>
* <span data-ttu-id="8ede5-447">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-447">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8ede5-448">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-448">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8ede5-449">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-449">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8ede5-450">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ede5-450">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ede5-451">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ede5-451">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ede5-452">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ede5-452">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ede5-453">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8ede5-453">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8ede5-454">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8ede5-454">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-455">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-455">Az.Storage</span></span>
* <span data-ttu-id="8ede5-456">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-456">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8ede5-457">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-457">New-AzStorageAccount</span></span>
* <span data-ttu-id="8ede5-458">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-458">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8ede5-459">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-459">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-460">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-460">Az.Websites</span></span>
* <span data-ttu-id="8ede5-461">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-461">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8ede5-462">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-462">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8ede5-463">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-463">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8ede5-464">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ede5-464">Az.Cdn</span></span>
* <span data-ttu-id="8ede5-465">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-465">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-466">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-466">Az.Compute</span></span>
* <span data-ttu-id="8ede5-467">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-467">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8ede5-468">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8ede5-468">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ede5-469">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-469">Az.EventHub</span></span>
* <span data-ttu-id="8ede5-470">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-470">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8ede5-471">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-471">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-472">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-472">Az.Network</span></span>
* <span data-ttu-id="8ede5-473">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-473">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8ede5-474">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-474">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ede5-475">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-475">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ede5-476">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-476">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-477">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-477">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-478">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-478">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-479">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-479">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-480">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-480">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ede5-481">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-481">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-482">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-482">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8ede5-483">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-483">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-484">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-484">Az.Sql</span></span>
* <span data-ttu-id="8ede5-485">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-485">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8ede5-486">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="8ede5-486">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8ede5-487">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-487">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8ede5-488">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-488">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-489">Az.Websites</span></span>
* <span data-ttu-id="8ede5-490">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-490">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8ede5-491">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-491">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8ede5-492">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ede5-492">Az.ApiManagement</span></span>
* <span data-ttu-id="8ede5-493">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-493">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8ede5-494">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="8ede5-494">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8ede5-495">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="8ede5-495">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8ede5-496">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8ede5-496">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8ede5-497">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-497">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8ede5-498">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8ede5-498">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8ede5-499">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="8ede5-499">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8ede5-500">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="8ede5-500">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8ede5-501">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-501">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8ede5-502">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="8ede5-502">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8ede5-503">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="8ede5-503">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8ede5-504">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="8ede5-504">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8ede5-505">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="8ede5-505">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8ede5-506">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-506">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8ede5-507">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="8ede5-507">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8ede5-508">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="8ede5-508">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8ede5-509">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="8ede5-509">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8ede5-510">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="8ede5-510">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8ede5-511">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-511">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="8ede5-512">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="8ede5-512">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8ede5-513">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-513">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8ede5-514">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-514">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8ede5-515">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8ede5-515">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8ede5-516">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-516">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="8ede5-517">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-517">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8ede5-518">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-518">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8ede5-519">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-519">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8ede5-520">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-520">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8ede5-521">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-521">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8ede5-522">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-522">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8ede5-523">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-523">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="8ede5-524">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8ede5-524">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8ede5-525">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-525">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8ede5-526">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-526">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8ede5-527">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="8ede5-527">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8ede5-528">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ede5-528">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8ede5-529">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ede5-529">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8ede5-530">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-530">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8ede5-531">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-531">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8ede5-532">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-532">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="8ede5-533">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8ede5-533">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8ede5-534">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="8ede5-534">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8ede5-535">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="8ede5-535">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8ede5-536">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-536">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8ede5-537">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-537">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8ede5-538">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8ede5-538">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8ede5-539">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="8ede5-539">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="8ede5-540">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-540">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8ede5-541">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-541">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8ede5-542">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="8ede5-542">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8ede5-543">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="8ede5-543">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8ede5-544">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="8ede5-544">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8ede5-545">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ede5-545">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8ede5-546">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-546">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8ede5-547">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="8ede5-547">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8ede5-548">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="8ede5-548">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8ede5-549">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-549">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8ede5-550">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8ede5-550">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8ede5-551">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8ede5-551">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8ede5-552">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-552">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8ede5-553">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-553">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8ede5-554">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8ede5-554">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8ede5-555">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8ede5-555">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8ede5-556">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-556">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8ede5-557">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-557">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8ede5-558">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="8ede5-558">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8ede5-559">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8ede5-559">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8ede5-560">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="8ede5-560">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8ede5-561">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8ede5-561">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8ede5-562">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8ede5-562">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8ede5-563">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8ede5-563">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8ede5-564">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="8ede5-564">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8ede5-565">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="8ede5-565">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8ede5-566">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-566">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8ede5-567">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="8ede5-567">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="8ede5-568">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8ede5-568">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8ede5-569">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="8ede5-569">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-570">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-570">Az.Automation</span></span>
* <span data-ttu-id="8ede5-571">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-571">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8ede5-572">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8ede5-572">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8ede5-573">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8ede5-573">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8ede5-574">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-574">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8ede5-575">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8ede5-575">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8ede5-576">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-576">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8ede5-577">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-577">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-578">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-578">Az.Compute</span></span>
* <span data-ttu-id="8ede5-579">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-579">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8ede5-580">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-580">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-581">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-581">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-582">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-582">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ede5-583">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-583">Az.Monitor</span></span>
* <span data-ttu-id="8ede5-584">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-584">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-585">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-585">Az.Network</span></span>
* <span data-ttu-id="8ede5-586">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-586">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8ede5-587">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ede5-587">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ede5-588">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ede5-588">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8ede5-589">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-589">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-590">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-590">Az.Resources</span></span>
* <span data-ttu-id="8ede5-591">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-591">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-592">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-592">Az.Sql</span></span>
* <span data-ttu-id="8ede5-593">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-593">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8ede5-594">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-594">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-595">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-596">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-596">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-597">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-597">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-598">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-598">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8ede5-599">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-599">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-600">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-600">Az.Compute</span></span>
* <span data-ttu-id="8ede5-601">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="8ede5-601">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8ede5-602">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8ede5-602">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8ede5-603">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-603">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8ede5-604">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-604">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8ede5-605">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-605">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8ede5-606">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-606">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="8ede5-607">重大な変更</span><span class="sxs-lookup"><span data-stu-id="8ede5-607">Breaking changes</span></span>
    - <span data-ttu-id="8ede5-608">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8ede5-608">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8ede5-609">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8ede5-609">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8ede5-610">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8ede5-610">Az.DeploymentManager</span></span>
* <span data-ttu-id="8ede5-611">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-611">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8ede5-612">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8ede5-612">Az.Dns</span></span>
* <span data-ttu-id="8ede5-613">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="8ede5-613">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8ede5-614">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-614">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8ede5-615">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-615">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ede5-616">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ede5-616">Az.FrontDoor</span></span>
* <span data-ttu-id="8ede5-617">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-617">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8ede5-618">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-618">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8ede5-619">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ede5-619">Az.HDInsight</span></span>
* <span data-ttu-id="8ede5-620">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-620">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8ede5-621">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ede5-621">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8ede5-622">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ede5-622">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8ede5-623">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-623">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8ede5-624">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-624">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8ede5-625">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-625">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8ede5-626">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="8ede5-626">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ede5-627">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-627">Az.Monitor</span></span>
* <span data-ttu-id="8ede5-628">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="8ede5-628">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="8ede5-629">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8ede5-629">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8ede5-630">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8ede5-630">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8ede5-631">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8ede5-631">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8ede5-632">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8ede5-632">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8ede5-633">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8ede5-633">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8ede5-634">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8ede5-634">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8ede5-635">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-635">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ede5-636">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-636">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ede5-637">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-637">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ede5-638">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-638">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ede5-639">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-639">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ede5-640">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="8ede5-640">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8ede5-641">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-641">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-642">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-642">Az.Network</span></span>
* <span data-ttu-id="8ede5-643">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-643">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8ede5-644">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-644">New cmdlets</span></span>
        - <span data-ttu-id="8ede5-645">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ede5-645">New-AzNatGateway</span></span>
        - <span data-ttu-id="8ede5-646">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ede5-646">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8ede5-647">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ede5-647">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8ede5-648">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ede5-648">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8ede5-649">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-649">Updated cmdlets</span></span>
        - <span data-ttu-id="8ede5-650">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8ede5-650">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8ede5-651">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8ede5-651">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8ede5-652">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="8ede5-652">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8ede5-653">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-653">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8ede5-654">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-654">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ede5-655">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-655">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ede5-656">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="8ede5-656">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8ede5-657">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-657">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8ede5-658">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-658">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-659">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-659">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-660">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ede5-660">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8ede5-661">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="8ede5-661">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8ede5-662">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="8ede5-662">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8ede5-663">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8ede5-663">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8ede5-664">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8ede5-664">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8ede5-665">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="8ede5-665">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8ede5-666">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8ede5-666">Az.Relay</span></span>
* <span data-ttu-id="8ede5-667">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-667">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-668">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-668">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-669">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-669">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-670">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-670">Az.Storage</span></span>
* <span data-ttu-id="8ede5-671">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="8ede5-671">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8ede5-672">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-672">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8ede5-673">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-673">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8ede5-674">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-674">New-AzStorageAccount</span></span>
* <span data-ttu-id="8ede5-675">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="8ede5-675">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8ede5-676">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-676">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8ede5-677">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-677">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8ede5-678">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ede5-678">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-679">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-679">Az.Websites</span></span>
* <span data-ttu-id="8ede5-680">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ede5-680">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8ede5-681">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="8ede5-681">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8ede5-682">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-682">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ede5-683">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ede5-683">Highlights since the last major release</span></span>
* <span data-ttu-id="8ede5-684">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ede5-684">General availability of `Az` module</span></span>
* <span data-ttu-id="8ede5-685">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ede5-685">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ede5-686">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ede5-686">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ede5-687">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-687">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ede5-688">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-688">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ede5-689">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-689">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ede5-690">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-690">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ede5-691">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-691">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-692">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-692">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ede5-693">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ede5-693">Az.Batch</span></span>
* <span data-ttu-id="8ede5-694">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-694">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ede5-695">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ede5-695">Az.Cdn</span></span>
* <span data-ttu-id="8ede5-696">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-696">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-697">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-697">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-698">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-698">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-699">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-699">Az.Compute</span></span>
* <span data-ttu-id="8ede5-700">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-700">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8ede5-701">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-701">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-702">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-702">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-703">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-703">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-704">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-704">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-705">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-705">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-706">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-706">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ede5-707">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ede5-707">Az.EventGrid</span></span>
* <span data-ttu-id="8ede5-708">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-708">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ede5-709">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-709">Az.EventHub</span></span>
* <span data-ttu-id="8ede5-710">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-710">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="8ede5-711">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ede5-711">Az.HDInsight</span></span>
* <span data-ttu-id="8ede5-712">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-712">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ede5-713">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-713">Az.IotHub</span></span>
* <span data-ttu-id="8ede5-714">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-714">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ede5-715">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-715">Az.KeyVault</span></span>
* <span data-ttu-id="8ede5-716">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-716">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-717">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-717">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8ede5-718">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8ede5-718">Az.MachineLearning</span></span>
* <span data-ttu-id="8ede5-719">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-719">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8ede5-720">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8ede5-720">Az.Media</span></span>
* <span data-ttu-id="8ede5-721">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-721">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ede5-722">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-722">Az.Monitor</span></span>
  * <span data-ttu-id="8ede5-723">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-723">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8ede5-724">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8ede5-724">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8ede5-725">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8ede5-725">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8ede5-726">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ede5-726">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8ede5-727">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ede5-727">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8ede5-728">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ede5-728">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8ede5-729">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-729">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-730">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-730">Az.Network</span></span>
* <span data-ttu-id="8ede5-731">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-731">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-732">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-732">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8ede5-733">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8ede5-733">Az.NotificationHubs</span></span>
* <span data-ttu-id="8ede5-734">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-734">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-735">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-735">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-736">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-736">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8ede5-737">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8ede5-737">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8ede5-738">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-738">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-739">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-739">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-740">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-740">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-741">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-741">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8ede5-742">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-742">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8ede5-743">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-743">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ede5-744">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ede5-744">Az.RedisCache</span></span>
* <span data-ttu-id="8ede5-745">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-745">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-746">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-746">Az.Resources</span></span>
* <span data-ttu-id="8ede5-747">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-747">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-748">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-748">Az.Sql</span></span>
* <span data-ttu-id="8ede5-749">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="8ede5-749">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8ede5-750">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-750">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-751">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-751">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8ede5-752">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-752">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8ede5-753">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="8ede5-753">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8ede5-754">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="8ede5-754">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8ede5-755">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-755">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-756">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-756">Az.Websites</span></span>
* <span data-ttu-id="8ede5-757">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-757">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8ede5-758">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-758">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ede5-759">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-759">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8ede5-760">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-760">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8ede5-761">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-761">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ede5-762">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ede5-762">Highlights since the last major release</span></span>
* <span data-ttu-id="8ede5-763">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ede5-763">General availability of `Az` module</span></span>
* <span data-ttu-id="8ede5-764">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ede5-764">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ede5-765">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ede5-765">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ede5-766">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-766">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ede5-767">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-767">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ede5-768">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-768">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ede5-769">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-769">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ede5-770">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-770">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-771">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-771">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ede5-772">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-772">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ede5-773">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="8ede5-773">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8ede5-774">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-774">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-775">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-775">Az.Automation</span></span>
* <span data-ttu-id="8ede5-776">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-776">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8ede5-777">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-777">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8ede5-778">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-778">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-779">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-779">Az.Compute</span></span>
* <span data-ttu-id="8ede5-780">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-780">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8ede5-781">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-781">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="8ede5-782">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-782">Az.ContainerInstance</span></span>
* <span data-ttu-id="8ede5-783">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-783">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-784">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-784">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-785">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-785">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8ede5-786">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-786">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-787">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-787">Az.Resources</span></span>
* <span data-ttu-id="8ede5-788">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-788">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8ede5-789">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-789">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8ede5-790">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="8ede5-790">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8ede5-791">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8ede5-791">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8ede5-792">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-792">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8ede5-793">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8ede5-793">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-794">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-794">Az.Sql</span></span>
* <span data-ttu-id="8ede5-795">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-795">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-796">Az.Storage</span></span>
* <span data-ttu-id="8ede5-797">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="8ede5-797">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8ede5-798">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8ede5-798">New-AzStorageContext</span></span>
* <span data-ttu-id="8ede5-799">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ede5-799">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8ede5-800">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8ede5-800">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8ede5-801">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8ede5-801">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8ede5-802">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-802">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8ede5-803">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-803">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8ede5-804">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ede5-804">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8ede5-805">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ede5-805">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8ede5-806">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ede5-806">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8ede5-807">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ede5-807">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8ede5-808">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ede5-808">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8ede5-809">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-809">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ede5-810">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ede5-810">Highlights since the last major release</span></span>
* <span data-ttu-id="8ede5-811">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ede5-811">General availability of `Az` module</span></span>
* <span data-ttu-id="8ede5-812">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ede5-812">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ede5-813">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ede5-813">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ede5-814">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-814">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ede5-815">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-815">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ede5-816">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-816">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ede5-817">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-817">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-818">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-818">Az.Automation</span></span>
* <span data-ttu-id="8ede5-819">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-819">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8ede5-820">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="8ede5-820">Dynamic grouping</span></span>
    * <span data-ttu-id="8ede5-821">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="8ede5-821">Pre-Post script</span></span>
    * <span data-ttu-id="8ede5-822">再起動設定</span><span class="sxs-lookup"><span data-stu-id="8ede5-822">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-823">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-823">Az.Compute</span></span>
* <span data-ttu-id="8ede5-824">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-824">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8ede5-825">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-825">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ede5-826">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-826">Az.KeyVault</span></span>
* <span data-ttu-id="8ede5-827">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-827">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-828">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-828">Az.Network</span></span>
* <span data-ttu-id="8ede5-829">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-829">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8ede5-830">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-830">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-831">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-831">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-832">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-832">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8ede5-833">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-833">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-834">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-834">Az.Resources</span></span>
* <span data-ttu-id="8ede5-835">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-835">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8ede5-836">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-836">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-837">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-837">Az.Sql</span></span>
* <span data-ttu-id="8ede5-838">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-838">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-839">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-839">Az.Storage</span></span>
* <span data-ttu-id="8ede5-840">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-840">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8ede5-841">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-841">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ede5-842">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-842">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ede5-843">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ede5-843">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ede5-844">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8ede5-844">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8ede5-845">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8ede5-845">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8ede5-846">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-846">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-847">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-847">Az.Websites</span></span>
* <span data-ttu-id="8ede5-848">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-848">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="8ede5-849">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-849">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-850">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-850">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-851">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-851">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8ede5-852">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-852">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-853">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-853">Az.Automation</span></span>
* <span data-ttu-id="8ede5-854">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-854">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8ede5-855">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-855">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8ede5-856">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-856">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ede5-857">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ede5-857">Az.Cdn</span></span>
* <span data-ttu-id="8ede5-858">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-858">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-859">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-859">Az.Compute</span></span>
* <span data-ttu-id="8ede5-860">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-860">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-861">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-861">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-862">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-862">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ede5-863">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ede5-863">Az.LogicApp</span></span>
* <span data-ttu-id="8ede5-864">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-864">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-865">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-865">Az.Network</span></span>
* <span data-ttu-id="8ede5-866">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-866">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-867">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-867">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-868">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-868">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8ede5-869">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-869">SDK Update</span></span>
* <span data-ttu-id="8ede5-870">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-870">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8ede5-871">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-871">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-872">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-872">Az.Resources</span></span>
* <span data-ttu-id="8ede5-873">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-873">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8ede5-874">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8ede5-874">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8ede5-875">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-875">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8ede5-876">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8ede5-876">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8ede5-877">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-877">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8ede5-878">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8ede5-878">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-879">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-879">Az.Sql</span></span>
* <span data-ttu-id="8ede5-880">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-880">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8ede5-881">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-881">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-882">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-882">Az.Storage</span></span>
* <span data-ttu-id="8ede5-883">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ede5-883">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8ede5-884">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-884">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8ede5-885">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-885">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ede5-886">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-886">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-887">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-887">Az.Automation</span></span>
* <span data-ttu-id="8ede5-888">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-888">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8ede5-889">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-889">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8ede5-890">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-890">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-891">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-891">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-892">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-892">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-893">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-893">Az.Compute</span></span>
* <span data-ttu-id="8ede5-894">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-894">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8ede5-895">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-895">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8ede5-896">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-896">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8ede5-897">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-897">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-898">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-898">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-899">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-899">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ede5-900">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-900">Az.EventHub</span></span>
* <span data-ttu-id="8ede5-901">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-901">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="8ede5-902">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-902">Az.KeyVault</span></span>
* <span data-ttu-id="8ede5-903">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-903">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ede5-904">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ede5-904">Az.LogicApp</span></span>
* <span data-ttu-id="8ede5-905">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-905">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8ede5-906">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-906">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8ede5-907">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-907">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8ede5-908">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ede5-908">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ede5-909">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ede5-909">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ede5-910">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ede5-910">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ede5-911">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ede5-911">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8ede5-912">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-912">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8ede5-913">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ede5-913">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ede5-914">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ede5-914">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ede5-915">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ede5-915">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ede5-916">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ede5-916">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8ede5-917">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-917">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ede5-918">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-918">Az.Monitor</span></span>
* <span data-ttu-id="8ede5-919">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-919">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-920">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-920">Az.Network</span></span>
* <span data-ttu-id="8ede5-921">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-921">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-922">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-922">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ede5-923">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-923">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8ede5-924">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-924">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="8ede5-925">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-925">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="8ede5-926">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-926">Az.Resources</span></span>
* <span data-ttu-id="8ede5-927">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8ede5-927">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8ede5-928">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8ede5-928">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8ede5-929">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8ede5-929">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8ede5-930">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-930">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-931">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-931">Az.Sql</span></span>
* <span data-ttu-id="8ede5-932">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-932">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8ede5-933">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-933">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-934">Az.Websites</span></span>
* <span data-ttu-id="8ede5-935">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-935">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8ede5-936">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-936">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-937">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-937">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-938">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-938">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ede5-939">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-939">Az.AnalysisServices</span></span>
<span data-ttu-id="8ede5-940">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8ede5-940">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-941">Az.Compute</span></span>
* <span data-ttu-id="8ede5-942">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-942">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8ede5-943">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-943">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8ede5-944">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-944">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-945">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-945">Az.RecoveryServices</span></span>
<span data-ttu-id="8ede5-946">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8ede5-946">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-947">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-947">Az.Resources</span></span>
* <span data-ttu-id="8ede5-948">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-948">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="8ede5-949">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8ede5-949">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8ede5-950">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-950">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="8ede5-951">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8ede5-951">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-952">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-952">Az.Sql</span></span>
* <span data-ttu-id="8ede5-953">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-953">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8ede5-954">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-954">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8ede5-955">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-955">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8ede5-956">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-956">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-957">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-957">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-958">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-958">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ede5-959">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-959">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ede5-960">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-960">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-961">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-961">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ede5-962">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-962">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8ede5-963">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-963">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-964">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-964">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-965">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-965">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ede5-966">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-966">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ede5-967">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-967">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8ede5-968">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8ede5-968">Az.Aks</span></span>
* <span data-ttu-id="8ede5-969">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-969">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ede5-970">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-970">Az.Automation</span></span>
* <span data-ttu-id="8ede5-971">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-971">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8ede5-972">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-972">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ede5-973">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ede5-973">Az.Cdn</span></span>
* <span data-ttu-id="8ede5-974">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-974">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-975">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-975">Az.Compute</span></span>
* <span data-ttu-id="8ede5-976">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-976">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8ede5-977">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-977">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8ede5-978">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-978">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8ede5-979">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8ede5-979">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8ede5-980">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-980">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ede5-981">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ede5-981">Az.DataFactory</span></span>
* <span data-ttu-id="8ede5-982">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-982">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-983">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-983">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-984">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="8ede5-984">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8ede5-985">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8ede5-985">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8ede5-986">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-986">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ede5-987">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-987">Az.IotHub</span></span>
* <span data-ttu-id="8ede5-988">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-988">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ede5-989">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-989">Az.KeyVault</span></span>
* <span data-ttu-id="8ede5-990">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-990">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-991">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-991">Az.Network</span></span>
* <span data-ttu-id="8ede5-992">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-992">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-993">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-993">Az.Resources</span></span>
* <span data-ttu-id="8ede5-994">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-994">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8ede5-995">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-995">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8ede5-996">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-996">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8ede5-997">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8ede5-997">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8ede5-998">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8ede5-998">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8ede5-999">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-999">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8ede5-1000">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8ede5-1000">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ede5-1001">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-1001">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-1002">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8ede5-1002">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8ede5-1003">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1003">Fix some error messages.</span></span>
* <span data-ttu-id="8ede5-1004">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1004">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8ede5-1005">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1005">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8ede5-1006">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8ede5-1006">Az.SignalR</span></span>
* <span data-ttu-id="8ede5-1007">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1007">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-1008">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1008">Az.Sql</span></span>
* <span data-ttu-id="8ede5-1009">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1009">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ede5-1010">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1010">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8ede5-1011">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1011">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8ede5-1012">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-1012">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-1013">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1013">Az.Storage</span></span>
* <span data-ttu-id="8ede5-1014">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1014">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ede5-1015">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="8ede5-1015">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8ede5-1016">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8ede5-1016">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8ede5-1017">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8ede5-1017">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8ede5-1018">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8ede5-1018">Az.TrafficManager</span></span>
* <span data-ttu-id="8ede5-1019">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1019">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-1020">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-1020">Az.Websites</span></span>
* <span data-ttu-id="8ede5-1021">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1021">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ede5-1022">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1022">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8ede5-1023">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8ede5-1023">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8ede5-1024">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1024">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ede5-1025">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-1025">Az.Accounts</span></span>
* <span data-ttu-id="8ede5-1026">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="8ede5-1026">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-1027">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1027">Az.Compute</span></span>
* <span data-ttu-id="8ede5-1028">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1028">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8ede5-1029">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1029">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8ede5-1030">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1030">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-1031">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-1031">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-1032">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1032">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8ede5-1033">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1033">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ede5-1034">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ede5-1034">Az.EventGrid</span></span>
* <span data-ttu-id="8ede5-1035">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1035">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8ede5-1036">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="8ede5-1036">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8ede5-1037">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ede5-1037">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8ede5-1038">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8ede5-1038">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8ede5-1039">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8ede5-1039">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8ede5-1040">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8ede5-1040">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8ede5-1041">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ede5-1041">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8ede5-1042">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8ede5-1042">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8ede5-1043">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8ede5-1043">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8ede5-1044">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8ede5-1044">Dead letter endpoint.</span></span>
* <span data-ttu-id="8ede5-1045">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1045">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8ede5-1046">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1046">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ede5-1047">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ede5-1047">Az.IotHub</span></span>
* <span data-ttu-id="8ede5-1048">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1048">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ede5-1049">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ede5-1049">Az.LogicApp</span></span>
* <span data-ttu-id="8ede5-1050">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="8ede5-1050">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-1051">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1051">Az.Resources</span></span>
* <span data-ttu-id="8ede5-1052">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1052">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8ede5-1053">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8ede5-1053">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8ede5-1054">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1054">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8ede5-1055">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1055">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8ede5-1056">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1056">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8ede5-1057">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8ede5-1057">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8ede5-1058">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8ede5-1058">Az.SignalR</span></span>
* <span data-ttu-id="8ede5-1059">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1059">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-1060">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1060">Az.Sql</span></span>
* <span data-ttu-id="8ede5-1061">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1061">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ede5-1062">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1062">Az.Storage</span></span>
* <span data-ttu-id="8ede5-1063">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="8ede5-1063">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8ede5-1064">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8ede5-1064">New-AzStorageContext</span></span>
* <span data-ttu-id="8ede5-1065">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1065">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8ede5-1066">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8ede5-1066">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-1067">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-1067">Az.Websites</span></span>
* <span data-ttu-id="8ede5-1068">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1068">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8ede5-1069">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1069">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8ede5-1070">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1070">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8ede5-1071">全般</span><span class="sxs-lookup"><span data-stu-id="8ede5-1071">General</span></span>

- <span data-ttu-id="8ede5-1072">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="8ede5-1072">General Availability of Az Module</span></span>
- <span data-ttu-id="8ede5-1073">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="8ede5-1073">Online help for each module</span></span>
- <span data-ttu-id="8ede5-1074">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1074">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8ede5-1075">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1075">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8ede5-1076">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ede5-1076">Az.Accounts</span></span>
- <span data-ttu-id="8ede5-1077">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1077">Changed from Az.Profile</span></span>
- <span data-ttu-id="8ede5-1078">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1078">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8ede5-1079">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ede5-1079">Az.ApiManagement</span></span>
- <span data-ttu-id="8ede5-1080">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="8ede5-1080">Fixes for #7002</span></span>
- <span data-ttu-id="8ede5-1081">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1081">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8ede5-1082">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ede5-1082">Az.Batch</span></span>
- <span data-ttu-id="8ede5-1083">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1083">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8ede5-1084">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1084">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8ede5-1085">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1085">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8ede5-1086">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8ede5-1086">Az.Billing</span></span>
- <span data-ttu-id="8ede5-1087">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1087">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8ede5-1088">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-1088">Az.CognitivServices</span></span>
- <span data-ttu-id="8ede5-1089">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1089">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8ede5-1090">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1090">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8ede5-1091">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1091">Az.ContainerInstance</span></span>
- <span data-ttu-id="8ede5-1092">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1092">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8ede5-1093">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8ede5-1093">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8ede5-1094">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1094">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-1095">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-1095">Az.DataLakeStore</span></span>
- <span data-ttu-id="8ede5-1096">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1096">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8ede5-1097">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ede5-1097">Az.Monitor</span></span>
- <span data-ttu-id="8ede5-1098">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1098">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8ede5-1099">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ede5-1099">Az.KeyVault</span></span>
- <span data-ttu-id="8ede5-1100">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1100">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8ede5-1101">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8ede5-1101">Az.MachineLearning</span></span>
- <span data-ttu-id="8ede5-1102">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1102">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8ede5-1103">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8ede5-1103">Az.Media</span></span>
- <span data-ttu-id="8ede5-1104">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1104">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8ede5-1105">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-1105">Az.Network</span></span>
<span data-ttu-id="8ede5-1106">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1106">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8ede5-1107">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ede5-1107">New cmdlets added:</span></span>
        - <span data-ttu-id="8ede5-1108">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1108">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1109">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1109">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1110">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1110">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1111">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1111">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1112">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1112">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1113">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-1113">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8ede5-1114">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8ede5-1114">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8ede5-1115">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ede5-1115">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8ede5-1116">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-1116">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8ede5-1117">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8ede5-1117">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8ede5-1118">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-1118">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8ede5-1119">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8ede5-1119">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8ede5-1120">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-1120">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8ede5-1121">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-1121">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8ede5-1122">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1122">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8ede5-1123">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-1123">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8ede5-1124">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ede5-1124">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8ede5-1125">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ede5-1125">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8ede5-1126">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ede5-1126">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8ede5-1127">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-1127">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8ede5-1128">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1128">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8ede5-1129">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-1129">Az.OperationalInsights</span></span>
- <span data-ttu-id="8ede5-1130">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1130">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8ede5-1131">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1131">Az.Profile</span></span>
- <span data-ttu-id="8ede5-1132">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1132">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-1133">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-1133">Az.RecoveryServices</span></span>
- <span data-ttu-id="8ede5-1134">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1134">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8ede5-1135">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1135">Az.Resources</span></span>
- <span data-ttu-id="8ede5-1136">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1136">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8ede5-1137">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-1137">Az.ServiceFabric</span></span>
- <span data-ttu-id="8ede5-1138">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ede5-1138">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8ede5-1139">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1139">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8ede5-1140">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8ede5-1140">Az.SIgnalR</span></span>
- <span data-ttu-id="8ede5-1141">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="8ede5-1141">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8ede5-1142">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1142">Az.Sql</span></span>
- <span data-ttu-id="8ede5-1143">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1143">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8ede5-1144">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1144">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8ede5-1145">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1145">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8ede5-1146">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1146">Az.Storage</span></span>
- <span data-ttu-id="8ede5-1147">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1147">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8ede5-1148">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-1148">Az.Websites</span></span>
- <span data-ttu-id="8ede5-1149">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ede5-1149">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8ede5-1150">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1150">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8ede5-1151">全般</span><span class="sxs-lookup"><span data-stu-id="8ede5-1151">General</span></span>

* <span data-ttu-id="8ede5-1152">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8ede5-1152">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8ede5-1153">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1153">Az.Compute</span></span>

* <span data-ttu-id="8ede5-1154">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1154">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-1155">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-1155">Az.DataLakeStore</span></span>

* <span data-ttu-id="8ede5-1156">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1156">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8ede5-1157">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ede5-1157">Az.FrontDoor</span></span>

* <span data-ttu-id="8ede5-1158">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1158">Fixed some broken links</span></span>
    - <span data-ttu-id="8ede5-1159">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1159">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8ede5-1160">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1160">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8ede5-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-1161">Az.RecoveryServices</span></span>

* <span data-ttu-id="8ede5-1162">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1162">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8ede5-1163">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1163">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8ede5-1164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1164">Az.Resources</span></span>

* <span data-ttu-id="8ede5-1165">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1165">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8ede5-1166">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1166">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8ede5-1167">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1167">Az.Sql</span></span>

* <span data-ttu-id="8ede5-1168">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8ede5-1168">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8ede5-1169">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1169">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8ede5-1170">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1170">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8ede5-1171">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1171">Az.Storage</span></span>

* <span data-ttu-id="8ede5-1172">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1172">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8ede5-1173">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1173">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8ede5-1174">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8ede5-1174">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8ede5-1175">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="8ede5-1175">Support Static Website configuration</span></span>
    - <span data-ttu-id="8ede5-1176">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ede5-1176">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8ede5-1177">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ede5-1177">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8ede5-1178">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-1178">Az.Websites</span></span>

* <span data-ttu-id="8ede5-1179">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8ede5-1179">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="8ede5-1180">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1180">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8ede5-1181">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="8ede5-1181">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8ede5-1182">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1182">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8ede5-1183">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ede5-1183">Az.ApiManagement</span></span>
* <span data-ttu-id="8ede5-1184">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1184">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8ede5-1185">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ede5-1185">Az.Automation</span></span>
* <span data-ttu-id="8ede5-1186">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ede5-1186">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8ede5-1187">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1187">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8ede5-1188">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1188">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8ede5-1189">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1189">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8ede5-1190">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1190">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8ede5-1191">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1191">Az.Compute</span></span>
* <span data-ttu-id="8ede5-1192">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1192">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8ede5-1193">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1193">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8ede5-1194">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1194">Az.ContainerInstance</span></span>
* <span data-ttu-id="8ede5-1195">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1195">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8ede5-1196">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8ede5-1196">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8ede5-1197">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1197">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8ede5-1198">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-1198">Az.Network</span></span>
* <span data-ttu-id="8ede5-1199">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1199">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8ede5-1200">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1200">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8ede5-1201">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1201">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="8ede5-1202">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1202">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8ede5-1203">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8ede5-1203">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8ede5-1204">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1204">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8ede5-1205">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1205">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8ede5-1206">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8ede5-1206">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8ede5-1207">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1207">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8ede5-1208">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1208">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8ede5-1209">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8ede5-1209">Az.Relay</span></span>
* <span data-ttu-id="8ede5-1210">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ede5-1210">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8ede5-1211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1211">Az.Resources</span></span>
* <span data-ttu-id="8ede5-1212">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1212">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8ede5-1213">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1213">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8ede5-1214">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8ede5-1214">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8ede5-1215">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-1215">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-1216">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1216">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8ede5-1217">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1217">Az.Sql</span></span>
* <span data-ttu-id="8ede5-1218">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1218">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8ede5-1219">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1219">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ede5-1220">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1220">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ede5-1221">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1221">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ede5-1222">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ede5-1222">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ede5-1223">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ede5-1223">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ede5-1224">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ede5-1224">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ede5-1225">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ede5-1225">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ede5-1226">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ede5-1226">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8ede5-1227">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1227">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8ede5-1228">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1228">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8ede5-1229">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1229">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8ede5-1230">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8ede5-1230">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8ede5-1231">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8ede5-1231">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8ede5-1232">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8ede5-1232">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8ede5-1233">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8ede5-1233">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8ede5-1234">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1234">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8ede5-1235">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1235">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8ede5-1236">全般</span><span class="sxs-lookup"><span data-stu-id="8ede5-1236">General</span></span>
* <span data-ttu-id="8ede5-1237">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ede5-1237">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8ede5-1238">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1238">Az.Profile</span></span>
* <span data-ttu-id="8ede5-1239">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1239">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8ede5-1240">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1240">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8ede5-1241">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1241">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8ede5-1242">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1242">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8ede5-1243">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1243">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8ede5-1244">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1244">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8ede5-1245">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1245">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-1246">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-1246">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-1247">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1247">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-1248">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1248">Az.Compute</span></span>
* <span data-ttu-id="8ede5-1249">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1249">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8ede5-1250">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="8ede5-1250">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8ede5-1251">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1251">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-1252">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-1252">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-1253">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1253">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8ede5-1254">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1254">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8ede5-1255">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8ede5-1255">Az.Insights</span></span>
* <span data-ttu-id="8ede5-1256">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1256">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8ede5-1257">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1257">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8ede5-1258">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1258">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8ede5-1259">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="8ede5-1259">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-1260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-1260">Az.Network</span></span>
* <span data-ttu-id="8ede5-1261">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="8ede5-1261">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8ede5-1262">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ede5-1262">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8ede5-1263">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8ede5-1263">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8ede5-1264">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8ede5-1264">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8ede5-1265">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8ede5-1265">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8ede5-1266">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ede5-1266">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8ede5-1267">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8ede5-1267">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ede5-1268">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ede5-1268">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ede5-1269">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1269">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-1270">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1270">Az.Resources</span></span>
* <span data-ttu-id="8ede5-1271">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1271">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8ede5-1272">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1272">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ede5-1273">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ede5-1273">Az.ServiceBus</span></span>
* <span data-ttu-id="8ede5-1274">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1274">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ede5-1275">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ede5-1275">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ede5-1276">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1276">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8ede5-1277">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1277">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8ede5-1278">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1278">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8ede5-1279">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1279">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8ede5-1280">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1280">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8ede5-1281">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1281">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8ede5-1282">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1282">Az.Profile</span></span>
* <span data-ttu-id="8ede5-1283">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1283">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8ede5-1284">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1284">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-1285">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1285">Az.Compute</span></span>
* <span data-ttu-id="8ede5-1286">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1286">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8ede5-1287">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1287">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ede5-1288">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ede5-1288">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ede5-1289">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1289">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8ede5-1290">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1290">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8ede5-1291">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1291">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8ede5-1292">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1292">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8ede5-1293">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1293">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-1294">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-1294">Az.Network</span></span>
* <span data-ttu-id="8ede5-1295">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1295">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8ede5-1296">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1296">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-1297">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1297">Az.Resources</span></span>
* <span data-ttu-id="8ede5-1298">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1298">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8ede5-1299">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1299">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8ede5-1300">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1300">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8ede5-1301">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1301">Azure.Storage</span></span>
* <span data-ttu-id="8ede5-1302">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1302">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8ede5-1303">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ede5-1303">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8ede5-1304">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8ede5-1304">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8ede5-1305">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1305">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8ede5-1306">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8ede5-1306">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="8ede5-1307">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ede5-1307">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ede5-1308">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1308">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ede5-1309">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ede5-1309">Az.Compute</span></span>
* <span data-ttu-id="8ede5-1310">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1310">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8ede5-1311">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1311">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8ede5-1312">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1312">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8ede5-1313">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8ede5-1313">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8ede5-1314">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1314">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ede5-1315">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ede5-1315">Az.Network</span></span>
* <span data-ttu-id="8ede5-1316">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1316">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8ede5-1317">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ede5-1317">new cmdlets added</span></span>
    - <span data-ttu-id="8ede5-1318">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1318">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ede5-1319">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1319">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ede5-1320">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1320">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ede5-1321">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ede5-1321">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ede5-1322">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-1322">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8ede5-1323">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ede5-1323">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8ede5-1324">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1324">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8ede5-1325">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1325">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8ede5-1326">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1326">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ede5-1327">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ede5-1327">Az.RedisCache</span></span>
* <span data-ttu-id="8ede5-1328">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="8ede5-1328">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8ede5-1329">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1329">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ede5-1330">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ede5-1330">Az.Resources</span></span>
* <span data-ttu-id="8ede5-1331">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1331">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8ede5-1332">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1332">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ede5-1333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ede5-1333">Az.Sql</span></span>
* <span data-ttu-id="8ede5-1334">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ede5-1334">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ede5-1335">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ede5-1335">Az.Websites</span></span>
* <span data-ttu-id="8ede5-1336">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="8ede5-1336">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8ede5-1337">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="8ede5-1337">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8ede5-1338">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="8ede5-1338">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8ede5-1339">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="8ede5-1339">Initial Release</span></span>
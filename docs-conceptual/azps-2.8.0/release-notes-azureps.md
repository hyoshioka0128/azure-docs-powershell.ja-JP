---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 83e6039153bcc2b8ccb7ceddfa91609f0d6c7b3f
ms.sourcegitcommit: b4ee3fbaaa2a329ea28308bd1902ae83a34db698
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/16/2019
ms.locfileid: "72380196"
---
## <a name="280---october-2019"></a><span data-ttu-id="b4d66-103">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-103">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="b4d66-104">全般</span><span class="sxs-lookup"><span data-stu-id="b4d66-104">General</span></span>
* <span data-ttu-id="b4d66-105">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-105">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="b4d66-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-106">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-107">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-107">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="b4d66-108">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-108">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-109">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-109">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="b4d66-110">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="b4d66-110">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-111">Az.Automation</span></span>
* <span data-ttu-id="b4d66-112">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-112">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="b4d66-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="b4d66-113">Az.Batch</span></span>
* <span data-ttu-id="b4d66-114">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-114">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-115">Az.Compute</span></span>
* <span data-ttu-id="b4d66-116">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-116">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="b4d66-117">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-117">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="b4d66-118">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-118">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="b4d66-119">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-119">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-120">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-121">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="b4d66-121">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="b4d66-122">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="b4d66-122">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="b4d66-123">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-123">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-125">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-125">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="b4d66-126">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="b4d66-126">Az.HealthcareApis</span></span>
* <span data-ttu-id="b4d66-127">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-127">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="b4d66-128">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-128">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="b4d66-129">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-129">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="b4d66-130">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-130">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-131">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-131">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-132">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="b4d66-132">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="b4d66-133">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="b4d66-133">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-134">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-135">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="b4d66-135">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="b4d66-136">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-136">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="b4d66-137">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="b4d66-137">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="b4d66-138">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-138">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-139">Az.Network</span></span>
* <span data-ttu-id="b4d66-140">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-140">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="b4d66-141">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-141">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="b4d66-142">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="b4d66-142">New cmdlets added:</span></span>
        - <span data-ttu-id="b4d66-143">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-143">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="b4d66-144">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-144">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="b4d66-145">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-145">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="b4d66-146">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-146">Updated cmdlets:</span></span>
        - <span data-ttu-id="b4d66-147">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-147">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="b4d66-148">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-148">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="b4d66-149">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-149">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="b4d66-150">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="b4d66-150">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="b4d66-151">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="b4d66-151">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="b4d66-152">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-152">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="b4d66-153">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-153">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="b4d66-154">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="b4d66-154">Az.RedisCache</span></span>
* <span data-ttu-id="b4d66-155">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-155">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-156">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-156">Az.Sql</span></span>
* <span data-ttu-id="b4d66-157">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-157">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-158">Az.Storage</span></span>
* <span data-ttu-id="b4d66-159">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="b4d66-159">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="b4d66-160">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b4d66-160">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="b4d66-161">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="b4d66-161">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="b4d66-162">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b4d66-162">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="b4d66-163">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-163">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="b4d66-164">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="b4d66-164">Az.StorageSync</span></span>
* <span data-ttu-id="b4d66-165">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-165">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-166">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-166">Az.Websites</span></span>
* <span data-ttu-id="b4d66-167">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="b4d66-167">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="b4d66-168">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-168">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="b4d66-169">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-169">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-170">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-170">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="b4d66-171">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-171">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="b4d66-172">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="b4d66-172">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-173">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-173">Az.Automation</span></span>
* <span data-ttu-id="b4d66-174">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-174">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="b4d66-175">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-175">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="b4d66-176">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-176">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-177">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-177">Az.Compute</span></span>
* <span data-ttu-id="b4d66-178">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-178">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="b4d66-179">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-179">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="b4d66-180">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-180">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="b4d66-181">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-181">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="b4d66-182">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-182">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="b4d66-183">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-183">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="b4d66-184">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-184">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="b4d66-185">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-185">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="b4d66-186">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-186">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-187">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-187">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-188">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-188">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="b4d66-189">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-189">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="b4d66-190">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="b4d66-190">Az.HDInsight</span></span>
* <span data-ttu-id="b4d66-191">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="b4d66-191">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-192">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-192">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-193">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-193">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="b4d66-194">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-194">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="b4d66-195">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b4d66-195">New cmdlets are:</span></span>
    - <span data-ttu-id="b4d66-196">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="b4d66-196">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="b4d66-197">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="b4d66-197">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="b4d66-198">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="b4d66-198">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="b4d66-199">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="b4d66-199">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-200">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-200">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-201">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="b4d66-201">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="b4d66-202">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-202">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="b4d66-203">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="b4d66-203">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="b4d66-204">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="b4d66-204">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="b4d66-205">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-205">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="b4d66-206">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-206">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="b4d66-207">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="b4d66-207">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="b4d66-208">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="b4d66-208">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="b4d66-209">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-209">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="b4d66-210">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="b4d66-210">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="b4d66-211">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-211">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="b4d66-212">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="b4d66-212">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="b4d66-213">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-213">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="b4d66-214">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-214">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="b4d66-215">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-215">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="b4d66-216">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="b4d66-216">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="b4d66-217">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-217">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="b4d66-218">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-218">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="b4d66-219">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-219">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="b4d66-220">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-220">Overall improved help files</span></span>
* <span data-ttu-id="b4d66-221">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-221">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-222">Az.Network</span></span>
* <span data-ttu-id="b4d66-223">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-223">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="b4d66-224">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-224">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="b4d66-225">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-225">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="b4d66-226">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-226">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="b4d66-227">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-227">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="b4d66-228">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-228">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="b4d66-229">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-229">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="b4d66-230">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-230">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="b4d66-231">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-231">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="b4d66-232">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-232">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="b4d66-233">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-233">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="b4d66-234">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-234">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="b4d66-235">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-235">New cmdlets</span></span>
        - <span data-ttu-id="b4d66-236">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="b4d66-236">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="b4d66-237">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-237">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="b4d66-238">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-238">Updated cmdlet:</span></span>
        - <span data-ttu-id="b4d66-239">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="b4d66-239">New-VpnSite</span></span>
        - <span data-ttu-id="b4d66-240">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="b4d66-240">Update-VpnSite</span></span>
        - <span data-ttu-id="b4d66-241">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-241">New-VpnConnection</span></span>
        - <span data-ttu-id="b4d66-242">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-242">Update-VpnConnection</span></span>
* <span data-ttu-id="b4d66-243">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-243">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-244">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-244">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-245">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-245">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="b4d66-246">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-246">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-247">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-247">Az.Resources</span></span>
* <span data-ttu-id="b4d66-248">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-248">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-249">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-249">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-250">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-250">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="b4d66-251">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-251">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="b4d66-252">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="b4d66-252">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="b4d66-253">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="b4d66-253">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="b4d66-254">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="b4d66-254">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="b4d66-255">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="b4d66-255">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="b4d66-256">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="b4d66-256">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="b4d66-257">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="b4d66-257">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="b4d66-258">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="b4d66-258">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="b4d66-259">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="b4d66-259">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="b4d66-260">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="b4d66-260">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="b4d66-261">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="b4d66-261">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="b4d66-262">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="b4d66-262">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="b4d66-263">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="b4d66-263">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="b4d66-264">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="b4d66-264">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="b4d66-265">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-265">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="b4d66-266">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="b4d66-266">Az.SignalR</span></span>
* <span data-ttu-id="b4d66-267">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="b4d66-267">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-268">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-268">Az.Sql</span></span>
* <span data-ttu-id="b4d66-269">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-269">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="b4d66-270">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-270">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="b4d66-271">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="b4d66-271">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="b4d66-272">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-272">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="b4d66-273">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="b4d66-273">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-274">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-274">Az.Storage</span></span>
* <span data-ttu-id="b4d66-275">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-275">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="b4d66-276">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="b4d66-276">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="b4d66-277">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-277">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="b4d66-278">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-278">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="b4d66-279">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-279">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="b4d66-280">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-280">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="b4d66-281">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="b4d66-281">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="b4d66-282">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="b4d66-282">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="b4d66-283">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="b4d66-283">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="b4d66-284">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="b4d66-284">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="b4d66-285">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="b4d66-285">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-286">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-286">Az.Websites</span></span>
* <span data-ttu-id="b4d66-287">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-287">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="b4d66-288">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="b4d66-288">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="b4d66-289">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-289">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="b4d66-290">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-290">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="b4d66-291">全般</span><span class="sxs-lookup"><span data-stu-id="b4d66-291">General</span></span>
* <span data-ttu-id="b4d66-292">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-292">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="b4d66-293">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-293">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-294">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="b4d66-294">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="b4d66-295">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="b4d66-295">Az.Aks</span></span>
* <span data-ttu-id="b4d66-296">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-296">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="b4d66-297">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="b4d66-297">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="b4d66-298">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-298">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-299">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="b4d66-299">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="b4d66-300">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="b4d66-300">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="b4d66-301">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-301">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="b4d66-302">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="b4d66-302">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="b4d66-303">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-303">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="b4d66-304">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="b4d66-304">Az.Batch</span></span>
* <span data-ttu-id="b4d66-305">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-305">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="b4d66-306">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="b4d66-306">Az.Cdn</span></span>
* <span data-ttu-id="b4d66-307">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-307">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-308">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-308">Az.Compute</span></span>
* <span data-ttu-id="b4d66-309">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-309">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="b4d66-310">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-310">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="b4d66-311">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-311">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="b4d66-312">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-312">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="b4d66-313">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="b4d66-313">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="b4d66-314">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="b4d66-314">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="b4d66-315">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-315">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="b4d66-316">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-316">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-317">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-317">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-318">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-318">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="b4d66-319">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-319">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="b4d66-320">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-320">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="b4d66-321">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-321">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-322">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-322">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-323">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-323">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="b4d66-324">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-324">Az.EventHub</span></span>
* <span data-ttu-id="b4d66-325">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="b4d66-325">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="b4d66-326">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="b4d66-326">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="b4d66-327">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-327">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="b4d66-328">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="b4d66-328">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="b4d66-329">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="b4d66-329">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="b4d66-330">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-330">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-331">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-331">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-332">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-332">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-333">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-333">Az.Network</span></span>
* <span data-ttu-id="b4d66-334">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-334">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="b4d66-335">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-335">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="b4d66-336">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-336">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="b4d66-337">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-337">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="b4d66-338">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-338">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="b4d66-339">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-339">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="b4d66-340">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-340">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-341">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-341">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-342">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-342">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="b4d66-343">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-343">Added example</span></span>
    - <span data-ttu-id="b4d66-344">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-344">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="b4d66-345">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-345">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="b4d66-346">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-346">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-347">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-347">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-348">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-348">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-349">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-349">Az.Resources</span></span>
* <span data-ttu-id="b4d66-350">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-350">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="b4d66-351">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-351">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="b4d66-352">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="b4d66-352">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="b4d66-353">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-353">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-354">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-354">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-355">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="b4d66-355">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="b4d66-356">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="b4d66-356">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="b4d66-357">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-357">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-358">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-359">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-359">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="b4d66-360">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="b4d66-360">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="b4d66-361">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="b4d66-361">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="b4d66-362">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-362">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="b4d66-363">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="b4d66-363">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="b4d66-364">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-364">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-365">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-365">Az.Sql</span></span>
* <span data-ttu-id="b4d66-366">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-366">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-367">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-367">Az.Storage</span></span>
* <span data-ttu-id="b4d66-368">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-368">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="b4d66-369">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="b4d66-369">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="b4d66-370">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-370">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="b4d66-371">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="b4d66-371">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="b4d66-372">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="b4d66-372">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="b4d66-373">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="b4d66-373">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-374">Az.Websites</span></span>
* <span data-ttu-id="b4d66-375">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-375">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="b4d66-376">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-376">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-377">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-377">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-378">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-378">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="b4d66-379">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-379">Az.ApplicationInsights</span></span>
* <span data-ttu-id="b4d66-380">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-380">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="b4d66-381">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-381">Az.Automation</span></span>
* <span data-ttu-id="b4d66-382">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-382">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-383">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-383">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-384">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-384">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-385">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-385">Az.Compute</span></span>
* <span data-ttu-id="b4d66-386">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-386">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="b4d66-387">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="b4d66-387">Az.ContainerRegistry</span></span>
* <span data-ttu-id="b4d66-388">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-388">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="b4d66-389">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="b4d66-389">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-390">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-390">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-391">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-391">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="b4d66-392">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-392">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="b4d66-393">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-393">Az.EventHub</span></span>
* <span data-ttu-id="b4d66-394">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="b4d66-394">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="b4d66-395">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-395">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="b4d66-396">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-396">Az.KeyVault</span></span>
* <span data-ttu-id="b4d66-397">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-397">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="b4d66-398">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="b4d66-398">Az.LogicApp</span></span>
* <span data-ttu-id="b4d66-399">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-399">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="b4d66-400">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-400">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="b4d66-401">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-401">Az.ManagedServices</span></span>
* <span data-ttu-id="b4d66-402">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-402">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-403">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-403">Az.Network</span></span>
* <span data-ttu-id="b4d66-404">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-404">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="b4d66-405">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-405">New cmdlets</span></span>
        - <span data-ttu-id="b4d66-406">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="b4d66-406">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="b4d66-407">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="b4d66-407">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="b4d66-408">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-408">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="b4d66-409">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-409">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="b4d66-410">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-410">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="b4d66-411">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-411">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="b4d66-412">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="b4d66-412">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="b4d66-413">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="b4d66-413">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="b4d66-414">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="b4d66-414">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="b4d66-415">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-415">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="b4d66-416">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-416">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="b4d66-417">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-417">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="b4d66-418">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="b4d66-418">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="b4d66-419">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-419">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="b4d66-420">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-420">Updated cmdlets</span></span>
        - <span data-ttu-id="b4d66-421">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-421">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="b4d66-422">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-422">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="b4d66-423">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-423">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="b4d66-424">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-424">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="b4d66-425">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-425">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="b4d66-426">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-426">Updated cmdlet:</span></span>
        - <span data-ttu-id="b4d66-427">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-427">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="b4d66-428">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-428">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="b4d66-429">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-429">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="b4d66-430">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-430">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="b4d66-431">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-431">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="b4d66-432">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-432">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-433">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-433">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-434">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-434">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="b4d66-435">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-435">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-436">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-436">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-437">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-437">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="b4d66-438">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-438">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="b4d66-439">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-439">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="b4d66-440">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-440">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="b4d66-441">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-441">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="b4d66-442">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-442">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="b4d66-443">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-443">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="b4d66-444">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-444">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="b4d66-445">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-445">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="b4d66-446">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-446">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-447">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-447">Az.Resources</span></span>
- <span data-ttu-id="b4d66-448">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-448">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="b4d66-449">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-449">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-450">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-450">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-451">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="b4d66-451">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="b4d66-452">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-452">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-453">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-453">Az.Sql</span></span>
* <span data-ttu-id="b4d66-454">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-454">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="b4d66-455">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-455">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="b4d66-456">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-456">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-457">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-457">Az.Storage</span></span>
* <span data-ttu-id="b4d66-458">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-458">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="b4d66-459">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="b4d66-459">Az.StorageSync</span></span>
* <span data-ttu-id="b4d66-460">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-460">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="b4d66-461">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-461">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-462">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-462">Az.Websites</span></span>
* <span data-ttu-id="b4d66-463">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-463">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="b4d66-464">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-464">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="b4d66-465">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-465">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="b4d66-466">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-466">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-467">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-467">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-468">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-468">Add support for profile cmdlets</span></span>
* <span data-ttu-id="b4d66-469">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-469">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="b4d66-470">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-470">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="b4d66-471">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="b4d66-471">Az.Advisor</span></span>
* <span data-ttu-id="b4d66-472">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-472">GA release of Az.Advisor</span></span>
* <span data-ttu-id="b4d66-473">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-473">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="b4d66-474">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-474">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-475">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="b4d66-475">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="b4d66-476">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="b4d66-476">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="b4d66-477">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-477">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="b4d66-478">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-478">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="b4d66-479">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-479">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="b4d66-480">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="b4d66-480">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="b4d66-481">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-481">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-482">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-482">Az.Automation</span></span>
* <span data-ttu-id="b4d66-483">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-483">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-484">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-484">Az.Compute</span></span>
* <span data-ttu-id="b4d66-485">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-485">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-486">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-486">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-487">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-487">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="b4d66-488">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="b4d66-488">Az.EventGrid</span></span>
* <span data-ttu-id="b4d66-489">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-489">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-490">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-490">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-491">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-491">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-492">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-492">Az.Network</span></span>
* <span data-ttu-id="b4d66-493">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-493">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="b4d66-494">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-494">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="b4d66-495">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-495">Az.PolicyInsights</span></span>
* <span data-ttu-id="b4d66-496">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-496">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="b4d66-497">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="b4d66-497">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-498">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-498">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-499">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-499">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-500">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-500">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-501">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-501">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-502">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-502">Az.Resources</span></span>
    - <span data-ttu-id="b4d66-503">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-503">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="b4d66-504">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-504">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="b4d66-505">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-505">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="b4d66-506">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-506">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-507">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-507">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-508">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="b4d66-508">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-509">Az.Sql</span></span>
* <span data-ttu-id="b4d66-510">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-510">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="b4d66-511">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-511">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="b4d66-512">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-512">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="b4d66-513">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-513">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="b4d66-514">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-514">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="b4d66-515">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-515">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="b4d66-516">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-516">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="b4d66-517">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="b4d66-517">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="b4d66-518">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-518">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-519">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-519">Az.Storage</span></span>
* <span data-ttu-id="b4d66-520">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-520">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="b4d66-521">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="b4d66-521">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="b4d66-522">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-522">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="b4d66-523">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="b4d66-523">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="b4d66-524">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-524">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="b4d66-525">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-525">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="b4d66-526">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-526">Set-AzStorageAccount</span></span>
* <span data-ttu-id="b4d66-527">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-527">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="b4d66-528">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="b4d66-528">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="b4d66-529">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="b4d66-529">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="b4d66-530">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="b4d66-530">Az.StorageSync</span></span>
* <span data-ttu-id="b4d66-531">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-531">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="b4d66-532">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-532">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-533">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-533">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-534">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-534">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="b4d66-535">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="b4d66-535">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="b4d66-536">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-536">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="b4d66-537">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="b4d66-537">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="b4d66-538">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="b4d66-538">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-539">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-539">Az.Compute</span></span>
* <span data-ttu-id="b4d66-540">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-540">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="b4d66-541">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-541">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="b4d66-542">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="b4d66-542">Az.Dns</span></span>
* <span data-ttu-id="b4d66-543">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-543">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="b4d66-544">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="b4d66-544">Az.EventGrid</span></span>
* <span data-ttu-id="b4d66-545">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-545">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="b4d66-546">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-546">New cmdlets:</span></span>
    - <span data-ttu-id="b4d66-547">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="b4d66-547">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="b4d66-548">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-548">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="b4d66-549">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="b4d66-549">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="b4d66-550">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-550">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="b4d66-551">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="b4d66-551">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="b4d66-552">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-552">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="b4d66-553">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="b4d66-553">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="b4d66-554">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-554">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="b4d66-555">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="b4d66-555">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="b4d66-556">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-556">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="b4d66-557">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="b4d66-557">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="b4d66-558">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-558">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="b4d66-559">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="b4d66-559">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="b4d66-560">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-560">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="b4d66-561">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="b4d66-561">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="b4d66-562">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-562">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="b4d66-563">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-563">Updated cmdlets:</span></span>
    - <span data-ttu-id="b4d66-564">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="b4d66-564">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="b4d66-565">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-565">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="b4d66-566">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-566">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="b4d66-567">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="b4d66-567">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="b4d66-568">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="b4d66-568">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="b4d66-569">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="b4d66-569">Event subscription expiration date,</span></span>
            - <span data-ttu-id="b4d66-570">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="b4d66-570">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="b4d66-571">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-571">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="b4d66-572">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="b4d66-572">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="b4d66-573">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="b4d66-573">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="b4d66-574">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-574">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="b4d66-575">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="b4d66-575">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="b4d66-576">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-576">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="b4d66-577">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-577">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="b4d66-578">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="b4d66-578">Az.FrontDoor</span></span>
* <span data-ttu-id="b4d66-579">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="b4d66-579">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="b4d66-580">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-580">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="b4d66-581">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="b4d66-581">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="b4d66-582">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-582">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-583">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-583">Az.Network</span></span>
* <span data-ttu-id="b4d66-584">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-584">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="b4d66-585">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-585">New cmdlets</span></span>
        - <span data-ttu-id="b4d66-586">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="b4d66-586">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="b4d66-587">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-587">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="b4d66-588">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-588">New cmdlets</span></span> 
        - <span data-ttu-id="b4d66-589">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="b4d66-589">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="b4d66-590">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-590">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="b4d66-591">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-591">New cmdlets</span></span> 
        - <span data-ttu-id="b4d66-592">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="b4d66-592">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="b4d66-593">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="b4d66-593">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="b4d66-594">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="b4d66-594">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="b4d66-595">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-595">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="b4d66-596">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-596">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="b4d66-597">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-597">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="b4d66-598">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-598">New cmdlets</span></span>
        - <span data-ttu-id="b4d66-599">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="b4d66-599">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="b4d66-600">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="b4d66-600">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="b4d66-601">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="b4d66-601">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="b4d66-602">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="b4d66-602">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="b4d66-603">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="b4d66-603">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="b4d66-604">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-604">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="b4d66-605">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-605">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="b4d66-606">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-606">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="b4d66-607">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-607">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="b4d66-608">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-608">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="b4d66-609">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-609">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="b4d66-610">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-610">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="b4d66-611">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-611">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="b4d66-612">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-612">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="b4d66-613">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-613">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="b4d66-614">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-614">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="b4d66-615">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-615">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="b4d66-616">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-616">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="b4d66-617">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="b4d66-617">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="b4d66-618">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-618">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="b4d66-619">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-619">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="b4d66-620">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="b4d66-620">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="b4d66-621">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-621">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="b4d66-622">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-622">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="b4d66-623">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-623">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="b4d66-624">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-624">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="b4d66-625">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-625">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-626">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-626">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-627">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-627">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-628">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-628">Az.Resources</span></span>
* <span data-ttu-id="b4d66-629">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="b4d66-629">Support for additional Template Export options</span></span>
    - <span data-ttu-id="b4d66-630">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-630">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="b4d66-631">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-631">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="b4d66-632">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-632">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-633">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-633">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-634">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-634">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-635">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-635">Az.Sql</span></span>
* <span data-ttu-id="b4d66-636">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-636">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="b4d66-637">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-637">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="b4d66-638">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-638">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="b4d66-639">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="b4d66-639">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="b4d66-640">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="b4d66-640">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="b4d66-641">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="b4d66-641">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="b4d66-642">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="b4d66-642">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="b4d66-643">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="b4d66-643">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-644">Az.Storage</span></span>
* <span data-ttu-id="b4d66-645">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-645">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="b4d66-646">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-646">New-AzStorageAccount</span></span>
* <span data-ttu-id="b4d66-647">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-647">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="b4d66-648">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-648">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-649">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-649">Az.Websites</span></span>
* <span data-ttu-id="b4d66-650">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-650">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="b4d66-651">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-651">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="b4d66-652">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-652">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="b4d66-653">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="b4d66-653">Az.Cdn</span></span>
* <span data-ttu-id="b4d66-654">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-654">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-655">Az.Compute</span></span>
* <span data-ttu-id="b4d66-656">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-656">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="b4d66-657">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="b4d66-657">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="b4d66-658">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-658">Az.EventHub</span></span>
* <span data-ttu-id="b4d66-659">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-659">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="b4d66-660">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-660">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-661">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-661">Az.Network</span></span>
* <span data-ttu-id="b4d66-662">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-662">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="b4d66-663">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-663">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="b4d66-664">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-664">Az.PolicyInsights</span></span>
* <span data-ttu-id="b4d66-665">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-665">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-666">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-666">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-667">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-667">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-668">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-668">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-669">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-669">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-670">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-670">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-671">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-671">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="b4d66-672">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-672">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-673">Az.Sql</span></span>
* <span data-ttu-id="b4d66-674">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-674">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="b4d66-675">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="b4d66-675">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="b4d66-676">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-676">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="b4d66-677">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-677">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-678">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-678">Az.Websites</span></span>
* <span data-ttu-id="b4d66-679">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-679">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="b4d66-680">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-680">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="b4d66-681">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-681">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-682">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-682">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="b4d66-683">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="b4d66-683">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="b4d66-684">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="b4d66-684">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="b4d66-685">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="b4d66-685">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="b4d66-686">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-686">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="b4d66-687">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="b4d66-687">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="b4d66-688">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="b4d66-688">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="b4d66-689">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-689">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="b4d66-690">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-690">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="b4d66-691">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="b4d66-691">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="b4d66-692">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="b4d66-692">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="b4d66-693">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="b4d66-693">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="b4d66-694">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-694">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="b4d66-695">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-695">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="b4d66-696">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="b4d66-696">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="b4d66-697">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="b4d66-697">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="b4d66-698">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="b4d66-698">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="b4d66-699">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="b4d66-699">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="b4d66-700">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-700">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="b4d66-701">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="b4d66-701">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="b4d66-702">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-702">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="b4d66-703">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-703">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="b4d66-704">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="b4d66-704">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="b4d66-705">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-705">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="b4d66-706">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-706">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="b4d66-707">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-707">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="b4d66-708">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-708">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="b4d66-709">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-709">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="b4d66-710">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-710">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="b4d66-711">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-711">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="b4d66-712">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-712">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="b4d66-713">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="b4d66-713">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="b4d66-714">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-714">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="b4d66-715">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-715">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="b4d66-716">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="b4d66-716">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="b4d66-717">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="b4d66-717">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="b4d66-718">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="b4d66-718">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="b4d66-719">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-719">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="b4d66-720">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-720">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="b4d66-721">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-721">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="b4d66-722">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="b4d66-722">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="b4d66-723">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="b4d66-723">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="b4d66-724">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="b4d66-724">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="b4d66-725">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-725">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="b4d66-726">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-726">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="b4d66-727">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="b4d66-727">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="b4d66-728">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="b4d66-728">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="b4d66-729">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-729">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="b4d66-730">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-730">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="b4d66-731">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="b4d66-731">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="b4d66-732">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="b4d66-732">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="b4d66-733">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="b4d66-733">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="b4d66-734">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="b4d66-734">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="b4d66-735">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-735">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="b4d66-736">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="b4d66-736">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="b4d66-737">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="b4d66-737">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="b4d66-738">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-738">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="b4d66-739">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="b4d66-739">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="b4d66-740">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="b4d66-740">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="b4d66-741">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-741">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="b4d66-742">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-742">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="b4d66-743">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="b4d66-743">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="b4d66-744">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="b4d66-744">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="b4d66-745">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-745">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="b4d66-746">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-746">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="b4d66-747">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="b4d66-747">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="b4d66-748">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="b4d66-748">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="b4d66-749">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="b4d66-749">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="b4d66-750">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="b4d66-750">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="b4d66-751">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="b4d66-751">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="b4d66-752">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="b4d66-752">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="b4d66-753">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="b4d66-753">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="b4d66-754">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="b4d66-754">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="b4d66-755">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-755">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="b4d66-756">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="b4d66-756">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="b4d66-757">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="b4d66-757">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="b4d66-758">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="b4d66-758">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-759">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-759">Az.Automation</span></span>
* <span data-ttu-id="b4d66-760">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-760">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="b4d66-761">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="b4d66-761">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="b4d66-762">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="b4d66-762">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="b4d66-763">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-763">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="b4d66-764">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="b4d66-764">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="b4d66-765">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-765">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="b4d66-766">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-766">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-767">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-767">Az.Compute</span></span>
* <span data-ttu-id="b4d66-768">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-768">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="b4d66-769">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-769">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-770">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-770">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-771">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-771">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-772">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-772">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-773">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-773">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-774">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-774">Az.Network</span></span>
* <span data-ttu-id="b4d66-775">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-775">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="b4d66-776">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="b4d66-776">Updated cmdlet:</span></span>
        - <span data-ttu-id="b4d66-777">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="b4d66-777">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="b4d66-778">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-778">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-779">Az.Resources</span></span>
* <span data-ttu-id="b4d66-780">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-780">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-781">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-781">Az.Sql</span></span>
* <span data-ttu-id="b4d66-782">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-782">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="b4d66-783">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-783">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-784">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-784">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-785">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-785">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-786">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-786">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-787">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-787">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="b4d66-788">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-788">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-789">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-789">Az.Compute</span></span>
* <span data-ttu-id="b4d66-790">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="b4d66-790">Proximity placement group feature.</span></span>
    - <span data-ttu-id="b4d66-791">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="b4d66-791">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="b4d66-792">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-792">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="b4d66-793">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-793">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="b4d66-794">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-794">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="b4d66-795">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-795">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="b4d66-796">重大な変更</span><span class="sxs-lookup"><span data-stu-id="b4d66-796">Breaking changes</span></span>
    - <span data-ttu-id="b4d66-797">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="b4d66-797">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="b4d66-798">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="b4d66-798">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="b4d66-799">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="b4d66-799">Az.DeploymentManager</span></span>
* <span data-ttu-id="b4d66-800">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-800">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="b4d66-801">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="b4d66-801">Az.Dns</span></span>
* <span data-ttu-id="b4d66-802">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="b4d66-802">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="b4d66-803">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-803">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="b4d66-804">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-804">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="b4d66-805">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="b4d66-805">Az.FrontDoor</span></span>
* <span data-ttu-id="b4d66-806">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-806">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="b4d66-807">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-807">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="b4d66-808">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="b4d66-808">Az.HDInsight</span></span>
* <span data-ttu-id="b4d66-809">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-809">Removed two cmdlets:</span></span>
    - <span data-ttu-id="b4d66-810">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="b4d66-810">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="b4d66-811">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="b4d66-811">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="b4d66-812">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-812">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="b4d66-813">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-813">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="b4d66-814">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-814">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="b4d66-815">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="b4d66-815">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-816">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-816">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-817">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="b4d66-817">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="b4d66-818">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="b4d66-818">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="b4d66-819">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="b4d66-819">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="b4d66-820">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="b4d66-820">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="b4d66-821">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="b4d66-821">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="b4d66-822">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="b4d66-822">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="b4d66-823">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="b4d66-823">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="b4d66-824">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-824">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="b4d66-825">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-825">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="b4d66-826">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-826">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="b4d66-827">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-827">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="b4d66-828">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-828">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="b4d66-829">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="b4d66-829">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="b4d66-830">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-830">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-831">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-831">Az.Network</span></span>
* <span data-ttu-id="b4d66-832">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-832">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="b4d66-833">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-833">New cmdlets</span></span>
        - <span data-ttu-id="b4d66-834">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="b4d66-834">New-AzNatGateway</span></span>
        - <span data-ttu-id="b4d66-835">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="b4d66-835">Get-AzNatGateway</span></span>
        - <span data-ttu-id="b4d66-836">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="b4d66-836">Set-AzNatGateway</span></span>
        - <span data-ttu-id="b4d66-837">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="b4d66-837">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="b4d66-838">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-838">Updated cmdlets</span></span>
        - <span data-ttu-id="b4d66-839">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="b4d66-839">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="b4d66-840">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="b4d66-840">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="b4d66-841">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="b4d66-841">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="b4d66-842">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-842">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="b4d66-843">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-843">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="b4d66-844">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-844">Az.PolicyInsights</span></span>
* <span data-ttu-id="b4d66-845">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="b4d66-845">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="b4d66-846">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-846">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="b4d66-847">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-847">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-848">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-848">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-849">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="b4d66-849">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="b4d66-850">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="b4d66-850">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="b4d66-851">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="b4d66-851">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="b4d66-852">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="b4d66-852">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="b4d66-853">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="b4d66-853">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="b4d66-854">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="b4d66-854">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="b4d66-855">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="b4d66-855">Az.Relay</span></span>
* <span data-ttu-id="b4d66-856">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-856">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-857">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-857">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-858">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-858">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-859">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-859">Az.Storage</span></span>
* <span data-ttu-id="b4d66-860">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="b4d66-860">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="b4d66-861">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-861">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="b4d66-862">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-862">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="b4d66-863">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-863">New-AzStorageAccount</span></span>
* <span data-ttu-id="b4d66-864">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="b4d66-864">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="b4d66-865">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-865">New-AzStorageAccount</span></span>
    - <span data-ttu-id="b4d66-866">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-866">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="b4d66-867">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="b4d66-867">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-868">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-868">Az.Websites</span></span>
* <span data-ttu-id="b4d66-869">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="b4d66-869">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="b4d66-870">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="b4d66-870">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="b4d66-871">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-871">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="b4d66-872">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="b4d66-872">Highlights since the last major release</span></span>
* <span data-ttu-id="b4d66-873">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="b4d66-873">General availability of `Az` module</span></span>
* <span data-ttu-id="b4d66-874">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="b4d66-874">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="b4d66-875">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="b4d66-875">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="b4d66-876">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-876">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="b4d66-877">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-877">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="b4d66-878">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-878">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="b4d66-879">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-879">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="b4d66-880">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-880">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-881">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-881">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="b4d66-882">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="b4d66-882">Az.Batch</span></span>
* <span data-ttu-id="b4d66-883">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-883">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="b4d66-884">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="b4d66-884">Az.Cdn</span></span>
* <span data-ttu-id="b4d66-885">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-885">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-886">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-886">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-887">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-887">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-888">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-888">Az.Compute</span></span>
* <span data-ttu-id="b4d66-889">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-889">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="b4d66-890">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-891">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-891">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-892">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-892">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-893">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-893">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-894">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-894">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-895">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-895">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="b4d66-896">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="b4d66-896">Az.EventGrid</span></span>
* <span data-ttu-id="b4d66-897">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-897">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="b4d66-898">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-898">Az.EventHub</span></span>
* <span data-ttu-id="b4d66-899">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-899">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="b4d66-900">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="b4d66-900">Az.HDInsight</span></span>
* <span data-ttu-id="b4d66-901">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-901">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-902">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-902">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-903">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-903">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="b4d66-904">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-904">Az.KeyVault</span></span>
* <span data-ttu-id="b4d66-905">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-905">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-906">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-906">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="b4d66-907">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="b4d66-907">Az.MachineLearning</span></span>
* <span data-ttu-id="b4d66-908">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-908">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="b4d66-909">Az.Media</span><span class="sxs-lookup"><span data-stu-id="b4d66-909">Az.Media</span></span>
* <span data-ttu-id="b4d66-910">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-911">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-911">Az.Monitor</span></span>
  * <span data-ttu-id="b4d66-912">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-912">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="b4d66-913">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="b4d66-913">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="b4d66-914">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="b4d66-914">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="b4d66-915">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="b4d66-915">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="b4d66-916">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="b4d66-916">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="b4d66-917">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="b4d66-917">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="b4d66-918">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-918">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-919">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-919">Az.Network</span></span>
* <span data-ttu-id="b4d66-920">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-920">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-921">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-921">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="b4d66-922">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="b4d66-922">Az.NotificationHubs</span></span>
* <span data-ttu-id="b4d66-923">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-923">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-924">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-924">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-925">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-925">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="b4d66-926">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="b4d66-926">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="b4d66-927">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-927">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-928">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-928">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-929">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-929">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-930">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-930">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="b4d66-931">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-931">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="b4d66-932">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-932">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="b4d66-933">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="b4d66-933">Az.RedisCache</span></span>
* <span data-ttu-id="b4d66-934">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-934">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-935">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-935">Az.Resources</span></span>
* <span data-ttu-id="b4d66-936">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-936">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-937">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-937">Az.Sql</span></span>
* <span data-ttu-id="b4d66-938">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="b4d66-938">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="b4d66-939">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-939">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-940">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-940">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="b4d66-941">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-941">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="b4d66-942">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="b4d66-942">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="b4d66-943">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="b4d66-943">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="b4d66-944">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-944">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-945">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-945">Az.Websites</span></span>
* <span data-ttu-id="b4d66-946">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-946">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="b4d66-947">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-947">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="b4d66-948">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-948">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="b4d66-949">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-949">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="b4d66-950">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-950">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="b4d66-951">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="b4d66-951">Highlights since the last major release</span></span>
* <span data-ttu-id="b4d66-952">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="b4d66-952">General availability of `Az` module</span></span>
* <span data-ttu-id="b4d66-953">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="b4d66-953">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="b4d66-954">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="b4d66-954">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="b4d66-955">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-955">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="b4d66-956">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-956">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="b4d66-957">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-957">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="b4d66-958">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-958">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="b4d66-959">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-959">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-960">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-960">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="b4d66-961">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-961">Az.AnalysisServices</span></span>
* <span data-ttu-id="b4d66-962">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="b4d66-962">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="b4d66-963">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-963">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-964">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-964">Az.Automation</span></span>
* <span data-ttu-id="b4d66-965">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-965">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="b4d66-966">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-966">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="b4d66-967">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-967">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-968">Az.Compute</span></span>
* <span data-ttu-id="b4d66-969">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-969">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="b4d66-970">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-970">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="b4d66-971">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-971">Az.ContainerInstance</span></span>
* <span data-ttu-id="b4d66-972">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-972">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-973">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-973">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-974">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-974">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="b4d66-975">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-975">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-976">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-976">Az.Resources</span></span>
* <span data-ttu-id="b4d66-977">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-977">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="b4d66-978">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-978">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="b4d66-979">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="b4d66-979">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="b4d66-980">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="b4d66-980">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="b4d66-981">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-981">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="b4d66-982">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="b4d66-982">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-983">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-983">Az.Sql</span></span>
* <span data-ttu-id="b4d66-984">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-984">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-985">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-985">Az.Storage</span></span>
* <span data-ttu-id="b4d66-986">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="b4d66-986">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="b4d66-987">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="b4d66-987">New-AzStorageContext</span></span>
* <span data-ttu-id="b4d66-988">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="b4d66-988">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="b4d66-989">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="b4d66-989">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="b4d66-990">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="b4d66-990">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="b4d66-991">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-991">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="b4d66-992">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-992">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="b4d66-993">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="b4d66-993">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="b4d66-994">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-994">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="b4d66-995">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-995">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="b4d66-996">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-996">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="b4d66-997">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="b4d66-997">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="b4d66-998">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-998">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="b4d66-999">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="b4d66-999">Highlights since the last major release</span></span>
* <span data-ttu-id="b4d66-1000">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="b4d66-1000">General availability of `Az` module</span></span>
* <span data-ttu-id="b4d66-1001">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="b4d66-1001">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="b4d66-1002">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="b4d66-1002">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="b4d66-1003">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1003">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="b4d66-1004">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1004">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="b4d66-1005">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1005">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="b4d66-1006">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1006">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-1007">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-1007">Az.Automation</span></span>
* <span data-ttu-id="b4d66-1008">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1008">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="b4d66-1009">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="b4d66-1009">Dynamic grouping</span></span>
    * <span data-ttu-id="b4d66-1010">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="b4d66-1010">Pre-Post script</span></span>
    * <span data-ttu-id="b4d66-1011">再起動設定</span><span class="sxs-lookup"><span data-stu-id="b4d66-1011">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1012">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1012">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1013">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1013">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="b4d66-1014">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1014">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="b4d66-1015">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-1015">Az.KeyVault</span></span>
* <span data-ttu-id="b4d66-1016">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1016">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1017">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1017">Az.Network</span></span>
* <span data-ttu-id="b4d66-1018">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1018">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="b4d66-1019">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1019">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1020">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1020">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-1021">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1021">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="b4d66-1022">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1022">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1023">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1023">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1024">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1024">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="b4d66-1025">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1025">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1026">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1026">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1027">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1027">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-1028">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1028">Az.Storage</span></span>
* <span data-ttu-id="b4d66-1029">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-1029">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="b4d66-1030">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1030">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="b4d66-1031">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1031">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="b4d66-1032">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1032">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="b4d66-1033">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="b4d66-1033">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="b4d66-1034">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="b4d66-1034">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="b4d66-1035">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-1035">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-1036">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1036">Az.Websites</span></span>
* <span data-ttu-id="b4d66-1037">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1037">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="b4d66-1038">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1038">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-1039">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1039">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-1040">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1040">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="b4d66-1041">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1041">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-1042">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-1042">Az.Automation</span></span>
* <span data-ttu-id="b4d66-1043">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1043">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="b4d66-1044">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1044">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="b4d66-1045">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1045">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="b4d66-1046">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="b4d66-1046">Az.Cdn</span></span>
* <span data-ttu-id="b4d66-1047">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1047">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1048">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1048">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1049">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1049">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-1050">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-1050">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-1051">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1051">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="b4d66-1052">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="b4d66-1052">Az.LogicApp</span></span>
* <span data-ttu-id="b4d66-1053">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1053">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1054">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1054">Az.Network</span></span>
* <span data-ttu-id="b4d66-1055">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1055">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1056">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1056">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-1057">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1057">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="b4d66-1058">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1058">SDK Update</span></span>
* <span data-ttu-id="b4d66-1059">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1059">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="b4d66-1060">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1060">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1061">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1061">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1062">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1062">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="b4d66-1063">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="b4d66-1063">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="b4d66-1064">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1064">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="b4d66-1065">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="b4d66-1065">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="b4d66-1066">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1066">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="b4d66-1067">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="b4d66-1067">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1068">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1068">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1069">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1069">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="b4d66-1070">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1070">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-1071">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1071">Az.Storage</span></span>
* <span data-ttu-id="b4d66-1072">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1072">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="b4d66-1073">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1073">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="b4d66-1074">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1074">Az.AnalysisServices</span></span>
* <span data-ttu-id="b4d66-1075">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1075">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-1076">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-1076">Az.Automation</span></span>
* <span data-ttu-id="b4d66-1077">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1077">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="b4d66-1078">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1078">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="b4d66-1079">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1079">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-1080">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1080">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-1081">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1081">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1082">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1082">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1083">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1083">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="b4d66-1084">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1084">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="b4d66-1085">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1085">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="b4d66-1086">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1086">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1087">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1087">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-1088">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1088">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="b4d66-1089">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-1089">Az.EventHub</span></span>
* <span data-ttu-id="b4d66-1090">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1090">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="b4d66-1091">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-1091">Az.KeyVault</span></span>
* <span data-ttu-id="b4d66-1092">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1092">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="b4d66-1093">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="b4d66-1093">Az.LogicApp</span></span>
* <span data-ttu-id="b4d66-1094">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1094">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="b4d66-1095">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1095">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="b4d66-1096">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1096">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="b4d66-1097">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="b4d66-1097">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="b4d66-1098">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="b4d66-1098">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="b4d66-1099">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="b4d66-1099">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="b4d66-1100">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="b4d66-1100">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="b4d66-1101">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1101">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="b4d66-1102">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4d66-1102">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="b4d66-1103">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4d66-1103">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="b4d66-1104">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4d66-1104">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="b4d66-1105">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4d66-1105">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="b4d66-1106">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1106">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="b4d66-1107">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-1107">Az.Monitor</span></span>
* <span data-ttu-id="b4d66-1108">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1108">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1109">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1109">Az.Network</span></span>
* <span data-ttu-id="b4d66-1110">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1110">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-1111">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-1111">Az.OperationalInsights</span></span>
* <span data-ttu-id="b4d66-1112">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1112">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="b4d66-1113">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1113">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="b4d66-1114">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1114">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="b4d66-1115">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1115">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1116">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="b4d66-1116">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="b4d66-1117">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="b4d66-1117">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="b4d66-1118">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="b4d66-1118">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="b4d66-1119">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1119">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1120">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1120">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1121">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1121">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="b4d66-1122">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1122">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-1123">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1123">Az.Websites</span></span>
* <span data-ttu-id="b4d66-1124">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1124">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="b4d66-1125">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1125">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-1126">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1126">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-1127">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1127">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="b4d66-1128">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1128">Az.AnalysisServices</span></span>
<span data-ttu-id="b4d66-1129">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="b4d66-1129">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1130">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1130">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1131">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1131">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="b4d66-1132">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1132">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="b4d66-1133">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1133">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1134">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1134">Az.RecoveryServices</span></span>
<span data-ttu-id="b4d66-1135">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="b4d66-1135">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1136">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1136">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1137">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1137">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="b4d66-1138">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="b4d66-1138">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="b4d66-1139">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1139">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="b4d66-1140">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="b4d66-1140">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1141">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1141">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1142">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1142">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="b4d66-1143">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1143">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="b4d66-1144">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1144">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="b4d66-1145">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1145">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-1146">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1146">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-1147">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-1147">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="b4d66-1148">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1148">Az.AnalysisServices</span></span>
* <span data-ttu-id="b4d66-1149">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-1149">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1150">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1150">Az.RecoveryServices</span></span>
* <span data-ttu-id="b4d66-1151">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-1151">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="b4d66-1152">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1152">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-1153">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1153">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-1154">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1154">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="b4d66-1155">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1155">Update incorrect online help URLs</span></span>
* <span data-ttu-id="b4d66-1156">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1156">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="b4d66-1157">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="b4d66-1157">Az.Aks</span></span>
* <span data-ttu-id="b4d66-1158">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1158">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="b4d66-1159">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-1159">Az.Automation</span></span>
* <span data-ttu-id="b4d66-1160">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1160">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="b4d66-1161">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1161">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="b4d66-1162">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="b4d66-1162">Az.Cdn</span></span>
* <span data-ttu-id="b4d66-1163">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1163">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1164">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1164">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1165">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1165">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="b4d66-1166">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1166">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="b4d66-1167">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1167">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="b4d66-1168">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="b4d66-1168">Az.ContainerRegistry</span></span>
* <span data-ttu-id="b4d66-1169">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1169">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="b4d66-1170">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="b4d66-1170">Az.DataFactory</span></span>
* <span data-ttu-id="b4d66-1171">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1171">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1172">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1172">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-1173">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="b4d66-1173">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="b4d66-1174">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="b4d66-1174">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="b4d66-1175">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1175">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-1176">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-1176">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-1177">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1177">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="b4d66-1178">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-1178">Az.KeyVault</span></span>
* <span data-ttu-id="b4d66-1179">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1179">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1180">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1180">Az.Network</span></span>
* <span data-ttu-id="b4d66-1181">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1181">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1182">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1182">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1183">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1183">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="b4d66-1184">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1184">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="b4d66-1185">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1185">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="b4d66-1186">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="b4d66-1186">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="b4d66-1187">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="b4d66-1187">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="b4d66-1188">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1188">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="b4d66-1189">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="b4d66-1189">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-1190">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-1190">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-1191">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="b4d66-1191">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="b4d66-1192">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1192">Fix some error messages.</span></span>
* <span data-ttu-id="b4d66-1193">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1193">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="b4d66-1194">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1194">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="b4d66-1195">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="b4d66-1195">Az.SignalR</span></span>
* <span data-ttu-id="b4d66-1196">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1196">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1197">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1197">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1198">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1198">Update incorrect online help URLs</span></span>
* <span data-ttu-id="b4d66-1199">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1199">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="b4d66-1200">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1200">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="b4d66-1201">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-1201">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-1202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1202">Az.Storage</span></span>
* <span data-ttu-id="b4d66-1203">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1203">Update incorrect online help URLs</span></span>
* <span data-ttu-id="b4d66-1204">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="b4d66-1204">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="b4d66-1205">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="b4d66-1205">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="b4d66-1206">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="b4d66-1206">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="b4d66-1207">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="b4d66-1207">Az.TrafficManager</span></span>
* <span data-ttu-id="b4d66-1208">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1208">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-1209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1209">Az.Websites</span></span>
* <span data-ttu-id="b4d66-1210">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1210">Update incorrect online help URLs</span></span>
* <span data-ttu-id="b4d66-1211">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1211">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="b4d66-1212">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="b4d66-1212">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="b4d66-1213">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1213">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="b4d66-1214">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1214">Az.Accounts</span></span>
* <span data-ttu-id="b4d66-1215">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="b4d66-1215">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1216">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1216">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1217">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1217">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="b4d66-1218">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1218">Updated the description of ID in help files</span></span>
* <span data-ttu-id="b4d66-1219">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1219">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1220">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1220">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-1221">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1221">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="b4d66-1222">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1222">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="b4d66-1223">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="b4d66-1223">Az.EventGrid</span></span>
* <span data-ttu-id="b4d66-1224">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1224">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="b4d66-1225">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="b4d66-1225">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="b4d66-1226">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="b4d66-1226">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="b4d66-1227">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="b4d66-1227">Event Time-To-Live,</span></span>
        - <span data-ttu-id="b4d66-1228">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="b4d66-1228">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="b4d66-1229">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="b4d66-1229">Dead letter endpoint.</span></span>
    - <span data-ttu-id="b4d66-1230">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="b4d66-1230">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="b4d66-1231">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="b4d66-1231">Event Time-To-Live,</span></span>
        - <span data-ttu-id="b4d66-1232">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="b4d66-1232">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="b4d66-1233">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="b4d66-1233">Dead letter endpoint.</span></span>
* <span data-ttu-id="b4d66-1234">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1234">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="b4d66-1235">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1235">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="b4d66-1236">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="b4d66-1236">Az.IotHub</span></span>
* <span data-ttu-id="b4d66-1237">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1237">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="b4d66-1238">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="b4d66-1238">Az.LogicApp</span></span>
* <span data-ttu-id="b4d66-1239">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="b4d66-1239">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1240">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1240">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1241">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1241">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="b4d66-1242">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="b4d66-1242">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="b4d66-1243">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1243">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="b4d66-1244">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1244">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="b4d66-1245">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1245">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="b4d66-1246">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="b4d66-1246">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="b4d66-1247">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="b4d66-1247">Az.SignalR</span></span>
* <span data-ttu-id="b4d66-1248">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1248">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1249">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1249">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1250">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1250">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="b4d66-1251">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1251">Az.Storage</span></span>
* <span data-ttu-id="b4d66-1252">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="b4d66-1252">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="b4d66-1253">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="b4d66-1253">New-AzStorageContext</span></span>
* <span data-ttu-id="b4d66-1254">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1254">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="b4d66-1255">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="b4d66-1255">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-1256">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1256">Az.Websites</span></span>
* <span data-ttu-id="b4d66-1257">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1257">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="b4d66-1258">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1258">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="b4d66-1259">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1259">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="b4d66-1260">全般</span><span class="sxs-lookup"><span data-stu-id="b4d66-1260">General</span></span>

- <span data-ttu-id="b4d66-1261">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="b4d66-1261">General Availability of Az Module</span></span>
- <span data-ttu-id="b4d66-1262">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="b4d66-1262">Online help for each module</span></span>
- <span data-ttu-id="b4d66-1263">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1263">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="b4d66-1264">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1264">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="b4d66-1265">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="b4d66-1265">Az.Accounts</span></span>
- <span data-ttu-id="b4d66-1266">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1266">Changed from Az.Profile</span></span>
- <span data-ttu-id="b4d66-1267">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1267">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="b4d66-1268">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-1268">Az.ApiManagement</span></span>
- <span data-ttu-id="b4d66-1269">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="b4d66-1269">Fixes for #7002</span></span>
- <span data-ttu-id="b4d66-1270">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1270">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="b4d66-1271">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="b4d66-1271">Az.Batch</span></span>
- <span data-ttu-id="b4d66-1272">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1272">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="b4d66-1273">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1273">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="b4d66-1274">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1274">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="b4d66-1275">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="b4d66-1275">Az.Billing</span></span>
- <span data-ttu-id="b4d66-1276">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1276">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="b4d66-1277">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1277">Az.CognitivServices</span></span>
- <span data-ttu-id="b4d66-1278">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1278">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="b4d66-1279">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1279">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="b4d66-1280">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1280">Az.ContainerInstance</span></span>
- <span data-ttu-id="b4d66-1281">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1281">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="b4d66-1282">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="b4d66-1282">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="b4d66-1283">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1283">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1284">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1284">Az.DataLakeStore</span></span>
- <span data-ttu-id="b4d66-1285">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1285">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="b4d66-1286">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="b4d66-1286">Az.Monitor</span></span>
- <span data-ttu-id="b4d66-1287">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1287">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="b4d66-1288">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="b4d66-1288">Az.KeyVault</span></span>
- <span data-ttu-id="b4d66-1289">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1289">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="b4d66-1290">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="b4d66-1290">Az.MachineLearning</span></span>
- <span data-ttu-id="b4d66-1291">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1291">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="b4d66-1292">Az.Media</span><span class="sxs-lookup"><span data-stu-id="b4d66-1292">Az.Media</span></span>
- <span data-ttu-id="b4d66-1293">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1293">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="b4d66-1294">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1294">Az.Network</span></span>
<span data-ttu-id="b4d66-1295">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1295">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="b4d66-1296">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="b4d66-1296">New cmdlets added:</span></span>
        - <span data-ttu-id="b4d66-1297">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1297">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1298">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1298">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1299">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1299">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1300">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1300">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1301">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1301">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1302">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-1302">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="b4d66-1303">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="b4d66-1303">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="b4d66-1304">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4d66-1304">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="b4d66-1305">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1305">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="b4d66-1306">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="b4d66-1306">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="b4d66-1307">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-1307">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="b4d66-1308">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="b4d66-1308">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="b4d66-1309">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-1309">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="b4d66-1310">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-1310">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="b4d66-1311">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1311">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="b4d66-1312">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1312">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="b4d66-1313">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b4d66-1313">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="b4d66-1314">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b4d66-1314">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="b4d66-1315">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="b4d66-1315">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="b4d66-1316">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1316">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="b4d66-1317">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1317">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="b4d66-1318">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-1318">Az.OperationalInsights</span></span>
- <span data-ttu-id="b4d66-1319">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1319">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="b4d66-1320">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1320">Az.Profile</span></span>
- <span data-ttu-id="b4d66-1321">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1321">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1322">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1322">Az.RecoveryServices</span></span>
- <span data-ttu-id="b4d66-1323">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1323">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="b4d66-1324">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1324">Az.Resources</span></span>
- <span data-ttu-id="b4d66-1325">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1325">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="b4d66-1326">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-1326">Az.ServiceFabric</span></span>
- <span data-ttu-id="b4d66-1327">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="b4d66-1327">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="b4d66-1328">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1328">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="b4d66-1329">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="b4d66-1329">Az.SIgnalR</span></span>
- <span data-ttu-id="b4d66-1330">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="b4d66-1330">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="b4d66-1331">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1331">Az.Sql</span></span>
- <span data-ttu-id="b4d66-1332">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1332">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="b4d66-1333">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1333">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="b4d66-1334">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1334">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="b4d66-1335">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1335">Az.Storage</span></span>
- <span data-ttu-id="b4d66-1336">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1336">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="b4d66-1337">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1337">Az.Websites</span></span>
- <span data-ttu-id="b4d66-1338">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="b4d66-1338">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="b4d66-1339">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1339">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="b4d66-1340">全般</span><span class="sxs-lookup"><span data-stu-id="b4d66-1340">General</span></span>

* <span data-ttu-id="b4d66-1341">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="b4d66-1341">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="b4d66-1342">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1342">Az.Compute</span></span>

* <span data-ttu-id="b4d66-1343">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1343">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1344">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1344">Az.DataLakeStore</span></span>

* <span data-ttu-id="b4d66-1345">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1345">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="b4d66-1346">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="b4d66-1346">Az.FrontDoor</span></span>

* <span data-ttu-id="b4d66-1347">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1347">Fixed some broken links</span></span>
    - <span data-ttu-id="b4d66-1348">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1348">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="b4d66-1349">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1349">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="b4d66-1350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1350">Az.RecoveryServices</span></span>

* <span data-ttu-id="b4d66-1351">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1351">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="b4d66-1352">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1352">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="b4d66-1353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1353">Az.Resources</span></span>

* <span data-ttu-id="b4d66-1354">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1354">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="b4d66-1355">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1355">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="b4d66-1356">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1356">Az.Sql</span></span>

* <span data-ttu-id="b4d66-1357">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="b4d66-1357">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="b4d66-1358">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1358">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="b4d66-1359">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1359">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="b4d66-1360">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1360">Az.Storage</span></span>

* <span data-ttu-id="b4d66-1361">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1361">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="b4d66-1362">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1362">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="b4d66-1363">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1363">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="b4d66-1364">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="b4d66-1364">Support Static Website configuration</span></span>
    - <span data-ttu-id="b4d66-1365">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="b4d66-1365">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="b4d66-1366">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="b4d66-1366">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="b4d66-1367">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1367">Az.Websites</span></span>

* <span data-ttu-id="b4d66-1368">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="b4d66-1368">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="b4d66-1369">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1369">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="b4d66-1370">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="b4d66-1370">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="b4d66-1371">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1371">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="b4d66-1372">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="b4d66-1372">Az.ApiManagement</span></span>
* <span data-ttu-id="b4d66-1373">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1373">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="b4d66-1374">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="b4d66-1374">Az.Automation</span></span>
* <span data-ttu-id="b4d66-1375">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="b4d66-1375">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="b4d66-1376">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1376">Added Update Management cmdlets</span></span>
* <span data-ttu-id="b4d66-1377">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1377">Added Source Control cmdlets</span></span>
* <span data-ttu-id="b4d66-1378">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1378">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="b4d66-1379">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1379">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="b4d66-1380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1380">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1381">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1381">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="b4d66-1382">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1382">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="b4d66-1383">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1383">Az.ContainerInstance</span></span>
* <span data-ttu-id="b4d66-1384">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1384">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="b4d66-1385">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="b4d66-1385">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="b4d66-1386">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1386">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="b4d66-1387">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1387">Az.Network</span></span>
* <span data-ttu-id="b4d66-1388">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1388">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="b4d66-1389">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1389">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="b4d66-1390">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1390">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="b4d66-1391">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1391">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="b4d66-1392">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="b4d66-1392">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="b4d66-1393">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1393">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="b4d66-1394">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1394">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="b4d66-1395">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="b4d66-1395">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="b4d66-1396">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1396">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="b4d66-1397">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1397">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="b4d66-1398">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="b4d66-1398">Az.Relay</span></span>
* <span data-ttu-id="b4d66-1399">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="b4d66-1399">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="b4d66-1400">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1400">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1401">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1401">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="b4d66-1402">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1402">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="b4d66-1403">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="b4d66-1403">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="b4d66-1404">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-1404">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-1405">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1405">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="b4d66-1406">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1406">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1407">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1407">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="b4d66-1408">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1408">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b4d66-1409">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1409">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b4d66-1410">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1410">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b4d66-1411">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="b4d66-1411">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="b4d66-1412">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b4d66-1412">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b4d66-1413">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b4d66-1413">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b4d66-1414">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b4d66-1414">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="b4d66-1415">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="b4d66-1415">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="b4d66-1416">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1416">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="b4d66-1417">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1417">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="b4d66-1418">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1418">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="b4d66-1419">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="b4d66-1419">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="b4d66-1420">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="b4d66-1420">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="b4d66-1421">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="b4d66-1421">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="b4d66-1422">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="b4d66-1422">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="b4d66-1423">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1423">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="b4d66-1424">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1424">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="b4d66-1425">全般</span><span class="sxs-lookup"><span data-stu-id="b4d66-1425">General</span></span>
* <span data-ttu-id="b4d66-1426">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="b4d66-1426">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="b4d66-1427">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1427">Az.Profile</span></span>
* <span data-ttu-id="b4d66-1428">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1428">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="b4d66-1429">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1429">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="b4d66-1430">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1430">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="b4d66-1431">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1431">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="b4d66-1432">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1432">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="b4d66-1433">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1433">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="b4d66-1434">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1434">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-1435">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1435">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-1436">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1436">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1437">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1437">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1438">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1438">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="b4d66-1439">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="b4d66-1439">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="b4d66-1440">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1440">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1441">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1441">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-1442">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1442">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="b4d66-1443">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1443">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="b4d66-1444">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="b4d66-1444">Az.Insights</span></span>
* <span data-ttu-id="b4d66-1445">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1445">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="b4d66-1446">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1446">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="b4d66-1447">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1447">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="b4d66-1448">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="b4d66-1448">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1449">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1449">Az.Network</span></span>
* <span data-ttu-id="b4d66-1450">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="b4d66-1450">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="b4d66-1451">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="b4d66-1451">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="b4d66-1452">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="b4d66-1452">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="b4d66-1453">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="b4d66-1453">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="b4d66-1454">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="b4d66-1454">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="b4d66-1455">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="b4d66-1455">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="b4d66-1456">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="b4d66-1456">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="b4d66-1457">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="b4d66-1457">Az.PolicyInsights</span></span>
* <span data-ttu-id="b4d66-1458">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1458">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1459">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1459">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1460">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1460">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="b4d66-1461">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1461">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="b4d66-1462">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="b4d66-1462">Az.ServiceBus</span></span>
* <span data-ttu-id="b4d66-1463">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1463">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="b4d66-1464">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="b4d66-1464">Az.ServiceFabric</span></span>
* <span data-ttu-id="b4d66-1465">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1465">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="b4d66-1466">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1466">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="b4d66-1467">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1467">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="b4d66-1468">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1468">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="b4d66-1469">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1469">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="b4d66-1470">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1470">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="b4d66-1471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1471">Az.Profile</span></span>
* <span data-ttu-id="b4d66-1472">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1472">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="b4d66-1473">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1473">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1474">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1474">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1475">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1475">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="b4d66-1476">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1476">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="b4d66-1477">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="b4d66-1477">Az.DataLakeStore</span></span>
* <span data-ttu-id="b4d66-1478">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1478">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="b4d66-1479">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1479">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="b4d66-1480">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1480">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="b4d66-1481">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1481">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="b4d66-1482">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1482">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1483">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1483">Az.Network</span></span>
* <span data-ttu-id="b4d66-1484">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1484">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="b4d66-1485">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1485">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1486">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1486">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1487">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1487">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="b4d66-1488">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1488">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="b4d66-1489">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1489">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="b4d66-1490">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1490">Azure.Storage</span></span>
* <span data-ttu-id="b4d66-1491">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1491">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="b4d66-1492">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1492">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="b4d66-1493">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="b4d66-1493">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="b4d66-1494">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1494">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="b4d66-1495">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="b4d66-1495">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="b4d66-1496">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="b4d66-1496">Az.CognitiveServices</span></span>
* <span data-ttu-id="b4d66-1497">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1497">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="b4d66-1498">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="b4d66-1498">Az.Compute</span></span>
* <span data-ttu-id="b4d66-1499">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1499">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="b4d66-1500">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1500">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="b4d66-1501">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1501">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="b4d66-1502">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="b4d66-1502">Az.DataFactoryV2</span></span>
* <span data-ttu-id="b4d66-1503">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1503">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="b4d66-1504">Az.Network</span><span class="sxs-lookup"><span data-stu-id="b4d66-1504">Az.Network</span></span>
* <span data-ttu-id="b4d66-1505">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1505">Added NetworkProfile functionality.</span></span> <span data-ttu-id="b4d66-1506">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="b4d66-1506">new cmdlets added</span></span>
    - <span data-ttu-id="b4d66-1507">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1507">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="b4d66-1508">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1508">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="b4d66-1509">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1509">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="b4d66-1510">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b4d66-1510">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="b4d66-1511">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-1511">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="b4d66-1512">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="b4d66-1512">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="b4d66-1513">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1513">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="b4d66-1514">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1514">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="b4d66-1515">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1515">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="b4d66-1516">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="b4d66-1516">Az.RedisCache</span></span>
* <span data-ttu-id="b4d66-1517">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="b4d66-1517">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="b4d66-1518">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1518">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="b4d66-1519">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="b4d66-1519">Az.Resources</span></span>
* <span data-ttu-id="b4d66-1520">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1520">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="b4d66-1521">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1521">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="b4d66-1522">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="b4d66-1522">Az.Sql</span></span>
* <span data-ttu-id="b4d66-1523">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="b4d66-1523">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="b4d66-1524">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="b4d66-1524">Az.Websites</span></span>
* <span data-ttu-id="b4d66-1525">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="b4d66-1525">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="b4d66-1526">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="b4d66-1526">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="b4d66-1527">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="b4d66-1527">0.2.0 - September 2018</span></span>
 <span data-ttu-id="b4d66-1528">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="b4d66-1528">Initial Release</span></span>

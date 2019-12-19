---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 98a24c805fbf43dd899119d43301b4261c1f60dc
ms.sourcegitcommit: f9445d1525eac8c165637e1a80fbc92b1ab005c2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/16/2019
ms.locfileid: "75035763"
---
## <a name="280---october-2019"></a><span data-ttu-id="ba2a5-103">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-103">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="ba2a5-104">全般</span><span class="sxs-lookup"><span data-stu-id="ba2a5-104">General</span></span>
* <span data-ttu-id="ba2a5-105">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-105">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-106">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-107">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-107">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-108">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-108">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-109">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-109">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="ba2a5-110">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="ba2a5-110">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-111">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-112">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-112">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="ba2a5-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ba2a5-113">Az.Batch</span></span>
* <span data-ttu-id="ba2a5-114">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-114">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-115">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-116">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-116">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="ba2a5-117">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-117">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="ba2a5-118">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-118">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="ba2a5-119">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-119">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-120">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-121">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-121">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="ba2a5-122">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-122">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="ba2a5-123">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-123">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-125">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-125">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="ba2a5-126">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="ba2a5-126">Az.HealthcareApis</span></span>
* <span data-ttu-id="ba2a5-127">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-127">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="ba2a5-128">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-128">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="ba2a5-129">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-129">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="ba2a5-130">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-130">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-131">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-131">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-132">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="ba2a5-132">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="ba2a5-133">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="ba2a5-133">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-134">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-135">New-AzActionGroupReceiver に新しいアクション グループ受信者が追加されました: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="ba2a5-135">New action group receivers added for New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="ba2a5-136">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-136">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="ba2a5-137">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="ba2a5-137">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="ba2a5-138">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-138">Webhooks now supports Azure active directory authentication.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-139">Az.Network</span></span>
* <span data-ttu-id="ba2a5-140">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-140">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="ba2a5-141">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-141">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="ba2a5-142">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ba2a5-142">New cmdlets added:</span></span>
        - <span data-ttu-id="ba2a5-143">New-AzIpsecTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-143">New-AzIpsecTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="ba2a5-144">省略可能なパラメーター -TrafficSelectorPolicies を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-144">Cmdlets updated with optional parameter -TrafficSelectorPolicies</span></span>
        - <span data-ttu-id="ba2a5-145">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-145">New-AzVirtualNetworkGatewayConnection</span></span>
        - <span data-ttu-id="ba2a5-146">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-146">Set-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ba2a5-147">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-147">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="ba2a5-148">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-148">Updated cmdlets:</span></span>
        - <span data-ttu-id="ba2a5-149">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-149">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ba2a5-150">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-150">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ba2a5-151">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-151">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ba2a5-152">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-152">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="ba2a5-153">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="ba2a5-153">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="ba2a5-154">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-154">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="ba2a5-155">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-155">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ba2a5-156">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ba2a5-156">Az.RedisCache</span></span>
* <span data-ttu-id="ba2a5-157">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-157">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-158">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-159">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-159">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-160">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-160">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-161">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-161">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="ba2a5-162">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-162">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ba2a5-163">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="ba2a5-163">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="ba2a5-164">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-164">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ba2a5-165">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-165">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ba2a5-166">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ba2a5-166">Az.StorageSync</span></span>
* <span data-ttu-id="ba2a5-167">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-167">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-168">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-168">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-169">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-169">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="ba2a5-170">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-170">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-171">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-171">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-172">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-172">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="ba2a5-173">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-173">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="ba2a5-174">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-174">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-175">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-175">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-176">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-176">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="ba2a5-177">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-177">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="ba2a5-178">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-178">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-179">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-179">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-180">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-180">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="ba2a5-181">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-181">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ba2a5-182">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-182">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="ba2a5-183">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-183">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="ba2a5-184">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-184">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="ba2a5-185">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-185">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="ba2a5-186">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-186">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="ba2a5-187">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-187">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="ba2a5-188">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-188">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-189">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-189">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-190">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-190">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="ba2a5-191">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-191">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="ba2a5-192">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ba2a5-192">Az.HDInsight</span></span>
* <span data-ttu-id="ba2a5-193">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-193">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-194">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-194">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-195">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-195">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="ba2a5-196">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-196">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="ba2a5-197">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-197">New cmdlets are:</span></span>
    - <span data-ttu-id="ba2a5-198">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ba2a5-198">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ba2a5-199">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ba2a5-199">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ba2a5-200">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ba2a5-200">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ba2a5-201">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ba2a5-201">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-202">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-202">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-203">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="ba2a5-203">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="ba2a5-204">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-204">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="ba2a5-205">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-205">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="ba2a5-206">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-206">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="ba2a5-207">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-207">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="ba2a5-208">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-208">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="ba2a5-209">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-209">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="ba2a5-210">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-210">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="ba2a5-211">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-211">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ba2a5-212">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-212">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="ba2a5-213">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-213">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ba2a5-214">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-214">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="ba2a5-215">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-215">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="ba2a5-216">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-216">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="ba2a5-217">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-217">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="ba2a5-218">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="ba2a5-218">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="ba2a5-219">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-219">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="ba2a5-220">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-220">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="ba2a5-221">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-221">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="ba2a5-222">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-222">Overall improved help files</span></span>
* <span data-ttu-id="ba2a5-223">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-223">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-224">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-224">Az.Network</span></span>
* <span data-ttu-id="ba2a5-225">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-225">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="ba2a5-226">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-226">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="ba2a5-227">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-227">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="ba2a5-228">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-228">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="ba2a5-229">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-229">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="ba2a5-230">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-230">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="ba2a5-231">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-231">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="ba2a5-232">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-232">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="ba2a5-233">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-233">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="ba2a5-234">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-234">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="ba2a5-235">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-235">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="ba2a5-236">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-236">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="ba2a5-237">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-237">New cmdlets</span></span>
        - <span data-ttu-id="ba2a5-238">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="ba2a5-238">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="ba2a5-239">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-239">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="ba2a5-240">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-240">Updated cmdlet:</span></span>
        - <span data-ttu-id="ba2a5-241">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ba2a5-241">New-VpnSite</span></span>
        - <span data-ttu-id="ba2a5-242">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ba2a5-242">Update-VpnSite</span></span>
        - <span data-ttu-id="ba2a5-243">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-243">New-VpnConnection</span></span>
        - <span data-ttu-id="ba2a5-244">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-244">Update-VpnConnection</span></span>
* <span data-ttu-id="ba2a5-245">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-245">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-247">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-247">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="ba2a5-248">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-248">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-249">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-249">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-250">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-250">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-251">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-251">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-252">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-252">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="ba2a5-253">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-253">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="ba2a5-254">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ba2a5-254">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ba2a5-255">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ba2a5-255">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ba2a5-256">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ba2a5-256">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ba2a5-257">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-257">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="ba2a5-258">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ba2a5-258">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ba2a5-259">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ba2a5-259">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ba2a5-260">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ba2a5-260">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ba2a5-261">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ba2a5-261">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ba2a5-262">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-262">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="ba2a5-263">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ba2a5-263">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ba2a5-264">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ba2a5-264">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ba2a5-265">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ba2a5-265">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ba2a5-266">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="ba2a5-266">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="ba2a5-267">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-267">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ba2a5-268">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ba2a5-268">Az.SignalR</span></span>
* <span data-ttu-id="ba2a5-269">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-269">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-270">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-270">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-271">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-271">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="ba2a5-272">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-272">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="ba2a5-273">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-273">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="ba2a5-274">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-274">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="ba2a5-275">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-275">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-276">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-276">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-277">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-277">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="ba2a5-278">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-278">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="ba2a5-279">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-279">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="ba2a5-280">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-280">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="ba2a5-281">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-281">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="ba2a5-282">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-282">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="ba2a5-283">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-283">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="ba2a5-284">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ba2a5-284">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ba2a5-285">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ba2a5-285">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ba2a5-286">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ba2a5-286">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ba2a5-287">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ba2a5-287">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-288">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-288">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-289">アプリを新しい ASP に移行するときに webapp タグが削除されるという問題を修正しています</span><span class="sxs-lookup"><span data-stu-id="ba2a5-289">Fixing issue where webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="ba2a5-290">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-290">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="ba2a5-291">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-291">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="ba2a5-292">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-292">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="ba2a5-293">全般</span><span class="sxs-lookup"><span data-stu-id="ba2a5-293">General</span></span>
* <span data-ttu-id="ba2a5-294">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-294">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-295">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-295">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-296">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-296">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="ba2a5-297">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ba2a5-297">Az.Aks</span></span>
* <span data-ttu-id="ba2a5-298">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-298">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="ba2a5-299">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="ba2a5-299">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-300">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-300">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-301">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="ba2a5-301">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="ba2a5-302">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-302">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="ba2a5-303">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-303">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="ba2a5-304">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="ba2a5-304">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="ba2a5-305">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-305">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ba2a5-306">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ba2a5-306">Az.Batch</span></span>
* <span data-ttu-id="ba2a5-307">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-307">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ba2a5-308">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ba2a5-308">Az.Cdn</span></span>
* <span data-ttu-id="ba2a5-309">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-309">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-310">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-310">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-311">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-311">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="ba2a5-312">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-312">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="ba2a5-313">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-313">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="ba2a5-314">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-314">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="ba2a5-315">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="ba2a5-315">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="ba2a5-316">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-316">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="ba2a5-317">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-317">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="ba2a5-318">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-318">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-319">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-319">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-320">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-320">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="ba2a5-321">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-321">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="ba2a5-322">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-322">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="ba2a5-323">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-323">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-324">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-324">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-325">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-325">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ba2a5-326">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-326">Az.EventHub</span></span>
* <span data-ttu-id="ba2a5-327">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="ba2a5-327">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="ba2a5-328">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="ba2a5-328">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="ba2a5-329">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-329">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="ba2a5-330">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="ba2a5-330">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="ba2a5-331">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ba2a5-331">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ba2a5-332">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-332">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-333">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-333">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-334">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-334">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-335">Az.Network</span></span>
* <span data-ttu-id="ba2a5-336">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-336">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="ba2a5-337">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-337">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="ba2a5-338">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-338">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="ba2a5-339">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-339">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="ba2a5-340">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-340">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="ba2a5-341">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-341">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="ba2a5-342">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-342">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-343">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-343">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-344">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-344">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="ba2a5-345">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-345">Added example</span></span>
    - <span data-ttu-id="ba2a5-346">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-346">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="ba2a5-347">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-347">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="ba2a5-348">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-348">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-349">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-349">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-350">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-350">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-351">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-352">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-352">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="ba2a5-353">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-353">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="ba2a5-354">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="ba2a5-354">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="ba2a5-355">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-355">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-356">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-356">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-357">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="ba2a5-357">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="ba2a5-358">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="ba2a5-358">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="ba2a5-359">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-359">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-360">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-360">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-361">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-361">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="ba2a5-362">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-362">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="ba2a5-363">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="ba2a5-363">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="ba2a5-364">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-364">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="ba2a5-365">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="ba2a5-365">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="ba2a5-366">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-366">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-367">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-367">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-368">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-368">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-369">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-370">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-370">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="ba2a5-371">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-371">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="ba2a5-372">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-372">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="ba2a5-373">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-373">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="ba2a5-374">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-374">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="ba2a5-375">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-375">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-376">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-376">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-377">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-377">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="ba2a5-378">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-378">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-379">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-379">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-380">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-380">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="ba2a5-381">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-381">Az.ApplicationInsights</span></span>
* <span data-ttu-id="ba2a5-382">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-382">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-383">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-383">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-384">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-384">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-385">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-385">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-386">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-386">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-387">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-387">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-388">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-388">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ba2a5-389">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ba2a5-389">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ba2a5-390">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-390">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="ba2a5-391">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="ba2a5-391">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-392">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-392">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-393">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-393">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="ba2a5-394">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-394">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ba2a5-395">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-395">Az.EventHub</span></span>
* <span data-ttu-id="ba2a5-396">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ba2a5-396">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ba2a5-397">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-397">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-398">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-398">Az.KeyVault</span></span>
* <span data-ttu-id="ba2a5-399">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-399">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ba2a5-400">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ba2a5-400">Az.LogicApp</span></span>
* <span data-ttu-id="ba2a5-401">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-401">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="ba2a5-402">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-402">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="ba2a5-403">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-403">Az.ManagedServices</span></span>
* <span data-ttu-id="ba2a5-404">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-404">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-405">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-405">Az.Network</span></span>
* <span data-ttu-id="ba2a5-406">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-406">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="ba2a5-407">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-407">New cmdlets</span></span>
        - <span data-ttu-id="ba2a5-408">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ba2a5-408">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ba2a5-409">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-409">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ba2a5-410">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-410">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ba2a5-411">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-411">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ba2a5-412">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-412">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ba2a5-413">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-413">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ba2a5-414">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="ba2a5-414">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="ba2a5-415">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-415">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="ba2a5-416">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="ba2a5-416">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="ba2a5-417">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-417">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="ba2a5-418">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-418">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="ba2a5-419">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-419">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="ba2a5-420">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-420">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="ba2a5-421">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-421">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="ba2a5-422">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-422">Updated cmdlets</span></span>
        - <span data-ttu-id="ba2a5-423">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-423">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ba2a5-424">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-424">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ba2a5-425">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-425">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ba2a5-426">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-426">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ba2a5-427">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-427">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="ba2a5-428">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-428">Updated cmdlet:</span></span>
        - <span data-ttu-id="ba2a5-429">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-429">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ba2a5-430">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-430">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ba2a5-431">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-431">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="ba2a5-432">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-432">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="ba2a5-433">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-433">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="ba2a5-434">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-434">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-435">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-435">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-436">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-436">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="ba2a5-437">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-437">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-438">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-438">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-439">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-439">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ba2a5-440">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-440">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="ba2a5-441">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-441">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="ba2a5-442">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-442">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ba2a5-443">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-443">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="ba2a5-444">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-444">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ba2a5-445">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-445">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="ba2a5-446">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-446">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ba2a5-447">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-447">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="ba2a5-448">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-448">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-449">Az.Resources</span></span>
- <span data-ttu-id="ba2a5-450">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-450">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="ba2a5-451">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-451">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-452">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-452">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-453">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ba2a5-453">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ba2a5-454">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-454">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-455">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-455">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-456">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-456">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="ba2a5-457">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-457">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="ba2a5-458">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-458">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-459">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-459">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-460">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-460">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ba2a5-461">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ba2a5-461">Az.StorageSync</span></span>
* <span data-ttu-id="ba2a5-462">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-462">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="ba2a5-463">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-463">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-464">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-464">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-465">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-465">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="ba2a5-466">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-466">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="ba2a5-467">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-467">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="ba2a5-468">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-468">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-469">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-469">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-470">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-470">Add support for profile cmdlets</span></span>
* <span data-ttu-id="ba2a5-471">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-471">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="ba2a5-472">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-472">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="ba2a5-473">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-473">Az.Advisor</span></span>
* <span data-ttu-id="ba2a5-474">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-474">GA release of Az.Advisor</span></span>
* <span data-ttu-id="ba2a5-475">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-475">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-476">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-476">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-477">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="ba2a5-477">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="ba2a5-478">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="ba2a5-478">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="ba2a5-479">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-479">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="ba2a5-480">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-480">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="ba2a5-481">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-481">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="ba2a5-482">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ba2a5-482">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="ba2a5-483">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-483">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-484">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-485">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-485">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-486">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-486">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-487">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-487">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-488">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-489">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-489">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ba2a5-490">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ba2a5-490">Az.EventGrid</span></span>
* <span data-ttu-id="ba2a5-491">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-491">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-492">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-492">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-493">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-493">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-494">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-494">Az.Network</span></span>
* <span data-ttu-id="ba2a5-495">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-495">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="ba2a5-496">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-496">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ba2a5-497">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-497">Az.PolicyInsights</span></span>
* <span data-ttu-id="ba2a5-498">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-498">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="ba2a5-499">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="ba2a5-499">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-500">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-500">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-501">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-501">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-502">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-502">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-503">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-503">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-504">Az.Resources</span></span>
    - <span data-ttu-id="ba2a5-505">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-505">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="ba2a5-506">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-506">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="ba2a5-507">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-507">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="ba2a5-508">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-508">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-509">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-509">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-510">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="ba2a5-510">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-511">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-511">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-512">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-512">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="ba2a5-513">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-513">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="ba2a5-514">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-514">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ba2a5-515">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-515">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ba2a5-516">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-516">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ba2a5-517">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-517">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ba2a5-518">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-518">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ba2a5-519">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ba2a5-519">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="ba2a5-520">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-520">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-521">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-521">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-522">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-522">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="ba2a5-523">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ba2a5-523">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="ba2a5-524">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-524">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="ba2a5-525">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="ba2a5-525">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="ba2a5-526">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-526">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="ba2a5-527">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-527">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="ba2a5-528">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-528">Set-AzStorageAccount</span></span>
* <span data-ttu-id="ba2a5-529">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-529">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="ba2a5-530">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ba2a5-530">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="ba2a5-531">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ba2a5-531">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ba2a5-532">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ba2a5-532">Az.StorageSync</span></span>
* <span data-ttu-id="ba2a5-533">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-533">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="ba2a5-534">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-534">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-535">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-535">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-536">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-536">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="ba2a5-537">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="ba2a5-537">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="ba2a5-538">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-538">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="ba2a5-539">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="ba2a5-539">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="ba2a5-540">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="ba2a5-540">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-541">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-541">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-542">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-542">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="ba2a5-543">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-543">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="ba2a5-544">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ba2a5-544">Az.Dns</span></span>
* <span data-ttu-id="ba2a5-545">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-545">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ba2a5-546">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ba2a5-546">Az.EventGrid</span></span>
* <span data-ttu-id="ba2a5-547">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-547">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="ba2a5-548">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-548">New cmdlets:</span></span>
    - <span data-ttu-id="ba2a5-549">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ba2a5-549">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ba2a5-550">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-550">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ba2a5-551">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ba2a5-551">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ba2a5-552">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-552">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="ba2a5-553">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ba2a5-553">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ba2a5-554">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-554">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ba2a5-555">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ba2a5-555">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ba2a5-556">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-556">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ba2a5-557">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ba2a5-557">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ba2a5-558">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-558">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="ba2a5-559">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-559">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ba2a5-560">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-560">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="ba2a5-561">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="ba2a5-561">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="ba2a5-562">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-562">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="ba2a5-563">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-563">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ba2a5-564">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-564">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="ba2a5-565">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-565">Updated cmdlets:</span></span>
    - <span data-ttu-id="ba2a5-566">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-566">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="ba2a5-567">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-567">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ba2a5-568">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-568">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ba2a5-569">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-569">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="ba2a5-570">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-570">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="ba2a5-571">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="ba2a5-571">Event subscription expiration date,</span></span>
            - <span data-ttu-id="ba2a5-572">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="ba2a5-572">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="ba2a5-573">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-573">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="ba2a5-574">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-574">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="ba2a5-575">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-575">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="ba2a5-576">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-576">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="ba2a5-577">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="ba2a5-577">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="ba2a5-578">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-578">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="ba2a5-579">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-579">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ba2a5-580">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-580">Az.FrontDoor</span></span>
* <span data-ttu-id="ba2a5-581">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="ba2a5-581">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="ba2a5-582">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-582">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="ba2a5-583">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="ba2a5-583">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="ba2a5-584">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-584">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-585">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-585">Az.Network</span></span>
* <span data-ttu-id="ba2a5-586">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-586">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="ba2a5-587">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-587">New cmdlets</span></span>
        - <span data-ttu-id="ba2a5-588">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="ba2a5-588">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="ba2a5-589">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-589">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="ba2a5-590">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-590">New cmdlets</span></span> 
        - <span data-ttu-id="ba2a5-591">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="ba2a5-591">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="ba2a5-592">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-592">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="ba2a5-593">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-593">New cmdlets</span></span> 
        - <span data-ttu-id="ba2a5-594">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-594">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="ba2a5-595">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-595">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ba2a5-596">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ba2a5-596">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ba2a5-597">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-597">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="ba2a5-598">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-598">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="ba2a5-599">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-599">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="ba2a5-600">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-600">New cmdlets</span></span>
        - <span data-ttu-id="ba2a5-601">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ba2a5-601">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ba2a5-602">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ba2a5-602">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ba2a5-603">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ba2a5-603">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ba2a5-604">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-604">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="ba2a5-605">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="ba2a5-605">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="ba2a5-606">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-606">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="ba2a5-607">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-607">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="ba2a5-608">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-608">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="ba2a5-609">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-609">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="ba2a5-610">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-610">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="ba2a5-611">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-611">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="ba2a5-612">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-612">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="ba2a5-613">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-613">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="ba2a5-614">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-614">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="ba2a5-615">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-615">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="ba2a5-616">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-616">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="ba2a5-617">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-617">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="ba2a5-618">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-618">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="ba2a5-619">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-619">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="ba2a5-620">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-620">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="ba2a5-621">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-621">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="ba2a5-622">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-622">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="ba2a5-623">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-623">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="ba2a5-624">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-624">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="ba2a5-625">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-625">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ba2a5-626">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-626">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ba2a5-627">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-627">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-628">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-628">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-629">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-629">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-630">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-630">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-631">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-631">Support for additional Template Export options</span></span>
    - <span data-ttu-id="ba2a5-632">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-632">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ba2a5-633">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-633">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ba2a5-634">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-634">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-635">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-635">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-636">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-636">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-637">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-637">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-638">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-638">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="ba2a5-639">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-639">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="ba2a5-640">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-640">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="ba2a5-641">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ba2a5-641">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ba2a5-642">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ba2a5-642">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ba2a5-643">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ba2a5-643">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ba2a5-644">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ba2a5-644">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="ba2a5-645">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ba2a5-645">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-646">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-646">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-647">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-647">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="ba2a5-648">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-648">New-AzStorageAccount</span></span>
* <span data-ttu-id="ba2a5-649">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-649">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="ba2a5-650">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-650">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-651">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-651">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-652">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-652">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="ba2a5-653">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-653">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="ba2a5-654">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-654">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="ba2a5-655">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ba2a5-655">Az.Cdn</span></span>
* <span data-ttu-id="ba2a5-656">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-656">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-657">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-657">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-658">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-658">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="ba2a5-659">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="ba2a5-659">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ba2a5-660">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-660">Az.EventHub</span></span>
* <span data-ttu-id="ba2a5-661">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-661">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="ba2a5-662">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-662">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-663">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-663">Az.Network</span></span>
* <span data-ttu-id="ba2a5-664">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-664">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="ba2a5-665">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-665">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ba2a5-666">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-666">Az.PolicyInsights</span></span>
* <span data-ttu-id="ba2a5-667">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-667">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-668">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-669">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-669">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-670">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-670">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-671">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-671">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-672">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-672">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-673">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-673">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="ba2a5-674">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-674">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-675">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-675">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-676">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-676">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="ba2a5-677">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="ba2a5-677">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="ba2a5-678">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-678">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="ba2a5-679">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-679">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-680">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-680">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-681">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-681">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="ba2a5-682">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-682">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-683">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-683">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-684">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-684">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="ba2a5-685">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-685">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="ba2a5-686">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-686">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="ba2a5-687">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-687">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="ba2a5-688">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-688">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="ba2a5-689">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-689">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="ba2a5-690">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-690">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="ba2a5-691">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-691">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="ba2a5-692">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-692">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="ba2a5-693">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-693">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="ba2a5-694">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-694">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="ba2a5-695">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-695">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="ba2a5-696">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-696">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="ba2a5-697">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-697">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="ba2a5-698">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-698">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="ba2a5-699">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-699">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="ba2a5-700">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-700">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="ba2a5-701">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-701">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="ba2a5-702">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-702">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="ba2a5-703">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="ba2a5-703">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="ba2a5-704">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-704">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="ba2a5-705">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-705">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="ba2a5-706">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-706">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="ba2a5-707">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-707">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="ba2a5-708">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-708">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="ba2a5-709">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-709">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="ba2a5-710">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-710">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="ba2a5-711">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-711">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="ba2a5-712">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-712">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="ba2a5-713">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-713">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="ba2a5-714">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-714">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="ba2a5-715">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="ba2a5-715">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="ba2a5-716">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-716">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="ba2a5-717">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-717">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ba2a5-718">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="ba2a5-718">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="ba2a5-719">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-719">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="ba2a5-720">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-720">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="ba2a5-721">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-721">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="ba2a5-722">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-722">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="ba2a5-723">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-723">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="ba2a5-724">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-724">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ba2a5-725">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-725">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="ba2a5-726">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-726">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="ba2a5-727">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-727">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ba2a5-728">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-728">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ba2a5-729">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-729">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ba2a5-730">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-730">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="ba2a5-731">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-731">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ba2a5-732">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-732">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="ba2a5-733">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-733">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="ba2a5-734">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-734">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="ba2a5-735">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-735">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="ba2a5-736">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-736">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="ba2a5-737">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-737">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="ba2a5-738">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-738">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="ba2a5-739">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-739">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="ba2a5-740">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-740">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ba2a5-741">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-741">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ba2a5-742">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-742">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ba2a5-743">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-743">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ba2a5-744">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-744">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ba2a5-745">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-745">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ba2a5-746">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="ba2a5-746">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ba2a5-747">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-747">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ba2a5-748">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-748">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="ba2a5-749">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-749">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="ba2a5-750">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="ba2a5-750">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="ba2a5-751">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-751">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="ba2a5-752">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="ba2a5-752">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="ba2a5-753">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-753">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="ba2a5-754">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="ba2a5-754">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="ba2a5-755">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-755">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="ba2a5-756">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-756">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="ba2a5-757">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-757">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="ba2a5-758">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-758">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="ba2a5-759">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-759">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="ba2a5-760">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="ba2a5-760">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-761">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-761">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-762">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-762">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="ba2a5-763">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="ba2a5-763">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="ba2a5-764">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="ba2a5-764">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="ba2a5-765">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-765">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="ba2a5-766">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="ba2a5-766">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="ba2a5-767">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-767">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="ba2a5-768">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-768">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-769">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-769">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-770">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-770">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="ba2a5-771">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-771">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-772">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-772">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-773">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-773">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-774">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-774">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-775">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-775">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-776">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-776">Az.Network</span></span>
* <span data-ttu-id="ba2a5-777">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-777">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="ba2a5-778">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-778">Updated cmdlet:</span></span>
        - <span data-ttu-id="ba2a5-779">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="ba2a5-779">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="ba2a5-780">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-780">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-781">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-781">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-782">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-782">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-783">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-783">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-784">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-784">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="ba2a5-785">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-785">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-786">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-787">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-787">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-788">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-788">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-789">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-789">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="ba2a5-790">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-790">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-791">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-791">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-792">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-792">Proximity placement group feature.</span></span>
    - <span data-ttu-id="ba2a5-793">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="ba2a5-793">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="ba2a5-794">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-794">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="ba2a5-795">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-795">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="ba2a5-796">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-796">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="ba2a5-797">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-797">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="ba2a5-798">重大な変更</span><span class="sxs-lookup"><span data-stu-id="ba2a5-798">Breaking changes</span></span>
    - <span data-ttu-id="ba2a5-799">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-799">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="ba2a5-800">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-800">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="ba2a5-801">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="ba2a5-801">Az.DeploymentManager</span></span>
* <span data-ttu-id="ba2a5-802">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-802">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="ba2a5-803">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ba2a5-803">Az.Dns</span></span>
* <span data-ttu-id="ba2a5-804">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="ba2a5-804">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="ba2a5-805">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-805">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="ba2a5-806">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-806">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ba2a5-807">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-807">Az.FrontDoor</span></span>
* <span data-ttu-id="ba2a5-808">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-808">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="ba2a5-809">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-809">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="ba2a5-810">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ba2a5-810">Az.HDInsight</span></span>
* <span data-ttu-id="ba2a5-811">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-811">Removed two cmdlets:</span></span>
    - <span data-ttu-id="ba2a5-812">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ba2a5-812">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="ba2a5-813">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ba2a5-813">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ba2a5-814">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-814">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ba2a5-815">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-815">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="ba2a5-816">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-816">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="ba2a5-817">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-817">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-818">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-818">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-819">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-819">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="ba2a5-820">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="ba2a5-820">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="ba2a5-821">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="ba2a5-821">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="ba2a5-822">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="ba2a5-822">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="ba2a5-823">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-823">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="ba2a5-824">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="ba2a5-824">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="ba2a5-825">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="ba2a5-825">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="ba2a5-826">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-826">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ba2a5-827">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-827">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ba2a5-828">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-828">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ba2a5-829">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-829">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ba2a5-830">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-830">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ba2a5-831">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="ba2a5-831">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="ba2a5-832">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-832">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-833">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-833">Az.Network</span></span>
* <span data-ttu-id="ba2a5-834">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-834">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="ba2a5-835">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-835">New cmdlets</span></span>
        - <span data-ttu-id="ba2a5-836">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ba2a5-836">New-AzNatGateway</span></span>
        - <span data-ttu-id="ba2a5-837">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ba2a5-837">Get-AzNatGateway</span></span>
        - <span data-ttu-id="ba2a5-838">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ba2a5-838">Set-AzNatGateway</span></span>
        - <span data-ttu-id="ba2a5-839">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ba2a5-839">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="ba2a5-840">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-840">Updated cmdlets</span></span>
        - <span data-ttu-id="ba2a5-841">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ba2a5-841">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="ba2a5-842">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ba2a5-842">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="ba2a5-843">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-843">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="ba2a5-844">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-844">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="ba2a5-845">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-845">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ba2a5-846">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-846">Az.PolicyInsights</span></span>
* <span data-ttu-id="ba2a5-847">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-847">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="ba2a5-848">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-848">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="ba2a5-849">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-849">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-850">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-850">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-851">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-851">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="ba2a5-852">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-852">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="ba2a5-853">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-853">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="ba2a5-854">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-854">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="ba2a5-855">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-855">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="ba2a5-856">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-856">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="ba2a5-857">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ba2a5-857">Az.Relay</span></span>
* <span data-ttu-id="ba2a5-858">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-858">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-859">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-859">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-860">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-860">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-861">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-861">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-862">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-862">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="ba2a5-863">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-863">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="ba2a5-864">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-864">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="ba2a5-865">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-865">New-AzStorageAccount</span></span>
* <span data-ttu-id="ba2a5-866">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="ba2a5-866">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="ba2a5-867">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-867">New-AzStorageAccount</span></span>
    - <span data-ttu-id="ba2a5-868">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-868">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="ba2a5-869">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ba2a5-869">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-870">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-870">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-871">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="ba2a5-871">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="ba2a5-872">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-872">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="ba2a5-873">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-873">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ba2a5-874">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ba2a5-874">Highlights since the last major release</span></span>
* <span data-ttu-id="ba2a5-875">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ba2a5-875">General availability of `Az` module</span></span>
* <span data-ttu-id="ba2a5-876">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ba2a5-876">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ba2a5-877">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ba2a5-877">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ba2a5-878">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-878">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ba2a5-879">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-879">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ba2a5-880">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-880">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ba2a5-881">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-881">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-882">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-882">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-883">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-883">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ba2a5-884">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ba2a5-884">Az.Batch</span></span>
* <span data-ttu-id="ba2a5-885">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-885">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ba2a5-886">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ba2a5-886">Az.Cdn</span></span>
* <span data-ttu-id="ba2a5-887">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-887">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-888">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-888">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-889">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-889">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-890">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-890">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-891">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-891">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="ba2a5-892">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-892">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-893">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-893">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-894">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-894">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-895">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-895">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-896">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-896">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-897">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-897">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ba2a5-898">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ba2a5-898">Az.EventGrid</span></span>
* <span data-ttu-id="ba2a5-899">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-899">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ba2a5-900">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-900">Az.EventHub</span></span>
* <span data-ttu-id="ba2a5-901">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-901">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="ba2a5-902">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ba2a5-902">Az.HDInsight</span></span>
* <span data-ttu-id="ba2a5-903">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-903">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-904">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-904">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-905">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-905">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-906">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-906">Az.KeyVault</span></span>
* <span data-ttu-id="ba2a5-907">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-907">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-908">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-908">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="ba2a5-909">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ba2a5-909">Az.MachineLearning</span></span>
* <span data-ttu-id="ba2a5-910">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="ba2a5-911">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ba2a5-911">Az.Media</span></span>
* <span data-ttu-id="ba2a5-912">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-912">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-913">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-913">Az.Monitor</span></span>
  * <span data-ttu-id="ba2a5-914">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-914">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="ba2a5-915">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="ba2a5-915">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="ba2a5-916">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="ba2a5-916">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="ba2a5-917">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ba2a5-917">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ba2a5-918">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ba2a5-918">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ba2a5-919">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ba2a5-919">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="ba2a5-920">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-920">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-921">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-921">Az.Network</span></span>
* <span data-ttu-id="ba2a5-922">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-922">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-923">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-923">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="ba2a5-924">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="ba2a5-924">Az.NotificationHubs</span></span>
* <span data-ttu-id="ba2a5-925">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-925">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-926">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-926">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-927">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-927">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="ba2a5-928">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ba2a5-928">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="ba2a5-929">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-929">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-930">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-930">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-931">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-931">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-932">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-932">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="ba2a5-933">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-933">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="ba2a5-934">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-934">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ba2a5-935">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ba2a5-935">Az.RedisCache</span></span>
* <span data-ttu-id="ba2a5-936">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-936">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-937">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-937">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-938">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-938">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-939">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-939">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-940">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="ba2a5-940">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="ba2a5-941">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-941">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-942">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-942">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="ba2a5-943">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-943">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="ba2a5-944">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-944">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="ba2a5-945">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-945">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="ba2a5-946">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-946">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-947">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-948">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-948">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="ba2a5-949">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-949">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ba2a5-950">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-950">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="ba2a5-951">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-951">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="ba2a5-952">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-952">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ba2a5-953">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ba2a5-953">Highlights since the last major release</span></span>
* <span data-ttu-id="ba2a5-954">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ba2a5-954">General availability of `Az` module</span></span>
* <span data-ttu-id="ba2a5-955">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ba2a5-955">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ba2a5-956">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ba2a5-956">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ba2a5-957">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-957">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ba2a5-958">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-958">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ba2a5-959">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-959">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ba2a5-960">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-960">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-961">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-961">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-962">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-962">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ba2a5-963">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-963">Az.AnalysisServices</span></span>
* <span data-ttu-id="ba2a5-964">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="ba2a5-964">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="ba2a5-965">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-965">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-966">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-966">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-967">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-967">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="ba2a5-968">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-968">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="ba2a5-969">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-969">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-970">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-970">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-971">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-971">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ba2a5-972">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-972">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="ba2a5-973">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-973">Az.ContainerInstance</span></span>
* <span data-ttu-id="ba2a5-974">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-974">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-975">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-975">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-976">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-976">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="ba2a5-977">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-977">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-978">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-978">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-979">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-979">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="ba2a5-980">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-980">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="ba2a5-981">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-981">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="ba2a5-982">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ba2a5-982">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="ba2a5-983">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-983">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="ba2a5-984">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ba2a5-984">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-985">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-985">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-986">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-986">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-987">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-987">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-988">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="ba2a5-988">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="ba2a5-989">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ba2a5-989">New-AzStorageContext</span></span>
* <span data-ttu-id="ba2a5-990">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-990">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="ba2a5-991">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ba2a5-991">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ba2a5-992">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ba2a5-992">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ba2a5-993">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-993">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="ba2a5-994">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-994">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="ba2a5-995">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-995">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="ba2a5-996">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-996">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ba2a5-997">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-997">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ba2a5-998">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-998">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="ba2a5-999">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ba2a5-999">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="ba2a5-1000">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1000">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ba2a5-1001">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1001">Highlights since the last major release</span></span>
* <span data-ttu-id="ba2a5-1002">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1002">General availability of `Az` module</span></span>
* <span data-ttu-id="ba2a5-1003">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1003">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ba2a5-1004">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1004">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ba2a5-1005">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1005">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ba2a5-1006">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1006">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ba2a5-1007">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1007">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1008">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1008">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1009">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1010">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1010">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="ba2a5-1011">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1011">Dynamic grouping</span></span>
    * <span data-ttu-id="ba2a5-1012">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1012">Pre-Post script</span></span>
    * <span data-ttu-id="ba2a5-1013">再起動設定</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1013">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1014">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1014">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1015">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1015">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="ba2a5-1016">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1016">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-1017">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1017">Az.KeyVault</span></span>
* <span data-ttu-id="ba2a5-1018">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1018">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1019">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1020">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1020">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="ba2a5-1021">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1021">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1022">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1022">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-1023">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1023">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="ba2a5-1024">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1024">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1025">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1025">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1026">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1026">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="ba2a5-1027">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1027">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1028">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1028">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1029">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1029">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-1030">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1030">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-1031">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1031">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="ba2a5-1032">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1032">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ba2a5-1033">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1033">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ba2a5-1034">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1034">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ba2a5-1035">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1035">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="ba2a5-1036">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1036">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="ba2a5-1037">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1037">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1038">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1038">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-1039">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1039">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="ba2a5-1040">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1040">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1041">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1041">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-1042">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1042">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="ba2a5-1043">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1043">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-1044">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1044">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1045">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1045">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="ba2a5-1046">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1046">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="ba2a5-1047">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1047">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ba2a5-1048">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1048">Az.Cdn</span></span>
* <span data-ttu-id="ba2a5-1049">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1049">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1050">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1050">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1051">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1051">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-1052">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1052">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-1053">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1053">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ba2a5-1054">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1054">Az.LogicApp</span></span>
* <span data-ttu-id="ba2a5-1055">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1055">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1056">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1056">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1057">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1057">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1058">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1058">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-1059">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1059">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="ba2a5-1060">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1060">SDK Update</span></span>
* <span data-ttu-id="ba2a5-1061">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1061">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="ba2a5-1062">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1062">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1063">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1063">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1064">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1064">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="ba2a5-1065">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1065">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="ba2a5-1066">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1066">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="ba2a5-1067">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1067">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="ba2a5-1068">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1068">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="ba2a5-1069">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1069">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1070">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1070">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1071">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1071">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="ba2a5-1072">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1072">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-1073">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1073">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-1074">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1074">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="ba2a5-1075">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1075">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="ba2a5-1076">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1076">Az.AnalysisServices</span></span>
* <span data-ttu-id="ba2a5-1077">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1077">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-1078">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1078">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1079">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1079">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="ba2a5-1080">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1080">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="ba2a5-1081">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1081">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-1082">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1082">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-1083">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1083">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1084">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1084">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1085">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1085">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="ba2a5-1086">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1086">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="ba2a5-1087">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1087">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="ba2a5-1088">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1088">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1089">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1089">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-1090">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1090">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ba2a5-1091">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1091">Az.EventHub</span></span>
* <span data-ttu-id="ba2a5-1092">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1092">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-1093">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1093">Az.KeyVault</span></span>
* <span data-ttu-id="ba2a5-1094">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1094">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ba2a5-1095">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1095">Az.LogicApp</span></span>
* <span data-ttu-id="ba2a5-1096">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1096">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="ba2a5-1097">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1097">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="ba2a5-1098">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1098">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="ba2a5-1099">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1099">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ba2a5-1100">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1100">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ba2a5-1101">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1101">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ba2a5-1102">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1102">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="ba2a5-1103">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1103">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="ba2a5-1104">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1104">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ba2a5-1105">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1105">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ba2a5-1106">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1106">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ba2a5-1107">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1107">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="ba2a5-1108">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1108">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ba2a5-1109">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1109">Az.Monitor</span></span>
* <span data-ttu-id="ba2a5-1110">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1110">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1111">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1111">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1112">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1112">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-1113">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1113">Az.OperationalInsights</span></span>
* <span data-ttu-id="ba2a5-1114">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1114">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="ba2a5-1115">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1115">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="ba2a5-1116">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1116">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1117">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1117">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1118">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1118">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ba2a5-1119">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1119">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="ba2a5-1120">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1120">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="ba2a5-1121">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1121">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1122">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1122">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1123">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1123">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="ba2a5-1124">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1124">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1125">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1125">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-1126">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1126">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="ba2a5-1127">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1127">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1128">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1128">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-1129">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1129">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ba2a5-1130">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1130">Az.AnalysisServices</span></span>
<span data-ttu-id="ba2a5-1131">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1131">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1132">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1132">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1133">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1133">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="ba2a5-1134">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1134">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="ba2a5-1135">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1135">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1136">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1136">Az.RecoveryServices</span></span>
<span data-ttu-id="ba2a5-1137">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1137">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1138">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1138">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1139">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1139">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="ba2a5-1140">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1140">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ba2a5-1141">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1141">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="ba2a5-1142">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1142">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1143">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1143">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1144">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1144">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="ba2a5-1145">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1145">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="ba2a5-1146">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1146">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="ba2a5-1147">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1147">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1148">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1148">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-1149">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1149">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ba2a5-1150">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1150">Az.AnalysisServices</span></span>
* <span data-ttu-id="ba2a5-1151">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1151">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1152">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1152">Az.RecoveryServices</span></span>
* <span data-ttu-id="ba2a5-1153">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1153">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="ba2a5-1154">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1154">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1155">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1155">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-1156">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1156">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ba2a5-1157">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1157">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ba2a5-1158">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1158">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="ba2a5-1159">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1159">Az.Aks</span></span>
* <span data-ttu-id="ba2a5-1160">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1160">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ba2a5-1161">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1161">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1162">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1162">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="ba2a5-1163">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1163">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ba2a5-1164">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1164">Az.Cdn</span></span>
* <span data-ttu-id="ba2a5-1165">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1165">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1166">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1166">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1167">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1167">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="ba2a5-1168">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1168">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="ba2a5-1169">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1169">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ba2a5-1170">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1170">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ba2a5-1171">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1171">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ba2a5-1172">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1172">Az.DataFactory</span></span>
* <span data-ttu-id="ba2a5-1173">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1173">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1174">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1174">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-1175">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1175">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="ba2a5-1176">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1176">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="ba2a5-1177">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1177">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-1178">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1178">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-1179">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1179">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-1180">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1180">Az.KeyVault</span></span>
* <span data-ttu-id="ba2a5-1181">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1181">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1182">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1182">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1183">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1183">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1184">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1185">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1185">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="ba2a5-1186">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1186">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="ba2a5-1187">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1187">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="ba2a5-1188">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1188">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="ba2a5-1189">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1189">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="ba2a5-1190">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1190">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="ba2a5-1191">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1191">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-1192">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1192">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-1193">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1193">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="ba2a5-1194">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1194">Fix some error messages.</span></span>
* <span data-ttu-id="ba2a5-1195">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1195">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="ba2a5-1196">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1196">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ba2a5-1197">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1197">Az.SignalR</span></span>
* <span data-ttu-id="ba2a5-1198">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1198">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1199">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1199">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1200">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1200">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ba2a5-1201">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1201">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="ba2a5-1202">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1202">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="ba2a5-1203">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1203">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-1204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1204">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-1205">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1205">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ba2a5-1206">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1206">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="ba2a5-1207">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1207">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="ba2a5-1208">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1208">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="ba2a5-1209">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1209">Az.TrafficManager</span></span>
* <span data-ttu-id="ba2a5-1210">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1210">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1211">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1211">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-1212">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1212">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ba2a5-1213">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1213">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="ba2a5-1214">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1214">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="ba2a5-1215">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1215">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1216">Az.Accounts</span></span>
* <span data-ttu-id="ba2a5-1217">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1217">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1218">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1219">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1219">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="ba2a5-1220">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1220">Updated the description of ID in help files</span></span>
* <span data-ttu-id="ba2a5-1221">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1221">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1222">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1222">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-1223">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1223">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="ba2a5-1224">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1224">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ba2a5-1225">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1225">Az.EventGrid</span></span>
* <span data-ttu-id="ba2a5-1226">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1226">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="ba2a5-1227">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1227">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="ba2a5-1228">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1228">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ba2a5-1229">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1229">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ba2a5-1230">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1230">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ba2a5-1231">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1231">Dead letter endpoint.</span></span>
    - <span data-ttu-id="ba2a5-1232">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1232">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ba2a5-1233">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1233">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ba2a5-1234">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1234">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ba2a5-1235">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1235">Dead letter endpoint.</span></span>
* <span data-ttu-id="ba2a5-1236">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1236">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="ba2a5-1237">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1237">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ba2a5-1238">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1238">Az.IotHub</span></span>
* <span data-ttu-id="ba2a5-1239">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1239">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ba2a5-1240">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1240">Az.LogicApp</span></span>
* <span data-ttu-id="ba2a5-1241">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1241">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1242">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1243">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1243">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="ba2a5-1244">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1244">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="ba2a5-1245">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1245">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ba2a5-1246">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1246">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="ba2a5-1247">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1247">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="ba2a5-1248">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1248">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ba2a5-1249">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1249">Az.SignalR</span></span>
* <span data-ttu-id="ba2a5-1250">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1250">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1251">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1251">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1252">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1252">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ba2a5-1253">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1253">Az.Storage</span></span>
* <span data-ttu-id="ba2a5-1254">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1254">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="ba2a5-1255">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1255">New-AzStorageContext</span></span>
* <span data-ttu-id="ba2a5-1256">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1256">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="ba2a5-1257">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1257">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1258">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1258">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-1259">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1259">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="ba2a5-1260">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1260">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="ba2a5-1261">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1261">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="ba2a5-1262">全般</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1262">General</span></span>

- <span data-ttu-id="ba2a5-1263">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1263">General Availability of Az Module</span></span>
- <span data-ttu-id="ba2a5-1264">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1264">Online help for each module</span></span>
- <span data-ttu-id="ba2a5-1265">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1265">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="ba2a5-1266">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1266">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="ba2a5-1267">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1267">Az.Accounts</span></span>
- <span data-ttu-id="ba2a5-1268">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1268">Changed from Az.Profile</span></span>
- <span data-ttu-id="ba2a5-1269">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1269">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-1270">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1270">Az.ApiManagement</span></span>
- <span data-ttu-id="ba2a5-1271">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1271">Fixes for #7002</span></span>
- <span data-ttu-id="ba2a5-1272">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1272">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="ba2a5-1273">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1273">Az.Batch</span></span>
- <span data-ttu-id="ba2a5-1274">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1274">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="ba2a5-1275">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1275">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="ba2a5-1276">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1276">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="ba2a5-1277">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1277">Az.Billing</span></span>
- <span data-ttu-id="ba2a5-1278">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1278">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="ba2a5-1279">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1279">Az.CognitivServices</span></span>
- <span data-ttu-id="ba2a5-1280">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1280">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="ba2a5-1281">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1281">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ba2a5-1282">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1282">Az.ContainerInstance</span></span>
- <span data-ttu-id="ba2a5-1283">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1283">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="ba2a5-1284">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1284">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="ba2a5-1285">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1285">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1286">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1286">Az.DataLakeStore</span></span>
- <span data-ttu-id="ba2a5-1287">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1287">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="ba2a5-1288">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1288">Az.Monitor</span></span>
- <span data-ttu-id="ba2a5-1289">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1289">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="ba2a5-1290">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1290">Az.KeyVault</span></span>
- <span data-ttu-id="ba2a5-1291">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1291">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="ba2a5-1292">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1292">Az.MachineLearning</span></span>
- <span data-ttu-id="ba2a5-1293">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1293">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="ba2a5-1294">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1294">Az.Media</span></span>
- <span data-ttu-id="ba2a5-1295">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1295">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1296">Az.Network</span></span>
<span data-ttu-id="ba2a5-1297">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1297">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="ba2a5-1298">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1298">New cmdlets added:</span></span>
        - <span data-ttu-id="ba2a5-1299">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1299">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1300">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1300">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1301">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1301">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1302">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1302">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1303">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1303">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1304">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1304">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="ba2a5-1305">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1305">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="ba2a5-1306">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1306">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="ba2a5-1307">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1307">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="ba2a5-1308">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1308">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="ba2a5-1309">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1309">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ba2a5-1310">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1310">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ba2a5-1311">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1311">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="ba2a5-1312">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1312">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="ba2a5-1313">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1313">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="ba2a5-1314">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1314">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="ba2a5-1315">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1315">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ba2a5-1316">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1316">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ba2a5-1317">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1317">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="ba2a5-1318">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1318">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="ba2a5-1319">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1319">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="ba2a5-1320">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1320">Az.OperationalInsights</span></span>
- <span data-ttu-id="ba2a5-1321">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1321">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="ba2a5-1322">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1322">Az.Profile</span></span>
- <span data-ttu-id="ba2a5-1323">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1323">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1324">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1324">Az.RecoveryServices</span></span>
- <span data-ttu-id="ba2a5-1325">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1325">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="ba2a5-1326">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1326">Az.Resources</span></span>
- <span data-ttu-id="ba2a5-1327">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1327">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-1328">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1328">Az.ServiceFabric</span></span>
- <span data-ttu-id="ba2a5-1329">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1329">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="ba2a5-1330">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1330">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="ba2a5-1331">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1331">Az.SIgnalR</span></span>
- <span data-ttu-id="ba2a5-1332">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1332">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="ba2a5-1333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1333">Az.Sql</span></span>
- <span data-ttu-id="ba2a5-1334">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1334">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="ba2a5-1335">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1335">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="ba2a5-1336">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1336">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="ba2a5-1337">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1337">Az.Storage</span></span>
- <span data-ttu-id="ba2a5-1338">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1338">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1339">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1339">Az.Websites</span></span>
- <span data-ttu-id="ba2a5-1340">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1340">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="ba2a5-1341">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1341">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="ba2a5-1342">全般</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1342">General</span></span>

* <span data-ttu-id="ba2a5-1343">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1343">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="ba2a5-1344">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1344">Az.Compute</span></span>

* <span data-ttu-id="ba2a5-1345">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1345">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1346">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1346">Az.DataLakeStore</span></span>

* <span data-ttu-id="ba2a5-1347">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1347">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="ba2a5-1348">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1348">Az.FrontDoor</span></span>

* <span data-ttu-id="ba2a5-1349">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1349">Fixed some broken links</span></span>
    - <span data-ttu-id="ba2a5-1350">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1350">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="ba2a5-1351">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1351">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ba2a5-1352">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1352">Az.RecoveryServices</span></span>

* <span data-ttu-id="ba2a5-1353">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1353">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="ba2a5-1354">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1354">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="ba2a5-1355">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1355">Az.Resources</span></span>

* <span data-ttu-id="ba2a5-1356">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1356">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="ba2a5-1357">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1357">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="ba2a5-1358">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1358">Az.Sql</span></span>

* <span data-ttu-id="ba2a5-1359">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1359">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="ba2a5-1360">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1360">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="ba2a5-1361">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1361">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="ba2a5-1362">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1362">Az.Storage</span></span>

* <span data-ttu-id="ba2a5-1363">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1363">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="ba2a5-1364">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1364">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="ba2a5-1365">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1365">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ba2a5-1366">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1366">Support Static Website configuration</span></span>
    - <span data-ttu-id="ba2a5-1367">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1367">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="ba2a5-1368">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1368">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1369">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1369">Az.Websites</span></span>

* <span data-ttu-id="ba2a5-1370">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1370">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="ba2a5-1371">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1371">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="ba2a5-1372">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1372">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="ba2a5-1373">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1373">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ba2a5-1374">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1374">Az.ApiManagement</span></span>
* <span data-ttu-id="ba2a5-1375">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1375">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="ba2a5-1376">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1376">Az.Automation</span></span>
* <span data-ttu-id="ba2a5-1377">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1377">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="ba2a5-1378">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1378">Added Update Management cmdlets</span></span>
* <span data-ttu-id="ba2a5-1379">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1379">Added Source Control cmdlets</span></span>
* <span data-ttu-id="ba2a5-1380">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1380">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="ba2a5-1381">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1381">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="ba2a5-1382">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1382">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1383">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1383">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="ba2a5-1384">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1384">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ba2a5-1385">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1385">Az.ContainerInstance</span></span>
* <span data-ttu-id="ba2a5-1386">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1386">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="ba2a5-1387">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1387">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ba2a5-1388">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1388">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1389">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1389">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1390">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1390">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="ba2a5-1391">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1391">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="ba2a5-1392">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1392">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="ba2a5-1393">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1393">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="ba2a5-1394">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1394">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ba2a5-1395">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1395">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="ba2a5-1396">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1396">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="ba2a5-1397">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1397">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="ba2a5-1398">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1398">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="ba2a5-1399">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1399">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="ba2a5-1400">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1400">Az.Relay</span></span>
* <span data-ttu-id="ba2a5-1401">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1401">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="ba2a5-1402">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1402">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1403">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1403">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="ba2a5-1404">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1404">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="ba2a5-1405">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1405">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-1406">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1406">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-1407">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1407">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="ba2a5-1408">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1408">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1409">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1409">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="ba2a5-1410">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1410">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ba2a5-1411">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1411">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ba2a5-1412">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1412">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ba2a5-1413">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1413">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ba2a5-1414">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1414">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ba2a5-1415">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1415">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ba2a5-1416">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1416">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ba2a5-1417">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1417">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="ba2a5-1418">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1418">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="ba2a5-1419">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1419">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="ba2a5-1420">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1420">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="ba2a5-1421">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1421">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ba2a5-1422">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1422">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ba2a5-1423">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1423">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="ba2a5-1424">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1424">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="ba2a5-1425">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1425">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="ba2a5-1426">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1426">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ba2a5-1427">全般</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1427">General</span></span>
* <span data-ttu-id="ba2a5-1428">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1428">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="ba2a5-1429">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1429">Az.Profile</span></span>
* <span data-ttu-id="ba2a5-1430">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1430">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="ba2a5-1431">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1431">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="ba2a5-1432">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1432">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="ba2a5-1433">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1433">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="ba2a5-1434">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1434">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="ba2a5-1435">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1435">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="ba2a5-1436">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1436">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-1437">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1437">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-1438">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1438">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1439">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1439">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1440">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1440">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="ba2a5-1441">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1441">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="ba2a5-1442">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1442">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1443">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1443">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-1444">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1444">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="ba2a5-1445">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1445">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="ba2a5-1446">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1446">Az.Insights</span></span>
* <span data-ttu-id="ba2a5-1447">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1447">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="ba2a5-1448">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1448">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="ba2a5-1449">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1449">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="ba2a5-1450">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1450">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1451">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1451">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1452">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1452">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="ba2a5-1453">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1453">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="ba2a5-1454">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1454">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="ba2a5-1455">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1455">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="ba2a5-1456">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1456">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="ba2a5-1457">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1457">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="ba2a5-1458">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1458">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ba2a5-1459">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1459">Az.PolicyInsights</span></span>
* <span data-ttu-id="ba2a5-1460">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1460">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1461">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1461">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1462">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1462">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="ba2a5-1463">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1463">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ba2a5-1464">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1464">Az.ServiceBus</span></span>
* <span data-ttu-id="ba2a5-1465">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1465">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ba2a5-1466">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1466">Az.ServiceFabric</span></span>
* <span data-ttu-id="ba2a5-1467">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1467">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="ba2a5-1468">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1468">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="ba2a5-1469">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1469">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="ba2a5-1470">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1470">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="ba2a5-1471">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1471">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="ba2a5-1472">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1472">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="ba2a5-1473">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1473">Az.Profile</span></span>
* <span data-ttu-id="ba2a5-1474">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1474">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="ba2a5-1475">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1475">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1476">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1476">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1477">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1477">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="ba2a5-1478">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1478">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ba2a5-1479">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1479">Az.DataLakeStore</span></span>
* <span data-ttu-id="ba2a5-1480">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1480">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="ba2a5-1481">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1481">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="ba2a5-1482">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1482">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ba2a5-1483">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1483">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ba2a5-1484">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1484">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1485">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1485">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1486">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1486">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="ba2a5-1487">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1487">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1488">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1488">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1489">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1489">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="ba2a5-1490">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1490">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="ba2a5-1491">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1491">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="ba2a5-1492">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1492">Azure.Storage</span></span>
* <span data-ttu-id="ba2a5-1493">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1493">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="ba2a5-1494">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1494">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="ba2a5-1495">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1495">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ba2a5-1496">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1496">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="ba2a5-1497">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1497">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="ba2a5-1498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1498">Az.CognitiveServices</span></span>
* <span data-ttu-id="ba2a5-1499">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1499">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ba2a5-1500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1500">Az.Compute</span></span>
* <span data-ttu-id="ba2a5-1501">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1501">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="ba2a5-1502">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1502">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="ba2a5-1503">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1503">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="ba2a5-1504">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1504">Az.DataFactoryV2</span></span>
* <span data-ttu-id="ba2a5-1505">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1505">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ba2a5-1506">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1506">Az.Network</span></span>
* <span data-ttu-id="ba2a5-1507">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1507">Added NetworkProfile functionality.</span></span> <span data-ttu-id="ba2a5-1508">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1508">new cmdlets added</span></span>
    - <span data-ttu-id="ba2a5-1509">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1509">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="ba2a5-1510">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1510">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="ba2a5-1511">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1511">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="ba2a5-1512">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1512">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="ba2a5-1513">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1513">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="ba2a5-1514">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1514">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="ba2a5-1515">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1515">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="ba2a5-1516">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1516">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="ba2a5-1517">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1517">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ba2a5-1518">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1518">Az.RedisCache</span></span>
* <span data-ttu-id="ba2a5-1519">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1519">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="ba2a5-1520">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1520">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="ba2a5-1521">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1521">Az.Resources</span></span>
* <span data-ttu-id="ba2a5-1522">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1522">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ba2a5-1523">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1523">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="ba2a5-1524">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1524">Az.Sql</span></span>
* <span data-ttu-id="ba2a5-1525">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1525">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ba2a5-1526">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1526">Az.Websites</span></span>
* <span data-ttu-id="ba2a5-1527">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1527">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="ba2a5-1528">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1528">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="ba2a5-1529">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1529">0.2.0 - September 2018</span></span>
 <span data-ttu-id="ba2a5-1530">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="ba2a5-1530">Initial Release</span></span>

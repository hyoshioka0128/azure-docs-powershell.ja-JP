---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: bcbb78809c2db63d665dc0c3d05e0614acce6045
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2020
ms.locfileid: "84122153"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="aadb3-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="aadb3-103">Azure PowerShell release notes</span></span>
## <a name="280---october-2019"></a><span data-ttu-id="aadb3-104">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-104">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="aadb3-105">全般</span><span class="sxs-lookup"><span data-stu-id="aadb3-105">General</span></span>
* <span data-ttu-id="aadb3-106">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-106">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aadb3-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-107">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-108">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-108">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="aadb3-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-109">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-110">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-110">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="aadb3-111">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="aadb3-111">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-112">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-112">Az.Automation</span></span>
* <span data-ttu-id="aadb3-113">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-113">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="aadb3-114">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aadb3-114">Az.Batch</span></span>
* <span data-ttu-id="aadb3-115">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-115">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-116">Az.Compute</span></span>
* <span data-ttu-id="aadb3-117">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-117">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="aadb3-118">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="aadb3-118">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="aadb3-119">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-119">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="aadb3-120">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-120">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-121">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-121">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-122">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="aadb3-122">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="aadb3-123">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="aadb3-123">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="aadb3-124">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-124">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-125">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-125">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-126">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="aadb3-126">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="aadb3-127">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="aadb3-127">Az.HealthcareApis</span></span>
* <span data-ttu-id="aadb3-128">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-128">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="aadb3-129">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-129">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="aadb3-130">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-130">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="aadb3-131">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-131">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-132">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-132">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-133">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="aadb3-133">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="aadb3-134">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="aadb3-134">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-135">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-136">New-AzActionGroupReceiver に新しいアクション グループ受信者が追加されました: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="aadb3-136">New action group receivers added for New-AzActionGroupReceiver:   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="aadb3-137">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-137">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="aadb3-138">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="aadb3-138">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="aadb3-139">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-139">Webhooks now supports Azure active directory authentication.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-140">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-140">Az.Network</span></span>
* <span data-ttu-id="aadb3-141">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-141">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="aadb3-142">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-142">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="aadb3-143">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="aadb3-143">New cmdlets added:</span></span>
        - <span data-ttu-id="aadb3-144">New-AzIpsecTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-144">New-AzIpsecTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="aadb3-145">省略可能なパラメーター -TrafficSelectorPolicies を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-145">Cmdlets updated with optional parameter -TrafficSelectorPolicies</span></span>
        - <span data-ttu-id="aadb3-146">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-146">New-AzVirtualNetworkGatewayConnection</span></span>
        - <span data-ttu-id="aadb3-147">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-147">Set-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="aadb3-148">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-148">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="aadb3-149">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-149">Updated cmdlets:</span></span>
        - <span data-ttu-id="aadb3-150">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-150">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="aadb3-151">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-151">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="aadb3-152">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-152">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="aadb3-153">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="aadb3-153">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="aadb3-154">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="aadb3-154">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="aadb3-155">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-155">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="aadb3-156">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-156">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="aadb3-157">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="aadb3-157">Az.RedisCache</span></span>
* <span data-ttu-id="aadb3-158">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-158">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-159">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-159">Az.Sql</span></span>
* <span data-ttu-id="aadb3-160">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-160">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-161">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-161">Az.Storage</span></span>
* <span data-ttu-id="aadb3-162">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="aadb3-162">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="aadb3-163">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aadb3-163">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="aadb3-164">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="aadb3-164">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="aadb3-165">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aadb3-165">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="aadb3-166">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-166">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="aadb3-167">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="aadb3-167">Az.StorageSync</span></span>
* <span data-ttu-id="aadb3-168">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-168">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-169">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-169">Az.Websites</span></span>
* <span data-ttu-id="aadb3-170">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="aadb3-170">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="aadb3-171">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-171">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="aadb3-172">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-172">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-173">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-173">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="aadb3-174">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-174">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="aadb3-175">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="aadb3-175">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-176">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-176">Az.Automation</span></span>
* <span data-ttu-id="aadb3-177">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-177">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="aadb3-178">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-178">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="aadb3-179">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-179">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-180">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-180">Az.Compute</span></span>
* <span data-ttu-id="aadb3-181">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-181">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="aadb3-182">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-182">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="aadb3-183">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-183">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="aadb3-184">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-184">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="aadb3-185">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-185">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="aadb3-186">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-186">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="aadb3-187">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-187">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="aadb3-188">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-188">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="aadb3-189">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-189">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-190">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-190">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-191">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-191">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="aadb3-192">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-192">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="aadb3-193">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="aadb3-193">Az.HDInsight</span></span>
* <span data-ttu-id="aadb3-194">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="aadb3-194">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-195">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-195">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-196">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-196">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="aadb3-197">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-197">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="aadb3-198">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="aadb3-198">New cmdlets are:</span></span>
    - <span data-ttu-id="aadb3-199">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="aadb3-199">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="aadb3-200">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="aadb3-200">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="aadb3-201">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="aadb3-201">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="aadb3-202">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="aadb3-202">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-203">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-203">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-204">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="aadb3-204">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="aadb3-205">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-205">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="aadb3-206">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="aadb3-206">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="aadb3-207">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="aadb3-207">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="aadb3-208">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-208">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="aadb3-209">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-209">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="aadb3-210">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="aadb3-210">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="aadb3-211">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="aadb3-211">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="aadb3-212">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-212">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="aadb3-213">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="aadb3-213">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="aadb3-214">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-214">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="aadb3-215">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="aadb3-215">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="aadb3-216">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-216">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="aadb3-217">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-217">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="aadb3-218">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-218">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="aadb3-219">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="aadb3-219">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="aadb3-220">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-220">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="aadb3-221">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-221">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="aadb3-222">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-222">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="aadb3-223">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-223">Overall improved help files</span></span>
* <span data-ttu-id="aadb3-224">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="aadb3-224">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-225">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-225">Az.Network</span></span>
* <span data-ttu-id="aadb3-226">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="aadb3-226">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="aadb3-227">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-227">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="aadb3-228">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-228">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="aadb3-229">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-229">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="aadb3-230">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-230">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="aadb3-231">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-231">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="aadb3-232">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-232">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="aadb3-233">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-233">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="aadb3-234">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-234">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="aadb3-235">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-235">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="aadb3-236">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-236">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="aadb3-237">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-237">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="aadb3-238">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-238">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-239">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="aadb3-239">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="aadb3-240">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-240">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="aadb3-241">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-241">Updated cmdlet:</span></span>
        - <span data-ttu-id="aadb3-242">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="aadb3-242">New-VpnSite</span></span>
        - <span data-ttu-id="aadb3-243">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="aadb3-243">Update-VpnSite</span></span>
        - <span data-ttu-id="aadb3-244">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-244">New-VpnConnection</span></span>
        - <span data-ttu-id="aadb3-245">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-245">Update-VpnConnection</span></span>
* <span data-ttu-id="aadb3-246">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-246">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-247">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-248">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-248">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="aadb3-249">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-249">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-250">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-250">Az.Resources</span></span>
* <span data-ttu-id="aadb3-251">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-251">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-252">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-252">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-253">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-253">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="aadb3-254">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-254">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="aadb3-255">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="aadb3-255">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="aadb3-256">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="aadb3-256">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="aadb3-257">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="aadb3-257">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="aadb3-258">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="aadb3-258">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="aadb3-259">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="aadb3-259">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="aadb3-260">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="aadb3-260">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="aadb3-261">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="aadb3-261">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="aadb3-262">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="aadb3-262">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="aadb3-263">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="aadb3-263">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="aadb3-264">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="aadb3-264">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="aadb3-265">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="aadb3-265">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="aadb3-266">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="aadb3-266">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="aadb3-267">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="aadb3-267">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="aadb3-268">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-268">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="aadb3-269">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="aadb3-269">Az.SignalR</span></span>
* <span data-ttu-id="aadb3-270">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="aadb3-270">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-271">Az.Sql</span></span>
* <span data-ttu-id="aadb3-272">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-272">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="aadb3-273">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-273">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="aadb3-274">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="aadb3-274">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="aadb3-275">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-275">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="aadb3-276">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="aadb3-276">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-277">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-277">Az.Storage</span></span>
* <span data-ttu-id="aadb3-278">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-278">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="aadb3-279">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="aadb3-279">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="aadb3-280">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-280">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="aadb3-281">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-281">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="aadb3-282">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-282">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="aadb3-283">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-283">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="aadb3-284">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="aadb3-284">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="aadb3-285">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="aadb3-285">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="aadb3-286">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="aadb3-286">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="aadb3-287">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="aadb3-287">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="aadb3-288">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="aadb3-288">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-289">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-289">Az.Websites</span></span>
* <span data-ttu-id="aadb3-290">アプリを新しい ASP に移行するときに webapp タグが削除されるという問題を修正しています</span><span class="sxs-lookup"><span data-stu-id="aadb3-290">Fixing issue where webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="aadb3-291">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="aadb3-291">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="aadb3-292">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-292">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="aadb3-293">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-293">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="aadb3-294">全般</span><span class="sxs-lookup"><span data-stu-id="aadb3-294">General</span></span>
* <span data-ttu-id="aadb3-295">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-295">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aadb3-296">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-296">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-297">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="aadb3-297">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="aadb3-298">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="aadb3-298">Az.Aks</span></span>
* <span data-ttu-id="aadb3-299">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-299">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="aadb3-300">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="aadb3-300">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="aadb3-301">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-301">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-302">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="aadb3-302">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="aadb3-303">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="aadb3-303">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="aadb3-304">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-304">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="aadb3-305">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="aadb3-305">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="aadb3-306">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-306">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="aadb3-307">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aadb3-307">Az.Batch</span></span>
* <span data-ttu-id="aadb3-308">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-308">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aadb3-309">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aadb3-309">Az.Cdn</span></span>
* <span data-ttu-id="aadb3-310">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-310">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-311">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-311">Az.Compute</span></span>
* <span data-ttu-id="aadb3-312">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-312">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="aadb3-313">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-313">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="aadb3-314">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-314">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="aadb3-315">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-315">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="aadb3-316">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="aadb3-316">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="aadb3-317">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="aadb3-317">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="aadb3-318">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-318">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="aadb3-319">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-319">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-320">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-320">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-321">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-321">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="aadb3-322">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-322">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="aadb3-323">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-323">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="aadb3-324">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-324">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-325">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-325">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-326">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-326">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aadb3-327">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-327">Az.EventHub</span></span>
* <span data-ttu-id="aadb3-328">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="aadb3-328">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="aadb3-329">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="aadb3-329">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="aadb3-330">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-330">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="aadb3-331">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="aadb3-331">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="aadb3-332">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="aadb3-332">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="aadb3-333">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-333">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-334">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-334">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-335">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-335">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-336">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-336">Az.Network</span></span>
* <span data-ttu-id="aadb3-337">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-337">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="aadb3-338">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-338">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="aadb3-339">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-339">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="aadb3-340">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-340">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="aadb3-341">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-341">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="aadb3-342">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-342">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="aadb3-343">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-343">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-344">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-344">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-345">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-345">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="aadb3-346">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-346">Added example</span></span>
    - <span data-ttu-id="aadb3-347">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-347">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="aadb3-348">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-348">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="aadb3-349">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-349">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-350">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-351">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-351">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-352">Az.Resources</span></span>
* <span data-ttu-id="aadb3-353">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-353">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="aadb3-354">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-354">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="aadb3-355">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="aadb3-355">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="aadb3-356">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-356">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-357">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-357">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-358">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="aadb3-358">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="aadb3-359">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="aadb3-359">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="aadb3-360">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-360">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-361">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-361">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-362">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-362">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="aadb3-363">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="aadb3-363">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="aadb3-364">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="aadb3-364">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="aadb3-365">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-365">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="aadb3-366">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="aadb3-366">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="aadb3-367">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-367">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-368">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-368">Az.Sql</span></span>
* <span data-ttu-id="aadb3-369">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-369">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-370">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-370">Az.Storage</span></span>
* <span data-ttu-id="aadb3-371">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-371">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="aadb3-372">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="aadb3-372">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="aadb3-373">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-373">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="aadb3-374">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="aadb3-374">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="aadb3-375">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="aadb3-375">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="aadb3-376">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="aadb3-376">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-377">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-377">Az.Websites</span></span>
* <span data-ttu-id="aadb3-378">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-378">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="aadb3-379">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-379">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-380">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-380">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-381">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-381">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="aadb3-382">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-382">Az.ApplicationInsights</span></span>
* <span data-ttu-id="aadb3-383">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-383">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-384">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-384">Az.Automation</span></span>
* <span data-ttu-id="aadb3-385">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-385">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-386">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-386">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-387">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-387">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-388">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-388">Az.Compute</span></span>
* <span data-ttu-id="aadb3-389">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-389">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="aadb3-390">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="aadb3-390">Az.ContainerRegistry</span></span>
* <span data-ttu-id="aadb3-391">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-391">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="aadb3-392">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="aadb3-392">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-393">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-393">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-394">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-394">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="aadb3-395">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-395">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aadb3-396">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-396">Az.EventHub</span></span>
* <span data-ttu-id="aadb3-397">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="aadb3-397">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="aadb3-398">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-398">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aadb3-399">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-399">Az.KeyVault</span></span>
* <span data-ttu-id="aadb3-400">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-400">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aadb3-401">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aadb3-401">Az.LogicApp</span></span>
* <span data-ttu-id="aadb3-402">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-402">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="aadb3-403">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-403">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="aadb3-404">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-404">Az.ManagedServices</span></span>
* <span data-ttu-id="aadb3-405">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-405">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-406">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-406">Az.Network</span></span>
* <span data-ttu-id="aadb3-407">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-407">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="aadb3-408">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-408">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-409">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="aadb3-409">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="aadb3-410">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="aadb3-410">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="aadb3-411">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-411">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="aadb3-412">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-412">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="aadb3-413">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-413">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="aadb3-414">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-414">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="aadb3-415">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="aadb3-415">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="aadb3-416">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="aadb3-416">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="aadb3-417">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="aadb3-417">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="aadb3-418">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-418">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="aadb3-419">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-419">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="aadb3-420">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-420">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="aadb3-421">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="aadb3-421">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="aadb3-422">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-422">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="aadb3-423">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-423">Updated cmdlets</span></span>
        - <span data-ttu-id="aadb3-424">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-424">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="aadb3-425">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-425">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="aadb3-426">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-426">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="aadb3-427">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-427">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="aadb3-428">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-428">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="aadb3-429">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-429">Updated cmdlet:</span></span>
        - <span data-ttu-id="aadb3-430">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-430">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="aadb3-431">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-431">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="aadb3-432">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-432">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="aadb3-433">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-433">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="aadb3-434">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-434">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="aadb3-435">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-435">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-436">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-436">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-437">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-437">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="aadb3-438">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-438">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-439">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-439">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-440">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-440">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="aadb3-441">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-441">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="aadb3-442">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-442">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="aadb3-443">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-443">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="aadb3-444">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-444">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="aadb3-445">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-445">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="aadb3-446">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-446">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="aadb3-447">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-447">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="aadb3-448">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-448">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="aadb3-449">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-449">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-450">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-450">Az.Resources</span></span>
- <span data-ttu-id="aadb3-451">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-451">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="aadb3-452">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-452">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-453">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-453">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-454">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="aadb3-454">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="aadb3-455">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-455">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-456">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-456">Az.Sql</span></span>
* <span data-ttu-id="aadb3-457">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-457">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="aadb3-458">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-458">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="aadb3-459">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-459">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-460">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-460">Az.Storage</span></span>
* <span data-ttu-id="aadb3-461">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-461">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="aadb3-462">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="aadb3-462">Az.StorageSync</span></span>
* <span data-ttu-id="aadb3-463">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-463">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="aadb3-464">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-464">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-465">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-465">Az.Websites</span></span>
* <span data-ttu-id="aadb3-466">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-466">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="aadb3-467">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-467">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="aadb3-468">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-468">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="aadb3-469">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-469">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-470">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-470">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-471">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-471">Add support for profile cmdlets</span></span>
* <span data-ttu-id="aadb3-472">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-472">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="aadb3-473">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-473">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="aadb3-474">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="aadb3-474">Az.Advisor</span></span>
* <span data-ttu-id="aadb3-475">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-475">GA release of Az.Advisor</span></span>
* <span data-ttu-id="aadb3-476">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-476">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="aadb3-477">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-477">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-478">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="aadb3-478">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="aadb3-479">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="aadb3-479">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="aadb3-480">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-480">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="aadb3-481">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-481">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="aadb3-482">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-482">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="aadb3-483">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="aadb3-483">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="aadb3-484">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-484">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-485">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-485">Az.Automation</span></span>
* <span data-ttu-id="aadb3-486">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-486">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-487">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-487">Az.Compute</span></span>
* <span data-ttu-id="aadb3-488">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-488">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-489">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-489">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-490">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-490">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aadb3-491">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aadb3-491">Az.EventGrid</span></span>
* <span data-ttu-id="aadb3-492">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-492">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-493">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-493">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-494">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-494">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-495">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-495">Az.Network</span></span>
* <span data-ttu-id="aadb3-496">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-496">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="aadb3-497">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-497">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="aadb3-498">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-498">Az.PolicyInsights</span></span>
* <span data-ttu-id="aadb3-499">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-499">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="aadb3-500">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="aadb3-500">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-501">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-501">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-502">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-502">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-503">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-503">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-504">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-504">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-505">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-505">Az.Resources</span></span>
    - <span data-ttu-id="aadb3-506">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-506">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="aadb3-507">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-507">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="aadb3-508">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-508">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="aadb3-509">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-509">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-510">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-510">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-511">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="aadb3-511">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-512">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-512">Az.Sql</span></span>
* <span data-ttu-id="aadb3-513">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-513">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="aadb3-514">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-514">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="aadb3-515">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-515">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="aadb3-516">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-516">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="aadb3-517">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-517">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="aadb3-518">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-518">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="aadb3-519">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-519">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="aadb3-520">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="aadb3-520">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="aadb3-521">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-521">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-522">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-522">Az.Storage</span></span>
* <span data-ttu-id="aadb3-523">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-523">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="aadb3-524">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="aadb3-524">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="aadb3-525">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-525">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="aadb3-526">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="aadb3-526">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="aadb3-527">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-527">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="aadb3-528">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-528">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="aadb3-529">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-529">Set-AzStorageAccount</span></span>
* <span data-ttu-id="aadb3-530">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-530">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="aadb3-531">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="aadb3-531">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="aadb3-532">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="aadb3-532">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="aadb3-533">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="aadb3-533">Az.StorageSync</span></span>
* <span data-ttu-id="aadb3-534">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-534">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="aadb3-535">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-535">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-536">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-536">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-537">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-537">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="aadb3-538">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="aadb3-538">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="aadb3-539">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-539">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="aadb3-540">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="aadb3-540">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="aadb3-541">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="aadb3-541">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-542">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-542">Az.Compute</span></span>
* <span data-ttu-id="aadb3-543">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-543">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="aadb3-544">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-544">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="aadb3-545">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="aadb3-545">Az.Dns</span></span>
* <span data-ttu-id="aadb3-546">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-546">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aadb3-547">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aadb3-547">Az.EventGrid</span></span>
* <span data-ttu-id="aadb3-548">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-548">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="aadb3-549">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-549">New cmdlets:</span></span>
    - <span data-ttu-id="aadb3-550">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="aadb3-550">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="aadb3-551">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-551">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="aadb3-552">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="aadb3-552">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="aadb3-553">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-553">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="aadb3-554">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="aadb3-554">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="aadb3-555">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-555">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="aadb3-556">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="aadb3-556">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="aadb3-557">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-557">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="aadb3-558">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="aadb3-558">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="aadb3-559">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-559">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="aadb3-560">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="aadb3-560">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="aadb3-561">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-561">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="aadb3-562">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="aadb3-562">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="aadb3-563">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-563">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="aadb3-564">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="aadb3-564">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="aadb3-565">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-565">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="aadb3-566">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-566">Updated cmdlets:</span></span>
    - <span data-ttu-id="aadb3-567">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="aadb3-567">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="aadb3-568">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-568">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="aadb3-569">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-569">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="aadb3-570">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="aadb3-570">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="aadb3-571">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="aadb3-571">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="aadb3-572">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="aadb3-572">Event subscription expiration date,</span></span>
            - <span data-ttu-id="aadb3-573">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="aadb3-573">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="aadb3-574">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-574">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="aadb3-575">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="aadb3-575">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="aadb3-576">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="aadb3-576">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="aadb3-577">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-577">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="aadb3-578">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="aadb3-578">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="aadb3-579">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-579">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="aadb3-580">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-580">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="aadb3-581">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="aadb3-581">Az.FrontDoor</span></span>
* <span data-ttu-id="aadb3-582">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="aadb3-582">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="aadb3-583">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-583">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="aadb3-584">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="aadb3-584">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="aadb3-585">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-585">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-586">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-586">Az.Network</span></span>
* <span data-ttu-id="aadb3-587">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-587">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="aadb3-588">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-588">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-589">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="aadb3-589">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="aadb3-590">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-590">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="aadb3-591">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-591">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-592">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="aadb3-592">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="aadb3-593">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-593">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="aadb3-594">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-594">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-595">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="aadb3-595">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="aadb3-596">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="aadb3-596">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="aadb3-597">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="aadb3-597">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="aadb3-598">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-598">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="aadb3-599">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-599">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="aadb3-600">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-600">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="aadb3-601">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-601">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-602">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="aadb3-602">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="aadb3-603">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="aadb3-603">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="aadb3-604">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="aadb3-604">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="aadb3-605">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="aadb3-605">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="aadb3-606">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="aadb3-606">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="aadb3-607">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-607">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="aadb3-608">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-608">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="aadb3-609">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-609">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="aadb3-610">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-610">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="aadb3-611">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-611">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="aadb3-612">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-612">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="aadb3-613">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-613">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="aadb3-614">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-614">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="aadb3-615">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-615">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="aadb3-616">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-616">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="aadb3-617">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-617">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="aadb3-618">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-618">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="aadb3-619">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-619">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="aadb3-620">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="aadb3-620">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="aadb3-621">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-621">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="aadb3-622">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-622">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="aadb3-623">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="aadb3-623">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="aadb3-624">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-624">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="aadb3-625">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-625">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="aadb3-626">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-626">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="aadb3-627">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-627">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="aadb3-628">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-628">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-629">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-629">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-630">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-630">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-631">Az.Resources</span></span>
* <span data-ttu-id="aadb3-632">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="aadb3-632">Support for additional Template Export options</span></span>
    - <span data-ttu-id="aadb3-633">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-633">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="aadb3-634">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-634">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="aadb3-635">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-635">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-636">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-636">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-637">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-637">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-638">Az.Sql</span></span>
* <span data-ttu-id="aadb3-639">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-639">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="aadb3-640">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-640">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="aadb3-641">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-641">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="aadb3-642">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="aadb3-642">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="aadb3-643">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="aadb3-643">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="aadb3-644">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="aadb3-644">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="aadb3-645">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="aadb3-645">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="aadb3-646">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="aadb3-646">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-647">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-647">Az.Storage</span></span>
* <span data-ttu-id="aadb3-648">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-648">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="aadb3-649">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-649">New-AzStorageAccount</span></span>
* <span data-ttu-id="aadb3-650">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-650">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="aadb3-651">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-651">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-652">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-652">Az.Websites</span></span>
* <span data-ttu-id="aadb3-653">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-653">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="aadb3-654">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-654">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="aadb3-655">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-655">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="aadb3-656">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aadb3-656">Az.Cdn</span></span>
* <span data-ttu-id="aadb3-657">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-657">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-658">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-658">Az.Compute</span></span>
* <span data-ttu-id="aadb3-659">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-659">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="aadb3-660">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="aadb3-660">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aadb3-661">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-661">Az.EventHub</span></span>
* <span data-ttu-id="aadb3-662">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-662">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="aadb3-663">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-663">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-664">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-664">Az.Network</span></span>
* <span data-ttu-id="aadb3-665">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-665">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="aadb3-666">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-666">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="aadb3-667">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-667">Az.PolicyInsights</span></span>
* <span data-ttu-id="aadb3-668">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-668">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-669">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-669">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-670">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-670">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-671">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-671">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-672">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-672">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-673">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-673">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-674">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-674">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="aadb3-675">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-675">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-676">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-676">Az.Sql</span></span>
* <span data-ttu-id="aadb3-677">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-677">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="aadb3-678">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="aadb3-678">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="aadb3-679">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-679">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="aadb3-680">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-680">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-681">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-681">Az.Websites</span></span>
* <span data-ttu-id="aadb3-682">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-682">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="aadb3-683">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-683">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="aadb3-684">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-684">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-685">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-685">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="aadb3-686">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="aadb3-686">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="aadb3-687">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="aadb3-687">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="aadb3-688">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="aadb3-688">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="aadb3-689">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-689">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="aadb3-690">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="aadb3-690">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="aadb3-691">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="aadb3-691">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="aadb3-692">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-692">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="aadb3-693">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-693">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="aadb3-694">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="aadb3-694">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="aadb3-695">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="aadb3-695">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="aadb3-696">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="aadb3-696">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="aadb3-697">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-697">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="aadb3-698">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-698">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="aadb3-699">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="aadb3-699">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="aadb3-700">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="aadb3-700">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="aadb3-701">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="aadb3-701">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="aadb3-702">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="aadb3-702">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="aadb3-703">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-703">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="aadb3-704">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="aadb3-704">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="aadb3-705">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-705">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="aadb3-706">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-706">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="aadb3-707">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="aadb3-707">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="aadb3-708">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-708">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="aadb3-709">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-709">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="aadb3-710">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-710">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="aadb3-711">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-711">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="aadb3-712">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-712">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="aadb3-713">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-713">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="aadb3-714">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-714">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="aadb3-715">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-715">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="aadb3-716">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="aadb3-716">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="aadb3-717">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-717">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="aadb3-718">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-718">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="aadb3-719">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="aadb3-719">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="aadb3-720">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="aadb3-720">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="aadb3-721">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="aadb3-721">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="aadb3-722">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-722">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="aadb3-723">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-723">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="aadb3-724">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-724">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="aadb3-725">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="aadb3-725">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="aadb3-726">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="aadb3-726">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="aadb3-727">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="aadb3-727">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="aadb3-728">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-728">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="aadb3-729">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-729">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="aadb3-730">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="aadb3-730">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="aadb3-731">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="aadb3-731">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="aadb3-732">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-732">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="aadb3-733">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-733">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="aadb3-734">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="aadb3-734">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="aadb3-735">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="aadb3-735">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="aadb3-736">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="aadb3-736">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="aadb3-737">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="aadb3-737">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="aadb3-738">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-738">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="aadb3-739">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="aadb3-739">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="aadb3-740">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="aadb3-740">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="aadb3-741">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-741">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="aadb3-742">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="aadb3-742">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="aadb3-743">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="aadb3-743">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="aadb3-744">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-744">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="aadb3-745">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-745">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="aadb3-746">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="aadb3-746">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="aadb3-747">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="aadb3-747">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="aadb3-748">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-748">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="aadb3-749">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-749">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="aadb3-750">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="aadb3-750">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="aadb3-751">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="aadb3-751">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="aadb3-752">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="aadb3-752">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="aadb3-753">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="aadb3-753">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="aadb3-754">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="aadb3-754">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="aadb3-755">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="aadb3-755">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="aadb3-756">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="aadb3-756">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="aadb3-757">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="aadb3-757">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="aadb3-758">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-758">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="aadb3-759">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="aadb3-759">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="aadb3-760">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="aadb3-760">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="aadb3-761">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="aadb3-761">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-762">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-762">Az.Automation</span></span>
* <span data-ttu-id="aadb3-763">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-763">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="aadb3-764">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="aadb3-764">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="aadb3-765">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="aadb3-765">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="aadb3-766">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-766">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="aadb3-767">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="aadb3-767">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="aadb3-768">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-768">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="aadb3-769">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-769">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-770">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-770">Az.Compute</span></span>
* <span data-ttu-id="aadb3-771">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-771">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="aadb3-772">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-772">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-773">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-773">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-774">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-774">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-775">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-775">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-776">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-776">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-777">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-777">Az.Network</span></span>
* <span data-ttu-id="aadb3-778">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-778">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="aadb3-779">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="aadb3-779">Updated cmdlet:</span></span>
        - <span data-ttu-id="aadb3-780">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="aadb3-780">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="aadb3-781">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-781">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-782">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-782">Az.Resources</span></span>
* <span data-ttu-id="aadb3-783">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-783">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-784">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-784">Az.Sql</span></span>
* <span data-ttu-id="aadb3-785">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-785">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="aadb3-786">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-786">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-787">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-787">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-788">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-788">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-789">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-789">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-790">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-790">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="aadb3-791">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-791">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-792">Az.Compute</span></span>
* <span data-ttu-id="aadb3-793">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="aadb3-793">Proximity placement group feature.</span></span>
    - <span data-ttu-id="aadb3-794">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="aadb3-794">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="aadb3-795">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-795">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="aadb3-796">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-796">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="aadb3-797">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-797">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="aadb3-798">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-798">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="aadb3-799">重大な変更</span><span class="sxs-lookup"><span data-stu-id="aadb3-799">Breaking changes</span></span>
    - <span data-ttu-id="aadb3-800">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="aadb3-800">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="aadb3-801">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="aadb3-801">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="aadb3-802">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="aadb3-802">Az.DeploymentManager</span></span>
* <span data-ttu-id="aadb3-803">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-803">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="aadb3-804">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="aadb3-804">Az.Dns</span></span>
* <span data-ttu-id="aadb3-805">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="aadb3-805">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="aadb3-806">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-806">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="aadb3-807">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-807">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="aadb3-808">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="aadb3-808">Az.FrontDoor</span></span>
* <span data-ttu-id="aadb3-809">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-809">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="aadb3-810">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-810">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="aadb3-811">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="aadb3-811">Az.HDInsight</span></span>
* <span data-ttu-id="aadb3-812">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-812">Removed two cmdlets:</span></span>
    - <span data-ttu-id="aadb3-813">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="aadb3-813">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="aadb3-814">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="aadb3-814">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="aadb3-815">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-815">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="aadb3-816">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-816">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="aadb3-817">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-817">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="aadb3-818">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="aadb3-818">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-819">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-819">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-820">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="aadb3-820">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="aadb3-821">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="aadb3-821">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="aadb3-822">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="aadb3-822">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="aadb3-823">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="aadb3-823">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="aadb3-824">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="aadb3-824">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="aadb3-825">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="aadb3-825">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="aadb3-826">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="aadb3-826">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="aadb3-827">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-827">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="aadb3-828">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-828">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="aadb3-829">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-829">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="aadb3-830">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-830">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="aadb3-831">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-831">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="aadb3-832">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="aadb3-832">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="aadb3-833">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-833">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-834">Az.Network</span></span>
* <span data-ttu-id="aadb3-835">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-835">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="aadb3-836">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-836">New cmdlets</span></span>
        - <span data-ttu-id="aadb3-837">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="aadb3-837">New-AzNatGateway</span></span>
        - <span data-ttu-id="aadb3-838">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="aadb3-838">Get-AzNatGateway</span></span>
        - <span data-ttu-id="aadb3-839">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="aadb3-839">Set-AzNatGateway</span></span>
        - <span data-ttu-id="aadb3-840">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="aadb3-840">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="aadb3-841">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-841">Updated cmdlets</span></span>
        - <span data-ttu-id="aadb3-842">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="aadb3-842">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="aadb3-843">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="aadb3-843">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="aadb3-844">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="aadb3-844">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="aadb3-845">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-845">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="aadb3-846">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-846">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="aadb3-847">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-847">Az.PolicyInsights</span></span>
* <span data-ttu-id="aadb3-848">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="aadb3-848">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="aadb3-849">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-849">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="aadb3-850">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-850">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-851">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-851">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-852">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="aadb3-852">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="aadb3-853">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="aadb3-853">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="aadb3-854">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="aadb3-854">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="aadb3-855">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="aadb3-855">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="aadb3-856">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="aadb3-856">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="aadb3-857">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="aadb3-857">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="aadb3-858">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="aadb3-858">Az.Relay</span></span>
* <span data-ttu-id="aadb3-859">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-859">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-860">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-860">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-861">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-861">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-862">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-862">Az.Storage</span></span>
* <span data-ttu-id="aadb3-863">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="aadb3-863">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="aadb3-864">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-864">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="aadb3-865">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-865">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="aadb3-866">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-866">New-AzStorageAccount</span></span>
* <span data-ttu-id="aadb3-867">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="aadb3-867">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="aadb3-868">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-868">New-AzStorageAccount</span></span>
    - <span data-ttu-id="aadb3-869">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-869">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="aadb3-870">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="aadb3-870">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-871">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-871">Az.Websites</span></span>
* <span data-ttu-id="aadb3-872">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="aadb3-872">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="aadb3-873">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="aadb3-873">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="aadb3-874">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-874">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aadb3-875">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="aadb3-875">Highlights since the last major release</span></span>
* <span data-ttu-id="aadb3-876">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="aadb3-876">General availability of `Az` module</span></span>
* <span data-ttu-id="aadb3-877">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aadb3-877">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aadb3-878">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aadb3-878">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aadb3-879">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-879">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aadb3-880">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-880">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aadb3-881">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-881">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aadb3-882">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-882">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aadb3-883">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-883">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-884">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-884">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="aadb3-885">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aadb3-885">Az.Batch</span></span>
* <span data-ttu-id="aadb3-886">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-886">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aadb3-887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aadb3-887">Az.Cdn</span></span>
* <span data-ttu-id="aadb3-888">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-888">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-889">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-889">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-890">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-891">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-891">Az.Compute</span></span>
* <span data-ttu-id="aadb3-892">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-892">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="aadb3-893">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-893">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-894">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-894">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-895">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-896">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-896">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-897">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-898">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-898">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aadb3-899">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aadb3-899">Az.EventGrid</span></span>
* <span data-ttu-id="aadb3-900">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-900">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aadb3-901">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-901">Az.EventHub</span></span>
* <span data-ttu-id="aadb3-902">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-902">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="aadb3-903">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="aadb3-903">Az.HDInsight</span></span>
* <span data-ttu-id="aadb3-904">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-904">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-905">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-905">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-906">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-906">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aadb3-907">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-907">Az.KeyVault</span></span>
* <span data-ttu-id="aadb3-908">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-908">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-909">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-909">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="aadb3-910">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="aadb3-910">Az.MachineLearning</span></span>
* <span data-ttu-id="aadb3-911">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-911">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="aadb3-912">Az.Media</span><span class="sxs-lookup"><span data-stu-id="aadb3-912">Az.Media</span></span>
* <span data-ttu-id="aadb3-913">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-913">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-914">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-914">Az.Monitor</span></span>
  * <span data-ttu-id="aadb3-915">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-915">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="aadb3-916">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="aadb3-916">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="aadb3-917">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="aadb3-917">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="aadb3-918">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aadb3-918">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="aadb3-919">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aadb3-919">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="aadb3-920">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="aadb3-920">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="aadb3-921">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-921">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-922">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-922">Az.Network</span></span>
* <span data-ttu-id="aadb3-923">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-923">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-924">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-924">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="aadb3-925">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="aadb3-925">Az.NotificationHubs</span></span>
* <span data-ttu-id="aadb3-926">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-926">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-927">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-927">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-928">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-928">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="aadb3-929">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="aadb3-929">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="aadb3-930">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-930">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-931">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-931">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-932">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-932">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-933">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-933">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="aadb3-934">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-934">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="aadb3-935">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-935">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="aadb3-936">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="aadb3-936">Az.RedisCache</span></span>
* <span data-ttu-id="aadb3-937">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-937">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-938">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-938">Az.Resources</span></span>
* <span data-ttu-id="aadb3-939">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-939">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-940">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-940">Az.Sql</span></span>
* <span data-ttu-id="aadb3-941">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="aadb3-941">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="aadb3-942">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-942">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-943">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-943">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="aadb3-944">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-944">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="aadb3-945">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="aadb3-945">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="aadb3-946">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="aadb3-946">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="aadb3-947">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-947">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-948">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-948">Az.Websites</span></span>
* <span data-ttu-id="aadb3-949">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-949">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="aadb3-950">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-950">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="aadb3-951">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-951">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="aadb3-952">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-952">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="aadb3-953">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-953">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aadb3-954">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="aadb3-954">Highlights since the last major release</span></span>
* <span data-ttu-id="aadb3-955">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="aadb3-955">General availability of `Az` module</span></span>
* <span data-ttu-id="aadb3-956">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aadb3-956">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aadb3-957">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aadb3-957">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aadb3-958">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-958">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aadb3-959">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-959">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aadb3-960">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-960">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aadb3-961">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-961">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="aadb3-962">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-962">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-963">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-963">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aadb3-964">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-964">Az.AnalysisServices</span></span>
* <span data-ttu-id="aadb3-965">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="aadb3-965">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="aadb3-966">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-966">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-967">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-967">Az.Automation</span></span>
* <span data-ttu-id="aadb3-968">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-968">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="aadb3-969">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-969">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="aadb3-970">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-970">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-971">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-971">Az.Compute</span></span>
* <span data-ttu-id="aadb3-972">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-972">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="aadb3-973">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-973">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="aadb3-974">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-974">Az.ContainerInstance</span></span>
* <span data-ttu-id="aadb3-975">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-975">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-976">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-976">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-977">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-977">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="aadb3-978">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-978">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-979">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-979">Az.Resources</span></span>
* <span data-ttu-id="aadb3-980">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-980">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="aadb3-981">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-981">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="aadb3-982">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="aadb3-982">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="aadb3-983">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="aadb3-983">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="aadb3-984">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-984">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="aadb3-985">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="aadb3-985">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-986">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-986">Az.Sql</span></span>
* <span data-ttu-id="aadb3-987">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-987">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-988">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-988">Az.Storage</span></span>
* <span data-ttu-id="aadb3-989">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="aadb3-989">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="aadb3-990">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="aadb3-990">New-AzStorageContext</span></span>
* <span data-ttu-id="aadb3-991">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="aadb3-991">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="aadb3-992">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="aadb3-992">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="aadb3-993">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="aadb3-993">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="aadb3-994">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-994">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="aadb3-995">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-995">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="aadb3-996">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="aadb3-996">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="aadb3-997">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-997">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="aadb3-998">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-998">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="aadb3-999">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-999">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="aadb3-1000">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="aadb3-1000">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="aadb3-1001">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1001">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="aadb3-1002">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="aadb3-1002">Highlights since the last major release</span></span>
* <span data-ttu-id="aadb3-1003">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="aadb3-1003">General availability of `Az` module</span></span>
* <span data-ttu-id="aadb3-1004">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="aadb3-1004">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="aadb3-1005">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="aadb3-1005">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="aadb3-1006">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1006">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="aadb3-1007">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1007">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aadb3-1008">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1008">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="aadb3-1009">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1009">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-1010">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-1010">Az.Automation</span></span>
* <span data-ttu-id="aadb3-1011">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1011">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="aadb3-1012">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="aadb3-1012">Dynamic grouping</span></span>
    * <span data-ttu-id="aadb3-1013">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="aadb3-1013">Pre-Post script</span></span>
    * <span data-ttu-id="aadb3-1014">再起動設定</span><span class="sxs-lookup"><span data-stu-id="aadb3-1014">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1015">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1016">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1016">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="aadb3-1017">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1017">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aadb3-1018">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-1018">Az.KeyVault</span></span>
* <span data-ttu-id="aadb3-1019">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1019">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1020">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1020">Az.Network</span></span>
* <span data-ttu-id="aadb3-1021">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1021">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="aadb3-1022">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1022">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1023">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1023">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-1024">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1024">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="aadb3-1025">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1025">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1026">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1026">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1027">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1027">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="aadb3-1028">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1028">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1029">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1029">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1030">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1030">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-1031">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1031">Az.Storage</span></span>
* <span data-ttu-id="aadb3-1032">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-1032">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="aadb3-1033">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1033">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aadb3-1034">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1034">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aadb3-1035">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1035">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="aadb3-1036">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="aadb3-1036">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="aadb3-1037">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="aadb3-1037">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="aadb3-1038">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-1038">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-1039">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1039">Az.Websites</span></span>
* <span data-ttu-id="aadb3-1040">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1040">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="aadb3-1041">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1041">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-1042">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1042">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-1043">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1043">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="aadb3-1044">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1044">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-1045">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-1045">Az.Automation</span></span>
* <span data-ttu-id="aadb3-1046">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1046">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="aadb3-1047">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1047">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="aadb3-1048">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1048">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aadb3-1049">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aadb3-1049">Az.Cdn</span></span>
* <span data-ttu-id="aadb3-1050">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1050">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1051">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1051">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1052">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1052">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-1053">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-1053">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-1054">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1054">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aadb3-1055">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aadb3-1055">Az.LogicApp</span></span>
* <span data-ttu-id="aadb3-1056">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1056">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1057">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1057">Az.Network</span></span>
* <span data-ttu-id="aadb3-1058">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1058">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1059">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1059">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-1060">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1060">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="aadb3-1061">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1061">SDK Update</span></span>
* <span data-ttu-id="aadb3-1062">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1062">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="aadb3-1063">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1063">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1064">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1064">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1065">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1065">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="aadb3-1066">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="aadb3-1066">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="aadb3-1067">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1067">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="aadb3-1068">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="aadb3-1068">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="aadb3-1069">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1069">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="aadb3-1070">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="aadb3-1070">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1071">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1071">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1072">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1072">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="aadb3-1073">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1073">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-1074">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1074">Az.Storage</span></span>
* <span data-ttu-id="aadb3-1075">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1075">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="aadb3-1076">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1076">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="aadb3-1077">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1077">Az.AnalysisServices</span></span>
* <span data-ttu-id="aadb3-1078">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1078">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-1079">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-1079">Az.Automation</span></span>
* <span data-ttu-id="aadb3-1080">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1080">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="aadb3-1081">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1081">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="aadb3-1082">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1082">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-1083">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1083">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-1084">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1084">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1085">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1085">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1086">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1086">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="aadb3-1087">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1087">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="aadb3-1088">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1088">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="aadb3-1089">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1089">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1090">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1090">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-1091">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1091">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="aadb3-1092">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-1092">Az.EventHub</span></span>
* <span data-ttu-id="aadb3-1093">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1093">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aadb3-1094">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-1094">Az.KeyVault</span></span>
* <span data-ttu-id="aadb3-1095">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1095">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aadb3-1096">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aadb3-1096">Az.LogicApp</span></span>
* <span data-ttu-id="aadb3-1097">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1097">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="aadb3-1098">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1098">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="aadb3-1099">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1099">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="aadb3-1100">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aadb3-1100">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aadb3-1101">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aadb3-1101">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aadb3-1102">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aadb3-1102">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="aadb3-1103">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="aadb3-1103">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="aadb3-1104">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1104">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="aadb3-1105">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aadb3-1105">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aadb3-1106">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aadb3-1106">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aadb3-1107">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aadb3-1107">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="aadb3-1108">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="aadb3-1108">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="aadb3-1109">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1109">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="aadb3-1110">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-1110">Az.Monitor</span></span>
* <span data-ttu-id="aadb3-1111">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1111">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1112">Az.Network</span></span>
* <span data-ttu-id="aadb3-1113">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1113">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-1114">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-1114">Az.OperationalInsights</span></span>
* <span data-ttu-id="aadb3-1115">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1115">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="aadb3-1116">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1116">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="aadb3-1117">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1117">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1118">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1118">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1119">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="aadb3-1119">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="aadb3-1120">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="aadb3-1120">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="aadb3-1121">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="aadb3-1121">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="aadb3-1122">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1122">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1123">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1123">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1124">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1124">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="aadb3-1125">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1125">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-1126">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1126">Az.Websites</span></span>
* <span data-ttu-id="aadb3-1127">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1127">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="aadb3-1128">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1128">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-1129">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1129">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-1130">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1130">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aadb3-1131">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1131">Az.AnalysisServices</span></span>
<span data-ttu-id="aadb3-1132">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="aadb3-1132">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1133">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1133">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1134">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1134">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="aadb3-1135">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1135">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="aadb3-1136">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1136">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1137">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1137">Az.RecoveryServices</span></span>
<span data-ttu-id="aadb3-1138">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="aadb3-1138">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1139">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1139">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1140">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1140">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="aadb3-1141">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="aadb3-1141">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="aadb3-1142">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1142">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="aadb3-1143">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="aadb3-1143">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1144">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1145">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1145">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="aadb3-1146">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1146">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="aadb3-1147">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1147">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="aadb3-1148">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1148">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1149">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-1150">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-1150">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="aadb3-1151">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1151">Az.AnalysisServices</span></span>
* <span data-ttu-id="aadb3-1152">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-1152">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1153">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1153">Az.RecoveryServices</span></span>
* <span data-ttu-id="aadb3-1154">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-1154">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="aadb3-1155">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1155">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-1156">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1156">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-1157">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1157">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="aadb3-1158">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1158">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aadb3-1159">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1159">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="aadb3-1160">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="aadb3-1160">Az.Aks</span></span>
* <span data-ttu-id="aadb3-1161">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1161">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="aadb3-1162">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-1162">Az.Automation</span></span>
* <span data-ttu-id="aadb3-1163">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1163">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="aadb3-1164">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1164">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="aadb3-1165">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="aadb3-1165">Az.Cdn</span></span>
* <span data-ttu-id="aadb3-1166">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1166">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1167">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1167">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1168">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1168">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="aadb3-1169">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1169">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="aadb3-1170">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1170">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="aadb3-1171">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="aadb3-1171">Az.ContainerRegistry</span></span>
* <span data-ttu-id="aadb3-1172">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1172">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="aadb3-1173">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="aadb3-1173">Az.DataFactory</span></span>
* <span data-ttu-id="aadb3-1174">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1174">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1175">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1175">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-1176">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="aadb3-1176">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="aadb3-1177">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="aadb3-1177">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="aadb3-1178">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1178">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-1179">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-1179">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-1180">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1180">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="aadb3-1181">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-1181">Az.KeyVault</span></span>
* <span data-ttu-id="aadb3-1182">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1182">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1183">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1183">Az.Network</span></span>
* <span data-ttu-id="aadb3-1184">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1184">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1185">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1185">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1186">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1186">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="aadb3-1187">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1187">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="aadb3-1188">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1188">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="aadb3-1189">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="aadb3-1189">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="aadb3-1190">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="aadb3-1190">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="aadb3-1191">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1191">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="aadb3-1192">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="aadb3-1192">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-1193">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-1193">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-1194">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="aadb3-1194">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="aadb3-1195">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1195">Fix some error messages.</span></span>
* <span data-ttu-id="aadb3-1196">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1196">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="aadb3-1197">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1197">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="aadb3-1198">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="aadb3-1198">Az.SignalR</span></span>
* <span data-ttu-id="aadb3-1199">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1199">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1200">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1200">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1201">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1201">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aadb3-1202">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1202">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="aadb3-1203">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1203">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="aadb3-1204">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-1204">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-1205">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1205">Az.Storage</span></span>
* <span data-ttu-id="aadb3-1206">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1206">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aadb3-1207">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="aadb3-1207">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="aadb3-1208">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="aadb3-1208">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="aadb3-1209">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="aadb3-1209">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="aadb3-1210">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="aadb3-1210">Az.TrafficManager</span></span>
* <span data-ttu-id="aadb3-1211">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1211">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-1212">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1212">Az.Websites</span></span>
* <span data-ttu-id="aadb3-1213">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1213">Update incorrect online help URLs</span></span>
* <span data-ttu-id="aadb3-1214">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1214">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="aadb3-1215">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="aadb3-1215">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="aadb3-1216">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1216">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="aadb3-1217">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1217">Az.Accounts</span></span>
* <span data-ttu-id="aadb3-1218">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="aadb3-1218">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1219">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1219">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1220">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1220">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="aadb3-1221">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1221">Updated the description of ID in help files</span></span>
* <span data-ttu-id="aadb3-1222">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1222">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1223">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1223">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-1224">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1224">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="aadb3-1225">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1225">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="aadb3-1226">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="aadb3-1226">Az.EventGrid</span></span>
* <span data-ttu-id="aadb3-1227">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1227">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="aadb3-1228">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="aadb3-1228">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="aadb3-1229">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="aadb3-1229">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="aadb3-1230">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="aadb3-1230">Event Time-To-Live,</span></span>
        - <span data-ttu-id="aadb3-1231">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="aadb3-1231">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="aadb3-1232">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="aadb3-1232">Dead letter endpoint.</span></span>
    - <span data-ttu-id="aadb3-1233">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="aadb3-1233">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="aadb3-1234">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="aadb3-1234">Event Time-To-Live,</span></span>
        - <span data-ttu-id="aadb3-1235">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="aadb3-1235">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="aadb3-1236">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="aadb3-1236">Dead letter endpoint.</span></span>
* <span data-ttu-id="aadb3-1237">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1237">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="aadb3-1238">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1238">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="aadb3-1239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="aadb3-1239">Az.IotHub</span></span>
* <span data-ttu-id="aadb3-1240">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1240">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="aadb3-1241">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="aadb3-1241">Az.LogicApp</span></span>
* <span data-ttu-id="aadb3-1242">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="aadb3-1242">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1243">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1243">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1244">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1244">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="aadb3-1245">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="aadb3-1245">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="aadb3-1246">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1246">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="aadb3-1247">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1247">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="aadb3-1248">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1248">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="aadb3-1249">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="aadb3-1249">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="aadb3-1250">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="aadb3-1250">Az.SignalR</span></span>
* <span data-ttu-id="aadb3-1251">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1251">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1252">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1252">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1253">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1253">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="aadb3-1254">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1254">Az.Storage</span></span>
* <span data-ttu-id="aadb3-1255">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="aadb3-1255">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="aadb3-1256">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="aadb3-1256">New-AzStorageContext</span></span>
* <span data-ttu-id="aadb3-1257">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1257">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="aadb3-1258">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="aadb3-1258">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-1259">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1259">Az.Websites</span></span>
* <span data-ttu-id="aadb3-1260">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1260">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="aadb3-1261">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1261">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="aadb3-1262">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1262">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="aadb3-1263">全般</span><span class="sxs-lookup"><span data-stu-id="aadb3-1263">General</span></span>

- <span data-ttu-id="aadb3-1264">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="aadb3-1264">General Availability of Az Module</span></span>
- <span data-ttu-id="aadb3-1265">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="aadb3-1265">Online help for each module</span></span>
- <span data-ttu-id="aadb3-1266">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1266">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="aadb3-1267">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1267">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="aadb3-1268">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="aadb3-1268">Az.Accounts</span></span>
- <span data-ttu-id="aadb3-1269">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1269">Changed from Az.Profile</span></span>
- <span data-ttu-id="aadb3-1270">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1270">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="aadb3-1271">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-1271">Az.ApiManagement</span></span>
- <span data-ttu-id="aadb3-1272">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="aadb3-1272">Fixes for #7002</span></span>
- <span data-ttu-id="aadb3-1273">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1273">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="aadb3-1274">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="aadb3-1274">Az.Batch</span></span>
- <span data-ttu-id="aadb3-1275">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1275">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="aadb3-1276">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1276">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="aadb3-1277">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1277">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="aadb3-1278">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="aadb3-1278">Az.Billing</span></span>
- <span data-ttu-id="aadb3-1279">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1279">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="aadb3-1280">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1280">Az.CognitivServices</span></span>
- <span data-ttu-id="aadb3-1281">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1281">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="aadb3-1282">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1282">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="aadb3-1283">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1283">Az.ContainerInstance</span></span>
- <span data-ttu-id="aadb3-1284">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1284">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="aadb3-1285">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="aadb3-1285">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="aadb3-1286">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1286">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1287">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1287">Az.DataLakeStore</span></span>
- <span data-ttu-id="aadb3-1288">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1288">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="aadb3-1289">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="aadb3-1289">Az.Monitor</span></span>
- <span data-ttu-id="aadb3-1290">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1290">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="aadb3-1291">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="aadb3-1291">Az.KeyVault</span></span>
- <span data-ttu-id="aadb3-1292">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1292">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="aadb3-1293">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="aadb3-1293">Az.MachineLearning</span></span>
- <span data-ttu-id="aadb3-1294">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1294">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="aadb3-1295">Az.Media</span><span class="sxs-lookup"><span data-stu-id="aadb3-1295">Az.Media</span></span>
- <span data-ttu-id="aadb3-1296">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1296">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="aadb3-1297">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1297">Az.Network</span></span>
<span data-ttu-id="aadb3-1298">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1298">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="aadb3-1299">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="aadb3-1299">New cmdlets added:</span></span>
        - <span data-ttu-id="aadb3-1300">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1300">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1301">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1301">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1302">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1302">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1303">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1303">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1304">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1304">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1305">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-1305">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="aadb3-1306">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="aadb3-1306">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="aadb3-1307">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="aadb3-1307">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="aadb3-1308">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1308">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="aadb3-1309">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="aadb3-1309">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="aadb3-1310">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-1310">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="aadb3-1311">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="aadb3-1311">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="aadb3-1312">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-1312">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="aadb3-1313">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-1313">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="aadb3-1314">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1314">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="aadb3-1315">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1315">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="aadb3-1316">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aadb3-1316">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="aadb3-1317">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aadb3-1317">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="aadb3-1318">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="aadb3-1318">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="aadb3-1319">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1319">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="aadb3-1320">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1320">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="aadb3-1321">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-1321">Az.OperationalInsights</span></span>
- <span data-ttu-id="aadb3-1322">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1322">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="aadb3-1323">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1323">Az.Profile</span></span>
- <span data-ttu-id="aadb3-1324">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1324">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1325">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1325">Az.RecoveryServices</span></span>
- <span data-ttu-id="aadb3-1326">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1326">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="aadb3-1327">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1327">Az.Resources</span></span>
- <span data-ttu-id="aadb3-1328">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1328">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="aadb3-1329">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-1329">Az.ServiceFabric</span></span>
- <span data-ttu-id="aadb3-1330">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="aadb3-1330">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="aadb3-1331">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1331">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="aadb3-1332">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="aadb3-1332">Az.SIgnalR</span></span>
- <span data-ttu-id="aadb3-1333">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="aadb3-1333">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="aadb3-1334">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1334">Az.Sql</span></span>
- <span data-ttu-id="aadb3-1335">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1335">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="aadb3-1336">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1336">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="aadb3-1337">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="aadb3-1338">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1338">Az.Storage</span></span>
- <span data-ttu-id="aadb3-1339">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1339">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="aadb3-1340">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1340">Az.Websites</span></span>
- <span data-ttu-id="aadb3-1341">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="aadb3-1341">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="aadb3-1342">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1342">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="aadb3-1343">全般</span><span class="sxs-lookup"><span data-stu-id="aadb3-1343">General</span></span>

* <span data-ttu-id="aadb3-1344">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="aadb3-1344">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="aadb3-1345">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1345">Az.Compute</span></span>

* <span data-ttu-id="aadb3-1346">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1346">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1347">Az.DataLakeStore</span></span>

* <span data-ttu-id="aadb3-1348">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1348">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="aadb3-1349">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="aadb3-1349">Az.FrontDoor</span></span>

* <span data-ttu-id="aadb3-1350">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1350">Fixed some broken links</span></span>
    - <span data-ttu-id="aadb3-1351">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1351">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="aadb3-1352">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1352">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="aadb3-1353">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1353">Az.RecoveryServices</span></span>

* <span data-ttu-id="aadb3-1354">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1354">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="aadb3-1355">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1355">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="aadb3-1356">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1356">Az.Resources</span></span>

* <span data-ttu-id="aadb3-1357">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1357">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="aadb3-1358">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1358">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="aadb3-1359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1359">Az.Sql</span></span>

* <span data-ttu-id="aadb3-1360">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="aadb3-1360">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="aadb3-1361">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1361">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="aadb3-1362">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1362">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="aadb3-1363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1363">Az.Storage</span></span>

* <span data-ttu-id="aadb3-1364">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1364">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="aadb3-1365">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1365">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="aadb3-1366">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1366">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="aadb3-1367">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="aadb3-1367">Support Static Website configuration</span></span>
    - <span data-ttu-id="aadb3-1368">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="aadb3-1368">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="aadb3-1369">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="aadb3-1369">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="aadb3-1370">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1370">Az.Websites</span></span>

* <span data-ttu-id="aadb3-1371">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="aadb3-1371">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="aadb3-1372">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1372">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="aadb3-1373">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="aadb3-1373">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="aadb3-1374">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1374">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="aadb3-1375">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="aadb3-1375">Az.ApiManagement</span></span>
* <span data-ttu-id="aadb3-1376">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1376">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="aadb3-1377">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="aadb3-1377">Az.Automation</span></span>
* <span data-ttu-id="aadb3-1378">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="aadb3-1378">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="aadb3-1379">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1379">Added Update Management cmdlets</span></span>
* <span data-ttu-id="aadb3-1380">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1380">Added Source Control cmdlets</span></span>
* <span data-ttu-id="aadb3-1381">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1381">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="aadb3-1382">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1382">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="aadb3-1383">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1383">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1384">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1384">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="aadb3-1385">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1385">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="aadb3-1386">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1386">Az.ContainerInstance</span></span>
* <span data-ttu-id="aadb3-1387">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1387">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="aadb3-1388">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="aadb3-1388">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="aadb3-1389">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1389">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="aadb3-1390">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1390">Az.Network</span></span>
* <span data-ttu-id="aadb3-1391">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1391">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="aadb3-1392">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1392">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="aadb3-1393">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1393">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="aadb3-1394">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1394">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="aadb3-1395">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="aadb3-1395">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="aadb3-1396">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1396">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="aadb3-1397">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1397">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="aadb3-1398">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="aadb3-1398">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="aadb3-1399">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1399">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="aadb3-1400">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1400">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="aadb3-1401">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="aadb3-1401">Az.Relay</span></span>
* <span data-ttu-id="aadb3-1402">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="aadb3-1402">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="aadb3-1403">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1403">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1404">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1404">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="aadb3-1405">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1405">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="aadb3-1406">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="aadb3-1406">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="aadb3-1407">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-1407">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-1408">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1408">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="aadb3-1409">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1409">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1410">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1410">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="aadb3-1411">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1411">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aadb3-1412">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1412">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aadb3-1413">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1413">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aadb3-1414">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="aadb3-1414">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="aadb3-1415">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aadb3-1415">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aadb3-1416">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aadb3-1416">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aadb3-1417">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aadb3-1417">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="aadb3-1418">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="aadb3-1418">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="aadb3-1419">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1419">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="aadb3-1420">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1420">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="aadb3-1421">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1421">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="aadb3-1422">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="aadb3-1422">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="aadb3-1423">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="aadb3-1423">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="aadb3-1424">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="aadb3-1424">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="aadb3-1425">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="aadb3-1425">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="aadb3-1426">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1426">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="aadb3-1427">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1427">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="aadb3-1428">全般</span><span class="sxs-lookup"><span data-stu-id="aadb3-1428">General</span></span>
* <span data-ttu-id="aadb3-1429">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="aadb3-1429">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="aadb3-1430">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1430">Az.Profile</span></span>
* <span data-ttu-id="aadb3-1431">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1431">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="aadb3-1432">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1432">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="aadb3-1433">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1433">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="aadb3-1434">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1434">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="aadb3-1435">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1435">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="aadb3-1436">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1436">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="aadb3-1437">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1437">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-1438">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1438">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-1439">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1439">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1440">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1440">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1441">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1441">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="aadb3-1442">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="aadb3-1442">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="aadb3-1443">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1443">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1444">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1444">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-1445">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1445">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="aadb3-1446">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1446">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="aadb3-1447">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="aadb3-1447">Az.Insights</span></span>
* <span data-ttu-id="aadb3-1448">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1448">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="aadb3-1449">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1449">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="aadb3-1450">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1450">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="aadb3-1451">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="aadb3-1451">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1452">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1452">Az.Network</span></span>
* <span data-ttu-id="aadb3-1453">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="aadb3-1453">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="aadb3-1454">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="aadb3-1454">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="aadb3-1455">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="aadb3-1455">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="aadb3-1456">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="aadb3-1456">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="aadb3-1457">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="aadb3-1457">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="aadb3-1458">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="aadb3-1458">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="aadb3-1459">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="aadb3-1459">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="aadb3-1460">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aadb3-1460">Az.PolicyInsights</span></span>
* <span data-ttu-id="aadb3-1461">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1461">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1462">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1462">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1463">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1463">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="aadb3-1464">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1464">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="aadb3-1465">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aadb3-1465">Az.ServiceBus</span></span>
* <span data-ttu-id="aadb3-1466">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1466">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="aadb3-1467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aadb3-1467">Az.ServiceFabric</span></span>
* <span data-ttu-id="aadb3-1468">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1468">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="aadb3-1469">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1469">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="aadb3-1470">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1470">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="aadb3-1471">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1471">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="aadb3-1472">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1472">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="aadb3-1473">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1473">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="aadb3-1474">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1474">Az.Profile</span></span>
* <span data-ttu-id="aadb3-1475">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1475">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="aadb3-1476">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1476">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1477">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1478">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1478">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="aadb3-1479">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1479">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="aadb3-1480">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="aadb3-1480">Az.DataLakeStore</span></span>
* <span data-ttu-id="aadb3-1481">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1481">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="aadb3-1482">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1482">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="aadb3-1483">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1483">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="aadb3-1484">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1484">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="aadb3-1485">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1485">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1486">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1486">Az.Network</span></span>
* <span data-ttu-id="aadb3-1487">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1487">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="aadb3-1488">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1488">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1489">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1489">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1490">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1490">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="aadb3-1491">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1491">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="aadb3-1492">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1492">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="aadb3-1493">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1493">Azure.Storage</span></span>
* <span data-ttu-id="aadb3-1494">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1494">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="aadb3-1495">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1495">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="aadb3-1496">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="aadb3-1496">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="aadb3-1497">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1497">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="aadb3-1498">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="aadb3-1498">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="aadb3-1499">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aadb3-1499">Az.CognitiveServices</span></span>
* <span data-ttu-id="aadb3-1500">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1500">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="aadb3-1501">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="aadb3-1501">Az.Compute</span></span>
* <span data-ttu-id="aadb3-1502">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1502">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="aadb3-1503">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1503">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="aadb3-1504">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1504">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="aadb3-1505">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="aadb3-1505">Az.DataFactoryV2</span></span>
* <span data-ttu-id="aadb3-1506">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1506">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="aadb3-1507">Az.Network</span><span class="sxs-lookup"><span data-stu-id="aadb3-1507">Az.Network</span></span>
* <span data-ttu-id="aadb3-1508">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1508">Added NetworkProfile functionality.</span></span> <span data-ttu-id="aadb3-1509">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="aadb3-1509">new cmdlets added</span></span>
    - <span data-ttu-id="aadb3-1510">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1510">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="aadb3-1511">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1511">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="aadb3-1512">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1512">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="aadb3-1513">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="aadb3-1513">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="aadb3-1514">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-1514">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="aadb3-1515">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="aadb3-1515">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="aadb3-1516">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1516">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="aadb3-1517">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1517">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="aadb3-1518">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1518">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="aadb3-1519">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="aadb3-1519">Az.RedisCache</span></span>
* <span data-ttu-id="aadb3-1520">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="aadb3-1520">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="aadb3-1521">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1521">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="aadb3-1522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="aadb3-1522">Az.Resources</span></span>
* <span data-ttu-id="aadb3-1523">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1523">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="aadb3-1524">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1524">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="aadb3-1525">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="aadb3-1525">Az.Sql</span></span>
* <span data-ttu-id="aadb3-1526">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="aadb3-1526">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="aadb3-1527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="aadb3-1527">Az.Websites</span></span>
* <span data-ttu-id="aadb3-1528">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="aadb3-1528">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="aadb3-1529">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="aadb3-1529">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="aadb3-1530">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="aadb3-1530">0.2.0 - September 2018</span></span>
 <span data-ttu-id="aadb3-1531">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="aadb3-1531">Initial Release</span></span>

---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 81afcd63e5ca7a776965849de9090b833f49acc7
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477235"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="5063b-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="5063b-103">Azure PowerShell release notes</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="5063b-104">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="5063b-104">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-105">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-105">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-106">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-106">Updated client side telemetry.</span></span>
* <span data-ttu-id="5063b-107">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-107">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="5063b-108">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-108">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-109">Az.Accounts</span></span>
* <span data-ttu-id="5063b-110">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-110">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-111">Az.Automation</span></span>
* <span data-ttu-id="5063b-112">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-112">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-113">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-113">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-114">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-114">Updated SDK to 7.0</span></span>
* <span data-ttu-id="5063b-115">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-115">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-116">Az.Compute</span></span>
* <span data-ttu-id="5063b-117">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-117">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-118">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-118">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-119">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-119">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-120">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-120">Az.IotHub</span></span>
* <span data-ttu-id="5063b-121">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-121">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="5063b-122">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-122">New Cmdlets are:</span></span>
    - <span data-ttu-id="5063b-123">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="5063b-123">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="5063b-124">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="5063b-124">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="5063b-125">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="5063b-125">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="5063b-126">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="5063b-126">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-127">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-127">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-128">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-128">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-129">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-129">Az.Monitor</span></span>
* <span data-ttu-id="5063b-130">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-130">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="5063b-131">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-131">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="5063b-132">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-132">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-133">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-133">Az.Network</span></span>
* <span data-ttu-id="5063b-134">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-134">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="5063b-135">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-135">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="5063b-136">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-136">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="5063b-137">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-137">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="5063b-138">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="5063b-138">No new cmdlets are added.</span></span> <span data-ttu-id="5063b-139">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="5063b-139">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-140">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-140">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-141">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-141">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-142">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-142">Az.Resources</span></span>
* <span data-ttu-id="5063b-143">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="5063b-143">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="5063b-144">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="5063b-144">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="5063b-145">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="5063b-145">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="5063b-146">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-146">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="5063b-147">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="5063b-147">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="5063b-148">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-148">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="5063b-149">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-149">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="5063b-150">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="5063b-150">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-151">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-151">Az.Sql</span></span>
* <span data-ttu-id="5063b-152">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-152">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="5063b-153">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-153">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="5063b-154">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="5063b-154">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="5063b-155">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="5063b-155">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="5063b-156">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-156">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="5063b-157">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="5063b-157">Az.StorageSync</span></span>
* <span data-ttu-id="5063b-158">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-158">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="5063b-159">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="5063b-159">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-160">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-160">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-161">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="5063b-161">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="5063b-162">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-162">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-163">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-163">Az.Accounts</span></span>
* <span data-ttu-id="5063b-164">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="5063b-164">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="5063b-165">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-165">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="5063b-166">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-166">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-167">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="5063b-167">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="5063b-168">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="5063b-168">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="5063b-169">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-169">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="5063b-170">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-170">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-171">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-171">Az.Compute</span></span>
* <span data-ttu-id="5063b-172">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="5063b-172">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="5063b-173">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-173">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="5063b-174">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-174">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="5063b-175">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-175">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="5063b-176">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-176">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-177">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-177">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-178">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-178">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="5063b-179">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="5063b-179">Az.DeploymentManager</span></span>
* <span data-ttu-id="5063b-180">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-180">Adds LIST operations for resources</span></span>
* <span data-ttu-id="5063b-181">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-181">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="5063b-182">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-182">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-183">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-183">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-184">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-184">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-185">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="5063b-185">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-186">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-186">Az.Network</span></span>
* <span data-ttu-id="5063b-187">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-187">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="5063b-188">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="5063b-188">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="5063b-189">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="5063b-189">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="5063b-190">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-190">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="5063b-191">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="5063b-191">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="5063b-192">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-192">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="5063b-193">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-193">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="5063b-194">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-194">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="5063b-195">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-195">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-196">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-196">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="5063b-197">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-197">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="5063b-198">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="5063b-198">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="5063b-199">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-199">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="5063b-200">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-200">Az.PolicyInsights</span></span>
* <span data-ttu-id="5063b-201">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-201">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="5063b-202">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-202">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="5063b-203">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-203">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="5063b-204">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-204">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-205">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-205">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-206">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-206">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="5063b-207">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-207">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-208">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-208">Az.Resources</span></span>
* <span data-ttu-id="5063b-209">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="5063b-209">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="5063b-210">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-210">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-211">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-211">Az.Sql</span></span>
<span data-ttu-id="5063b-212">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-212">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-213">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-213">Az.Storage</span></span>
* <span data-ttu-id="5063b-214">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-214">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="5063b-215">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-215">New-AzStorageAccount</span></span>
* <span data-ttu-id="5063b-216">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="5063b-216">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="5063b-217">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-217">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-218">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-218">Az.Websites</span></span>
* <span data-ttu-id="5063b-219">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-219">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="5063b-220">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-220">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="5063b-221">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="5063b-221">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-222">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-222">Az.Accounts</span></span>
* <span data-ttu-id="5063b-223">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-223">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-224">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-224">Az.Cdn</span></span>
* <span data-ttu-id="5063b-225">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="5063b-225">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-226">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-226">Az.Compute</span></span>
* <span data-ttu-id="5063b-227">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-227">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="5063b-228">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-228">Az.ContainerInstance</span></span>
* <span data-ttu-id="5063b-229">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-229">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="5063b-230">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="5063b-230">Az.DataBoxEdge</span></span>
* <span data-ttu-id="5063b-231">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-231">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="5063b-232">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-232">Get the Edge Storage Container</span></span>
* <span data-ttu-id="5063b-233">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-233">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="5063b-234">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-234">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="5063b-235">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-235">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="5063b-236">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-236">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="5063b-237">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-237">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="5063b-238">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="5063b-238">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="5063b-239">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-239">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="5063b-240">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-240">Get the Edge Storage Account</span></span>
* <span data-ttu-id="5063b-241">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-241">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="5063b-242">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-242">Create new Edge Storage Account</span></span>
* <span data-ttu-id="5063b-243">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-243">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="5063b-244">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-244">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="5063b-245">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="5063b-245">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="5063b-246">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="5063b-246">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="5063b-247">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-247">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="5063b-248">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="5063b-248">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-249">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-249">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-250">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-250">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="5063b-251">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-251">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="5063b-252">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="5063b-252">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="5063b-253">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="5063b-253">Az.DevTestLabs</span></span>
* <span data-ttu-id="5063b-254">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-254">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-255">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-255">Az.EventHub</span></span>
* <span data-ttu-id="5063b-256">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-256">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="5063b-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-257">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-258">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-258">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="5063b-259">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="5063b-259">Az.MachineLearning</span></span>
* <span data-ttu-id="5063b-260">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-260">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="5063b-261">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="5063b-261">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="5063b-262">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="5063b-262">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="5063b-263">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="5063b-263">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="5063b-264">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="5063b-264">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="5063b-265">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="5063b-265">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="5063b-266">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="5063b-266">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="5063b-267">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="5063b-267">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-268">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-268">Az.Network</span></span>
* <span data-ttu-id="5063b-269">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="5063b-269">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-270">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-270">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-271">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="5063b-271">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="5063b-272">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-272">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="5063b-273">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-273">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="5063b-274">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-274">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-275">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-275">Az.Resources</span></span>
* <span data-ttu-id="5063b-276">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-276">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-277">Az.Sql</span></span>
* <span data-ttu-id="5063b-278">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-278">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="5063b-279">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-279">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="5063b-280">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="5063b-280">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="5063b-281">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-281">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-282">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-282">Az.Storage</span></span>
* <span data-ttu-id="5063b-283">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-283">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="5063b-284">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-284">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="5063b-285">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-285">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="5063b-286">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-286">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="5063b-287">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="5063b-287">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="5063b-288">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-288">General</span></span>
* <span data-ttu-id="5063b-289">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-289">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-290">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-290">Az.Accounts</span></span>
* <span data-ttu-id="5063b-291">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="5063b-291">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="5063b-292">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="5063b-292">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="5063b-293">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-293">Az.Batch</span></span>
* <span data-ttu-id="5063b-294">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="5063b-294">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-295">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-295">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-296">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-296">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-297">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-297">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-298">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-298">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="5063b-299">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-299">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="5063b-300">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="5063b-300">Az.HealthcareApis</span></span>
* <span data-ttu-id="5063b-301">例外処理</span><span class="sxs-lookup"><span data-stu-id="5063b-301">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-302">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-302">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-303">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-303">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="5063b-304">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="5063b-304">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="5063b-305">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-305">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-306">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-306">Az.Monitor</span></span>
* <span data-ttu-id="5063b-307">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="5063b-307">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="5063b-308">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="5063b-308">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="5063b-309">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="5063b-309">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-310">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-310">Az.Network</span></span>
* <span data-ttu-id="5063b-311">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-311">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-312">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-312">Az.Resources</span></span>
* <span data-ttu-id="5063b-313">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-313">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="5063b-314">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-314">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-315">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-315">Az.Sql</span></span>
* <span data-ttu-id="5063b-316">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="5063b-316">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-317">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-317">Az.Storage</span></span>
* <span data-ttu-id="5063b-318">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-318">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="5063b-319">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="5063b-319">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="5063b-320">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="5063b-320">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="5063b-321">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="5063b-321">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="5063b-322">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="5063b-322">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="5063b-323">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-323">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="5063b-324">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-324">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="5063b-325">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-325">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="5063b-326">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-326">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="5063b-327">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-327">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="5063b-328">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="5063b-328">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="5063b-329">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-329">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="5063b-330">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="5063b-330">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="5063b-331">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="5063b-331">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-332">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-332">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-333">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="5063b-333">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="5063b-334">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="5063b-334">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-335">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-335">Az.Compute</span></span>
* <span data-ttu-id="5063b-336">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="5063b-336">VM Reapply feature</span></span>
    - <span data-ttu-id="5063b-337">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-337">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="5063b-338">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="5063b-338">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="5063b-339">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="5063b-339">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="5063b-340">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="5063b-340">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="5063b-341">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-341">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="5063b-342">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-342">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="5063b-343">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="5063b-343">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="5063b-344">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-344">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="5063b-345">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-345">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="5063b-346">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-346">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="5063b-347">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="5063b-347">Az.DataBoxEdge</span></span>
* <span data-ttu-id="5063b-348">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-348">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="5063b-349">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-349">Get the Order</span></span>
* <span data-ttu-id="5063b-350">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-350">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="5063b-351">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-351">Create new Order</span></span>
* <span data-ttu-id="5063b-352">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-352">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="5063b-353">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-353">Remove the Order</span></span>
* <span data-ttu-id="5063b-354">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="5063b-354">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="5063b-355">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="5063b-355">Now creates Local Share</span></span>
* <span data-ttu-id="5063b-356">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-356">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="5063b-357">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-357">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="5063b-358">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-358">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="5063b-359">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="5063b-359">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="5063b-360">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-360">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="5063b-361">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-361">Gets the information about Triggers</span></span>
* <span data-ttu-id="5063b-362">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-362">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="5063b-363">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-363">Create new Triggers</span></span>
* <span data-ttu-id="5063b-364">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-364">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="5063b-365">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-365">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-366">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-366">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-367">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-367">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="5063b-368">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-368">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-369">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-369">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-370">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-370">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-371">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-371">Az.EventHub</span></span>
* <span data-ttu-id="5063b-372">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-372">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-373">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-374">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-374">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="5063b-375">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-375">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="5063b-376">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-376">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="5063b-377">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="5063b-377">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-378">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-378">Az.Network</span></span>
* <span data-ttu-id="5063b-379">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="5063b-379">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="5063b-380">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="5063b-380">Az.PrivateDns</span></span>
* <span data-ttu-id="5063b-381">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-381">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-382">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-382">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-383">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-383">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="5063b-384">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="5063b-384">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="5063b-385">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-385">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="5063b-386">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5063b-386">Az.RedisCache</span></span>
* <span data-ttu-id="5063b-387">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-387">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="5063b-388">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-388">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="5063b-389">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-389">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-390">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-390">Az.Resources</span></span>
- <span data-ttu-id="5063b-391">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-391">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="5063b-392">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-392">Updated create policy definition help example</span></span>
- <span data-ttu-id="5063b-393">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-393">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="5063b-394">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-394">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="5063b-395">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="5063b-395">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-396">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-396">Az.Sql</span></span>
* <span data-ttu-id="5063b-397">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-397">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="5063b-398">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-398">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="5063b-399">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="5063b-399">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="5063b-400">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-400">General</span></span>
* <span data-ttu-id="5063b-401">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="5063b-401">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-402">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-402">Az.Accounts</span></span>
* <span data-ttu-id="5063b-403">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-403">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="5063b-404">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="5063b-404">Az.Advisor</span></span>
* <span data-ttu-id="5063b-405">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-405">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="5063b-406">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-406">Az.Batch</span></span>
* <span data-ttu-id="5063b-407">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-407">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="5063b-408">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="5063b-408">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="5063b-409">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="5063b-409">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="5063b-410">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-410">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="5063b-411">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="5063b-411">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="5063b-412">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-412">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="5063b-413">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="5063b-413">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="5063b-414">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="5063b-414">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="5063b-415">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="5063b-415">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="5063b-416">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-416">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="5063b-417">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-417">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="5063b-418">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="5063b-418">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="5063b-419">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-419">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="5063b-420">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-420">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="5063b-421">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-421">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="5063b-422">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-422">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="5063b-423">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-423">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="5063b-424">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-424">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="5063b-425">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-425">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="5063b-426">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5063b-426">This operation is no longer supported.</span></span>
* <span data-ttu-id="5063b-427">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-427">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="5063b-428">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-428">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="5063b-429">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-429">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="5063b-430">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="5063b-430">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="5063b-431">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="5063b-431">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="5063b-432">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-432">New non-verified images are also now returned.</span></span> <span data-ttu-id="5063b-433">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="5063b-433">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="5063b-434">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-434">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="5063b-435">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-435">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="5063b-436">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="5063b-436">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="5063b-437">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-437">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="5063b-438">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="5063b-438">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="5063b-439">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-439">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="5063b-440">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="5063b-440">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="5063b-441">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="5063b-441">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="5063b-442">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="5063b-442">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-443">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-443">Az.Cdn</span></span>
* <span data-ttu-id="5063b-444">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-444">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="5063b-445">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-445">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-446">Az.Compute</span></span>
* <span data-ttu-id="5063b-447">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="5063b-447">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="5063b-448">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="5063b-448">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="5063b-449">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="5063b-449">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="5063b-450">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="5063b-450">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="5063b-451">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-451">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="5063b-452">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-452">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="5063b-453">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="5063b-453">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="5063b-454">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-454">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="5063b-455">重大な変更</span><span class="sxs-lookup"><span data-stu-id="5063b-455">Breaking changes</span></span>
    - <span data-ttu-id="5063b-456">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="5063b-456">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="5063b-457">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="5063b-457">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-458">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-458">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-459">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-459">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-460">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-460">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-461">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="5063b-461">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="5063b-462">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="5063b-462">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="5063b-463">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="5063b-463">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="5063b-464">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-464">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="5063b-465">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-465">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="5063b-466">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-466">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-467">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-467">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-468">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-468">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="5063b-469">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-469">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-470">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-470">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="5063b-471">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5063b-471">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="5063b-472">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-472">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="5063b-473">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-473">Removed five cmdlets:</span></span>
    - <span data-ttu-id="5063b-474">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="5063b-474">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="5063b-475">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="5063b-475">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="5063b-476">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="5063b-476">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="5063b-477">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="5063b-477">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="5063b-478">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="5063b-478">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="5063b-479">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-479">Added three cmdlets:</span></span>
    - <span data-ttu-id="5063b-480">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="5063b-480">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="5063b-481">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="5063b-481">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="5063b-482">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="5063b-482">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="5063b-483">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-483">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="5063b-484">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-484">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="5063b-485">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-485">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="5063b-486">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="5063b-486">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="5063b-487">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-487">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="5063b-488">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-488">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="5063b-489">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-489">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="5063b-490">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-490">Added some scenario test cases.</span></span>
* <span data-ttu-id="5063b-491">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="5063b-491">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-492">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-492">Az.IotHub</span></span>
* <span data-ttu-id="5063b-493">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="5063b-493">Breaking changes:</span></span>
    - <span data-ttu-id="5063b-494">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-494">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="5063b-495">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-495">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="5063b-496">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-496">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="5063b-497">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-497">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="5063b-498">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-498">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="5063b-499">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-499">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="5063b-500">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-500">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="5063b-501">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-501">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="5063b-502">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-502">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="5063b-503">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-503">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="5063b-504">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-504">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="5063b-505">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-505">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-506">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-506">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-507">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-507">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-508">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-508">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="5063b-509">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-509">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="5063b-510">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-510">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-511">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-511">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-512">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-512">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-513">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-513">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-514">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-514">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-515">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-515">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-516">Az.Resources</span></span>
* <span data-ttu-id="5063b-517">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-517">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-518">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-518">Az.Network</span></span>
* <span data-ttu-id="5063b-519">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="5063b-519">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="5063b-520">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-520">Updated cmdlet:</span></span>
        - <span data-ttu-id="5063b-521">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-521">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-522">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-522">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-523">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-523">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-524">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-524">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-525">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-525">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="5063b-526">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5063b-526">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="5063b-527">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-527">New cmdlet:</span></span>
        - <span data-ttu-id="5063b-528">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="5063b-528">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="5063b-529">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-529">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="5063b-530">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-530">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="5063b-531">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-531">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="5063b-532">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-532">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="5063b-533">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-533">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="5063b-534">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-534">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="5063b-535">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-535">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="5063b-536">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-536">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-537">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="5063b-537">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="5063b-538">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-538">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="5063b-539">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-539">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="5063b-540">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-540">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="5063b-541">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="5063b-541">Set-AzVirtualHub</span></span>
* <span data-ttu-id="5063b-542">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-542">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="5063b-543">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-543">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="5063b-544">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-544">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="5063b-545">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-545">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="5063b-546">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-546">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="5063b-547">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-547">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="5063b-548">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-548">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="5063b-549">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-549">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-550">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-550">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="5063b-551">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-551">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="5063b-552">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-552">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="5063b-553">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-553">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="5063b-554">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-554">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="5063b-555">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-555">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="5063b-556">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-556">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="5063b-557">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-557">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="5063b-558">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-558">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-559">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="5063b-559">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="5063b-560">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="5063b-560">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="5063b-561">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="5063b-561">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="5063b-562">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="5063b-562">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="5063b-563">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="5063b-563">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="5063b-564">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-564">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="5063b-565">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-565">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="5063b-566">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-566">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="5063b-567">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-567">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="5063b-568">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-568">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="5063b-569">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-569">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="5063b-570">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-570">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="5063b-571">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-571">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="5063b-572">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-572">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="5063b-573">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-573">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="5063b-574">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-574">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="5063b-575">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-575">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="5063b-576">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-576">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-577">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-577">New-AzIpGroup</span></span>
        - <span data-ttu-id="5063b-578">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-578">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="5063b-579">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-579">Get-AzIpGroup</span></span>
        - <span data-ttu-id="5063b-580">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-580">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-581">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-581">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-582">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="5063b-582">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-583">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-583">Az.Sql</span></span>
* <span data-ttu-id="5063b-584">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-584">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="5063b-585">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-585">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="5063b-586">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-586">Removed deprecated aliases:</span></span>
* <span data-ttu-id="5063b-587">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="5063b-587">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="5063b-588">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="5063b-588">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="5063b-589">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-589">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="5063b-590">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-590">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="5063b-591">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="5063b-591">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="5063b-592">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-592">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-593">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-593">Az.Storage</span></span>
* <span data-ttu-id="5063b-594">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-594">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="5063b-595">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-595">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="5063b-596">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-596">Set-AzStorageAccount</span></span>
* <span data-ttu-id="5063b-597">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="5063b-597">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="5063b-598">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="5063b-598">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="5063b-599">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="5063b-599">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="5063b-600">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="5063b-600">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="5063b-601">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-601">General</span></span>
* <span data-ttu-id="5063b-602">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="5063b-602">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-603">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-603">Az.Accounts</span></span>
* <span data-ttu-id="5063b-604">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-604">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="5063b-605">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-605">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-606">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-606">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="5063b-607">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="5063b-607">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-608">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-608">Az.Automation</span></span>
* <span data-ttu-id="5063b-609">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-609">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="5063b-610">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-610">Az.Batch</span></span>
* <span data-ttu-id="5063b-611">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="5063b-611">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-612">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-612">Az.Compute</span></span>
* <span data-ttu-id="5063b-613">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-613">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="5063b-614">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-614">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="5063b-615">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-615">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="5063b-616">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-616">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-617">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-618">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="5063b-618">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="5063b-619">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="5063b-619">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="5063b-620">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-620">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-621">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-621">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-622">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-622">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="5063b-623">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="5063b-623">Az.HealthcareApis</span></span>
* <span data-ttu-id="5063b-624">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-624">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="5063b-625">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-625">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="5063b-626">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-626">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="5063b-627">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-627">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-628">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-628">Az.IotHub</span></span>
* <span data-ttu-id="5063b-629">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="5063b-629">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="5063b-630">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="5063b-630">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="5063b-631">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-631">Az.Monitor</span></span>
* <span data-ttu-id="5063b-632">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="5063b-632">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="5063b-633">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="5063b-633">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="5063b-634">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="5063b-634">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="5063b-635">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-635">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-636">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-636">Az.Network</span></span>
* <span data-ttu-id="5063b-637">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-637">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="5063b-638">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-638">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="5063b-639">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-639">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-640">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-640">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="5063b-641">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-641">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5063b-642">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-642">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="5063b-643">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-643">Updated cmdlets:</span></span>
        - <span data-ttu-id="5063b-644">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-644">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="5063b-645">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-645">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="5063b-646">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-646">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="5063b-647">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="5063b-647">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="5063b-648">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="5063b-648">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="5063b-649">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="5063b-649">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="5063b-650">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="5063b-650">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="5063b-651">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5063b-651">Az.RedisCache</span></span>
* <span data-ttu-id="5063b-652">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-652">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-653">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-653">Az.Sql</span></span>
* <span data-ttu-id="5063b-654">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-654">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-655">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-655">Az.Storage</span></span>
* <span data-ttu-id="5063b-656">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="5063b-656">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="5063b-657">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5063b-657">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="5063b-658">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5063b-658">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="5063b-659">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5063b-659">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="5063b-660">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-660">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="5063b-661">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="5063b-661">Az.StorageSync</span></span>
* <span data-ttu-id="5063b-662">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-662">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-663">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-663">Az.Websites</span></span>
* <span data-ttu-id="5063b-664">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="5063b-664">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="5063b-665">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="5063b-665">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="5063b-666">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-666">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-667">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-667">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="5063b-668">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-668">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="5063b-669">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="5063b-669">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-670">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-670">Az.Automation</span></span>
* <span data-ttu-id="5063b-671">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-671">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="5063b-672">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-672">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="5063b-673">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-673">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-674">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-674">Az.Compute</span></span>
* <span data-ttu-id="5063b-675">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-675">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="5063b-676">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-676">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="5063b-677">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-677">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="5063b-678">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="5063b-678">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="5063b-679">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="5063b-679">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="5063b-680">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-680">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="5063b-681">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-681">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="5063b-682">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-682">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="5063b-683">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-683">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-684">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-684">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-685">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-685">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="5063b-686">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-686">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="5063b-687">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-687">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-688">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="5063b-688">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-689">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-689">Az.IotHub</span></span>
* <span data-ttu-id="5063b-690">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-690">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="5063b-691">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-691">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="5063b-692">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5063b-692">New cmdlets are:</span></span>
    - <span data-ttu-id="5063b-693">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="5063b-693">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="5063b-694">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="5063b-694">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="5063b-695">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="5063b-695">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="5063b-696">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="5063b-696">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-697">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-697">Az.Monitor</span></span>
* <span data-ttu-id="5063b-698">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="5063b-698">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="5063b-699">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="5063b-699">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="5063b-700">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="5063b-700">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="5063b-701">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="5063b-701">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="5063b-702">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-702">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="5063b-703">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-703">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="5063b-704">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="5063b-704">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="5063b-705">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="5063b-705">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="5063b-706">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-706">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="5063b-707">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-707">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="5063b-708">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-708">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="5063b-709">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="5063b-709">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="5063b-710">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-710">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="5063b-711">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-711">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="5063b-712">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-712">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="5063b-713">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="5063b-713">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="5063b-714">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="5063b-714">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="5063b-715">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="5063b-715">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="5063b-716">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-716">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="5063b-717">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-717">Overall improved help files</span></span>
* <span data-ttu-id="5063b-718">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-718">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-719">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-719">Az.Network</span></span>
* <span data-ttu-id="5063b-720">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-720">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="5063b-721">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-721">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="5063b-722">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="5063b-722">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="5063b-723">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-723">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="5063b-724">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-724">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="5063b-725">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-725">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="5063b-726">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-726">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="5063b-727">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-727">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="5063b-728">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-728">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="5063b-729">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-729">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="5063b-730">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-730">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="5063b-731">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-731">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="5063b-732">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-732">New cmdlets</span></span>
        - <span data-ttu-id="5063b-733">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="5063b-733">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="5063b-734">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-734">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="5063b-735">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-735">Updated cmdlet:</span></span>
        - <span data-ttu-id="5063b-736">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="5063b-736">New-VpnSite</span></span>
        - <span data-ttu-id="5063b-737">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="5063b-737">Update-VpnSite</span></span>
        - <span data-ttu-id="5063b-738">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-738">New-VpnConnection</span></span>
        - <span data-ttu-id="5063b-739">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-739">Update-VpnConnection</span></span>
* <span data-ttu-id="5063b-740">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-740">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-741">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-741">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-742">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-742">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="5063b-743">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-743">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-744">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-744">Az.Resources</span></span>
* <span data-ttu-id="5063b-745">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-745">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-746">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-746">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-747">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-747">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="5063b-748">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-748">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="5063b-749">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="5063b-749">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="5063b-750">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="5063b-750">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="5063b-751">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="5063b-751">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="5063b-752">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="5063b-752">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="5063b-753">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="5063b-753">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="5063b-754">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="5063b-754">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="5063b-755">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="5063b-755">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="5063b-756">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="5063b-756">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="5063b-757">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="5063b-757">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="5063b-758">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="5063b-758">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="5063b-759">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="5063b-759">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="5063b-760">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="5063b-760">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="5063b-761">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="5063b-761">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="5063b-762">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="5063b-762">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="5063b-763">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="5063b-763">Az.SignalR</span></span>
* <span data-ttu-id="5063b-764">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="5063b-764">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-765">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-765">Az.Sql</span></span>
* <span data-ttu-id="5063b-766">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-766">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="5063b-767">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-767">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="5063b-768">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-768">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="5063b-769">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-769">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="5063b-770">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="5063b-770">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-771">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-771">Az.Storage</span></span>
* <span data-ttu-id="5063b-772">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-772">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="5063b-773">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-773">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="5063b-774">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5063b-774">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="5063b-775">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5063b-775">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="5063b-776">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="5063b-776">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="5063b-777">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5063b-777">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="5063b-778">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-778">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="5063b-779">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-779">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="5063b-780">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-780">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="5063b-781">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-781">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="5063b-782">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="5063b-782">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-783">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-783">Az.Websites</span></span>
* <span data-ttu-id="5063b-784">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-784">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="5063b-785">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="5063b-785">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="5063b-786">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-786">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="5063b-787">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="5063b-787">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="5063b-788">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-788">General</span></span>
* <span data-ttu-id="5063b-789">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-789">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-790">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-790">Az.Accounts</span></span>
* <span data-ttu-id="5063b-791">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="5063b-791">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="5063b-792">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="5063b-792">Az.Aks</span></span>
* <span data-ttu-id="5063b-793">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-793">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="5063b-794">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="5063b-794">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="5063b-795">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-795">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-796">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="5063b-796">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="5063b-797">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="5063b-797">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="5063b-798">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-798">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="5063b-799">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="5063b-799">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="5063b-800">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-800">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="5063b-801">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-801">Az.Batch</span></span>
* <span data-ttu-id="5063b-802">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-802">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-803">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-803">Az.Cdn</span></span>
* <span data-ttu-id="5063b-804">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-804">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-805">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-805">Az.Compute</span></span>
* <span data-ttu-id="5063b-806">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-806">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="5063b-807">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-807">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="5063b-808">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-808">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="5063b-809">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-809">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="5063b-810">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="5063b-810">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="5063b-811">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="5063b-811">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="5063b-812">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-812">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="5063b-813">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-813">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-814">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-814">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-815">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-815">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="5063b-816">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-816">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="5063b-817">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-817">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="5063b-818">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-818">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-819">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-819">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-820">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-820">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-821">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-821">Az.EventHub</span></span>
* <span data-ttu-id="5063b-822">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="5063b-822">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="5063b-823">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="5063b-823">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="5063b-824">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-824">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="5063b-825">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="5063b-825">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="5063b-826">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="5063b-826">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="5063b-827">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-827">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-828">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-828">Az.Monitor</span></span>
* <span data-ttu-id="5063b-829">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-829">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-830">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-830">Az.Network</span></span>
* <span data-ttu-id="5063b-831">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-831">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="5063b-832">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-832">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="5063b-833">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-833">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="5063b-834">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-834">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="5063b-835">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="5063b-835">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="5063b-836">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-836">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="5063b-837">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-837">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-838">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-838">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-839">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-839">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="5063b-840">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-840">Added example</span></span>
    - <span data-ttu-id="5063b-841">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-841">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="5063b-842">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-842">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="5063b-843">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-843">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-844">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-844">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-845">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-845">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-846">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-846">Az.Resources</span></span>
* <span data-ttu-id="5063b-847">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-847">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="5063b-848">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-848">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="5063b-849">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="5063b-849">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="5063b-850">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-850">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-851">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-851">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-852">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="5063b-852">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="5063b-853">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="5063b-853">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="5063b-854">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-854">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-855">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-855">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-856">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-856">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="5063b-857">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="5063b-857">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="5063b-858">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="5063b-858">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="5063b-859">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-859">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="5063b-860">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="5063b-860">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="5063b-861">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-861">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-862">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-862">Az.Sql</span></span>
* <span data-ttu-id="5063b-863">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-863">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-864">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-864">Az.Storage</span></span>
* <span data-ttu-id="5063b-865">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-865">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="5063b-866">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-866">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="5063b-867">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5063b-867">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="5063b-868">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="5063b-868">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="5063b-869">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-869">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="5063b-870">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="5063b-870">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-871">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-871">Az.Websites</span></span>
* <span data-ttu-id="5063b-872">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-872">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="5063b-873">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="5063b-873">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-874">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-874">Az.Accounts</span></span>
* <span data-ttu-id="5063b-875">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-875">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="5063b-876">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-876">Az.ApplicationInsights</span></span>
* <span data-ttu-id="5063b-877">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-877">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="5063b-878">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-878">Az.Automation</span></span>
* <span data-ttu-id="5063b-879">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-879">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-880">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-880">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-881">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-881">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-882">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-882">Az.Compute</span></span>
* <span data-ttu-id="5063b-883">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-883">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="5063b-884">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="5063b-884">Az.ContainerRegistry</span></span>
* <span data-ttu-id="5063b-885">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-885">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="5063b-886">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="5063b-886">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-887">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-887">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-888">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-888">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="5063b-889">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-889">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-890">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-890">Az.EventHub</span></span>
* <span data-ttu-id="5063b-891">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="5063b-891">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="5063b-892">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-892">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-893">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-893">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-894">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-894">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="5063b-895">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5063b-895">Az.LogicApp</span></span>
* <span data-ttu-id="5063b-896">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-896">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="5063b-897">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-897">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="5063b-898">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="5063b-898">Az.ManagedServices</span></span>
* <span data-ttu-id="5063b-899">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-899">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-900">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-900">Az.Network</span></span>
* <span data-ttu-id="5063b-901">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-901">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="5063b-902">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-902">New cmdlets</span></span>
        - <span data-ttu-id="5063b-903">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="5063b-903">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="5063b-904">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="5063b-904">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="5063b-905">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-905">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-906">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-906">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-907">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-907">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-908">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-908">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="5063b-909">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="5063b-909">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="5063b-910">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="5063b-910">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="5063b-911">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="5063b-911">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="5063b-912">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-912">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="5063b-913">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-913">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="5063b-914">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-914">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="5063b-915">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="5063b-915">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="5063b-916">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-916">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="5063b-917">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-917">Updated cmdlets</span></span>
        - <span data-ttu-id="5063b-918">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-918">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="5063b-919">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-919">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="5063b-920">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-920">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="5063b-921">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-921">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5063b-922">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-922">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="5063b-923">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-923">Updated cmdlet:</span></span>
        - <span data-ttu-id="5063b-924">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-924">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="5063b-925">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-925">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="5063b-926">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-926">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="5063b-927">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="5063b-927">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="5063b-928">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-928">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="5063b-929">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5063b-929">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-930">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-930">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-931">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-931">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="5063b-932">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-932">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-933">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-933">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-934">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-934">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="5063b-935">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-935">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="5063b-936">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-936">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="5063b-937">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-937">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="5063b-938">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-938">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="5063b-939">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-939">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="5063b-940">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-940">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="5063b-941">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-941">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="5063b-942">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-942">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="5063b-943">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-943">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-944">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-944">Az.Resources</span></span>
- <span data-ttu-id="5063b-945">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-945">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="5063b-946">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-946">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-947">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-947">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-948">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="5063b-948">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="5063b-949">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-949">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-950">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-950">Az.Sql</span></span>
* <span data-ttu-id="5063b-951">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-951">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="5063b-952">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-952">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="5063b-953">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-953">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-954">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-954">Az.Storage</span></span>
* <span data-ttu-id="5063b-955">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-955">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="5063b-956">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="5063b-956">Az.StorageSync</span></span>
* <span data-ttu-id="5063b-957">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-957">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="5063b-958">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-958">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-959">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-959">Az.Websites</span></span>
* <span data-ttu-id="5063b-960">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-960">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="5063b-961">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-961">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="5063b-962">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-962">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="5063b-963">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="5063b-963">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-964">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-964">Az.Accounts</span></span>
* <span data-ttu-id="5063b-965">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="5063b-965">Add support for profile cmdlets</span></span>
* <span data-ttu-id="5063b-966">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="5063b-966">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="5063b-967">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="5063b-967">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="5063b-968">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="5063b-968">Az.Advisor</span></span>
* <span data-ttu-id="5063b-969">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="5063b-969">GA release of Az.Advisor</span></span>
* <span data-ttu-id="5063b-970">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-970">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="5063b-971">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-971">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-972">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="5063b-972">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="5063b-973">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="5063b-973">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="5063b-974">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-974">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="5063b-975">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-975">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="5063b-976">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-976">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="5063b-977">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="5063b-977">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="5063b-978">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-978">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-979">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-979">Az.Automation</span></span>
* <span data-ttu-id="5063b-980">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-980">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-981">Az.Compute</span></span>
* <span data-ttu-id="5063b-982">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="5063b-982">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-983">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-983">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-984">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="5063b-984">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="5063b-985">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5063b-985">Az.EventGrid</span></span>
* <span data-ttu-id="5063b-986">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-986">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-987">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-987">Az.IotHub</span></span>
* <span data-ttu-id="5063b-988">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-988">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-989">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-989">Az.Network</span></span>
* <span data-ttu-id="5063b-990">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-990">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="5063b-991">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-991">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="5063b-992">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-992">Az.PolicyInsights</span></span>
* <span data-ttu-id="5063b-993">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-993">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="5063b-994">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="5063b-994">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-995">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-995">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-996">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-996">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-997">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-997">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-998">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-998">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-999">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-999">Az.Resources</span></span>
    - <span data-ttu-id="5063b-1000">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1000">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="5063b-1001">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1001">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="5063b-1002">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1002">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="5063b-1003">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1003">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-1004">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-1004">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-1005">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="5063b-1005">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1006">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1006">Az.Sql</span></span>
* <span data-ttu-id="5063b-1007">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1007">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="5063b-1008">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1008">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="5063b-1009">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1009">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="5063b-1010">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1010">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="5063b-1011">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1011">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="5063b-1012">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1012">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="5063b-1013">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1013">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="5063b-1014">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="5063b-1014">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="5063b-1015">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1015">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1016">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1016">Az.Storage</span></span>
* <span data-ttu-id="5063b-1017">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1017">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="5063b-1018">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="5063b-1018">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="5063b-1019">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1019">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="5063b-1020">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="5063b-1020">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="5063b-1021">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1021">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="5063b-1022">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1022">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="5063b-1023">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1023">Set-AzStorageAccount</span></span>
* <span data-ttu-id="5063b-1024">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1024">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="5063b-1025">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="5063b-1025">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="5063b-1026">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="5063b-1026">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="5063b-1027">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="5063b-1027">Az.StorageSync</span></span>
* <span data-ttu-id="5063b-1028">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1028">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="5063b-1029">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1029">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1030">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1030">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1031">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1031">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="5063b-1032">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="5063b-1032">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="5063b-1033">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1033">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="5063b-1034">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="5063b-1034">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="5063b-1035">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="5063b-1035">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1036">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1036">Az.Compute</span></span>
* <span data-ttu-id="5063b-1037">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1037">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="5063b-1038">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1038">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="5063b-1039">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="5063b-1039">Az.Dns</span></span>
* <span data-ttu-id="5063b-1040">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1040">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="5063b-1041">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5063b-1041">Az.EventGrid</span></span>
* <span data-ttu-id="5063b-1042">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1042">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="5063b-1043">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-1043">New cmdlets:</span></span>
    - <span data-ttu-id="5063b-1044">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="5063b-1044">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="5063b-1045">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1045">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="5063b-1046">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="5063b-1046">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="5063b-1047">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1047">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="5063b-1048">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="5063b-1048">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="5063b-1049">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1049">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="5063b-1050">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="5063b-1050">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="5063b-1051">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1051">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="5063b-1052">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="5063b-1052">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="5063b-1053">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1053">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="5063b-1054">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="5063b-1054">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="5063b-1055">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1055">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="5063b-1056">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="5063b-1056">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="5063b-1057">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1057">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="5063b-1058">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="5063b-1058">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="5063b-1059">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1059">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="5063b-1060">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-1060">Updated cmdlets:</span></span>
    - <span data-ttu-id="5063b-1061">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="5063b-1061">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="5063b-1062">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1062">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="5063b-1063">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1063">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="5063b-1064">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="5063b-1064">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="5063b-1065">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="5063b-1065">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="5063b-1066">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="5063b-1066">Event subscription expiration date,</span></span>
            - <span data-ttu-id="5063b-1067">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="5063b-1067">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="5063b-1068">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1068">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="5063b-1069">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="5063b-1069">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="5063b-1070">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="5063b-1070">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="5063b-1071">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1071">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="5063b-1072">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="5063b-1072">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="5063b-1073">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1073">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="5063b-1074">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1074">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-1075">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-1075">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-1076">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="5063b-1076">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="5063b-1077">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1077">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="5063b-1078">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="5063b-1078">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="5063b-1079">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1079">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1080">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1080">Az.Network</span></span>
* <span data-ttu-id="5063b-1081">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1081">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="5063b-1082">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1082">New cmdlets</span></span>
        - <span data-ttu-id="5063b-1083">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="5063b-1083">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="5063b-1084">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1084">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="5063b-1085">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1085">New cmdlets</span></span> 
        - <span data-ttu-id="5063b-1086">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="5063b-1086">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="5063b-1087">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1087">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="5063b-1088">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1088">New cmdlets</span></span> 
        - <span data-ttu-id="5063b-1089">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="5063b-1089">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="5063b-1090">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="5063b-1090">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="5063b-1091">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="5063b-1091">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="5063b-1092">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-1092">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="5063b-1093">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-1093">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="5063b-1094">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1094">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="5063b-1095">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1095">New cmdlets</span></span>
        - <span data-ttu-id="5063b-1096">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="5063b-1096">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="5063b-1097">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="5063b-1097">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="5063b-1098">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="5063b-1098">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="5063b-1099">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="5063b-1099">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="5063b-1100">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="5063b-1100">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="5063b-1101">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1101">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="5063b-1102">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1102">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="5063b-1103">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1103">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="5063b-1104">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1104">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="5063b-1105">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1105">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="5063b-1106">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1106">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="5063b-1107">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1107">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="5063b-1108">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1108">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="5063b-1109">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1109">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="5063b-1110">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1110">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="5063b-1111">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1111">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="5063b-1112">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1112">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="5063b-1113">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1113">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="5063b-1114">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="5063b-1114">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="5063b-1115">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1115">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="5063b-1116">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1116">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="5063b-1117">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="5063b-1117">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="5063b-1118">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1118">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="5063b-1119">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1119">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="5063b-1120">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1120">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="5063b-1121">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1121">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="5063b-1122">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1122">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-1123">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1123">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-1124">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1124">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1125">Az.Resources</span></span>
* <span data-ttu-id="5063b-1126">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="5063b-1126">Support for additional Template Export options</span></span>
    - <span data-ttu-id="5063b-1127">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1127">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="5063b-1128">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1128">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="5063b-1129">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1129">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-1130">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1130">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-1131">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1131">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1132">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1132">Az.Sql</span></span>
* <span data-ttu-id="5063b-1133">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1133">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="5063b-1134">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1134">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="5063b-1135">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1135">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="5063b-1136">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="5063b-1136">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="5063b-1137">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="5063b-1137">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="5063b-1138">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="5063b-1138">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="5063b-1139">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="5063b-1139">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="5063b-1140">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="5063b-1140">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1141">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1141">Az.Storage</span></span>
* <span data-ttu-id="5063b-1142">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1142">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="5063b-1143">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1143">New-AzStorageAccount</span></span>
* <span data-ttu-id="5063b-1144">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1144">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="5063b-1145">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1145">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1146">Az.Websites</span></span>
* <span data-ttu-id="5063b-1147">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1147">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="5063b-1148">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1148">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="5063b-1149">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1149">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="5063b-1150">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-1150">Az.Cdn</span></span>
* <span data-ttu-id="5063b-1151">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1151">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1152">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1152">Az.Compute</span></span>
* <span data-ttu-id="5063b-1153">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1153">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="5063b-1154">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="5063b-1154">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-1155">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1155">Az.EventHub</span></span>
* <span data-ttu-id="5063b-1156">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1156">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="5063b-1157">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1157">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1158">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1158">Az.Network</span></span>
* <span data-ttu-id="5063b-1159">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1159">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="5063b-1160">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1160">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="5063b-1161">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1161">Az.PolicyInsights</span></span>
* <span data-ttu-id="5063b-1162">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1162">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1163">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1163">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1164">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1164">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-1165">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-1165">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-1166">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1166">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-1167">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1167">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-1168">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1168">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="5063b-1169">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1169">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1170">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1170">Az.Sql</span></span>
* <span data-ttu-id="5063b-1171">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1171">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="5063b-1172">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="5063b-1172">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="5063b-1173">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1173">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="5063b-1174">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1174">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1175">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1175">Az.Websites</span></span>
* <span data-ttu-id="5063b-1176">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1176">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="5063b-1177">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1177">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="5063b-1178">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-1178">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-1179">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1179">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="5063b-1180">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-1180">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="5063b-1181">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-1181">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="5063b-1182">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-1182">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="5063b-1183">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1183">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="5063b-1184">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-1184">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="5063b-1185">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-1185">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="5063b-1186">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-1186">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="5063b-1187">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1187">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="5063b-1188">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-1188">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="5063b-1189">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-1189">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="5063b-1190">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-1190">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="5063b-1191">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-1191">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="5063b-1192">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1192">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="5063b-1193">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="5063b-1193">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="5063b-1194">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-1194">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="5063b-1195">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="5063b-1195">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="5063b-1196">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="5063b-1196">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="5063b-1197">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1197">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="5063b-1198">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="5063b-1198">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="5063b-1199">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1199">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="5063b-1200">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1200">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="5063b-1201">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="5063b-1201">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="5063b-1202">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1202">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="5063b-1203">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1203">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="5063b-1204">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1204">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="5063b-1205">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-1205">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="5063b-1206">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="5063b-1206">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="5063b-1207">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1207">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="5063b-1208">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1208">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="5063b-1209">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1209">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="5063b-1210">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="5063b-1210">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="5063b-1211">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1211">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="5063b-1212">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1212">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="5063b-1213">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="5063b-1213">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="5063b-1214">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="5063b-1214">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="5063b-1215">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="5063b-1215">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="5063b-1216">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1216">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="5063b-1217">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1217">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="5063b-1218">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1218">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="5063b-1219">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="5063b-1219">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="5063b-1220">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="5063b-1220">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="5063b-1221">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="5063b-1221">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="5063b-1222">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1222">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="5063b-1223">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1223">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="5063b-1224">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="5063b-1224">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="5063b-1225">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="5063b-1225">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="5063b-1226">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1226">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="5063b-1227">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1227">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="5063b-1228">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="5063b-1228">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="5063b-1229">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="5063b-1229">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="5063b-1230">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="5063b-1230">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="5063b-1231">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="5063b-1231">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="5063b-1232">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1232">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="5063b-1233">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="5063b-1233">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="5063b-1234">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="5063b-1234">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="5063b-1235">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1235">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="5063b-1236">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="5063b-1236">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="5063b-1237">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="5063b-1237">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="5063b-1238">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1238">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="5063b-1239">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1239">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="5063b-1240">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="5063b-1240">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="5063b-1241">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="5063b-1241">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="5063b-1242">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1242">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="5063b-1243">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1243">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="5063b-1244">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="5063b-1244">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="5063b-1245">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="5063b-1245">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="5063b-1246">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="5063b-1246">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="5063b-1247">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="5063b-1247">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="5063b-1248">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="5063b-1248">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="5063b-1249">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="5063b-1249">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="5063b-1250">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="5063b-1250">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="5063b-1251">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="5063b-1251">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="5063b-1252">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1252">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="5063b-1253">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="5063b-1253">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="5063b-1254">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="5063b-1254">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="5063b-1255">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="5063b-1255">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1256">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1256">Az.Automation</span></span>
* <span data-ttu-id="5063b-1257">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1257">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="5063b-1258">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="5063b-1258">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="5063b-1259">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="5063b-1259">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="5063b-1260">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1260">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="5063b-1261">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="5063b-1261">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="5063b-1262">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1262">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="5063b-1263">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1263">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1264">Az.Compute</span></span>
* <span data-ttu-id="5063b-1265">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1265">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="5063b-1266">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1266">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1267">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1267">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1268">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1268">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-1269">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-1269">Az.Monitor</span></span>
* <span data-ttu-id="5063b-1270">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1270">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1271">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1271">Az.Network</span></span>
* <span data-ttu-id="5063b-1272">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1272">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="5063b-1273">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="5063b-1273">Updated cmdlet:</span></span>
        - <span data-ttu-id="5063b-1274">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-1274">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="5063b-1275">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1275">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1276">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1276">Az.Resources</span></span>
* <span data-ttu-id="5063b-1277">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1277">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1278">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1278">Az.Sql</span></span>
* <span data-ttu-id="5063b-1279">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-1279">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="5063b-1280">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1280">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1281">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1281">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1282">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1282">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-1283">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1283">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-1284">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1284">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="5063b-1285">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1285">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1286">Az.Compute</span></span>
* <span data-ttu-id="5063b-1287">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="5063b-1287">Proximity placement group feature.</span></span>
    - <span data-ttu-id="5063b-1288">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-1288">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="5063b-1289">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-1289">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="5063b-1290">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1290">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="5063b-1291">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1291">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="5063b-1292">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1292">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="5063b-1293">重大な変更</span><span class="sxs-lookup"><span data-stu-id="5063b-1293">Breaking changes</span></span>
    - <span data-ttu-id="5063b-1294">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="5063b-1294">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="5063b-1295">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="5063b-1295">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="5063b-1296">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="5063b-1296">Az.DeploymentManager</span></span>
* <span data-ttu-id="5063b-1297">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="5063b-1297">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="5063b-1298">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="5063b-1298">Az.Dns</span></span>
* <span data-ttu-id="5063b-1299">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="5063b-1299">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="5063b-1300">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="5063b-1300">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="5063b-1301">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1301">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="5063b-1302">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-1302">Az.FrontDoor</span></span>
* <span data-ttu-id="5063b-1303">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="5063b-1303">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="5063b-1304">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="5063b-1304">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="5063b-1305">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-1305">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-1306">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1306">Removed two cmdlets:</span></span>
    - <span data-ttu-id="5063b-1307">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="5063b-1307">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="5063b-1308">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="5063b-1308">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="5063b-1309">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1309">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="5063b-1310">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1310">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="5063b-1311">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1311">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="5063b-1312">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="5063b-1312">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-1313">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-1313">Az.Monitor</span></span>
* <span data-ttu-id="5063b-1314">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="5063b-1314">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="5063b-1315">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="5063b-1315">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="5063b-1316">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="5063b-1316">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="5063b-1317">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="5063b-1317">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="5063b-1318">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="5063b-1318">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="5063b-1319">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="5063b-1319">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="5063b-1320">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="5063b-1320">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="5063b-1321">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1321">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="5063b-1322">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1322">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="5063b-1323">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1323">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="5063b-1324">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1324">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="5063b-1325">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1325">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="5063b-1326">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="5063b-1326">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="5063b-1327">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1327">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1328">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1328">Az.Network</span></span>
* <span data-ttu-id="5063b-1329">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1329">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="5063b-1330">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1330">New cmdlets</span></span>
        - <span data-ttu-id="5063b-1331">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="5063b-1331">New-AzNatGateway</span></span>
        - <span data-ttu-id="5063b-1332">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="5063b-1332">Get-AzNatGateway</span></span>
        - <span data-ttu-id="5063b-1333">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="5063b-1333">Set-AzNatGateway</span></span>
        - <span data-ttu-id="5063b-1334">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="5063b-1334">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="5063b-1335">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1335">Updated cmdlets</span></span>
        - <span data-ttu-id="5063b-1336">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="5063b-1336">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="5063b-1337">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="5063b-1337">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="5063b-1338">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="5063b-1338">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="5063b-1339">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1339">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="5063b-1340">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1340">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="5063b-1341">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1341">Az.PolicyInsights</span></span>
* <span data-ttu-id="5063b-1342">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-1342">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="5063b-1343">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1343">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="5063b-1344">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="5063b-1344">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1345">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1345">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1346">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-1346">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="5063b-1347">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="5063b-1347">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="5063b-1348">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="5063b-1348">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="5063b-1349">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="5063b-1349">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="5063b-1350">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="5063b-1350">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="5063b-1351">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="5063b-1351">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="5063b-1352">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="5063b-1352">Az.Relay</span></span>
* <span data-ttu-id="5063b-1353">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1353">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-1354">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-1354">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-1355">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1355">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1356">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1356">Az.Storage</span></span>
* <span data-ttu-id="5063b-1357">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="5063b-1357">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="5063b-1358">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1358">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="5063b-1359">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1359">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="5063b-1360">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1360">New-AzStorageAccount</span></span>
* <span data-ttu-id="5063b-1361">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="5063b-1361">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="5063b-1362">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1362">New-AzStorageAccount</span></span>
    - <span data-ttu-id="5063b-1363">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1363">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="5063b-1364">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5063b-1364">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1365">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1365">Az.Websites</span></span>
* <span data-ttu-id="5063b-1366">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="5063b-1366">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="5063b-1367">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="5063b-1367">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="5063b-1368">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1368">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-1369">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-1369">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-1370">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="5063b-1370">General availability of `Az` module</span></span>
* <span data-ttu-id="5063b-1371">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="5063b-1371">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="5063b-1372">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="5063b-1372">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="5063b-1373">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1373">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="5063b-1374">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1374">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="5063b-1375">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1375">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="5063b-1376">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1376">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-1377">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1377">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1378">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1378">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="5063b-1379">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-1379">Az.Batch</span></span>
* <span data-ttu-id="5063b-1380">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1380">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-1381">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-1381">Az.Cdn</span></span>
* <span data-ttu-id="5063b-1382">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1382">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-1383">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1383">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-1384">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1384">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1385">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1385">Az.Compute</span></span>
* <span data-ttu-id="5063b-1386">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1386">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="5063b-1387">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1387">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1388">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1388">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-1389">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-1389">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-1390">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1390">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1391">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1391">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1392">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1392">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="5063b-1393">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5063b-1393">Az.EventGrid</span></span>
* <span data-ttu-id="5063b-1394">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1394">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-1395">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1395">Az.EventHub</span></span>
* <span data-ttu-id="5063b-1396">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1396">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="5063b-1397">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5063b-1397">Az.HDInsight</span></span>
* <span data-ttu-id="5063b-1398">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1398">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-1399">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1399">Az.IotHub</span></span>
* <span data-ttu-id="5063b-1400">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1400">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-1401">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-1401">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-1402">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1402">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1403">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1403">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="5063b-1404">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="5063b-1404">Az.MachineLearning</span></span>
* <span data-ttu-id="5063b-1405">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1405">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="5063b-1406">Az.Media</span><span class="sxs-lookup"><span data-stu-id="5063b-1406">Az.Media</span></span>
* <span data-ttu-id="5063b-1407">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1407">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-1408">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-1408">Az.Monitor</span></span>
  * <span data-ttu-id="5063b-1409">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1409">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="5063b-1410">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="5063b-1410">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="5063b-1411">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="5063b-1411">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="5063b-1412">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="5063b-1412">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="5063b-1413">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="5063b-1413">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="5063b-1414">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="5063b-1414">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="5063b-1415">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1415">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1416">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1416">Az.Network</span></span>
* <span data-ttu-id="5063b-1417">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1417">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1418">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1418">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="5063b-1419">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="5063b-1419">Az.NotificationHubs</span></span>
* <span data-ttu-id="5063b-1420">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1420">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-1421">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1421">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-1422">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1422">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="5063b-1423">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5063b-1423">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="5063b-1424">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1424">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1425">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1425">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1426">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1426">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1427">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1427">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="5063b-1428">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1428">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="5063b-1429">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1429">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="5063b-1430">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5063b-1430">Az.RedisCache</span></span>
* <span data-ttu-id="5063b-1431">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1431">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1432">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1432">Az.Resources</span></span>
* <span data-ttu-id="5063b-1433">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1433">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1434">Az.Sql</span></span>
* <span data-ttu-id="5063b-1435">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="5063b-1435">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="5063b-1436">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1436">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1437">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1437">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="5063b-1438">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1438">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="5063b-1439">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="5063b-1439">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="5063b-1440">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="5063b-1440">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="5063b-1441">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1441">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1442">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1442">Az.Websites</span></span>
* <span data-ttu-id="5063b-1443">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1443">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="5063b-1444">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1444">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="5063b-1445">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1445">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="5063b-1446">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1446">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="5063b-1447">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1447">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-1448">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-1448">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-1449">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="5063b-1449">General availability of `Az` module</span></span>
* <span data-ttu-id="5063b-1450">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="5063b-1450">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="5063b-1451">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="5063b-1451">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="5063b-1452">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1452">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="5063b-1453">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1453">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="5063b-1454">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1454">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="5063b-1455">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1455">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="5063b-1456">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1456">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1457">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1457">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="5063b-1458">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1458">Az.AnalysisServices</span></span>
* <span data-ttu-id="5063b-1459">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="5063b-1459">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="5063b-1460">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1460">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1461">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1461">Az.Automation</span></span>
* <span data-ttu-id="5063b-1462">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1462">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="5063b-1463">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1463">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="5063b-1464">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1464">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1465">Az.Compute</span></span>
* <span data-ttu-id="5063b-1466">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1466">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="5063b-1467">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1467">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="5063b-1468">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1468">Az.ContainerInstance</span></span>
* <span data-ttu-id="5063b-1469">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1469">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-1470">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-1470">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-1471">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1471">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="5063b-1472">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1472">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1473">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1473">Az.Resources</span></span>
* <span data-ttu-id="5063b-1474">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1474">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="5063b-1475">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1475">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="5063b-1476">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="5063b-1476">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="5063b-1477">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="5063b-1477">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="5063b-1478">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1478">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="5063b-1479">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="5063b-1479">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1480">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1480">Az.Sql</span></span>
* <span data-ttu-id="5063b-1481">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1481">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1482">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1482">Az.Storage</span></span>
* <span data-ttu-id="5063b-1483">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="5063b-1483">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="5063b-1484">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="5063b-1484">New-AzStorageContext</span></span>
* <span data-ttu-id="5063b-1485">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="5063b-1485">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="5063b-1486">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="5063b-1486">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="5063b-1487">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="5063b-1487">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="5063b-1488">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1488">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="5063b-1489">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1489">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="5063b-1490">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="5063b-1490">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="5063b-1491">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5063b-1491">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="5063b-1492">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5063b-1492">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="5063b-1493">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5063b-1493">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="5063b-1494">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5063b-1494">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="5063b-1495">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1495">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="5063b-1496">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="5063b-1496">Highlights since the last major release</span></span>
* <span data-ttu-id="5063b-1497">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="5063b-1497">General availability of `Az` module</span></span>
* <span data-ttu-id="5063b-1498">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="5063b-1498">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="5063b-1499">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="5063b-1499">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="5063b-1500">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1500">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="5063b-1501">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1501">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="5063b-1502">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1502">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="5063b-1503">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1503">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1504">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1504">Az.Automation</span></span>
* <span data-ttu-id="5063b-1505">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1505">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="5063b-1506">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="5063b-1506">Dynamic grouping</span></span>
    * <span data-ttu-id="5063b-1507">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="5063b-1507">Pre-Post script</span></span>
    * <span data-ttu-id="5063b-1508">再起動設定</span><span class="sxs-lookup"><span data-stu-id="5063b-1508">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1509">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1509">Az.Compute</span></span>
* <span data-ttu-id="5063b-1510">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1510">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="5063b-1511">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1511">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-1512">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-1512">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-1513">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1513">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1514">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1514">Az.Network</span></span>
* <span data-ttu-id="5063b-1515">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1515">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="5063b-1516">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1516">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1517">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1517">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1518">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1518">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="5063b-1519">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1519">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1520">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1520">Az.Resources</span></span>
* <span data-ttu-id="5063b-1521">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1521">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="5063b-1522">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1522">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1523">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1523">Az.Sql</span></span>
* <span data-ttu-id="5063b-1524">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1524">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1525">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1525">Az.Storage</span></span>
* <span data-ttu-id="5063b-1526">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1526">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="5063b-1527">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1527">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="5063b-1528">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1528">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="5063b-1529">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="5063b-1529">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="5063b-1530">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="5063b-1530">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="5063b-1531">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="5063b-1531">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="5063b-1532">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1532">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1533">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1533">Az.Websites</span></span>
* <span data-ttu-id="5063b-1534">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1534">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="5063b-1535">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1535">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1536">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1536">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1537">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1537">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="5063b-1538">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1538">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1539">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1539">Az.Automation</span></span>
* <span data-ttu-id="5063b-1540">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1540">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="5063b-1541">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1541">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="5063b-1542">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1542">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-1543">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-1543">Az.Cdn</span></span>
* <span data-ttu-id="5063b-1544">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-1544">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1545">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1545">Az.Compute</span></span>
* <span data-ttu-id="5063b-1546">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1546">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-1547">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-1547">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-1548">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1548">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="5063b-1549">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5063b-1549">Az.LogicApp</span></span>
* <span data-ttu-id="5063b-1550">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1550">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1551">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1551">Az.Network</span></span>
* <span data-ttu-id="5063b-1552">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1552">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1553">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1553">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1554">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1554">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="5063b-1555">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1555">SDK Update</span></span>
* <span data-ttu-id="5063b-1556">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1556">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="5063b-1557">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1557">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1558">Az.Resources</span></span>
* <span data-ttu-id="5063b-1559">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1559">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="5063b-1560">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="5063b-1560">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="5063b-1561">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1561">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="5063b-1562">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="5063b-1562">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="5063b-1563">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1563">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="5063b-1564">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="5063b-1564">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1565">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1565">Az.Sql</span></span>
* <span data-ttu-id="5063b-1566">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1566">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="5063b-1567">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1567">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1568">Az.Storage</span></span>
* <span data-ttu-id="5063b-1569">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="5063b-1569">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="5063b-1570">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1570">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="5063b-1571">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1571">Az.AnalysisServices</span></span>
* <span data-ttu-id="5063b-1572">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-1572">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1573">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1573">Az.Automation</span></span>
* <span data-ttu-id="5063b-1574">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1574">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="5063b-1575">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1575">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="5063b-1576">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1576">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-1577">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1577">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-1578">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1578">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1579">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1579">Az.Compute</span></span>
* <span data-ttu-id="5063b-1580">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1580">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="5063b-1581">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1581">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="5063b-1582">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1582">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="5063b-1583">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-1583">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1584">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1584">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1585">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1585">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="5063b-1586">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1586">Az.EventHub</span></span>
* <span data-ttu-id="5063b-1587">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1587">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-1588">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-1588">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-1589">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1589">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="5063b-1590">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5063b-1590">Az.LogicApp</span></span>
* <span data-ttu-id="5063b-1591">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1591">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="5063b-1592">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1592">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="5063b-1593">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1593">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="5063b-1594">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="5063b-1594">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="5063b-1595">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="5063b-1595">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="5063b-1596">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="5063b-1596">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="5063b-1597">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="5063b-1597">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="5063b-1598">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1598">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="5063b-1599">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-1599">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="5063b-1600">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-1600">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="5063b-1601">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-1601">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="5063b-1602">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-1602">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="5063b-1603">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1603">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="5063b-1604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-1604">Az.Monitor</span></span>
* <span data-ttu-id="5063b-1605">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1605">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1606">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1606">Az.Network</span></span>
* <span data-ttu-id="5063b-1607">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1607">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-1608">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1608">Az.OperationalInsights</span></span>
* <span data-ttu-id="5063b-1609">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1609">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="5063b-1610">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1610">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="5063b-1611">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1611">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="5063b-1612">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1612">Az.Resources</span></span>
* <span data-ttu-id="5063b-1613">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="5063b-1613">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="5063b-1614">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="5063b-1614">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="5063b-1615">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="5063b-1615">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="5063b-1616">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1616">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1617">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1617">Az.Sql</span></span>
* <span data-ttu-id="5063b-1618">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1618">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="5063b-1619">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1619">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1620">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1620">Az.Websites</span></span>
* <span data-ttu-id="5063b-1621">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1621">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="5063b-1622">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1622">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1623">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1623">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1624">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1624">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="5063b-1625">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1625">Az.AnalysisServices</span></span>
<span data-ttu-id="5063b-1626">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="5063b-1626">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1627">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1627">Az.Compute</span></span>
* <span data-ttu-id="5063b-1628">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1628">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="5063b-1629">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1629">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="5063b-1630">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1630">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1631">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1631">Az.RecoveryServices</span></span>
<span data-ttu-id="5063b-1632">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="5063b-1632">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1633">Az.Resources</span></span>
* <span data-ttu-id="5063b-1634">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1634">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="5063b-1635">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="5063b-1635">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="5063b-1636">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1636">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="5063b-1637">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="5063b-1637">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1638">Az.Sql</span></span>
* <span data-ttu-id="5063b-1639">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1639">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="5063b-1640">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1640">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="5063b-1641">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1641">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="5063b-1642">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1642">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1643">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1643">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1644">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="5063b-1644">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="5063b-1645">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1645">Az.AnalysisServices</span></span>
* <span data-ttu-id="5063b-1646">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="5063b-1646">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1647">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1647">Az.RecoveryServices</span></span>
* <span data-ttu-id="5063b-1648">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="5063b-1648">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="5063b-1649">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1649">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1650">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1650">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1651">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1651">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="5063b-1652">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="5063b-1653">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1653">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="5063b-1654">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="5063b-1654">Az.Aks</span></span>
* <span data-ttu-id="5063b-1655">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1655">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="5063b-1656">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1656">Az.Automation</span></span>
* <span data-ttu-id="5063b-1657">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1657">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="5063b-1658">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1658">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="5063b-1659">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="5063b-1659">Az.Cdn</span></span>
* <span data-ttu-id="5063b-1660">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1660">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1661">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1661">Az.Compute</span></span>
* <span data-ttu-id="5063b-1662">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1662">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="5063b-1663">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1663">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="5063b-1664">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1664">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="5063b-1665">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="5063b-1665">Az.ContainerRegistry</span></span>
* <span data-ttu-id="5063b-1666">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1666">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="5063b-1667">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5063b-1667">Az.DataFactory</span></span>
* <span data-ttu-id="5063b-1668">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1668">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1669">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1669">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1670">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="5063b-1670">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="5063b-1671">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="5063b-1671">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="5063b-1672">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1672">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-1673">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1673">Az.IotHub</span></span>
* <span data-ttu-id="5063b-1674">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1674">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="5063b-1675">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-1675">Az.KeyVault</span></span>
* <span data-ttu-id="5063b-1676">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1676">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1677">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1677">Az.Network</span></span>
* <span data-ttu-id="5063b-1678">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1678">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1679">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1679">Az.Resources</span></span>
* <span data-ttu-id="5063b-1680">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1680">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="5063b-1681">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1681">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="5063b-1682">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1682">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="5063b-1683">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="5063b-1683">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="5063b-1684">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="5063b-1684">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="5063b-1685">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1685">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="5063b-1686">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="5063b-1686">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-1687">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1687">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-1688">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="5063b-1688">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="5063b-1689">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1689">Fix some error messages.</span></span>
* <span data-ttu-id="5063b-1690">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1690">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="5063b-1691">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1691">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="5063b-1692">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="5063b-1692">Az.SignalR</span></span>
* <span data-ttu-id="5063b-1693">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1693">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1694">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1694">Az.Sql</span></span>
* <span data-ttu-id="5063b-1695">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1695">Update incorrect online help URLs</span></span>
* <span data-ttu-id="5063b-1696">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1696">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="5063b-1697">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1697">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="5063b-1698">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1698">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1699">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1699">Az.Storage</span></span>
* <span data-ttu-id="5063b-1700">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1700">Update incorrect online help URLs</span></span>
* <span data-ttu-id="5063b-1701">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="5063b-1701">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="5063b-1702">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="5063b-1702">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="5063b-1703">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="5063b-1703">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="5063b-1704">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5063b-1704">Az.TrafficManager</span></span>
* <span data-ttu-id="5063b-1705">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1705">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1706">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1706">Az.Websites</span></span>
* <span data-ttu-id="5063b-1707">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1707">Update incorrect online help URLs</span></span>
* <span data-ttu-id="5063b-1708">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1708">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="5063b-1709">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="5063b-1709">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="5063b-1710">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1710">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="5063b-1711">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1711">Az.Accounts</span></span>
* <span data-ttu-id="5063b-1712">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="5063b-1712">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1713">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1713">Az.Compute</span></span>
* <span data-ttu-id="5063b-1714">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1714">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="5063b-1715">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="5063b-1715">Updated the description of ID in help files</span></span>
* <span data-ttu-id="5063b-1716">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1716">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1717">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1717">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1718">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1718">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="5063b-1719">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1719">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="5063b-1720">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5063b-1720">Az.EventGrid</span></span>
* <span data-ttu-id="5063b-1721">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1721">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="5063b-1722">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="5063b-1722">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="5063b-1723">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="5063b-1723">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="5063b-1724">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="5063b-1724">Event Time-To-Live,</span></span>
        - <span data-ttu-id="5063b-1725">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="5063b-1725">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="5063b-1726">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="5063b-1726">Dead letter endpoint.</span></span>
    - <span data-ttu-id="5063b-1727">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="5063b-1727">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="5063b-1728">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="5063b-1728">Event Time-To-Live,</span></span>
        - <span data-ttu-id="5063b-1729">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="5063b-1729">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="5063b-1730">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="5063b-1730">Dead letter endpoint.</span></span>
* <span data-ttu-id="5063b-1731">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1731">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="5063b-1732">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1732">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="5063b-1733">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="5063b-1733">Az.IotHub</span></span>
* <span data-ttu-id="5063b-1734">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1734">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="5063b-1735">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5063b-1735">Az.LogicApp</span></span>
* <span data-ttu-id="5063b-1736">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="5063b-1736">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1737">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1737">Az.Resources</span></span>
* <span data-ttu-id="5063b-1738">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1738">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="5063b-1739">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="5063b-1739">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="5063b-1740">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1740">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="5063b-1741">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1741">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="5063b-1742">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="5063b-1742">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="5063b-1743">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="5063b-1743">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="5063b-1744">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="5063b-1744">Az.SignalR</span></span>
* <span data-ttu-id="5063b-1745">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1745">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-1746">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1746">Az.Sql</span></span>
* <span data-ttu-id="5063b-1747">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1747">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="5063b-1748">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1748">Az.Storage</span></span>
* <span data-ttu-id="5063b-1749">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="5063b-1749">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="5063b-1750">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="5063b-1750">New-AzStorageContext</span></span>
* <span data-ttu-id="5063b-1751">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1751">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="5063b-1752">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="5063b-1752">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-1753">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1753">Az.Websites</span></span>
* <span data-ttu-id="5063b-1754">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1754">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="5063b-1755">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1755">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="5063b-1756">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1756">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="5063b-1757">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-1757">General</span></span>

- <span data-ttu-id="5063b-1758">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="5063b-1758">General Availability of Az Module</span></span>
- <span data-ttu-id="5063b-1759">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="5063b-1759">Online help for each module</span></span>
- <span data-ttu-id="5063b-1760">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1760">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="5063b-1761">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1761">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="5063b-1762">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="5063b-1762">Az.Accounts</span></span>
- <span data-ttu-id="5063b-1763">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1763">Changed from Az.Profile</span></span>
- <span data-ttu-id="5063b-1764">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1764">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="5063b-1765">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-1765">Az.ApiManagement</span></span>
- <span data-ttu-id="5063b-1766">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="5063b-1766">Fixes for #7002</span></span>
- <span data-ttu-id="5063b-1767">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1767">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="5063b-1768">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="5063b-1768">Az.Batch</span></span>
- <span data-ttu-id="5063b-1769">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1769">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="5063b-1770">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1770">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="5063b-1771">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1771">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="5063b-1772">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="5063b-1772">Az.Billing</span></span>
- <span data-ttu-id="5063b-1773">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1773">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="5063b-1774">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1774">Az.CognitivServices</span></span>
- <span data-ttu-id="5063b-1775">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1775">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="5063b-1776">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1776">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="5063b-1777">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1777">Az.ContainerInstance</span></span>
- <span data-ttu-id="5063b-1778">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1778">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="5063b-1779">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5063b-1779">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="5063b-1780">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1780">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1781">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1781">Az.DataLakeStore</span></span>
- <span data-ttu-id="5063b-1782">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1782">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="5063b-1783">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="5063b-1783">Az.Monitor</span></span>
- <span data-ttu-id="5063b-1784">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1784">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="5063b-1785">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5063b-1785">Az.KeyVault</span></span>
- <span data-ttu-id="5063b-1786">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1786">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="5063b-1787">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="5063b-1787">Az.MachineLearning</span></span>
- <span data-ttu-id="5063b-1788">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="5063b-1788">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="5063b-1789">Az.Media</span><span class="sxs-lookup"><span data-stu-id="5063b-1789">Az.Media</span></span>
- <span data-ttu-id="5063b-1790">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1790">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="5063b-1791">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1791">Az.Network</span></span>
<span data-ttu-id="5063b-1792">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1792">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="5063b-1793">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-1793">New cmdlets added:</span></span>
        - <span data-ttu-id="5063b-1794">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1794">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1795">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1795">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1796">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1796">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1797">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1797">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1798">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1798">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1799">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1799">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="5063b-1800">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="5063b-1800">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="5063b-1801">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="5063b-1801">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="5063b-1802">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1802">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="5063b-1803">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5063b-1803">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="5063b-1804">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1804">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="5063b-1805">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="5063b-1805">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="5063b-1806">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-1806">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="5063b-1807">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-1807">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="5063b-1808">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1808">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="5063b-1809">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1809">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="5063b-1810">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="5063b-1810">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="5063b-1811">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="5063b-1811">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="5063b-1812">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="5063b-1812">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="5063b-1813">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1813">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="5063b-1814">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1814">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="5063b-1815">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1815">Az.OperationalInsights</span></span>
- <span data-ttu-id="5063b-1816">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1816">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="5063b-1817">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="5063b-1817">Az.Profile</span></span>
- <span data-ttu-id="5063b-1818">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1818">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1819">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1819">Az.RecoveryServices</span></span>
- <span data-ttu-id="5063b-1820">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1820">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="5063b-1821">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1821">Az.Resources</span></span>
- <span data-ttu-id="5063b-1822">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1822">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="5063b-1823">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1823">Az.ServiceFabric</span></span>
- <span data-ttu-id="5063b-1824">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="5063b-1824">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="5063b-1825">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1825">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="5063b-1826">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="5063b-1826">Az.SIgnalR</span></span>
- <span data-ttu-id="5063b-1827">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="5063b-1827">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="5063b-1828">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1828">Az.Sql</span></span>
- <span data-ttu-id="5063b-1829">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1829">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="5063b-1830">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1830">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="5063b-1831">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1831">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="5063b-1832">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1832">Az.Storage</span></span>
- <span data-ttu-id="5063b-1833">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1833">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="5063b-1834">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1834">Az.Websites</span></span>
- <span data-ttu-id="5063b-1835">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="5063b-1835">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="5063b-1836">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1836">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="5063b-1837">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-1837">General</span></span>

* <span data-ttu-id="5063b-1838">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="5063b-1838">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="5063b-1839">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1839">Az.Compute</span></span>

* <span data-ttu-id="5063b-1840">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1840">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1841">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1841">Az.DataLakeStore</span></span>

* <span data-ttu-id="5063b-1842">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1842">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="5063b-1843">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="5063b-1843">Az.FrontDoor</span></span>

* <span data-ttu-id="5063b-1844">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1844">Fixed some broken links</span></span>
    - <span data-ttu-id="5063b-1845">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1845">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="5063b-1846">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1846">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="5063b-1847">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1847">Az.RecoveryServices</span></span>

* <span data-ttu-id="5063b-1848">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1848">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="5063b-1849">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1849">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="5063b-1850">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1850">Az.Resources</span></span>

* <span data-ttu-id="5063b-1851">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1851">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="5063b-1852">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1852">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="5063b-1853">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1853">Az.Sql</span></span>

* <span data-ttu-id="5063b-1854">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="5063b-1854">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="5063b-1855">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1855">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="5063b-1856">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1856">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="5063b-1857">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1857">Az.Storage</span></span>

* <span data-ttu-id="5063b-1858">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1858">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="5063b-1859">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1859">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="5063b-1860">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="5063b-1860">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="5063b-1861">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="5063b-1861">Support Static Website configuration</span></span>
    - <span data-ttu-id="5063b-1862">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="5063b-1862">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="5063b-1863">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="5063b-1863">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="5063b-1864">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-1864">Az.Websites</span></span>

* <span data-ttu-id="5063b-1865">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="5063b-1865">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="5063b-1866">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1866">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="5063b-1867">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="5063b-1867">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="5063b-1868">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1868">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="5063b-1869">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5063b-1869">Az.ApiManagement</span></span>
* <span data-ttu-id="5063b-1870">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1870">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="5063b-1871">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="5063b-1871">Az.Automation</span></span>
* <span data-ttu-id="5063b-1872">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="5063b-1872">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="5063b-1873">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1873">Added Update Management cmdlets</span></span>
* <span data-ttu-id="5063b-1874">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1874">Added Source Control cmdlets</span></span>
* <span data-ttu-id="5063b-1875">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1875">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="5063b-1876">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1876">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="5063b-1877">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1877">Az.Compute</span></span>
* <span data-ttu-id="5063b-1878">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1878">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="5063b-1879">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1879">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="5063b-1880">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1880">Az.ContainerInstance</span></span>
* <span data-ttu-id="5063b-1881">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1881">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="5063b-1882">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="5063b-1882">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="5063b-1883">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1883">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="5063b-1884">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1884">Az.Network</span></span>
* <span data-ttu-id="5063b-1885">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1885">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="5063b-1886">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1886">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="5063b-1887">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1887">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="5063b-1888">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1888">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="5063b-1889">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5063b-1889">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5063b-1890">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1890">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="5063b-1891">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1891">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="5063b-1892">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5063b-1892">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5063b-1893">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1893">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="5063b-1894">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1894">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="5063b-1895">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="5063b-1895">Az.Relay</span></span>
* <span data-ttu-id="5063b-1896">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="5063b-1896">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="5063b-1897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1897">Az.Resources</span></span>
* <span data-ttu-id="5063b-1898">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1898">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="5063b-1899">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1899">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="5063b-1900">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="5063b-1900">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="5063b-1901">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1901">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-1902">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1902">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="5063b-1903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-1903">Az.Sql</span></span>
* <span data-ttu-id="5063b-1904">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1904">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="5063b-1905">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1905">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5063b-1906">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1906">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5063b-1907">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1907">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5063b-1908">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="5063b-1908">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="5063b-1909">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5063b-1909">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5063b-1910">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5063b-1910">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5063b-1911">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5063b-1911">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="5063b-1912">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="5063b-1912">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="5063b-1913">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="5063b-1913">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="5063b-1914">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1914">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="5063b-1915">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1915">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="5063b-1916">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="5063b-1916">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="5063b-1917">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="5063b-1917">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="5063b-1918">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="5063b-1918">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="5063b-1919">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="5063b-1919">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="5063b-1920">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1920">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="5063b-1921">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1921">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5063b-1922">全般</span><span class="sxs-lookup"><span data-stu-id="5063b-1922">General</span></span>
* <span data-ttu-id="5063b-1923">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="5063b-1923">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="5063b-1924">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="5063b-1924">Az.Profile</span></span>
* <span data-ttu-id="5063b-1925">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1925">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="5063b-1926">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1926">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="5063b-1927">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1927">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="5063b-1928">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1928">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="5063b-1929">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1929">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="5063b-1930">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1930">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="5063b-1931">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1931">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-1932">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1932">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-1933">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1933">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1934">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1934">Az.Compute</span></span>
* <span data-ttu-id="5063b-1935">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1935">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="5063b-1936">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="5063b-1936">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="5063b-1937">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1937">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1938">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1938">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1939">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1939">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="5063b-1940">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1940">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="5063b-1941">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="5063b-1941">Az.Insights</span></span>
* <span data-ttu-id="5063b-1942">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1942">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="5063b-1943">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="5063b-1943">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="5063b-1944">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1944">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="5063b-1945">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="5063b-1945">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1946">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1946">Az.Network</span></span>
* <span data-ttu-id="5063b-1947">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="5063b-1947">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="5063b-1948">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-1948">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="5063b-1949">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="5063b-1949">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="5063b-1950">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5063b-1950">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="5063b-1951">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="5063b-1951">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="5063b-1952">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="5063b-1952">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="5063b-1953">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5063b-1953">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="5063b-1954">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5063b-1954">Az.PolicyInsights</span></span>
* <span data-ttu-id="5063b-1955">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1955">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1956">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1956">Az.Resources</span></span>
* <span data-ttu-id="5063b-1957">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1957">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="5063b-1958">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1958">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="5063b-1959">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5063b-1959">Az.ServiceBus</span></span>
* <span data-ttu-id="5063b-1960">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1960">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="5063b-1961">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5063b-1961">Az.ServiceFabric</span></span>
* <span data-ttu-id="5063b-1962">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1962">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="5063b-1963">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1963">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="5063b-1964">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="5063b-1964">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="5063b-1965">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="5063b-1965">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="5063b-1966">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1966">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="5063b-1967">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1967">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="5063b-1968">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="5063b-1968">Az.Profile</span></span>
* <span data-ttu-id="5063b-1969">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1969">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="5063b-1970">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1970">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1971">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1971">Az.Compute</span></span>
* <span data-ttu-id="5063b-1972">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1972">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="5063b-1973">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1973">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="5063b-1974">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5063b-1974">Az.DataLakeStore</span></span>
* <span data-ttu-id="5063b-1975">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1975">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="5063b-1976">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1976">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="5063b-1977">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1977">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5063b-1978">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1978">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5063b-1979">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="5063b-1979">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-1980">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-1980">Az.Network</span></span>
* <span data-ttu-id="5063b-1981">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1981">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="5063b-1982">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1982">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-1983">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-1983">Az.Resources</span></span>
* <span data-ttu-id="5063b-1984">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1984">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="5063b-1985">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1985">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="5063b-1986">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="5063b-1986">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="5063b-1987">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5063b-1987">Azure.Storage</span></span>
* <span data-ttu-id="5063b-1988">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1988">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="5063b-1989">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="5063b-1989">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="5063b-1990">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="5063b-1990">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="5063b-1991">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1991">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="5063b-1992">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="5063b-1992">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="5063b-1993">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5063b-1993">Az.CognitiveServices</span></span>
* <span data-ttu-id="5063b-1994">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1994">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="5063b-1995">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="5063b-1995">Az.Compute</span></span>
* <span data-ttu-id="5063b-1996">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1996">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="5063b-1997">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-1997">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="5063b-1998">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-1998">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="5063b-1999">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5063b-1999">Az.DataFactoryV2</span></span>
* <span data-ttu-id="5063b-2000">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-2000">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="5063b-2001">Az.Network</span><span class="sxs-lookup"><span data-stu-id="5063b-2001">Az.Network</span></span>
* <span data-ttu-id="5063b-2002">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="5063b-2002">Added NetworkProfile functionality.</span></span> <span data-ttu-id="5063b-2003">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="5063b-2003">new cmdlets added</span></span>
    - <span data-ttu-id="5063b-2004">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5063b-2004">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="5063b-2005">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5063b-2005">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="5063b-2006">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5063b-2006">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="5063b-2007">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5063b-2007">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="5063b-2008">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-2008">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="5063b-2009">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="5063b-2009">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="5063b-2010">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2010">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="5063b-2011">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2011">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="5063b-2012">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2012">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="5063b-2013">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5063b-2013">Az.RedisCache</span></span>
* <span data-ttu-id="5063b-2014">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="5063b-2014">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="5063b-2015">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2015">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="5063b-2016">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="5063b-2016">Az.Resources</span></span>
* <span data-ttu-id="5063b-2017">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2017">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="5063b-2018">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2018">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="5063b-2019">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="5063b-2019">Az.Sql</span></span>
* <span data-ttu-id="5063b-2020">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="5063b-2020">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="5063b-2021">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="5063b-2021">Az.Websites</span></span>
* <span data-ttu-id="5063b-2022">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="5063b-2022">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="5063b-2023">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="5063b-2023">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="5063b-2024">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="5063b-2024">0.2.0 - September 2018</span></span>
 <span data-ttu-id="5063b-2025">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="5063b-2025">Initial Release</span></span>

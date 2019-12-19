---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: f77d901169b0d98b2425a2e50d33a1789150b770
ms.sourcegitcommit: e598dc45a26ff5a71112383252b350d750144a47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/17/2019
ms.locfileid: "75182555"
---
## <a name="320---december-2019"></a><span data-ttu-id="6953c-103">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="6953c-103">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="6953c-104">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-104">General</span></span>
* <span data-ttu-id="6953c-105">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-105">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-106">Az.Accounts</span></span>
* <span data-ttu-id="6953c-107">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="6953c-107">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="6953c-108">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="6953c-108">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="6953c-109">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-109">Az.Batch</span></span>
* <span data-ttu-id="6953c-110">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="6953c-110">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-111">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-111">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-112">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-112">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="6953c-113">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-113">Az.FrontDoor</span></span>
* <span data-ttu-id="6953c-114">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-114">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="6953c-115">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-115">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="6953c-116">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="6953c-116">Az.HealthcareApis</span></span>
* <span data-ttu-id="6953c-117">例外処理</span><span class="sxs-lookup"><span data-stu-id="6953c-117">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-118">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-118">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-119">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-119">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="6953c-120">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="6953c-120">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="6953c-121">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-121">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-122">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-122">Az.Monitor</span></span>
* <span data-ttu-id="6953c-123">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="6953c-123">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="6953c-124">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="6953c-124">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="6953c-125">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="6953c-125">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-126">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-126">Az.Network</span></span>
* <span data-ttu-id="6953c-127">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-127">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-128">Az.Resources</span></span>
* <span data-ttu-id="6953c-129">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-129">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="6953c-130">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-130">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-131">Az.Sql</span></span>
* <span data-ttu-id="6953c-132">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="6953c-132">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-133">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-133">Az.Storage</span></span>
* <span data-ttu-id="6953c-134">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-134">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="6953c-135">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="6953c-135">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="6953c-136">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="6953c-136">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="6953c-137">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="6953c-137">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="6953c-138">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="6953c-138">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="6953c-139">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-139">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="6953c-140">管理プレーンのファイル共有コマンドレットで 5120 を超える QuotaGiB の共有をサポートし、パラメーター別名 'Quota' をパラメーター 'QuotaGiB' に追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-140">Support Share QuotaGiB more than 5120 in Management plane File Share cmdlets, and add parameter alias 'Quota' to parameter 'QuotaGiB'</span></span> 
    - <span data-ttu-id="6953c-141">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-141">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="6953c-142">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-142">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="6953c-143">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-143">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="6953c-144">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="6953c-144">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="6953c-145">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-145">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="6953c-146">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="6953c-146">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="6953c-147">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6953c-147">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="6953c-148">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="6953c-148">Highlights since the last major release</span></span>
* <span data-ttu-id="6953c-149">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="6953c-149">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="6953c-150">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="6953c-150">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-151">Az.Compute</span></span>
* <span data-ttu-id="6953c-152">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="6953c-152">VM Reapply feature</span></span>
    - <span data-ttu-id="6953c-153">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-153">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="6953c-154">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="6953c-154">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="6953c-155">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="6953c-155">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="6953c-156">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="6953c-156">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="6953c-157">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-157">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="6953c-158">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-158">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="6953c-159">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="6953c-159">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="6953c-160">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-160">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="6953c-161">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-161">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="6953c-162">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-162">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="6953c-163">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="6953c-163">Az.DataBoxEdge</span></span>
* <span data-ttu-id="6953c-164">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-164">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="6953c-165">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-165">Get the Order</span></span>
* <span data-ttu-id="6953c-166">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-166">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="6953c-167">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-167">Create new Order</span></span>
* <span data-ttu-id="6953c-168">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-168">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="6953c-169">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-169">Remove the Order</span></span>
* <span data-ttu-id="6953c-170">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="6953c-170">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="6953c-171">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="6953c-171">Now creates Local Share</span></span>
* <span data-ttu-id="6953c-172">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-172">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="6953c-173">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-173">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="6953c-174">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-174">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="6953c-175">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="6953c-175">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="6953c-176">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-176">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="6953c-177">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-177">Gets the information about Triggers</span></span>
* <span data-ttu-id="6953c-178">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-178">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="6953c-179">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-179">Create new Triggers</span></span>
* <span data-ttu-id="6953c-180">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-180">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="6953c-181">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-181">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-182">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-182">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-183">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-183">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="6953c-184">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-184">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-185">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-185">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-186">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-186">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-187">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-187">Az.EventHub</span></span>
* <span data-ttu-id="6953c-188">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-188">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="6953c-189">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-189">Az.FrontDoor</span></span>
* <span data-ttu-id="6953c-190">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-190">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="6953c-191">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-191">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="6953c-192">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-192">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="6953c-193">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="6953c-193">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-194">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-194">Az.Network</span></span>
* <span data-ttu-id="6953c-195">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="6953c-195">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="6953c-196">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="6953c-196">Az.PrivateDns</span></span>
* <span data-ttu-id="6953c-197">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-197">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-198">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-198">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-199">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-199">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="6953c-200">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="6953c-200">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="6953c-201">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-201">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="6953c-202">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="6953c-202">Az.RedisCache</span></span>
* <span data-ttu-id="6953c-203">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-203">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="6953c-204">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-204">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="6953c-205">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-205">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-206">Az.Resources</span></span>
- <span data-ttu-id="6953c-207">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-207">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="6953c-208">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-208">Updated create policy definition help example</span></span>
- <span data-ttu-id="6953c-209">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-209">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="6953c-210">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-210">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="6953c-211">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="6953c-211">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-212">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-212">Az.Sql</span></span>
* <span data-ttu-id="6953c-213">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-213">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="6953c-214">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-214">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="6953c-215">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6953c-215">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="6953c-216">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-216">General</span></span>
* <span data-ttu-id="6953c-217">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="6953c-217">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-218">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-218">Az.Accounts</span></span>
* <span data-ttu-id="6953c-219">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-219">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="6953c-220">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="6953c-220">Az.Advisor</span></span>
* <span data-ttu-id="6953c-221">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-221">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="6953c-222">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-222">Az.Batch</span></span>
* <span data-ttu-id="6953c-223">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-223">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="6953c-224">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="6953c-224">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="6953c-225">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="6953c-225">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="6953c-226">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-226">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="6953c-227">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="6953c-227">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="6953c-228">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-228">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="6953c-229">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="6953c-229">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="6953c-230">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="6953c-230">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="6953c-231">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="6953c-231">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="6953c-232">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-232">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="6953c-233">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-233">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="6953c-234">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="6953c-234">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="6953c-235">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-235">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="6953c-236">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-236">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="6953c-237">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-237">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="6953c-238">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-238">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="6953c-239">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-239">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="6953c-240">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-240">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="6953c-241">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-241">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="6953c-242">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6953c-242">This operation is no longer supported.</span></span>
* <span data-ttu-id="6953c-243">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-243">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="6953c-244">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-244">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="6953c-245">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-245">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="6953c-246">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="6953c-246">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="6953c-247">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="6953c-247">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="6953c-248">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-248">New non-verified images are also now returned.</span></span> <span data-ttu-id="6953c-249">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="6953c-249">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="6953c-250">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-250">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="6953c-251">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-251">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="6953c-252">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="6953c-252">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="6953c-253">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-253">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="6953c-254">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="6953c-254">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="6953c-255">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-255">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="6953c-256">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="6953c-256">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="6953c-257">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="6953c-257">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="6953c-258">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="6953c-258">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6953c-259">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-259">Az.Cdn</span></span>
* <span data-ttu-id="6953c-260">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-260">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="6953c-261">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-261">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-262">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-262">Az.Compute</span></span>
* <span data-ttu-id="6953c-263">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="6953c-263">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="6953c-264">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="6953c-264">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="6953c-265">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="6953c-265">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="6953c-266">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="6953c-266">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="6953c-267">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-267">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="6953c-268">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-268">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="6953c-269">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="6953c-269">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="6953c-270">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-270">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="6953c-271">重大な変更</span><span class="sxs-lookup"><span data-stu-id="6953c-271">Breaking changes</span></span>
    - <span data-ttu-id="6953c-272">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="6953c-272">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="6953c-273">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="6953c-273">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-274">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-274">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-275">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-275">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-276">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-276">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-277">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="6953c-277">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="6953c-278">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="6953c-278">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="6953c-279">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="6953c-279">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="6953c-280">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-280">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="6953c-281">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-281">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="6953c-282">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-282">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="6953c-283">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-283">Az.FrontDoor</span></span>
* <span data-ttu-id="6953c-284">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-284">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="6953c-285">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="6953c-285">Az.HDInsight</span></span>
* <span data-ttu-id="6953c-286">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-286">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="6953c-287">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="6953c-287">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="6953c-288">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-288">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="6953c-289">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-289">Removed five cmdlets:</span></span>
    - <span data-ttu-id="6953c-290">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="6953c-290">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="6953c-291">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="6953c-291">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="6953c-292">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="6953c-292">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="6953c-293">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="6953c-293">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="6953c-294">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="6953c-294">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="6953c-295">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-295">Added three cmdlets:</span></span>
    - <span data-ttu-id="6953c-296">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="6953c-296">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="6953c-297">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="6953c-297">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="6953c-298">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="6953c-298">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="6953c-299">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-299">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="6953c-300">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-300">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="6953c-301">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-301">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="6953c-302">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="6953c-302">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="6953c-303">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-303">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="6953c-304">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-304">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="6953c-305">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-305">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="6953c-306">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-306">Added some scenario test cases.</span></span>
* <span data-ttu-id="6953c-307">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="6953c-307">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-308">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-308">Az.IotHub</span></span>
* <span data-ttu-id="6953c-309">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="6953c-309">Breaking changes:</span></span>
    - <span data-ttu-id="6953c-310">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-310">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="6953c-311">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-311">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="6953c-312">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-312">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="6953c-313">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-313">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="6953c-314">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-314">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="6953c-315">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-315">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="6953c-316">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-316">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="6953c-317">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-317">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="6953c-318">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-318">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="6953c-319">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-319">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="6953c-320">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-320">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="6953c-321">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-321">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-322">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-322">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-323">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-323">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-324">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-324">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="6953c-325">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-325">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="6953c-326">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-326">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-327">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-327">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-328">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-328">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-329">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-329">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-330">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-330">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-331">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-331">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-332">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-332">Az.Resources</span></span>
* <span data-ttu-id="6953c-333">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-333">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-334">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-334">Az.Network</span></span>
* <span data-ttu-id="6953c-335">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="6953c-335">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="6953c-336">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-336">Updated cmdlet:</span></span>
        - <span data-ttu-id="6953c-337">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-337">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-338">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-338">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-339">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-339">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-340">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-340">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-341">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-341">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="6953c-342">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6953c-342">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="6953c-343">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-343">New cmdlet:</span></span>
        - <span data-ttu-id="6953c-344">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="6953c-344">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="6953c-345">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-345">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="6953c-346">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-346">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="6953c-347">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-347">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="6953c-348">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-348">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="6953c-349">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-349">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="6953c-350">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-350">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="6953c-351">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-351">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="6953c-352">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-352">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-353">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="6953c-353">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="6953c-354">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-354">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="6953c-355">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-355">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="6953c-356">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-356">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="6953c-357">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="6953c-357">Set-AzVirtualHub</span></span>
* <span data-ttu-id="6953c-358">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-358">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="6953c-359">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6953c-359">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="6953c-360">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-360">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="6953c-361">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-361">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="6953c-362">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-362">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="6953c-363">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-363">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="6953c-364">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-364">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="6953c-365">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-365">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-366">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-366">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="6953c-367">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6953c-367">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="6953c-368">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-368">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="6953c-369">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-369">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="6953c-370">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-370">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="6953c-371">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-371">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="6953c-372">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-372">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="6953c-373">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-373">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="6953c-374">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-374">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-375">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="6953c-375">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="6953c-376">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="6953c-376">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="6953c-377">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="6953c-377">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="6953c-378">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="6953c-378">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="6953c-379">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="6953c-379">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="6953c-380">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-380">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="6953c-381">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6953c-381">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="6953c-382">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-382">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="6953c-383">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-383">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="6953c-384">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-384">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="6953c-385">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-385">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="6953c-386">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6953c-386">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="6953c-387">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-387">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="6953c-388">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-388">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="6953c-389">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-389">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="6953c-390">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-390">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="6953c-391">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-391">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="6953c-392">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-392">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-393">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-393">New-AzIpGroup</span></span>
        - <span data-ttu-id="6953c-394">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-394">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="6953c-395">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-395">Get-AzIpGroup</span></span>
        - <span data-ttu-id="6953c-396">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-396">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-397">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-397">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-398">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="6953c-398">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-399">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-399">Az.Sql</span></span>
* <span data-ttu-id="6953c-400">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-400">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="6953c-401">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-401">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="6953c-402">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-402">Removed deprecated aliases:</span></span>
* <span data-ttu-id="6953c-403">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="6953c-403">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="6953c-404">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="6953c-404">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="6953c-405">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-405">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="6953c-406">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-406">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="6953c-407">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="6953c-407">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="6953c-408">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-408">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-409">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-409">Az.Storage</span></span>
* <span data-ttu-id="6953c-410">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-410">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="6953c-411">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-411">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="6953c-412">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-412">Set-AzStorageAccount</span></span>
* <span data-ttu-id="6953c-413">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="6953c-413">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="6953c-414">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="6953c-414">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="6953c-415">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="6953c-415">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="6953c-416">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="6953c-416">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="6953c-417">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-417">General</span></span>
* <span data-ttu-id="6953c-418">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="6953c-418">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-419">Az.Accounts</span></span>
* <span data-ttu-id="6953c-420">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-420">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="6953c-421">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-421">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-422">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-422">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="6953c-423">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="6953c-423">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-424">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-424">Az.Automation</span></span>
* <span data-ttu-id="6953c-425">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-425">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="6953c-426">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-426">Az.Batch</span></span>
* <span data-ttu-id="6953c-427">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="6953c-427">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-428">Az.Compute</span></span>
* <span data-ttu-id="6953c-429">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-429">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="6953c-430">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-430">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="6953c-431">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-431">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="6953c-432">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-432">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-433">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-433">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-434">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="6953c-434">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="6953c-435">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="6953c-435">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="6953c-436">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-436">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-437">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-437">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-438">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-438">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="6953c-439">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="6953c-439">Az.HealthcareApis</span></span>
* <span data-ttu-id="6953c-440">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-440">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="6953c-441">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-441">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="6953c-442">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-442">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="6953c-443">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-443">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-444">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-444">Az.IotHub</span></span>
* <span data-ttu-id="6953c-445">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="6953c-445">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="6953c-446">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="6953c-446">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="6953c-447">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-447">Az.Monitor</span></span>
* <span data-ttu-id="6953c-448">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="6953c-448">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="6953c-449">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="6953c-449">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="6953c-450">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="6953c-450">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="6953c-451">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-451">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-452">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-452">Az.Network</span></span>
* <span data-ttu-id="6953c-453">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-453">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="6953c-454">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-454">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="6953c-455">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-455">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-456">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-456">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="6953c-457">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-457">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="6953c-458">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-458">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="6953c-459">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-459">Updated cmdlets:</span></span>
        - <span data-ttu-id="6953c-460">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-460">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="6953c-461">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-461">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="6953c-462">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-462">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="6953c-463">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="6953c-463">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="6953c-464">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="6953c-464">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="6953c-465">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="6953c-465">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="6953c-466">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="6953c-466">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="6953c-467">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="6953c-467">Az.RedisCache</span></span>
* <span data-ttu-id="6953c-468">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-468">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-469">Az.Sql</span></span>
* <span data-ttu-id="6953c-470">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-470">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-471">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-471">Az.Storage</span></span>
* <span data-ttu-id="6953c-472">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="6953c-472">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="6953c-473">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6953c-473">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="6953c-474">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="6953c-474">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="6953c-475">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6953c-475">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="6953c-476">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-476">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="6953c-477">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="6953c-477">Az.StorageSync</span></span>
* <span data-ttu-id="6953c-478">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-478">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-479">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-479">Az.Websites</span></span>
* <span data-ttu-id="6953c-480">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="6953c-480">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="6953c-481">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="6953c-481">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="6953c-482">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-482">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-483">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-483">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="6953c-484">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-484">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="6953c-485">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="6953c-485">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-486">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-486">Az.Automation</span></span>
* <span data-ttu-id="6953c-487">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-487">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="6953c-488">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-488">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="6953c-489">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-489">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-490">Az.Compute</span></span>
* <span data-ttu-id="6953c-491">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-491">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="6953c-492">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-492">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="6953c-493">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-493">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="6953c-494">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="6953c-494">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="6953c-495">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="6953c-495">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="6953c-496">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-496">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="6953c-497">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-497">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="6953c-498">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-498">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="6953c-499">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-499">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-500">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-501">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-501">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="6953c-502">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-502">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="6953c-503">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="6953c-503">Az.HDInsight</span></span>
* <span data-ttu-id="6953c-504">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="6953c-504">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-505">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-505">Az.IotHub</span></span>
* <span data-ttu-id="6953c-506">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-506">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="6953c-507">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-507">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="6953c-508">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6953c-508">New cmdlets are:</span></span>
    - <span data-ttu-id="6953c-509">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="6953c-509">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="6953c-510">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="6953c-510">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="6953c-511">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="6953c-511">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="6953c-512">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="6953c-512">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-513">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-513">Az.Monitor</span></span>
* <span data-ttu-id="6953c-514">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="6953c-514">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="6953c-515">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="6953c-515">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="6953c-516">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="6953c-516">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="6953c-517">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="6953c-517">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="6953c-518">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-518">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="6953c-519">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-519">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="6953c-520">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="6953c-520">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="6953c-521">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="6953c-521">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="6953c-522">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-522">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="6953c-523">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-523">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="6953c-524">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-524">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="6953c-525">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="6953c-525">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="6953c-526">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-526">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="6953c-527">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-527">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="6953c-528">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-528">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="6953c-529">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="6953c-529">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="6953c-530">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="6953c-530">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="6953c-531">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="6953c-531">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="6953c-532">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-532">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="6953c-533">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="6953c-533">Overall improved help files</span></span>
* <span data-ttu-id="6953c-534">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-534">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-535">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-535">Az.Network</span></span>
* <span data-ttu-id="6953c-536">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-536">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="6953c-537">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-537">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="6953c-538">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="6953c-538">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="6953c-539">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="6953c-539">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="6953c-540">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="6953c-540">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="6953c-541">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-541">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="6953c-542">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-542">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="6953c-543">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-543">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="6953c-544">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-544">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="6953c-545">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-545">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="6953c-546">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-546">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="6953c-547">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-547">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="6953c-548">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-548">New cmdlets</span></span>
        - <span data-ttu-id="6953c-549">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="6953c-549">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="6953c-550">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-550">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="6953c-551">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-551">Updated cmdlet:</span></span>
        - <span data-ttu-id="6953c-552">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="6953c-552">New-VpnSite</span></span>
        - <span data-ttu-id="6953c-553">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="6953c-553">Update-VpnSite</span></span>
        - <span data-ttu-id="6953c-554">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-554">New-VpnConnection</span></span>
        - <span data-ttu-id="6953c-555">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-555">Update-VpnConnection</span></span>
* <span data-ttu-id="6953c-556">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-556">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-557">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-557">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-558">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-558">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="6953c-559">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-559">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-560">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-560">Az.Resources</span></span>
* <span data-ttu-id="6953c-561">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-561">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-562">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-562">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-563">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-563">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="6953c-564">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-564">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="6953c-565">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="6953c-565">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="6953c-566">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="6953c-566">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="6953c-567">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6953c-567">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="6953c-568">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="6953c-568">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="6953c-569">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="6953c-569">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="6953c-570">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="6953c-570">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="6953c-571">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="6953c-571">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="6953c-572">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6953c-572">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="6953c-573">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="6953c-573">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="6953c-574">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="6953c-574">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="6953c-575">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="6953c-575">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="6953c-576">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6953c-576">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="6953c-577">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="6953c-577">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="6953c-578">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="6953c-578">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="6953c-579">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="6953c-579">Az.SignalR</span></span>
* <span data-ttu-id="6953c-580">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="6953c-580">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-581">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-581">Az.Sql</span></span>
* <span data-ttu-id="6953c-582">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-582">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="6953c-583">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-583">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="6953c-584">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-584">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="6953c-585">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-585">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="6953c-586">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="6953c-586">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-587">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-587">Az.Storage</span></span>
* <span data-ttu-id="6953c-588">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-588">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="6953c-589">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-589">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="6953c-590">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="6953c-590">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="6953c-591">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="6953c-591">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="6953c-592">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="6953c-592">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="6953c-593">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="6953c-593">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="6953c-594">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-594">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="6953c-595">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-595">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="6953c-596">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-596">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="6953c-597">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-597">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="6953c-598">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="6953c-598">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-599">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-599">Az.Websites</span></span>
* <span data-ttu-id="6953c-600">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-600">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="6953c-601">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="6953c-601">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="6953c-602">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-602">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="6953c-603">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="6953c-603">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="6953c-604">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-604">General</span></span>
* <span data-ttu-id="6953c-605">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-605">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-606">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-606">Az.Accounts</span></span>
* <span data-ttu-id="6953c-607">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="6953c-607">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="6953c-608">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="6953c-608">Az.Aks</span></span>
* <span data-ttu-id="6953c-609">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-609">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="6953c-610">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="6953c-610">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="6953c-611">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-611">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-612">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="6953c-612">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="6953c-613">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="6953c-613">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="6953c-614">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-614">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="6953c-615">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="6953c-615">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="6953c-616">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-616">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="6953c-617">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-617">Az.Batch</span></span>
* <span data-ttu-id="6953c-618">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-618">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6953c-619">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-619">Az.Cdn</span></span>
* <span data-ttu-id="6953c-620">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-620">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-621">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-621">Az.Compute</span></span>
* <span data-ttu-id="6953c-622">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-622">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="6953c-623">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-623">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="6953c-624">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-624">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="6953c-625">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-625">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="6953c-626">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="6953c-626">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="6953c-627">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="6953c-627">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="6953c-628">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-628">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="6953c-629">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-629">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-630">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-630">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-631">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-631">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="6953c-632">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-632">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="6953c-633">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="6953c-633">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="6953c-634">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-634">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-635">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-635">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-636">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-636">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-637">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-637">Az.EventHub</span></span>
* <span data-ttu-id="6953c-638">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="6953c-638">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="6953c-639">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="6953c-639">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="6953c-640">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-640">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="6953c-641">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="6953c-641">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="6953c-642">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="6953c-642">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="6953c-643">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-643">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-644">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-644">Az.Monitor</span></span>
* <span data-ttu-id="6953c-645">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-645">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-646">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-646">Az.Network</span></span>
* <span data-ttu-id="6953c-647">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-647">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="6953c-648">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-648">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="6953c-649">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-649">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="6953c-650">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-650">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="6953c-651">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="6953c-651">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="6953c-652">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-652">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="6953c-653">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-653">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-654">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-654">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-655">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-655">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="6953c-656">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-656">Added example</span></span>
    - <span data-ttu-id="6953c-657">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-657">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="6953c-658">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-658">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="6953c-659">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-659">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-660">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-660">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-661">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-661">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-662">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-662">Az.Resources</span></span>
* <span data-ttu-id="6953c-663">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-663">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="6953c-664">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-664">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="6953c-665">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="6953c-665">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="6953c-666">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-666">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-667">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-667">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-668">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="6953c-668">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="6953c-669">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="6953c-669">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="6953c-670">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-670">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-671">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-671">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-672">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-672">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="6953c-673">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="6953c-673">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="6953c-674">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="6953c-674">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="6953c-675">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-675">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="6953c-676">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="6953c-676">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="6953c-677">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-677">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-678">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-678">Az.Sql</span></span>
* <span data-ttu-id="6953c-679">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-679">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-680">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-680">Az.Storage</span></span>
* <span data-ttu-id="6953c-681">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-681">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="6953c-682">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-682">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="6953c-683">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="6953c-683">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="6953c-684">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="6953c-684">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="6953c-685">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-685">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="6953c-686">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="6953c-686">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-687">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-687">Az.Websites</span></span>
* <span data-ttu-id="6953c-688">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-688">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="6953c-689">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="6953c-689">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-690">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-690">Az.Accounts</span></span>
* <span data-ttu-id="6953c-691">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-691">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="6953c-692">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-692">Az.ApplicationInsights</span></span>
* <span data-ttu-id="6953c-693">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-693">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="6953c-694">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-694">Az.Automation</span></span>
* <span data-ttu-id="6953c-695">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-695">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-696">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-696">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-697">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-697">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-698">Az.Compute</span></span>
* <span data-ttu-id="6953c-699">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-699">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="6953c-700">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="6953c-700">Az.ContainerRegistry</span></span>
* <span data-ttu-id="6953c-701">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-701">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="6953c-702">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="6953c-702">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-703">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-703">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-704">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-704">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="6953c-705">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-705">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-706">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-706">Az.EventHub</span></span>
* <span data-ttu-id="6953c-707">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="6953c-707">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="6953c-708">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-708">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-709">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-709">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-710">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-710">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6953c-711">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6953c-711">Az.LogicApp</span></span>
* <span data-ttu-id="6953c-712">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-712">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="6953c-713">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-713">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="6953c-714">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="6953c-714">Az.ManagedServices</span></span>
* <span data-ttu-id="6953c-715">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-715">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-716">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-716">Az.Network</span></span>
* <span data-ttu-id="6953c-717">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-717">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="6953c-718">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-718">New cmdlets</span></span>
        - <span data-ttu-id="6953c-719">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="6953c-719">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="6953c-720">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="6953c-720">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="6953c-721">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-721">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-722">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-722">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-723">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-723">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-724">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-724">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="6953c-725">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="6953c-725">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="6953c-726">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="6953c-726">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="6953c-727">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="6953c-727">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="6953c-728">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-728">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="6953c-729">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-729">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="6953c-730">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-730">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="6953c-731">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="6953c-731">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="6953c-732">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-732">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="6953c-733">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-733">Updated cmdlets</span></span>
        - <span data-ttu-id="6953c-734">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-734">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="6953c-735">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-735">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="6953c-736">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-736">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="6953c-737">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-737">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="6953c-738">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-738">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="6953c-739">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-739">Updated cmdlet:</span></span>
        - <span data-ttu-id="6953c-740">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-740">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="6953c-741">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-741">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="6953c-742">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-742">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="6953c-743">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="6953c-743">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="6953c-744">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-744">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="6953c-745">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6953c-745">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-746">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-746">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-747">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-747">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="6953c-748">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-748">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-749">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-749">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-750">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-750">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="6953c-751">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-751">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="6953c-752">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-752">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="6953c-753">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-753">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="6953c-754">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-754">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="6953c-755">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-755">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="6953c-756">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-756">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="6953c-757">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-757">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="6953c-758">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-758">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="6953c-759">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-759">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-760">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-760">Az.Resources</span></span>
- <span data-ttu-id="6953c-761">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-761">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="6953c-762">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-762">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-763">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-763">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-764">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="6953c-764">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="6953c-765">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-765">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-766">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-766">Az.Sql</span></span>
* <span data-ttu-id="6953c-767">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-767">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="6953c-768">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-768">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="6953c-769">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-769">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-770">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-770">Az.Storage</span></span>
* <span data-ttu-id="6953c-771">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-771">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="6953c-772">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="6953c-772">Az.StorageSync</span></span>
* <span data-ttu-id="6953c-773">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-773">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="6953c-774">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-774">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-775">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-775">Az.Websites</span></span>
* <span data-ttu-id="6953c-776">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-776">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="6953c-777">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-777">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="6953c-778">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-778">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="6953c-779">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="6953c-779">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-780">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-780">Az.Accounts</span></span>
* <span data-ttu-id="6953c-781">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="6953c-781">Add support for profile cmdlets</span></span>
* <span data-ttu-id="6953c-782">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="6953c-782">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="6953c-783">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="6953c-783">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="6953c-784">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="6953c-784">Az.Advisor</span></span>
* <span data-ttu-id="6953c-785">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="6953c-785">GA release of Az.Advisor</span></span>
* <span data-ttu-id="6953c-786">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-786">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="6953c-787">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-787">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-788">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="6953c-788">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="6953c-789">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="6953c-789">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="6953c-790">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-790">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="6953c-791">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-791">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="6953c-792">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-792">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="6953c-793">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="6953c-793">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="6953c-794">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-794">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-795">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-795">Az.Automation</span></span>
* <span data-ttu-id="6953c-796">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-796">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-797">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-797">Az.Compute</span></span>
* <span data-ttu-id="6953c-798">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="6953c-798">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-799">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-799">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-800">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="6953c-800">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="6953c-801">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="6953c-801">Az.EventGrid</span></span>
* <span data-ttu-id="6953c-802">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-802">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-803">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-803">Az.IotHub</span></span>
* <span data-ttu-id="6953c-804">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-804">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-805">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-805">Az.Network</span></span>
* <span data-ttu-id="6953c-806">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-806">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="6953c-807">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="6953c-807">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="6953c-808">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-808">Az.PolicyInsights</span></span>
* <span data-ttu-id="6953c-809">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-809">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="6953c-810">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="6953c-810">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-811">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-811">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-812">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-812">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-813">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-813">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-814">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-814">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-815">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-815">Az.Resources</span></span>
    - <span data-ttu-id="6953c-816">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-816">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="6953c-817">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-817">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="6953c-818">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-818">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="6953c-819">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-819">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-820">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-820">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-821">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="6953c-821">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-822">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-822">Az.Sql</span></span>
* <span data-ttu-id="6953c-823">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-823">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="6953c-824">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-824">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="6953c-825">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-825">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="6953c-826">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-826">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="6953c-827">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-827">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="6953c-828">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-828">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="6953c-829">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-829">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="6953c-830">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="6953c-830">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="6953c-831">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-831">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-832">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-832">Az.Storage</span></span>
* <span data-ttu-id="6953c-833">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-833">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="6953c-834">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="6953c-834">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="6953c-835">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-835">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="6953c-836">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="6953c-836">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="6953c-837">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-837">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="6953c-838">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-838">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="6953c-839">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-839">Set-AzStorageAccount</span></span>
* <span data-ttu-id="6953c-840">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-840">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="6953c-841">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="6953c-841">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="6953c-842">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="6953c-842">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="6953c-843">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="6953c-843">Az.StorageSync</span></span>
* <span data-ttu-id="6953c-844">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-844">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="6953c-845">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="6953c-845">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-846">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-846">Az.Accounts</span></span>
* <span data-ttu-id="6953c-847">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-847">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="6953c-848">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="6953c-848">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="6953c-849">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-849">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="6953c-850">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="6953c-850">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="6953c-851">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="6953c-851">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-852">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-852">Az.Compute</span></span>
* <span data-ttu-id="6953c-853">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-853">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="6953c-854">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-854">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="6953c-855">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="6953c-855">Az.Dns</span></span>
* <span data-ttu-id="6953c-856">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-856">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="6953c-857">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="6953c-857">Az.EventGrid</span></span>
* <span data-ttu-id="6953c-858">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-858">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="6953c-859">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-859">New cmdlets:</span></span>
    - <span data-ttu-id="6953c-860">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="6953c-860">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="6953c-861">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="6953c-861">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="6953c-862">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="6953c-862">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="6953c-863">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6953c-863">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="6953c-864">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="6953c-864">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="6953c-865">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="6953c-865">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="6953c-866">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="6953c-866">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="6953c-867">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="6953c-867">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="6953c-868">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="6953c-868">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="6953c-869">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="6953c-869">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="6953c-870">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="6953c-870">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="6953c-871">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="6953c-871">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="6953c-872">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="6953c-872">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="6953c-873">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6953c-873">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="6953c-874">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="6953c-874">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="6953c-875">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="6953c-875">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="6953c-876">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-876">Updated cmdlets:</span></span>
    - <span data-ttu-id="6953c-877">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="6953c-877">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="6953c-878">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-878">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="6953c-879">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-879">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="6953c-880">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="6953c-880">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="6953c-881">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="6953c-881">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="6953c-882">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="6953c-882">Event subscription expiration date,</span></span>
            - <span data-ttu-id="6953c-883">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="6953c-883">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="6953c-884">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-884">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="6953c-885">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="6953c-885">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="6953c-886">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="6953c-886">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="6953c-887">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-887">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="6953c-888">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="6953c-888">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="6953c-889">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-889">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="6953c-890">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-890">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="6953c-891">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-891">Az.FrontDoor</span></span>
* <span data-ttu-id="6953c-892">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="6953c-892">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="6953c-893">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-893">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="6953c-894">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="6953c-894">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="6953c-895">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-895">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-896">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-896">Az.Network</span></span>
* <span data-ttu-id="6953c-897">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-897">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="6953c-898">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-898">New cmdlets</span></span>
        - <span data-ttu-id="6953c-899">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="6953c-899">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="6953c-900">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-900">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="6953c-901">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-901">New cmdlets</span></span> 
        - <span data-ttu-id="6953c-902">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="6953c-902">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="6953c-903">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-903">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="6953c-904">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-904">New cmdlets</span></span> 
        - <span data-ttu-id="6953c-905">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="6953c-905">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="6953c-906">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="6953c-906">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="6953c-907">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="6953c-907">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="6953c-908">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-908">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="6953c-909">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-909">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="6953c-910">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-910">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="6953c-911">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-911">New cmdlets</span></span>
        - <span data-ttu-id="6953c-912">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="6953c-912">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="6953c-913">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="6953c-913">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="6953c-914">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="6953c-914">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="6953c-915">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="6953c-915">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="6953c-916">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="6953c-916">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="6953c-917">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-917">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="6953c-918">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-918">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="6953c-919">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-919">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="6953c-920">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-920">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="6953c-921">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-921">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="6953c-922">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-922">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="6953c-923">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-923">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="6953c-924">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-924">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="6953c-925">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-925">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="6953c-926">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-926">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="6953c-927">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-927">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="6953c-928">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-928">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="6953c-929">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-929">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="6953c-930">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="6953c-930">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="6953c-931">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-931">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="6953c-932">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-932">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="6953c-933">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="6953c-933">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="6953c-934">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="6953c-934">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="6953c-935">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-935">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="6953c-936">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-936">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="6953c-937">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-937">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="6953c-938">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-938">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-939">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-939">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-940">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="6953c-940">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-941">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-941">Az.Resources</span></span>
* <span data-ttu-id="6953c-942">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="6953c-942">Support for additional Template Export options</span></span>
    - <span data-ttu-id="6953c-943">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-943">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="6953c-944">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-944">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="6953c-945">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-945">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-946">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-946">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-947">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-947">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-948">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-948">Az.Sql</span></span>
* <span data-ttu-id="6953c-949">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-949">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="6953c-950">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-950">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="6953c-951">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="6953c-951">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="6953c-952">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="6953c-952">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="6953c-953">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="6953c-953">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="6953c-954">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="6953c-954">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="6953c-955">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="6953c-955">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="6953c-956">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="6953c-956">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-957">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-957">Az.Storage</span></span>
* <span data-ttu-id="6953c-958">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-958">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="6953c-959">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-959">New-AzStorageAccount</span></span>
* <span data-ttu-id="6953c-960">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="6953c-960">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="6953c-961">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-961">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-962">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-962">Az.Websites</span></span>
* <span data-ttu-id="6953c-963">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="6953c-963">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="6953c-964">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-964">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="6953c-965">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="6953c-965">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="6953c-966">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-966">Az.Cdn</span></span>
* <span data-ttu-id="6953c-967">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-967">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-968">Az.Compute</span></span>
* <span data-ttu-id="6953c-969">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-969">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="6953c-970">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="6953c-970">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-971">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-971">Az.EventHub</span></span>
* <span data-ttu-id="6953c-972">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-972">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="6953c-973">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-973">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-974">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-974">Az.Network</span></span>
* <span data-ttu-id="6953c-975">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-975">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="6953c-976">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-976">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="6953c-977">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-977">Az.PolicyInsights</span></span>
* <span data-ttu-id="6953c-978">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-978">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-979">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-979">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-980">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-980">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-981">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-981">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-982">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-982">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-983">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-983">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-984">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-984">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="6953c-985">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-985">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-986">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-986">Az.Sql</span></span>
* <span data-ttu-id="6953c-987">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-987">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="6953c-988">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="6953c-988">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="6953c-989">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-989">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="6953c-990">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-990">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-991">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-991">Az.Websites</span></span>
* <span data-ttu-id="6953c-992">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-992">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="6953c-993">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="6953c-993">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="6953c-994">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-994">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-995">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="6953c-995">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="6953c-996">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-996">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="6953c-997">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-997">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="6953c-998">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-998">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="6953c-999">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="6953c-999">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="6953c-1000">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-1000">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="6953c-1001">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-1001">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="6953c-1002">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-1002">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="6953c-1003">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1003">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="6953c-1004">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-1004">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="6953c-1005">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-1005">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="6953c-1006">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-1006">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="6953c-1007">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-1007">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="6953c-1008">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1008">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="6953c-1009">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="6953c-1009">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="6953c-1010">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-1010">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="6953c-1011">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="6953c-1011">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="6953c-1012">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="6953c-1012">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="6953c-1013">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1013">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="6953c-1014">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="6953c-1014">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="6953c-1015">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1015">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="6953c-1016">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1016">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="6953c-1017">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="6953c-1017">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="6953c-1018">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1018">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="6953c-1019">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1019">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="6953c-1020">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1020">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="6953c-1021">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1021">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="6953c-1022">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1022">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="6953c-1023">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1023">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="6953c-1024">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1024">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="6953c-1025">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1025">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="6953c-1026">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="6953c-1026">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="6953c-1027">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1027">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="6953c-1028">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1028">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="6953c-1029">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="6953c-1029">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="6953c-1030">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="6953c-1030">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="6953c-1031">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="6953c-1031">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="6953c-1032">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1032">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="6953c-1033">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1033">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="6953c-1034">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1034">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="6953c-1035">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="6953c-1035">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="6953c-1036">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="6953c-1036">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="6953c-1037">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="6953c-1037">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="6953c-1038">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1038">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="6953c-1039">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1039">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="6953c-1040">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="6953c-1040">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="6953c-1041">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="6953c-1041">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="6953c-1042">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1042">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="6953c-1043">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1043">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="6953c-1044">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="6953c-1044">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="6953c-1045">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="6953c-1045">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="6953c-1046">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="6953c-1046">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="6953c-1047">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="6953c-1047">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="6953c-1048">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1048">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="6953c-1049">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="6953c-1049">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="6953c-1050">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="6953c-1050">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="6953c-1051">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1051">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="6953c-1052">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="6953c-1052">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="6953c-1053">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="6953c-1053">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="6953c-1054">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1054">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="6953c-1055">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1055">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="6953c-1056">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="6953c-1056">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="6953c-1057">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="6953c-1057">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="6953c-1058">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1058">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="6953c-1059">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1059">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="6953c-1060">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="6953c-1060">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="6953c-1061">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="6953c-1061">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="6953c-1062">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="6953c-1062">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="6953c-1063">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="6953c-1063">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="6953c-1064">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="6953c-1064">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="6953c-1065">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="6953c-1065">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="6953c-1066">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="6953c-1066">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="6953c-1067">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="6953c-1067">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="6953c-1068">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="6953c-1068">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="6953c-1069">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="6953c-1069">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="6953c-1070">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="6953c-1070">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="6953c-1071">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="6953c-1071">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1072">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1072">Az.Automation</span></span>
* <span data-ttu-id="6953c-1073">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1073">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="6953c-1074">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="6953c-1074">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="6953c-1075">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="6953c-1075">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="6953c-1076">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1076">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="6953c-1077">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="6953c-1077">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="6953c-1078">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1078">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="6953c-1079">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1079">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1080">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1080">Az.Compute</span></span>
* <span data-ttu-id="6953c-1081">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1081">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="6953c-1082">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-1082">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1083">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1083">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1084">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1084">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-1085">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-1085">Az.Monitor</span></span>
* <span data-ttu-id="6953c-1086">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1086">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1087">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1087">Az.Network</span></span>
* <span data-ttu-id="6953c-1088">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1088">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="6953c-1089">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="6953c-1089">Updated cmdlet:</span></span>
        - <span data-ttu-id="6953c-1090">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-1090">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="6953c-1091">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1091">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1092">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1092">Az.Resources</span></span>
* <span data-ttu-id="6953c-1093">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1093">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1094">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1094">Az.Sql</span></span>
* <span data-ttu-id="6953c-1095">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-1095">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="6953c-1096">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1096">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1097">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1097">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1098">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1098">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-1099">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1099">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-1100">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1100">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="6953c-1101">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1101">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1102">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1102">Az.Compute</span></span>
* <span data-ttu-id="6953c-1103">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="6953c-1103">Proximity placement group feature.</span></span>
    - <span data-ttu-id="6953c-1104">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-1104">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="6953c-1105">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-1105">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="6953c-1106">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1106">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="6953c-1107">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1107">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="6953c-1108">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1108">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="6953c-1109">重大な変更</span><span class="sxs-lookup"><span data-stu-id="6953c-1109">Breaking changes</span></span>
    - <span data-ttu-id="6953c-1110">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="6953c-1110">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="6953c-1111">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="6953c-1111">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="6953c-1112">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="6953c-1112">Az.DeploymentManager</span></span>
* <span data-ttu-id="6953c-1113">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1113">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="6953c-1114">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="6953c-1114">Az.Dns</span></span>
* <span data-ttu-id="6953c-1115">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="6953c-1115">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="6953c-1116">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1116">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="6953c-1117">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1117">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="6953c-1118">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-1118">Az.FrontDoor</span></span>
* <span data-ttu-id="6953c-1119">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1119">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="6953c-1120">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="6953c-1120">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="6953c-1121">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="6953c-1121">Az.HDInsight</span></span>
* <span data-ttu-id="6953c-1122">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1122">Removed two cmdlets:</span></span>
    - <span data-ttu-id="6953c-1123">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="6953c-1123">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="6953c-1124">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="6953c-1124">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="6953c-1125">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1125">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="6953c-1126">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1126">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="6953c-1127">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1127">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="6953c-1128">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="6953c-1128">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-1129">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-1129">Az.Monitor</span></span>
* <span data-ttu-id="6953c-1130">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="6953c-1130">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="6953c-1131">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="6953c-1131">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="6953c-1132">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="6953c-1132">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="6953c-1133">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="6953c-1133">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="6953c-1134">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="6953c-1134">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="6953c-1135">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="6953c-1135">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="6953c-1136">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="6953c-1136">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="6953c-1137">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1137">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="6953c-1138">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1138">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="6953c-1139">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1139">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="6953c-1140">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1140">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="6953c-1141">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1141">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="6953c-1142">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="6953c-1142">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="6953c-1143">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1143">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1144">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1144">Az.Network</span></span>
* <span data-ttu-id="6953c-1145">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1145">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="6953c-1146">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1146">New cmdlets</span></span>
        - <span data-ttu-id="6953c-1147">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="6953c-1147">New-AzNatGateway</span></span>
        - <span data-ttu-id="6953c-1148">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="6953c-1148">Get-AzNatGateway</span></span>
        - <span data-ttu-id="6953c-1149">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="6953c-1149">Set-AzNatGateway</span></span>
        - <span data-ttu-id="6953c-1150">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="6953c-1150">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="6953c-1151">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1151">Updated cmdlets</span></span>
        - <span data-ttu-id="6953c-1152">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="6953c-1152">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="6953c-1153">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="6953c-1153">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="6953c-1154">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="6953c-1154">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="6953c-1155">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1155">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="6953c-1156">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1156">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="6953c-1157">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-1157">Az.PolicyInsights</span></span>
* <span data-ttu-id="6953c-1158">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-1158">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="6953c-1159">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1159">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="6953c-1160">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1160">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1161">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-1162">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-1162">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="6953c-1163">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="6953c-1163">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="6953c-1164">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="6953c-1164">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="6953c-1165">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="6953c-1165">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="6953c-1166">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="6953c-1166">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="6953c-1167">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="6953c-1167">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="6953c-1168">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="6953c-1168">Az.Relay</span></span>
* <span data-ttu-id="6953c-1169">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1169">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-1170">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-1170">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-1171">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1171">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1172">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1172">Az.Storage</span></span>
* <span data-ttu-id="6953c-1173">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="6953c-1173">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="6953c-1174">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1174">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="6953c-1175">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1175">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="6953c-1176">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-1176">New-AzStorageAccount</span></span>
* <span data-ttu-id="6953c-1177">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="6953c-1177">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="6953c-1178">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-1178">New-AzStorageAccount</span></span>
    - <span data-ttu-id="6953c-1179">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-1179">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="6953c-1180">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6953c-1180">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1181">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1181">Az.Websites</span></span>
* <span data-ttu-id="6953c-1182">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="6953c-1182">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="6953c-1183">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="6953c-1183">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="6953c-1184">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1184">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="6953c-1185">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="6953c-1185">Highlights since the last major release</span></span>
* <span data-ttu-id="6953c-1186">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="6953c-1186">General availability of `Az` module</span></span>
* <span data-ttu-id="6953c-1187">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="6953c-1187">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="6953c-1188">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="6953c-1188">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="6953c-1189">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1189">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="6953c-1190">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1190">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="6953c-1191">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1191">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="6953c-1192">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1192">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-1193">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1193">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1194">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1194">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="6953c-1195">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-1195">Az.Batch</span></span>
* <span data-ttu-id="6953c-1196">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1196">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6953c-1197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-1197">Az.Cdn</span></span>
* <span data-ttu-id="6953c-1198">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1198">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-1199">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1199">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-1200">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1200">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1201">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1201">Az.Compute</span></span>
* <span data-ttu-id="6953c-1202">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1202">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="6953c-1203">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1204">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1204">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-1205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-1205">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-1206">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1206">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1207">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1207">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1208">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="6953c-1209">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="6953c-1209">Az.EventGrid</span></span>
* <span data-ttu-id="6953c-1210">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1210">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-1211">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-1211">Az.EventHub</span></span>
* <span data-ttu-id="6953c-1212">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1212">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="6953c-1213">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="6953c-1213">Az.HDInsight</span></span>
* <span data-ttu-id="6953c-1214">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1214">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-1215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-1215">Az.IotHub</span></span>
* <span data-ttu-id="6953c-1216">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1216">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-1217">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-1217">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-1218">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1218">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1219">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1219">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="6953c-1220">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="6953c-1220">Az.MachineLearning</span></span>
* <span data-ttu-id="6953c-1221">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="6953c-1222">Az.Media</span><span class="sxs-lookup"><span data-stu-id="6953c-1222">Az.Media</span></span>
* <span data-ttu-id="6953c-1223">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-1224">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-1224">Az.Monitor</span></span>
  * <span data-ttu-id="6953c-1225">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1225">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="6953c-1226">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="6953c-1226">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="6953c-1227">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="6953c-1227">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="6953c-1228">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="6953c-1228">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="6953c-1229">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="6953c-1229">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="6953c-1230">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="6953c-1230">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="6953c-1231">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1231">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1232">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1232">Az.Network</span></span>
* <span data-ttu-id="6953c-1233">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1233">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1234">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1234">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="6953c-1235">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="6953c-1235">Az.NotificationHubs</span></span>
* <span data-ttu-id="6953c-1236">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1236">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-1237">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-1237">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-1238">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="6953c-1239">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="6953c-1239">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="6953c-1240">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1240">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1241">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1241">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-1242">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1242">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1243">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1243">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="6953c-1244">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1244">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="6953c-1245">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1245">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="6953c-1246">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="6953c-1246">Az.RedisCache</span></span>
* <span data-ttu-id="6953c-1247">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1248">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1248">Az.Resources</span></span>
* <span data-ttu-id="6953c-1249">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1249">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1250">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1250">Az.Sql</span></span>
* <span data-ttu-id="6953c-1251">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="6953c-1251">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="6953c-1252">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1253">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1253">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="6953c-1254">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1254">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="6953c-1255">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="6953c-1255">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="6953c-1256">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="6953c-1256">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="6953c-1257">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1257">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1258">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1258">Az.Websites</span></span>
* <span data-ttu-id="6953c-1259">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1259">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="6953c-1260">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1260">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="6953c-1261">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1261">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="6953c-1262">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1262">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="6953c-1263">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1263">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="6953c-1264">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="6953c-1264">Highlights since the last major release</span></span>
* <span data-ttu-id="6953c-1265">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="6953c-1265">General availability of `Az` module</span></span>
* <span data-ttu-id="6953c-1266">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="6953c-1266">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="6953c-1267">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="6953c-1267">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="6953c-1268">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1268">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="6953c-1269">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1269">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="6953c-1270">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1270">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="6953c-1271">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1271">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="6953c-1272">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1272">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1273">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1273">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="6953c-1274">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1274">Az.AnalysisServices</span></span>
* <span data-ttu-id="6953c-1275">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="6953c-1275">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="6953c-1276">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1276">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1277">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1277">Az.Automation</span></span>
* <span data-ttu-id="6953c-1278">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1278">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="6953c-1279">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1279">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="6953c-1280">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1280">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1281">Az.Compute</span></span>
* <span data-ttu-id="6953c-1282">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1282">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="6953c-1283">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1283">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="6953c-1284">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1284">Az.ContainerInstance</span></span>
* <span data-ttu-id="6953c-1285">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1285">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-1286">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-1286">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-1287">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1287">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="6953c-1288">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1288">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1289">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1289">Az.Resources</span></span>
* <span data-ttu-id="6953c-1290">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1290">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="6953c-1291">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1291">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="6953c-1292">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="6953c-1292">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="6953c-1293">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="6953c-1293">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="6953c-1294">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1294">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="6953c-1295">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="6953c-1295">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1296">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1296">Az.Sql</span></span>
* <span data-ttu-id="6953c-1297">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1297">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1298">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1298">Az.Storage</span></span>
* <span data-ttu-id="6953c-1299">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="6953c-1299">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="6953c-1300">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="6953c-1300">New-AzStorageContext</span></span>
* <span data-ttu-id="6953c-1301">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="6953c-1301">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="6953c-1302">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="6953c-1302">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="6953c-1303">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="6953c-1303">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="6953c-1304">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-1304">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="6953c-1305">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-1305">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="6953c-1306">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="6953c-1306">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="6953c-1307">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="6953c-1307">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="6953c-1308">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="6953c-1308">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="6953c-1309">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="6953c-1309">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="6953c-1310">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="6953c-1310">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="6953c-1311">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1311">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="6953c-1312">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="6953c-1312">Highlights since the last major release</span></span>
* <span data-ttu-id="6953c-1313">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="6953c-1313">General availability of `Az` module</span></span>
* <span data-ttu-id="6953c-1314">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="6953c-1314">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="6953c-1315">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="6953c-1315">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="6953c-1316">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1316">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="6953c-1317">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1317">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="6953c-1318">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1318">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="6953c-1319">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1319">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1320">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1320">Az.Automation</span></span>
* <span data-ttu-id="6953c-1321">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1321">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="6953c-1322">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="6953c-1322">Dynamic grouping</span></span>
    * <span data-ttu-id="6953c-1323">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="6953c-1323">Pre-Post script</span></span>
    * <span data-ttu-id="6953c-1324">再起動設定</span><span class="sxs-lookup"><span data-stu-id="6953c-1324">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1325">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1325">Az.Compute</span></span>
* <span data-ttu-id="6953c-1326">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1326">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="6953c-1327">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1327">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-1328">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-1328">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-1329">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1329">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1330">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1330">Az.Network</span></span>
* <span data-ttu-id="6953c-1331">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1331">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="6953c-1332">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1332">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1333">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1333">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-1334">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1334">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="6953c-1335">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1335">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1336">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1336">Az.Resources</span></span>
* <span data-ttu-id="6953c-1337">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1337">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="6953c-1338">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1338">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1339">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1339">Az.Sql</span></span>
* <span data-ttu-id="6953c-1340">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1340">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1341">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1341">Az.Storage</span></span>
* <span data-ttu-id="6953c-1342">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-1342">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="6953c-1343">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-1343">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="6953c-1344">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-1344">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="6953c-1345">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="6953c-1345">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="6953c-1346">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="6953c-1346">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="6953c-1347">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="6953c-1347">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="6953c-1348">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1348">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1349">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1349">Az.Websites</span></span>
* <span data-ttu-id="6953c-1350">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1350">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="6953c-1351">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1351">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1352">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1352">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1353">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1353">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="6953c-1354">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1354">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1355">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1355">Az.Automation</span></span>
* <span data-ttu-id="6953c-1356">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1356">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="6953c-1357">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1357">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="6953c-1358">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="6953c-1358">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6953c-1359">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-1359">Az.Cdn</span></span>
* <span data-ttu-id="6953c-1360">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-1360">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1361">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1361">Az.Compute</span></span>
* <span data-ttu-id="6953c-1362">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1362">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-1363">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-1363">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-1364">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1364">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6953c-1365">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6953c-1365">Az.LogicApp</span></span>
* <span data-ttu-id="6953c-1366">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1366">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1367">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1367">Az.Network</span></span>
* <span data-ttu-id="6953c-1368">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1368">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1369">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-1370">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1370">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="6953c-1371">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1371">SDK Update</span></span>
* <span data-ttu-id="6953c-1372">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1372">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="6953c-1373">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1373">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1374">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1374">Az.Resources</span></span>
* <span data-ttu-id="6953c-1375">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1375">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="6953c-1376">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="6953c-1376">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="6953c-1377">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1377">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="6953c-1378">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="6953c-1378">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="6953c-1379">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1379">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="6953c-1380">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="6953c-1380">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1381">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1381">Az.Sql</span></span>
* <span data-ttu-id="6953c-1382">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1382">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="6953c-1383">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1383">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1384">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1384">Az.Storage</span></span>
* <span data-ttu-id="6953c-1385">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="6953c-1385">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="6953c-1386">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1386">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="6953c-1387">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1387">Az.AnalysisServices</span></span>
* <span data-ttu-id="6953c-1388">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-1388">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1389">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1389">Az.Automation</span></span>
* <span data-ttu-id="6953c-1390">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1390">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="6953c-1391">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1391">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="6953c-1392">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1392">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-1393">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1393">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-1394">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1394">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1395">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1395">Az.Compute</span></span>
* <span data-ttu-id="6953c-1396">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1396">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="6953c-1397">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1397">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="6953c-1398">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1398">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="6953c-1399">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1399">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1400">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1400">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1401">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1401">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6953c-1402">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6953c-1402">Az.EventHub</span></span>
* <span data-ttu-id="6953c-1403">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1403">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-1404">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-1404">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-1405">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1405">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6953c-1406">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6953c-1406">Az.LogicApp</span></span>
* <span data-ttu-id="6953c-1407">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1407">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="6953c-1408">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1408">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="6953c-1409">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1409">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="6953c-1410">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6953c-1410">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6953c-1411">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6953c-1411">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6953c-1412">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6953c-1412">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6953c-1413">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6953c-1413">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="6953c-1414">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1414">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="6953c-1415">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6953c-1415">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6953c-1416">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6953c-1416">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6953c-1417">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6953c-1417">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6953c-1418">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6953c-1418">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="6953c-1419">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1419">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6953c-1420">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-1420">Az.Monitor</span></span>
* <span data-ttu-id="6953c-1421">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1421">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1422">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1422">Az.Network</span></span>
* <span data-ttu-id="6953c-1423">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1423">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-1424">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-1424">Az.OperationalInsights</span></span>
* <span data-ttu-id="6953c-1425">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1425">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="6953c-1426">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1426">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="6953c-1427">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1427">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="6953c-1428">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1428">Az.Resources</span></span>
* <span data-ttu-id="6953c-1429">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="6953c-1429">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="6953c-1430">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="6953c-1430">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="6953c-1431">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="6953c-1431">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="6953c-1432">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1432">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1433">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1433">Az.Sql</span></span>
* <span data-ttu-id="6953c-1434">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1434">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="6953c-1435">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1435">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1436">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1436">Az.Websites</span></span>
* <span data-ttu-id="6953c-1437">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1437">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="6953c-1438">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1438">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1439">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1439">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1440">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1440">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="6953c-1441">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1441">Az.AnalysisServices</span></span>
<span data-ttu-id="6953c-1442">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="6953c-1442">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1443">Az.Compute</span></span>
* <span data-ttu-id="6953c-1444">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1444">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="6953c-1445">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1445">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="6953c-1446">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1446">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1447">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1447">Az.RecoveryServices</span></span>
<span data-ttu-id="6953c-1448">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="6953c-1448">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1449">Az.Resources</span></span>
* <span data-ttu-id="6953c-1450">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1450">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="6953c-1451">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="6953c-1451">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="6953c-1452">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1452">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="6953c-1453">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="6953c-1453">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1454">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1454">Az.Sql</span></span>
* <span data-ttu-id="6953c-1455">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1455">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="6953c-1456">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1456">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="6953c-1457">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1457">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="6953c-1458">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1458">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1459">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1459">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1460">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1460">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="6953c-1461">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1461">Az.AnalysisServices</span></span>
* <span data-ttu-id="6953c-1462">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1462">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1463">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1463">Az.RecoveryServices</span></span>
* <span data-ttu-id="6953c-1464">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1464">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="6953c-1465">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1465">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1466">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1467">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1467">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="6953c-1468">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1468">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6953c-1469">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1469">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="6953c-1470">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="6953c-1470">Az.Aks</span></span>
* <span data-ttu-id="6953c-1471">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1471">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6953c-1472">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1472">Az.Automation</span></span>
* <span data-ttu-id="6953c-1473">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1473">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="6953c-1474">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1474">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6953c-1475">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6953c-1475">Az.Cdn</span></span>
* <span data-ttu-id="6953c-1476">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1476">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1477">Az.Compute</span></span>
* <span data-ttu-id="6953c-1478">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1478">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="6953c-1479">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1479">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="6953c-1480">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1480">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="6953c-1481">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="6953c-1481">Az.ContainerRegistry</span></span>
* <span data-ttu-id="6953c-1482">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1482">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6953c-1483">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6953c-1483">Az.DataFactory</span></span>
* <span data-ttu-id="6953c-1484">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1484">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1485">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1485">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1486">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="6953c-1486">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="6953c-1487">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="6953c-1487">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="6953c-1488">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1488">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-1489">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-1489">Az.IotHub</span></span>
* <span data-ttu-id="6953c-1490">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1490">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6953c-1491">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-1491">Az.KeyVault</span></span>
* <span data-ttu-id="6953c-1492">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1492">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1493">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1493">Az.Network</span></span>
* <span data-ttu-id="6953c-1494">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1494">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1495">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1495">Az.Resources</span></span>
* <span data-ttu-id="6953c-1496">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1496">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="6953c-1497">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1497">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="6953c-1498">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1498">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="6953c-1499">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="6953c-1499">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="6953c-1500">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="6953c-1500">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="6953c-1501">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1501">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="6953c-1502">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="6953c-1502">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-1503">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-1503">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-1504">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="6953c-1504">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="6953c-1505">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1505">Fix some error messages.</span></span>
* <span data-ttu-id="6953c-1506">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1506">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="6953c-1507">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1507">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="6953c-1508">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="6953c-1508">Az.SignalR</span></span>
* <span data-ttu-id="6953c-1509">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1509">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1510">Az.Sql</span></span>
* <span data-ttu-id="6953c-1511">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1511">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6953c-1512">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1512">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="6953c-1513">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1513">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="6953c-1514">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-1514">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1515">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1515">Az.Storage</span></span>
* <span data-ttu-id="6953c-1516">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6953c-1517">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="6953c-1517">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="6953c-1518">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="6953c-1518">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="6953c-1519">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="6953c-1519">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="6953c-1520">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="6953c-1520">Az.TrafficManager</span></span>
* <span data-ttu-id="6953c-1521">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1521">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1522">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1522">Az.Websites</span></span>
* <span data-ttu-id="6953c-1523">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1523">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6953c-1524">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1524">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="6953c-1525">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="6953c-1525">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="6953c-1526">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1526">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6953c-1527">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1527">Az.Accounts</span></span>
* <span data-ttu-id="6953c-1528">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="6953c-1528">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1529">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1529">Az.Compute</span></span>
* <span data-ttu-id="6953c-1530">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1530">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="6953c-1531">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="6953c-1531">Updated the description of ID in help files</span></span>
* <span data-ttu-id="6953c-1532">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1532">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1533">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1533">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1534">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1534">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="6953c-1535">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1535">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="6953c-1536">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="6953c-1536">Az.EventGrid</span></span>
* <span data-ttu-id="6953c-1537">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1537">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="6953c-1538">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="6953c-1538">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="6953c-1539">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="6953c-1539">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="6953c-1540">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="6953c-1540">Event Time-To-Live,</span></span>
        - <span data-ttu-id="6953c-1541">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="6953c-1541">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="6953c-1542">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="6953c-1542">Dead letter endpoint.</span></span>
    - <span data-ttu-id="6953c-1543">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="6953c-1543">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="6953c-1544">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="6953c-1544">Event Time-To-Live,</span></span>
        - <span data-ttu-id="6953c-1545">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="6953c-1545">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="6953c-1546">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="6953c-1546">Dead letter endpoint.</span></span>
* <span data-ttu-id="6953c-1547">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1547">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="6953c-1548">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1548">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6953c-1549">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6953c-1549">Az.IotHub</span></span>
* <span data-ttu-id="6953c-1550">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1550">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6953c-1551">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6953c-1551">Az.LogicApp</span></span>
* <span data-ttu-id="6953c-1552">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="6953c-1552">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1553">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1553">Az.Resources</span></span>
* <span data-ttu-id="6953c-1554">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1554">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="6953c-1555">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="6953c-1555">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="6953c-1556">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1556">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="6953c-1557">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1557">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="6953c-1558">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="6953c-1558">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="6953c-1559">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="6953c-1559">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="6953c-1560">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="6953c-1560">Az.SignalR</span></span>
* <span data-ttu-id="6953c-1561">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1561">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1562">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1562">Az.Sql</span></span>
* <span data-ttu-id="6953c-1563">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1563">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6953c-1564">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1564">Az.Storage</span></span>
* <span data-ttu-id="6953c-1565">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="6953c-1565">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="6953c-1566">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="6953c-1566">New-AzStorageContext</span></span>
* <span data-ttu-id="6953c-1567">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1567">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="6953c-1568">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="6953c-1568">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1569">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1569">Az.Websites</span></span>
* <span data-ttu-id="6953c-1570">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1570">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="6953c-1571">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1571">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="6953c-1572">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1572">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="6953c-1573">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-1573">General</span></span>

- <span data-ttu-id="6953c-1574">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="6953c-1574">General Availability of Az Module</span></span>
- <span data-ttu-id="6953c-1575">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="6953c-1575">Online help for each module</span></span>
- <span data-ttu-id="6953c-1576">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1576">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="6953c-1577">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1577">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="6953c-1578">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6953c-1578">Az.Accounts</span></span>
- <span data-ttu-id="6953c-1579">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1579">Changed from Az.Profile</span></span>
- <span data-ttu-id="6953c-1580">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1580">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="6953c-1581">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-1581">Az.ApiManagement</span></span>
- <span data-ttu-id="6953c-1582">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="6953c-1582">Fixes for #7002</span></span>
- <span data-ttu-id="6953c-1583">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1583">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="6953c-1584">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6953c-1584">Az.Batch</span></span>
- <span data-ttu-id="6953c-1585">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1585">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="6953c-1586">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1586">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="6953c-1587">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1587">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="6953c-1588">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="6953c-1588">Az.Billing</span></span>
- <span data-ttu-id="6953c-1589">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1589">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="6953c-1590">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1590">Az.CognitivServices</span></span>
- <span data-ttu-id="6953c-1591">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1591">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="6953c-1592">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1592">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="6953c-1593">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1593">Az.ContainerInstance</span></span>
- <span data-ttu-id="6953c-1594">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1594">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="6953c-1595">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="6953c-1595">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="6953c-1596">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1596">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1597">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1597">Az.DataLakeStore</span></span>
- <span data-ttu-id="6953c-1598">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1598">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="6953c-1599">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6953c-1599">Az.Monitor</span></span>
- <span data-ttu-id="6953c-1600">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1600">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="6953c-1601">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6953c-1601">Az.KeyVault</span></span>
- <span data-ttu-id="6953c-1602">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1602">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="6953c-1603">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="6953c-1603">Az.MachineLearning</span></span>
- <span data-ttu-id="6953c-1604">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="6953c-1604">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="6953c-1605">Az.Media</span><span class="sxs-lookup"><span data-stu-id="6953c-1605">Az.Media</span></span>
- <span data-ttu-id="6953c-1606">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1606">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="6953c-1607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1607">Az.Network</span></span>
<span data-ttu-id="6953c-1608">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1608">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="6953c-1609">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-1609">New cmdlets added:</span></span>
        - <span data-ttu-id="6953c-1610">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1610">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1611">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1611">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1612">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1612">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1613">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1613">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1614">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1614">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1615">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1615">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="6953c-1616">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="6953c-1616">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="6953c-1617">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="6953c-1617">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="6953c-1618">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1618">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="6953c-1619">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="6953c-1619">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="6953c-1620">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1620">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="6953c-1621">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="6953c-1621">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="6953c-1622">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-1622">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="6953c-1623">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-1623">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="6953c-1624">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1624">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="6953c-1625">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1625">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="6953c-1626">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6953c-1626">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="6953c-1627">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6953c-1627">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="6953c-1628">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6953c-1628">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="6953c-1629">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1629">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="6953c-1630">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1630">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="6953c-1631">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-1631">Az.OperationalInsights</span></span>
- <span data-ttu-id="6953c-1632">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1632">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="6953c-1633">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6953c-1633">Az.Profile</span></span>
- <span data-ttu-id="6953c-1634">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1634">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1635">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1635">Az.RecoveryServices</span></span>
- <span data-ttu-id="6953c-1636">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1636">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="6953c-1637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1637">Az.Resources</span></span>
- <span data-ttu-id="6953c-1638">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1638">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="6953c-1639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-1639">Az.ServiceFabric</span></span>
- <span data-ttu-id="6953c-1640">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="6953c-1640">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="6953c-1641">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1641">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="6953c-1642">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="6953c-1642">Az.SIgnalR</span></span>
- <span data-ttu-id="6953c-1643">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="6953c-1643">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="6953c-1644">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1644">Az.Sql</span></span>
- <span data-ttu-id="6953c-1645">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1645">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="6953c-1646">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1646">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="6953c-1647">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1647">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="6953c-1648">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1648">Az.Storage</span></span>
- <span data-ttu-id="6953c-1649">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1649">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="6953c-1650">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1650">Az.Websites</span></span>
- <span data-ttu-id="6953c-1651">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6953c-1651">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="6953c-1652">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1652">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="6953c-1653">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-1653">General</span></span>

* <span data-ttu-id="6953c-1654">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="6953c-1654">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="6953c-1655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1655">Az.Compute</span></span>

* <span data-ttu-id="6953c-1656">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1656">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1657">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1657">Az.DataLakeStore</span></span>

* <span data-ttu-id="6953c-1658">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1658">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="6953c-1659">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6953c-1659">Az.FrontDoor</span></span>

* <span data-ttu-id="6953c-1660">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1660">Fixed some broken links</span></span>
    - <span data-ttu-id="6953c-1661">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1661">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="6953c-1662">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1662">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="6953c-1663">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1663">Az.RecoveryServices</span></span>

* <span data-ttu-id="6953c-1664">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1664">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="6953c-1665">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1665">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="6953c-1666">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1666">Az.Resources</span></span>

* <span data-ttu-id="6953c-1667">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1667">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="6953c-1668">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1668">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="6953c-1669">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1669">Az.Sql</span></span>

* <span data-ttu-id="6953c-1670">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="6953c-1670">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="6953c-1671">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1671">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="6953c-1672">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1672">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="6953c-1673">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1673">Az.Storage</span></span>

* <span data-ttu-id="6953c-1674">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1674">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="6953c-1675">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1675">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="6953c-1676">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="6953c-1676">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="6953c-1677">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="6953c-1677">Support Static Website configuration</span></span>
    - <span data-ttu-id="6953c-1678">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="6953c-1678">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="6953c-1679">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="6953c-1679">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="6953c-1680">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1680">Az.Websites</span></span>

* <span data-ttu-id="6953c-1681">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="6953c-1681">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="6953c-1682">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1682">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="6953c-1683">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="6953c-1683">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="6953c-1684">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1684">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="6953c-1685">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6953c-1685">Az.ApiManagement</span></span>
* <span data-ttu-id="6953c-1686">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1686">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="6953c-1687">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6953c-1687">Az.Automation</span></span>
* <span data-ttu-id="6953c-1688">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="6953c-1688">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="6953c-1689">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1689">Added Update Management cmdlets</span></span>
* <span data-ttu-id="6953c-1690">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1690">Added Source Control cmdlets</span></span>
* <span data-ttu-id="6953c-1691">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1691">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="6953c-1692">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1692">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="6953c-1693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1693">Az.Compute</span></span>
* <span data-ttu-id="6953c-1694">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1694">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="6953c-1695">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1695">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="6953c-1696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1696">Az.ContainerInstance</span></span>
* <span data-ttu-id="6953c-1697">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1697">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="6953c-1698">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="6953c-1698">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="6953c-1699">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1699">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="6953c-1700">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1700">Az.Network</span></span>
* <span data-ttu-id="6953c-1701">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1701">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="6953c-1702">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1702">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="6953c-1703">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1703">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="6953c-1704">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1704">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="6953c-1705">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="6953c-1705">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="6953c-1706">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1706">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="6953c-1707">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1707">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="6953c-1708">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="6953c-1708">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="6953c-1709">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1709">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="6953c-1710">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1710">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="6953c-1711">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="6953c-1711">Az.Relay</span></span>
* <span data-ttu-id="6953c-1712">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="6953c-1712">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="6953c-1713">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1713">Az.Resources</span></span>
* <span data-ttu-id="6953c-1714">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1714">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="6953c-1715">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1715">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="6953c-1716">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="6953c-1716">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="6953c-1717">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-1717">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-1718">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1718">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="6953c-1719">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1719">Az.Sql</span></span>
* <span data-ttu-id="6953c-1720">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1720">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="6953c-1721">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1721">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6953c-1722">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1722">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6953c-1723">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1723">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6953c-1724">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6953c-1724">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6953c-1725">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6953c-1725">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6953c-1726">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6953c-1726">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6953c-1727">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6953c-1727">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6953c-1728">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6953c-1728">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="6953c-1729">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="6953c-1729">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="6953c-1730">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1730">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="6953c-1731">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1731">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="6953c-1732">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="6953c-1732">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="6953c-1733">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="6953c-1733">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="6953c-1734">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="6953c-1734">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="6953c-1735">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="6953c-1735">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="6953c-1736">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1736">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="6953c-1737">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1737">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="6953c-1738">全般</span><span class="sxs-lookup"><span data-stu-id="6953c-1738">General</span></span>
* <span data-ttu-id="6953c-1739">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="6953c-1739">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="6953c-1740">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6953c-1740">Az.Profile</span></span>
* <span data-ttu-id="6953c-1741">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1741">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="6953c-1742">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1742">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="6953c-1743">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1743">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="6953c-1744">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1744">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="6953c-1745">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1745">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="6953c-1746">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1746">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="6953c-1747">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1747">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-1748">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1748">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-1749">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1749">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1750">Az.Compute</span></span>
* <span data-ttu-id="6953c-1751">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1751">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="6953c-1752">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="6953c-1752">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="6953c-1753">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1753">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1754">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1754">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1755">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1755">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="6953c-1756">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1756">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="6953c-1757">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="6953c-1757">Az.Insights</span></span>
* <span data-ttu-id="6953c-1758">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1758">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="6953c-1759">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="6953c-1759">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="6953c-1760">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1760">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="6953c-1761">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="6953c-1761">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1762">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1762">Az.Network</span></span>
* <span data-ttu-id="6953c-1763">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="6953c-1763">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="6953c-1764">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-1764">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="6953c-1765">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="6953c-1765">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="6953c-1766">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="6953c-1766">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="6953c-1767">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="6953c-1767">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="6953c-1768">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="6953c-1768">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="6953c-1769">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="6953c-1769">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="6953c-1770">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="6953c-1770">Az.PolicyInsights</span></span>
* <span data-ttu-id="6953c-1771">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1771">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1772">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1772">Az.Resources</span></span>
* <span data-ttu-id="6953c-1773">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1773">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="6953c-1774">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1774">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6953c-1775">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6953c-1775">Az.ServiceBus</span></span>
* <span data-ttu-id="6953c-1776">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1776">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6953c-1777">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6953c-1777">Az.ServiceFabric</span></span>
* <span data-ttu-id="6953c-1778">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1778">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="6953c-1779">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1779">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="6953c-1780">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="6953c-1780">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="6953c-1781">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="6953c-1781">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="6953c-1782">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1782">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="6953c-1783">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1783">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="6953c-1784">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6953c-1784">Az.Profile</span></span>
* <span data-ttu-id="6953c-1785">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1785">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="6953c-1786">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1786">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1787">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1787">Az.Compute</span></span>
* <span data-ttu-id="6953c-1788">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1788">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="6953c-1789">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1789">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6953c-1790">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6953c-1790">Az.DataLakeStore</span></span>
* <span data-ttu-id="6953c-1791">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1791">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="6953c-1792">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1792">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="6953c-1793">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1793">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="6953c-1794">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1794">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="6953c-1795">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="6953c-1795">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1796">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1796">Az.Network</span></span>
* <span data-ttu-id="6953c-1797">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1797">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="6953c-1798">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1798">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1799">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1799">Az.Resources</span></span>
* <span data-ttu-id="6953c-1800">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1800">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="6953c-1801">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1801">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="6953c-1802">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1802">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="6953c-1803">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="6953c-1803">Azure.Storage</span></span>
* <span data-ttu-id="6953c-1804">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1804">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="6953c-1805">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="6953c-1805">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="6953c-1806">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="6953c-1806">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="6953c-1807">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1807">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="6953c-1808">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="6953c-1808">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="6953c-1809">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6953c-1809">Az.CognitiveServices</span></span>
* <span data-ttu-id="6953c-1810">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1810">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6953c-1811">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6953c-1811">Az.Compute</span></span>
* <span data-ttu-id="6953c-1812">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1812">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="6953c-1813">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1813">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="6953c-1814">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1814">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="6953c-1815">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="6953c-1815">Az.DataFactoryV2</span></span>
* <span data-ttu-id="6953c-1816">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1816">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6953c-1817">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6953c-1817">Az.Network</span></span>
* <span data-ttu-id="6953c-1818">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6953c-1818">Added NetworkProfile functionality.</span></span> <span data-ttu-id="6953c-1819">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6953c-1819">new cmdlets added</span></span>
    - <span data-ttu-id="6953c-1820">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6953c-1820">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="6953c-1821">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6953c-1821">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="6953c-1822">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6953c-1822">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="6953c-1823">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6953c-1823">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="6953c-1824">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-1824">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="6953c-1825">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="6953c-1825">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="6953c-1826">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1826">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="6953c-1827">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1827">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="6953c-1828">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1828">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="6953c-1829">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="6953c-1829">Az.RedisCache</span></span>
* <span data-ttu-id="6953c-1830">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="6953c-1830">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="6953c-1831">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1831">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="6953c-1832">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6953c-1832">Az.Resources</span></span>
* <span data-ttu-id="6953c-1833">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1833">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="6953c-1834">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1834">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="6953c-1835">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6953c-1835">Az.Sql</span></span>
* <span data-ttu-id="6953c-1836">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6953c-1836">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6953c-1837">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6953c-1837">Az.Websites</span></span>
* <span data-ttu-id="6953c-1838">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="6953c-1838">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="6953c-1839">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="6953c-1839">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="6953c-1840">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="6953c-1840">0.2.0 - September 2018</span></span>
 <span data-ttu-id="6953c-1841">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="6953c-1841">Initial Release</span></span>

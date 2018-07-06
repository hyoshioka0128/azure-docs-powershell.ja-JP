---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 3811e28dda69d194d23934943fb47d562f869fc4
ms.sourcegitcommit: 5a5b6dd216d5f805204244146cf6f88ad2f34fb4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/19/2018
ms.locfileid: "36237815"
---
# <a name="release-notes"></a><span data-ttu-id="c89c6-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="c89c6-103">Release notes</span></span>

<span data-ttu-id="c89c6-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c89c6-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="630---june-2018"></a><span data-ttu-id="c89c6-105">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="c89c6-105">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c89c6-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c89c6-106">AzureRM.Profile</span></span>
* <span data-ttu-id="c89c6-107">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-107">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="c89c6-108">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="c89c6-108">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="c89c6-109">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c89c6-109">Azure.Storage</span></span>
* <span data-ttu-id="c89c6-110">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-110">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c89c6-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c89c6-111">AzureRM.Compute</span></span>
* <span data-ttu-id="c89c6-112">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-112">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="c89c6-113">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-113">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="c89c6-114">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c89c6-114">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c89c6-115">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c89c6-115">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c89c6-116">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="c89c6-116">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="c89c6-117">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-117">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="c89c6-118">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c89c6-118">Start-AzureRmVM</span></span>
    - <span data-ttu-id="c89c6-119">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c89c6-119">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="c89c6-120">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c89c6-120">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="c89c6-121">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="c89c6-121">Set-AzureRmVM</span></span>
    - <span data-ttu-id="c89c6-122">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="c89c6-122">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="c89c6-123">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c89c6-123">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="c89c6-124">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="c89c6-124">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="c89c6-125">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="c89c6-125">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="c89c6-126">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c89c6-126">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="c89c6-127">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c89c6-127">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="c89c6-128">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c89c6-128">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="c89c6-129">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="c89c6-129">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="c89c6-130">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="c89c6-130">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="c89c6-131">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="c89c6-131">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="c89c6-132">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="c89c6-132">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="c89c6-133">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="c89c6-133">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="c89c6-134">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="c89c6-134">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="c89c6-135">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="c89c6-135">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="c89c6-136">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="c89c6-136">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="c89c6-137">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c89c6-137">AzureRM.EventGrid</span></span>
* <span data-ttu-id="c89c6-138">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-138">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="c89c6-139">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c89c6-139">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c89c6-140">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-140">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="c89c6-141">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c89c6-141">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="c89c6-142">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="c89c6-142">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="c89c6-143">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="c89c6-143">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="c89c6-144">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-144">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="c89c6-145">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c89c6-145">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c89c6-146">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-146">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="c89c6-147">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットが上書きされます。</span><span class="sxs-lookup"><span data-stu-id="c89c6-147">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c89c6-148">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c89c6-148">AzureRM.Sql</span></span>
* <span data-ttu-id="c89c6-149">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-149">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c89c6-150">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c89c6-150">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c89c6-151">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-151">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c89c6-152">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c89c6-152">AzureRM.Websites</span></span>
* <span data-ttu-id="c89c6-153">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="c89c6-153">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="c89c6-154">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="c89c6-154">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="c89c6-155">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="c89c6-155">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="c89c6-156">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c89c6-156">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="c89c6-157">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-157">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="c89c6-158">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="c89c6-158">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c89c6-159">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c89c6-159">AzureRM.Profile</span></span>
* <span data-ttu-id="c89c6-160">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-160">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="c89c6-161">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="c89c6-161">AzureRM.Compute</span></span>
* <span data-ttu-id="c89c6-162">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="c89c6-162">VMSS VM Update feature</span></span>
    - <span data-ttu-id="c89c6-163">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-163">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="c89c6-164">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-164">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="c89c6-165">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c89c6-165">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="c89c6-166">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-166">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="c89c6-167">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-167">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="c89c6-168">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-168">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="c89c6-169">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-169">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="c89c6-170">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-170">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="c89c6-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c89c6-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="c89c6-172">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-172">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="c89c6-173">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c89c6-173">AzureRM.Network</span></span>
* <span data-ttu-id="c89c6-174">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="c89c6-174">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="c89c6-175">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="c89c6-175">AzureRM.Resources</span></span>
* <span data-ttu-id="c89c6-176">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-176">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="c89c6-177">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="c89c6-177">AzureRM.Scheduler</span></span>
* <span data-ttu-id="c89c6-178">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-178">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="c89c6-179">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c89c6-179">AzureRM.Sql</span></span>
* <span data-ttu-id="c89c6-180">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c89c6-180">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="c89c6-181">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c89c6-181">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c89c6-182">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c89c6-182">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c89c6-183">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c89c6-183">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c89c6-184">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c89c6-184">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c89c6-185">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c89c6-185">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="c89c6-186">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="c89c6-186">AzureRM.Websites</span></span>
* <span data-ttu-id="c89c6-187">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-187">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="c89c6-188">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="c89c6-188">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="c89c6-189">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="c89c6-189">AzureRM.Profile</span></span>
* <span data-ttu-id="c89c6-190">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-190">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="c89c6-191">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c89c6-191">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="c89c6-192">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="c89c6-192">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="c89c6-193">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c89c6-193">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="c89c6-194">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-194">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="c89c6-195">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-195">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="c89c6-196">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-196">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="c89c6-197">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-197">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="c89c6-198">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-198">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="c89c6-199">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-199">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="c89c6-200">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-200">Added support for MSI identity</span></span>
* <span data-ttu-id="c89c6-201">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="c89c6-201">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="c89c6-202">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="c89c6-202">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="c89c6-203">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="c89c6-203">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="c89c6-204">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="c89c6-204">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="c89c6-205">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="c89c6-205">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="c89c6-206">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="c89c6-206">AzureRM.Batch</span></span>
* <span data-ttu-id="c89c6-207">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-207">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="c89c6-208">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-208">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="c89c6-209">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="c89c6-209">AzureRM.Consumption</span></span>
* <span data-ttu-id="c89c6-210">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-210">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="c89c6-211">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c89c6-211">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="c89c6-212">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-212">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="c89c6-213">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-213">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="c89c6-214">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-214">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="c89c6-215">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="c89c6-215">AzureRM.Network</span></span>
* <span data-ttu-id="c89c6-216">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-216">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="c89c6-217">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-217">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="c89c6-218">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="c89c6-218">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="c89c6-219">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-219">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="c89c6-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c89c6-220">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c89c6-221">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-221">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="c89c6-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c89c6-222">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="c89c6-223">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-223">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="c89c6-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="c89c6-224">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="c89c6-225">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c89c6-225">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="c89c6-226">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="c89c6-226">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="c89c6-227">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="c89c6-227">AzureRM.Sql</span></span>
* <span data-ttu-id="c89c6-228">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-228">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="c89c6-229">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="c89c6-229">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="c89c6-230">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-230">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="c89c6-231">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c89c6-231">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="c89c6-232">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c89c6-232">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="c89c6-233">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c89c6-233">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="c89c6-234">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="c89c6-234">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="c89c6-235">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="c89c6-235">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="c89c6-236">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="c89c6-236">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="c89c6-237">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="c89c6-237">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="c89c6-238">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c89c6-238">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="c89c6-239">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="c89c6-239">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
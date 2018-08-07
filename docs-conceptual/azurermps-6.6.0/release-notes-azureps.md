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
ms.openlocfilehash: 3961f5c37869d0dc877b85bad535f399181040db
ms.sourcegitcommit: fd11600079ee3844986552bccc4e274a231332b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2018
ms.locfileid: "39368179"
---
# <a name="release-notes"></a><span data-ttu-id="1234f-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="1234f-103">Release notes</span></span>

<span data-ttu-id="1234f-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1234f-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="660---july-2018"></a><span data-ttu-id="1234f-105">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="1234f-105">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1234f-106">全般</span><span class="sxs-lookup"><span data-stu-id="1234f-106">General</span></span>
* <span data-ttu-id="1234f-107">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-107">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1234f-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-108">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-109">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-109">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span> <span data-ttu-id="1234f-110">既定値は常に true ですが、個々のリソースによって既定値がオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="1234f-110">Default is always true, individual resources and overridet the default.</span></span>
* <span data-ttu-id="1234f-111">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-111">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1234f-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1234f-112">Azure.Storage</span></span>
* <span data-ttu-id="1234f-113">DefaulfProfile からストレージ コンテキストを取得できるようになりました</span><span class="sxs-lookup"><span data-stu-id="1234f-113">Support get Storage Context from DefaulfProfile</span></span>
* <span data-ttu-id="1234f-114">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-114">Add Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1234f-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1234f-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1234f-116">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="1234f-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="1234f-117">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-117">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="1234f-118">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="1234f-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="1234f-119">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-119">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="1234f-120">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="1234f-120">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="1234f-121">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="1234f-121">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1234f-122">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1234f-122">AzureRM.Compute</span></span>
* <span data-ttu-id="1234f-123">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-123">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="1234f-124">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-124">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="1234f-125">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="1234f-125">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="1234f-126">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="1234f-126">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="1234f-127">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-127">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="1234f-128">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-128">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="1234f-129">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-129">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="1234f-130">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-130">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="1234f-131">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-131">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="1234f-132">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-132">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="1234f-133">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1234f-133">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="1234f-134">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-134">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="1234f-135">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="1234f-135">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="1234f-136">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-136">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="1234f-137">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-137">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1234f-138">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1234f-138">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1234f-139">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-139">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1234f-140">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1234f-140">AzureRM.EventHub</span></span>
* <span data-ttu-id="1234f-141">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-141">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="1234f-142">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="1234f-142">AzureRM.Insights</span></span>
* <span data-ttu-id="1234f-143">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-143">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="1234f-144">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="1234f-144">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1234f-145">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1234f-145">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1234f-146">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-146">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1234f-147">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1234f-147">AzureRM.Network</span></span>
* <span data-ttu-id="1234f-148">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-148">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1234f-149">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1234f-149">AzureRM.Resources</span></span>
* <span data-ttu-id="1234f-150">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-150">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="1234f-151">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-151">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1234f-152">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1234f-152">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1234f-153">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-153">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="1234f-154">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-154">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="1234f-155">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-155">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-156">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-156">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="1234f-157">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="1234f-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="1234f-158">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-158">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="1234f-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="1234f-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="1234f-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="1234f-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="1234f-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="1234f-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="1234f-162">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-162">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="1234f-163">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-163">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="1234f-164">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="1234f-164">AzureRM.Storage</span></span>
* <span data-ttu-id="1234f-165">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-165">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="1234f-166">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="1234f-166">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="1234f-167">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1234f-167">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="1234f-168">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1234f-168">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="1234f-169">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="1234f-169">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="1234f-170">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="1234f-170">AzureRM.Tags</span></span>
* <span data-ttu-id="1234f-171">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="1234f-171">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="1234f-172">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="1234f-172">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1234f-173">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-173">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-174">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-174">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1234f-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1234f-175">Azure.Storage</span></span>
* <span data-ttu-id="1234f-176">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="1234f-176">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="1234f-177">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1234f-177">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="1234f-178">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1234f-178">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="1234f-179">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1234f-179">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="1234f-180">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-180">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="1234f-181">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="1234f-181">AzureRM.Automation</span></span>
* <span data-ttu-id="1234f-182">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-182">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1234f-183">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1234f-183">AzureRM.Compute</span></span>
* <span data-ttu-id="1234f-184">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-184">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="1234f-185">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-185">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="1234f-186">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-186">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="1234f-187">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-187">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="1234f-188">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-188">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1234f-189">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1234f-189">AzureRM.EventHub</span></span>
* <span data-ttu-id="1234f-190">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-190">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1234f-191">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1234f-191">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1234f-192">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-192">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="1234f-193">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1234f-193">AzureRM.LogicApp</span></span>
* <span data-ttu-id="1234f-194">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-194">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1234f-195">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1234f-195">AzureRM.Network</span></span>
* <span data-ttu-id="1234f-196">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="1234f-196">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="1234f-197">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-197">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="1234f-198">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-198">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="1234f-199">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-199">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="1234f-200">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-200">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="1234f-201">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="1234f-201">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="1234f-202">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="1234f-202">AzureRM.Relay</span></span>
* <span data-ttu-id="1234f-203">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-203">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1234f-204">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1234f-204">AzureRM.Resources</span></span>
* <span data-ttu-id="1234f-205">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-205">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="1234f-206">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="1234f-206">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="1234f-207">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-207">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="1234f-208">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-208">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="1234f-209">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-209">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="1234f-210">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1234f-210">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1234f-211">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-211">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="1234f-212">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-212">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="1234f-213">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1234f-213">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1234f-214">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1234f-214">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1234f-215">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1234f-215">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1234f-216">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1234f-216">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="1234f-217">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="1234f-217">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="1234f-218">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-218">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="1234f-219">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1234f-219">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="1234f-220">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-220">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1234f-221">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-221">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-222">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-222">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="1234f-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="1234f-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="1234f-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="1234f-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1234f-225">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1234f-225">AzureRM.Websites</span></span>
* <span data-ttu-id="1234f-226">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="1234f-226">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="1234f-227">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="1234f-228">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="1234f-228">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="1234f-229">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="1234f-229">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1234f-230">全般</span><span class="sxs-lookup"><span data-stu-id="1234f-230">General</span></span>
* <span data-ttu-id="1234f-231">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-231">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="1234f-232">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-232">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-233">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-233">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1234f-234">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1234f-234">AzureRM.Compute</span></span>
* <span data-ttu-id="1234f-235">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="1234f-235">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="1234f-236">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-236">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="1234f-237">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-237">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="1234f-238">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="1234f-238">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="1234f-239">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-239">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="1234f-240">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="1234f-240">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="1234f-241">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="1234f-241">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="1234f-242">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1234f-242">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="1234f-243">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="1234f-243">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="1234f-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1234f-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="1234f-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1234f-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="1234f-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="1234f-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1234f-247">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1234f-247">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1234f-248">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="1234f-248">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="1234f-249">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="1234f-249">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="1234f-250">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-250">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="1234f-251">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-251">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="1234f-252">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="1234f-252">AzureRM.EventHub</span></span>
* <span data-ttu-id="1234f-253">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-253">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="1234f-254">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-254">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="1234f-255">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="1234f-255">Provided Default Parameter set.</span></span>
* <span data-ttu-id="1234f-256">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="1234f-256">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1234f-257">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1234f-257">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1234f-258">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-258">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="1234f-259">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1234f-259">AzureRM.Network</span></span>
* <span data-ttu-id="1234f-260">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="1234f-260">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="1234f-261">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-261">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="1234f-262">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-262">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="1234f-263">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-263">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="1234f-264">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-264">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1234f-265">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-265">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1234f-266">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-266">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="1234f-267">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-267">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1234f-268">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-268">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1234f-269">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-269">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="1234f-270">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1234f-270">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1234f-271">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-271">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="1234f-272">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1234f-272">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="1234f-273">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="1234f-273">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1234f-274">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1234f-274">AzureRM.Resources</span></span>
* <span data-ttu-id="1234f-275">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-275">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="1234f-276">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="1234f-276">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="1234f-277">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="1234f-277">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="1234f-278">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-278">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="1234f-279">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-279">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="1234f-280">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-280">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="1234f-281">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-281">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="1234f-282">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-282">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="1234f-283">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-283">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="1234f-284">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-284">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="1234f-285">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-285">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="1234f-286">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-286">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="1234f-287">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-287">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="1234f-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1234f-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="1234f-289">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="1234f-289">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1234f-290">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-290">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-291">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="1234f-291">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="1234f-292">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-292">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="1234f-293">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="1234f-293">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1234f-294">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-294">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-295">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-295">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="1234f-296">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="1234f-296">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="1234f-297">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1234f-297">Azure.Storage</span></span>
* <span data-ttu-id="1234f-298">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-298">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1234f-299">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1234f-299">AzureRM.Compute</span></span>
* <span data-ttu-id="1234f-300">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-300">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="1234f-301">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-301">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="1234f-302">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="1234f-302">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="1234f-303">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="1234f-303">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="1234f-304">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="1234f-304">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="1234f-305">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-305">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="1234f-306">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1234f-306">Start-AzureRmVM</span></span>
    - <span data-ttu-id="1234f-307">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1234f-307">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="1234f-308">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1234f-308">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="1234f-309">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="1234f-309">Set-AzureRmVM</span></span>
    - <span data-ttu-id="1234f-310">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="1234f-310">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="1234f-311">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1234f-311">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="1234f-312">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="1234f-312">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="1234f-313">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="1234f-313">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="1234f-314">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1234f-314">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="1234f-315">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1234f-315">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="1234f-316">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1234f-316">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="1234f-317">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="1234f-317">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="1234f-318">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="1234f-318">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="1234f-319">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="1234f-319">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="1234f-320">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="1234f-320">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="1234f-321">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="1234f-321">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="1234f-322">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="1234f-322">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="1234f-323">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="1234f-323">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="1234f-324">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="1234f-324">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="1234f-325">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1234f-325">AzureRM.EventGrid</span></span>
* <span data-ttu-id="1234f-326">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1234f-326">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="1234f-327">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1234f-327">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1234f-328">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-328">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="1234f-329">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1234f-329">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="1234f-330">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="1234f-330">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="1234f-331">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="1234f-331">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="1234f-332">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-332">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="1234f-333">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1234f-333">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1234f-334">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-334">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="1234f-335">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="1234f-335">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1234f-336">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-336">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-337">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-337">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1234f-338">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1234f-338">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1234f-339">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-339">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1234f-340">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1234f-340">AzureRM.Websites</span></span>
* <span data-ttu-id="1234f-341">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="1234f-341">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="1234f-342">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="1234f-342">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="1234f-343">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="1234f-343">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="1234f-344">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1234f-344">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="1234f-345">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-345">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="1234f-346">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="1234f-346">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1234f-347">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-347">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-348">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-348">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="1234f-349">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="1234f-349">AzureRM.Compute</span></span>
* <span data-ttu-id="1234f-350">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="1234f-350">VMSS VM Update feature</span></span>
    - <span data-ttu-id="1234f-351">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-351">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="1234f-352">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-352">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="1234f-353">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1234f-353">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="1234f-354">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-354">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="1234f-355">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-355">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="1234f-356">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-356">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="1234f-357">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-357">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="1234f-358">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="1234f-358">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="1234f-359">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1234f-359">AzureRM.KeyVault</span></span>
* <span data-ttu-id="1234f-360">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-360">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="1234f-361">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1234f-361">AzureRM.Network</span></span>
* <span data-ttu-id="1234f-362">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="1234f-362">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="1234f-363">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="1234f-363">AzureRM.Resources</span></span>
* <span data-ttu-id="1234f-364">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-364">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="1234f-365">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="1234f-365">AzureRM.Scheduler</span></span>
* <span data-ttu-id="1234f-366">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1234f-366">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="1234f-367">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-367">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-368">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="1234f-368">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="1234f-369">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1234f-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="1234f-370">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="1234f-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="1234f-371">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="1234f-371">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="1234f-372">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1234f-372">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="1234f-373">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1234f-373">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="1234f-374">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="1234f-374">AzureRM.Websites</span></span>
* <span data-ttu-id="1234f-375">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="1234f-375">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="1234f-376">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="1234f-376">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="1234f-377">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1234f-377">AzureRM.Profile</span></span>
* <span data-ttu-id="1234f-378">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-378">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="1234f-379">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1234f-379">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="1234f-380">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="1234f-380">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="1234f-381">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1234f-381">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="1234f-382">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-382">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="1234f-383">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-383">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="1234f-384">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-384">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="1234f-385">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1234f-385">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="1234f-386">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-386">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="1234f-387">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-387">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="1234f-388">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-388">Added support for MSI identity</span></span>
* <span data-ttu-id="1234f-389">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="1234f-389">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="1234f-390">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="1234f-390">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="1234f-391">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="1234f-391">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="1234f-392">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="1234f-392">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="1234f-393">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="1234f-393">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="1234f-394">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="1234f-394">AzureRM.Batch</span></span>
* <span data-ttu-id="1234f-395">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="1234f-395">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="1234f-396">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="1234f-396">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="1234f-397">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="1234f-397">AzureRM.Consumption</span></span>
* <span data-ttu-id="1234f-398">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-398">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="1234f-399">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1234f-399">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="1234f-400">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-400">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="1234f-401">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-401">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="1234f-402">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-402">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="1234f-403">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="1234f-403">AzureRM.Network</span></span>
* <span data-ttu-id="1234f-404">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-404">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="1234f-405">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-405">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="1234f-406">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="1234f-406">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="1234f-407">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-407">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="1234f-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1234f-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="1234f-409">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-409">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="1234f-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1234f-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="1234f-411">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-411">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="1234f-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="1234f-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="1234f-413">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1234f-413">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="1234f-414">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="1234f-414">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="1234f-415">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="1234f-415">AzureRM.Sql</span></span>
* <span data-ttu-id="1234f-416">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1234f-416">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="1234f-417">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="1234f-417">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="1234f-418">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1234f-418">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="1234f-419">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="1234f-419">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="1234f-420">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1234f-420">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="1234f-421">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1234f-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="1234f-422">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="1234f-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="1234f-423">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="1234f-423">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="1234f-424">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="1234f-424">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="1234f-425">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="1234f-425">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="1234f-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1234f-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="1234f-427">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="1234f-427">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 8d53923f76506469cdc2c111faf7c4568b54f7de
ms.sourcegitcommit: cef87acc9f2a0d296bef74f526afd2e067e8146b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "84294795"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="35cec-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="35cec-103">Azure PowerShell release notes</span></span>

## <a name="420---june-2020"></a><span data-ttu-id="35cec-104">4.2.0 - 2020 年 6 月</span><span class="sxs-lookup"><span data-stu-id="35cec-104">4.2.0 - June 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-105">Az.Accounts</span></span>
* <span data-ttu-id="35cec-106">Az で Azure Automation または PowerShell ジョブのログがスキップされる可能性がある問題を修正しました [#11492]</span><span class="sxs-lookup"><span data-stu-id="35cec-106">Fixed an issue that may cause Az to skip logs in Azure Automation or PowerShell jobs [#11492]</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="35cec-107">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="35cec-107">Az.AnalysisServices</span></span>
* <span data-ttu-id="35cec-108">データ プレーン コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-108">Updated assembly version of data plane cmdlets</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-109">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-110">サービス管理コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-110">Updated assembly version of service management cmdlets</span></span>

#### <a name="azbilling"></a><span data-ttu-id="35cec-111">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="35cec-111">Az.Billing</span></span>
* <span data-ttu-id="35cec-112">使用量コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-112">Updated assembly version of consumption cmdlets</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-113">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-113">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-114">PrivateEndpoint と PublicNetworkAccess コントロールをサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-114">Support PrivateEndpoint and PublicNetworkAccess control.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-115">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-116">データ ファクトリ V2 コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-116">Updated assembly version of data factory V2 cmdlets</span></span>

#### <a name="azdatashare"></a><span data-ttu-id="35cec-117">Az.DataShare</span><span class="sxs-lookup"><span data-stu-id="35cec-117">Az.DataShare</span></span>
* <span data-ttu-id="35cec-118">''Az.DataShare'' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-118">General availability of ''Az.DataShare'' module</span></span>

#### <a name="azdesktopvirtualization"></a><span data-ttu-id="35cec-119">Az.DesktopVirtualization</span><span class="sxs-lookup"><span data-stu-id="35cec-119">Az.DesktopVirtualization</span></span>
* <span data-ttu-id="35cec-120">''Az.DesktopVirtualization'' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-120">General availability of ''Az.DesktopVirtualization'' module</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-121">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-121">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-122">SDK を 0.21.0 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="35cec-122">Upgraded SDK to 0.21.0</span></span>
* <span data-ttu-id="35cec-123">省略可能なパラメーターを以下に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-123">Added optional parameters to</span></span> 
    - <span data-ttu-id="35cec-124">'New-AzOperationalInsightsSavedSearch'</span><span class="sxs-lookup"><span data-stu-id="35cec-124">'New-AzOperationalInsightsSavedSearch'</span></span>
    - <span data-ttu-id="35cec-125">'Set-AzOperationalInsightsSavedSearch'</span><span class="sxs-lookup"><span data-stu-id="35cec-125">'Set-AzOperationalInsightsSavedSearch'</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-126">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-126">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-127">'Start-AzPolicyComplianceScan' の例 3 を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-127">Corrected example 3 for 'Start-AzPolicyComplianceScan'</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="35cec-128">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="35cec-128">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="35cec-129">PowerBI コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-129">Updated assembly version of PowerBI cmdlets</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="35cec-130">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="35cec-130">Az.PrivateDns</span></span>
* <span data-ttu-id="35cec-131">Remove-AzPrivateDnsRecordSet の詳細出力文字列形式を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-131">Corrected verbose output string formatting for Remove-AzPrivateDnsRecordSet</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-132">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-132">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-133">ゾーンからゾーンへのレプリケーションの復旧計画を xml 入力から作成するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-133">Azure Site Recovery support for creating recovery plan for zone to zone replication from xml input.</span></span>
* <span data-ttu-id="35cec-134">SiteRecovery および Backup コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-134">Updated assembly version of SiteRecovery and Backup cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-135">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-135">Az.Resources</span></span>
* <span data-ttu-id="35cec-136">Get-AzDeploymentScriptLog および Save-AzDeploymentScriptLog コマンドレットに Tail パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-136">Added Tail parameter to Get-AzDeploymentScriptLog and Save-AzDeploymentScriptLog cmdlets</span></span>
* <span data-ttu-id="35cec-137">Output プロパティをフォーマットし、Get-AzDeploymentScript コマンドレットの出力に表示します</span><span class="sxs-lookup"><span data-stu-id="35cec-137">Formatted Output property and show it on the Get-AzDeploymentScript cmdlet output</span></span>
* <span data-ttu-id="35cec-138">-DeploymentScriptInputObject parameter を -DeploymentScriptObject に名前変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-138">Renamed -DeploymentScriptInputObject parameter to -DeploymentScriptObject</span></span>
* <span data-ttu-id="35cec-139">コマンドレット メッセージで欠落しているファイル/ターゲット名を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-139">Fixed missing file/target name in cmdlet messages.</span></span>
* <span data-ttu-id="35cec-140">リソース マネージャーとタグのコマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-140">Updated assembly version of resource manager and tags cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-141">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-141">Az.Sql</span></span>
* <span data-ttu-id="35cec-142">UsePrivateLinkConnection を 'New-AzSqlSyncGroup'、'Update-AzSqlSyncGroup'、'New-AzSqlSyncMember' および 'Update-AzSqlSyncMember' に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-142">Added UsePrivateLinkConnection to 'New-AzSqlSyncGroup', 'Update-AzSqlSyncGroup', 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="35cec-143">SyncMemberAzureDatabaseResourceId を 'New-AzSqlSyncMember' と 'Update-AzSqlSyncMember' に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-143">Added SyncMemberAzureDatabaseResourceId to 'New-AzSqlSyncMember' and 'Update-AzSqlSyncMember'</span></span>
* <span data-ttu-id="35cec-144">Set SQL Server Azure Active Directory Admin コマンドレットにゲスト ユーザー参照のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-144">Added Guest user lookup support to Set SQL Server Azure Active Directory Admin cmdlet</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-145">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-145">Az.Storage</span></span>
* <span data-ttu-id="35cec-146">データ プレーン コマンドレットのアセンブリ バージョンを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-146">Updated assembly version of data plane cmdlets</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="35cec-147">4.1.0 - 2020 年 5 月</span><span class="sxs-lookup"><span data-stu-id="35cec-147">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="35cec-148">前回のリリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-148">Highlights since the last release</span></span>
* <span data-ttu-id="35cec-149">次の PowerShell バージョンをサポートしました。Windows PowerShell 5.1、PowerShell Core 6.2.4+、PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="35cec-149">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="35cec-150">Az.Functions の一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-150">General availability of Az.Functions</span></span> 
* <span data-ttu-id="35cec-151">Az.ApiManagement、Az.Batch、Az.Compute、Az.KeyVault、Az.Monitor、Az.Network、Az.OperationalInsights、Az.Resources、Az.Storage にメジャー リリースがあります</span><span class="sxs-lookup"><span data-stu-id="35cec-151">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-152">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-152">Az.Accounts</span></span>
* <span data-ttu-id="35cec-153">パラメーター 'AzureSynapseAnalyticsEndpointResourceId' および 'AzureSynapseAnalyticsEndpointSuffix' を受け入れるように 'Add-AzEnvironment' と 'Set-AzEnvironment' を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-153">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="35cec-154">Azure.Core 関連アセンブリを Az.Accounts に追加しました。サポートされている PowerShell プラットフォームには、Windows PowerShell 5.1、PowerShell Core 6.2.4、PowerShell 7 以降が含まれます</span><span class="sxs-lookup"><span data-stu-id="35cec-154">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="35cec-155">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="35cec-155">Az.Aks</span></span>
* <span data-ttu-id="35cec-156">API バージョンを 2019-10-01 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="35cec-156">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="35cec-157">Windows コンテナーを使用した AKS の作成をサポートしました</span><span class="sxs-lookup"><span data-stu-id="35cec-157">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="35cec-158">次の新しいコマンドレットを提供しました。'New-AzAksNodePool'、'Update-AzAksNodePool'、'Remove-AzAksNodePool'、'Get-AzAksNodePool'、'Install-AzAksKubectl'、'Get-AzAksVersion'</span><span class="sxs-lookup"><span data-stu-id="35cec-158">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-159">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-159">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-160">'New-AzApiManagement' と 'Set-AzApiManagement': [-AssignIdentity] パラメーターの名前を [-SystemAssignedIdentity] に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-160">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="35cec-161">'New-AzApiManagement' と 'Set-AzApiManagement':新しいパラメーター [-UserAssignedIdentity <String[]>] を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-161">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="35cec-162">'Get-AzApiManagementProperty': 名前を 'Get-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-162">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="35cec-163">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-163">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="35cec-164">'New-AzApiManagementProperty': 名前を 'New-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-164">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="35cec-165">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-165">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="35cec-166">'Set-AzApiManagementProperty': 名前を 'Set-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-166">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="35cec-167">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-167">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="35cec-168">'Remove-AzApiManagementProperty': 名前を 'Remove-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-168">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="35cec-169">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-169">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="35cec-170">新しい 'Get-AzApiManagementAuthorizationServerClientSecret' コマンドレットを追加しました。'Get-AzApiManagementAuthorizationServer' ではクライアント シークレットは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="35cec-170">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="35cec-171">新しい 'Get-AzApiManagementNamedValueSecretValue' コマンドレットを追加しました。'Get-AzApiManagementNamedValue' ではシークレット値は返されません。</span><span class="sxs-lookup"><span data-stu-id="35cec-171">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="35cec-172">新しい 'Get-AzApiManagementOpenIdConnectProviderClientSecret' コマンドレットを追加しました。'Get-AzApiManagementOpenIdConnectProvider' ではクライアント シークレットは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="35cec-172">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="35cec-173">新しい 'Get-AzApiManagementSubscriptionKey' コマンドレットを追加しました。'Get-AzApiManagementSubscription' ではサブスクリプション キーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="35cec-173">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="35cec-174">新しい 'Get-AzApiManagementTenantAccessSecret' コマンドレットを追加しました。'Get-AzApiManagementTenantAccess' ではキーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="35cec-174">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="35cec-175">新しい 'Get-AzApiManagementTenantGitAccessSecret' コマンドレットを追加しました。'Get-AzApiManagementTenantGitAccess' ではキーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="35cec-175">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="35cec-176">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-176">Az.ApplicationInsights</span></span>
* <span data-ttu-id="35cec-177">次のパラメーターを追加しました。'New-AzApplicationInsights' 用の 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery'</span><span class="sxs-lookup"><span data-stu-id="35cec-177">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="35cec-178">コマンドレット 'Update-AzApplicationInsights' を作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-178">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="35cec-179">リンクされているストレージ アカウント用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-179">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-180">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-180">Az.Batch</span></span>
* <span data-ttu-id="35cec-181">'Microsoft.Azure.Batch' SDK バージョン 13.0.0 と 'Microsoft.Azure.Management.Batch' SDK バージョン 9.0.0 を使用するように Az.Batch を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-181">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="35cec-182">新しい '-CertificateKind' パラメーターを使用して追加する証明書の種類を選択する機能を 'New-AzBatchCertificate' に追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-182">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="35cec-183">以前は常に '' であった 'PSApplication' から 'ApplicationPackages' プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-183">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="35cec-184">アプリケーション内の特定のパッケージは 'Get-AzBatchApplicationPackage' を使用して取得できるようになっています。</span><span class="sxs-lookup"><span data-stu-id="35cec-184">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="35cec-185">次に例を示します。'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'</span><span class="sxs-lookup"><span data-stu-id="35cec-185">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="35cec-186">'New-AzBatchPool' を使用してプールを作成する場合に、'PSImageReference' の 'VirtualMachineImageId' プロパティが Shared Image Gallery のイメージのみを参照できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-186">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="35cec-187">'New-AzBatchPool' を使用してプールを作成する場合に、'PSNetworkConfiguration' の新しい 'PublicIPAddressConfiguration' プロパティを使用して、そのプールをパブリック IP なしでプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="35cec-187">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="35cec-188">'PSNetworkConfiguration' の 'PublicIPs' プロパティも 'PSPublicIPAddressConfiguration' に移動しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-188">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="35cec-189">このプロパティは、'IPAddressProvisioningType ' が 'UserManaged' の場合にのみ指定できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-189">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-190">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-190">Az.Compute</span></span>
* <span data-ttu-id="35cec-191">'Update-AzVM' コマンドレットに HostId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-191">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="35cec-192">'New-AzVMConfig'、'New-AzVmssConfig'、'Update-AzVmss'、'Set-AzVMOperatingSystem'、'Set-AzVmssOsProfile' コマンドレットのヘルプ ドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-192">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="35cec-193">重大な変更</span><span class="sxs-lookup"><span data-stu-id="35cec-193">Breaking changes</span></span>
    - <span data-ttu-id="35cec-194">FilterExpression パラメーターが 'Get-AzVMImage' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-194">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="35cec-195">AssignIdentity パラメーターが 'New-AzVmssConfig'、'New-AzVMConfig'、'Update-AzVM' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-195">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="35cec-196">AutomaticRepairMaxInstanceRepairsPercent が 'New-AzVmssConfig' と 'Update-AzVmss' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-196">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="35cec-197">AvailabilitySetsColocationStatus、VirtualMachinesColocationStatus、VirtualMachineScaleSetsColocationStatus プロパティが ProximityPlacementGroup から削除されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-197">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="35cec-198">MaxInstanceRepairsPercent プロパティが AutomaticRepairsPolicy から削除されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-198">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="35cec-199">AvailabilitySets、VirtualMachines、VirtualMachineScaleSets の種類が IList<SubResource> から IList<SubResourceWithColocationStatus> に変更されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-199">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="35cec-200">'Get-AzVM' コマンドレットの説明を、わかりやすくするために更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-200">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-201">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-202">Managed IR でデータ フロー ランタイム プロパティの CRUD をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-202">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-203">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-203">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-204">Front Door ルール エンジン オブジェクトを作成、更新、取得、削除するための新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-204">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="35cec-205">Front Door ルール エンジン オブジェクトを構築するためのヘルパー コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-205">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="35cec-206">Front Door ルーティング規則オブジェクトにルール エンジン参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-206">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="35cec-207">Front Door バックエンド オブジェクトにプライベート リンク パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-207">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="35cec-208">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="35cec-208">Az.Functions</span></span>
* <span data-ttu-id="35cec-209">''Az.Functions'' モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-209">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-210">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-210">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-211">お客様が管理するキー ディスクの暗号化をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-211">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="35cec-212">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="35cec-212">Az.HealthcareApis</span></span>
* <span data-ttu-id="35cec-213">アクセス ポリシーの既定値が現在のプリンシパルではなくなりました</span><span class="sxs-lookup"><span data-stu-id="35cec-213">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-214">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-214">Az.IotHub</span></span>
* <span data-ttu-id="35cec-215">SQL に似た言語を使用して情報を取得するために、IoT ハブ内でクエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-215">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="35cec-216">'Add-AzIotHubDevice' が子デバイスなしで Edge 対応デバイスを作成できない問題を修正しました [#11597]</span><span class="sxs-lookup"><span data-stu-id="35cec-216">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="35cec-217">Iot Hub、デバイス、またはモジュールの SAS トークンを生成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-217">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="35cec-218">構成メトリック クエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-218">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="35cec-219">大規模な IoT Edge 自動デプロイを管理します。</span><span class="sxs-lookup"><span data-stu-id="35cec-219">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="35cec-220">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-220">New cmdlets are:</span></span>
    - <span data-ttu-id="35cec-221">'Add-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-221">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="35cec-222">'Get-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-222">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="35cec-223">'Remove-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-223">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="35cec-224">'Set-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-224">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="35cec-225">IoT Edge デプロイ メトリック クエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-225">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="35cec-226">指定されたエッジ デバイスに構成内容を適用するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-226">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-227">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-227">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-228">次の 2 つの別名を削除しました。'New-AzKeyVaultCertificateAdministratorDetails' と 'New-AzKeyVaultCertificateOrganizationDetails'</span><span class="sxs-lookup"><span data-stu-id="35cec-228">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="35cec-229">キー コンテナーを作成するときに、論理的な削除を既定で有効にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-229">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="35cec-230">キー コンテナーを作成するときに、特定のネットワークの場所からのアクセスを管理するようにネットワーク ルールを設定できます</span><span class="sxs-lookup"><span data-stu-id="35cec-230">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="35cec-231">Bring Your Own Key (BYOK) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-231">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="35cec-232">'Add-AzKeyVaultKey' で、キー交換キーの生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-232">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="35cec-233">'Get-AzKeyVaultKey' で、PEM 形式の公開キーのダウンロードをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-233">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="35cec-234">'Add-AzKeyVaultKey' のヘルプ ドキュメントの 'KeyOps' 部分を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-234">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-235">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-235">Az.Monitor</span></span>
* <span data-ttu-id="35cec-236">保持ポリシーがすべてのカテゴリに適用されないという 'Set-AzDiagnosticSettings' のバグを修正しました [#11589]</span><span class="sxs-lookup"><span data-stu-id="35cec-236">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="35cec-237">メトリック アラート V2 の WebTest 可用性基準をサポートしました</span><span class="sxs-lookup"><span data-stu-id="35cec-237">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="35cec-238">'New-AzMetricAlertRuleV2Criteria': WebTest 可用性基準を作成するためのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-238">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="35cec-239">'Add-AzMetricAlertRuleV2': 新しい WebTest 可用性基準をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-239">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="35cec-240">PSLogProfile 内の RetentionPolicy の冗長な定義を削除しました [#7608]</span><span class="sxs-lookup"><span data-stu-id="35cec-240">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="35cec-241">PSEventData で定義された冗長なプロパティを削除しました [#11353]</span><span class="sxs-lookup"><span data-stu-id="35cec-241">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="35cec-242">'Get-AzLog' の名前を 'Get-AzActivityLog' に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-242">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-243">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-243">Az.Network</span></span>
* <span data-ttu-id="35cec-244">ゾーンの既定の動作が変更されることを通知するための、破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-244">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="35cec-245">'New-AzPublicIpAddress'</span><span class="sxs-lookup"><span data-stu-id="35cec-245">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="35cec-246">'New-AzPublicIpPrefix'</span><span class="sxs-lookup"><span data-stu-id="35cec-246">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="35cec-247">'New-AzLoadBalancerFrontendIpConfig'</span><span class="sxs-lookup"><span data-stu-id="35cec-247">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="35cec-248">新しい最上位リソース SecurityPartnerProvider のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-248">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="35cec-249">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-249">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-250">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="35cec-250">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="35cec-251">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="35cec-251">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="35cec-252">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="35cec-252">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="35cec-253">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="35cec-253">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="35cec-254">'RequiredZoneNames' を 'PSPrivateLinkResource' に、'GroupId' を 'PSPrivateEndpointConnection' に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-254">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="35cec-255">New-AzNetworkWatcherConnectionMonitorTestConfigurationObject の SuccessThresholdRoundTripTimeMs パラメーターの誤った種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-255">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="35cec-256">AllowVnetToVnetTraffic 引数の既定値を True に設定するように VirtualWan コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-256">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="35cec-257">'New-AzVirtualWan'</span><span class="sxs-lookup"><span data-stu-id="35cec-257">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="35cec-258">'Update-AzVirtualWan'</span><span class="sxs-lookup"><span data-stu-id="35cec-258">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="35cec-259">プライベート エンドポイントの DNS ゾーン グループをサポートする新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-259">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="35cec-260">'New-AzPrivateDnsZoneConfig'</span><span class="sxs-lookup"><span data-stu-id="35cec-260">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="35cec-261">'Get-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="35cec-261">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="35cec-262">'New-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="35cec-262">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="35cec-263">'Set-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="35cec-263">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="35cec-264">'Remove-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="35cec-264">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="35cec-265">'DNSEnableProxy'、'DNSRequireProxyForNetworkRules'、'DNSServers' パラメーターを 'AzureFirewall' に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-265">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="35cec-266">'EnableDnsProxy'、'DnsProxyNotRequiredForNetworkRule'、'DnsServer' パラメーターを 'AzureFirewall' に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-266">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="35cec-267">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-267">Updated cmdlet:</span></span>
        - <span data-ttu-id="35cec-268">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="35cec-268">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-269">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-269">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-270">生成された新しい SDK を適用するようにレガシ コードを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-270">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="35cec-271">非推奨になった API が原因でコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-271">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="35cec-272">'Get-AzOperationalInsightsSavedSearchResult' (別名 'Get-AzOperationalInsightsSavedSearchResults')</span><span class="sxs-lookup"><span data-stu-id="35cec-272">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="35cec-273">'Get-AzOperationalInsightsSearchResult' (別名 'Get-AzOperationalInsightsSearchResults')</span><span class="sxs-lookup"><span data-stu-id="35cec-273">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="35cec-274">'Get-AzOperationalInsightsLinkTarget' (別名 'Get-AzOperationalInsightsLinkTargets')</span><span class="sxs-lookup"><span data-stu-id="35cec-274">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="35cec-275">'Set-AzOperationalInsightsWorkspace' と 'New-AzOperationalInsightsWorkspace' のパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-275">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="35cec-276">リンクされているストレージ アカウント用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-276">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="35cec-277">クラスターおよびリンクされたサービス用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-277">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-278">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-278">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-279">Azure Site Recovery で、Azure to Azure プロバイダーの近接配置グループ仮想マシンを保護するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-279">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="35cec-280">Azure Site Recovery でゾーン間レプリケーションのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-280">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="35cec-281">Azure Backup で、Azure FileShare 回復ポイントの長期保持サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-281">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="35cec-282">Azure Backup で、'Get-AzRecoveryServicesBackupItem' コマンドレット出力にディスク除外プロパティを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-282">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="35cec-283">Site Recovery サービスのコンテナー資格情報ファイルのプライベート エンドポイントを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-283">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-284">Az.Resources</span></span>
* <span data-ttu-id="35cec-285">新しいロール定義を作成するときの表示遅延に関するメッセージ警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-285">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="35cec-286">厳密に型指定されたオブジェクトを出力するようにポリシー コマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-286">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="35cec-287">'Get-AzResourceLock' コマンドレットで使用されていた '-TenantLevel' パラメーターを削除しました [#11335]</span><span class="sxs-lookup"><span data-stu-id="35cec-287">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="35cec-288">'Remove-AzResourceGroup -Id ResourceId' を修正しました [#9882]</span><span class="sxs-lookup"><span data-stu-id="35cec-288">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="35cec-289">リソース グループ スコープで Resource Manager テンプレートの What-If 結果を取得するための新しいコマンドレットを追加しました。'Get-AzDeploymentResourceGroupWhatIfResult'</span><span class="sxs-lookup"><span data-stu-id="35cec-289">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="35cec-290">サブスクリプション スコープで Resource Manager テンプレートの What-If 結果を取得するための新しいコマンドレットを追加しました。'Get-AzDeploymentWhatIfResult'</span><span class="sxs-lookup"><span data-stu-id="35cec-290">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="35cec-291">エイリアス:'Get-AzSubscriptionDeploymentWhatIf'</span><span class="sxs-lookup"><span data-stu-id="35cec-291">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="35cec-292">ARM テンプレートの What-If 結果を使用するために、'New-AzDeployment' と 'New-AzResourceGroupDeployment' の '-WhatIf' と '-Confirm' パラメーターをオーバーライドしました</span><span class="sxs-lookup"><span data-stu-id="35cec-292">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="35cec-293">デプロイ コマンドレットの 'ApiVersion' パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-293">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="35cec-294">デプロイの失敗に対する改善されたエラー メッセージを表示する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-294">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="35cec-295">デプロイの失敗に対する correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-295">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="35cec-296">デプロイ スクリプトの出力に 'error' プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-296">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="35cec-297">nuget Microsoft.Azure.Management.ResourceManager を '3.7.1-preview' に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-297">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="35cec-298">DeploymentValidateResult の Error プロパティがnuget 3.7.1-preview から読み取り専用に変更されたため、特定のテスト ケースを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-298">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="35cec-299">SDK ResourceManager 3.7.1-preview から GenericResourceExpanded を取得しました</span><span class="sxs-lookup"><span data-stu-id="35cec-299">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="35cec-300">デプロイ用のすべての Get コマンドレットおよび以下に対するタグ サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-300">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="35cec-301">'New-AzDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-301">'New-AzDeployment'</span></span>
    - <span data-ttu-id="35cec-302">'New-AzManagementGroupDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-302">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="35cec-303">'New-AzResourceGroupDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-303">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="35cec-304">'New-AzTenantDeployment'</span><span class="sxs-lookup"><span data-stu-id="35cec-304">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-305">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-305">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-306">--SecretIdentifier を使用した証明書の追加で、誤った証明書の拇印を取得していたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-306">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-307">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-307">Az.Sql</span></span>
* <span data-ttu-id="35cec-308">以下のパフォーマンスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-308">Enhance performance of:</span></span>
    - <span data-ttu-id="35cec-309">'Set-AzSqlDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="35cec-309">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="35cec-310">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="35cec-310">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="35cec-311">'Remove-AzSqlDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="35cec-311">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="35cec-312">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="35cec-312">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="35cec-313">'Enable-AzSqlDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="35cec-313">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="35cec-314">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="35cec-314">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="35cec-315">'Disable-AzSqlDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="35cec-315">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="35cec-316">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="35cec-316">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="35cec-317">コマンドレット 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy' から 'RetentionDays' パラメーターのクライアント側の検証を削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-317">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="35cec-318">Vnet のストレージ アカウントを監査し、Storage Blob Data Contributor ロールの作成時のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-318">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-319">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-319">Az.Storage</span></span>
* <span data-ttu-id="35cec-320">コマンドレット 'Get-AzStorageAccount' でアカウントを取得/一覧表示するために '-AsJob' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-320">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="35cec-321">KeyvaultEncryption を使用してストレージ アカウントを更新するときに KeyVersion をオプションにして、キーの自動ローテーションをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-321">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="35cec-322">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="35cec-322">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="35cec-323">Azure File Directory の削除がパイプラインで失敗することを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-323">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="35cec-324">'Remove-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="35cec-324">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="35cec-325">[#9880] を修正しました。swagger に合わせて NetWorkRule DefaultAction 値の定義を変更しています。</span><span class="sxs-lookup"><span data-stu-id="35cec-325">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="35cec-326">'Update-AzStorageAccountNetworkRuleSet'</span><span class="sxs-lookup"><span data-stu-id="35cec-326">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="35cec-327">'Get-AzStorageAccountNetworkRuleSet'</span><span class="sxs-lookup"><span data-stu-id="35cec-327">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="35cec-328">[#11624] を修正しました。サーバー障害を回避するため、NetworkRules の追加時に重複するルールをスキップします</span><span class="sxs-lookup"><span data-stu-id="35cec-328">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="35cec-329">'Add-AzStorageAccountNetworkRule'</span><span class="sxs-lookup"><span data-stu-id="35cec-329">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="35cec-330">Microsoft.Azure.Cosmos.Table SDK を 1.0.7 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="35cec-330">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="35cec-331">DataLake Gen2 項目の一覧表示で一部の項目のみが返されたときに、ContinuationToken を使用して再度一覧表示するようにユーザーに促す警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-331">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="35cec-332">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="35cec-332">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="35cec-333">Azure Files Active Directory Domain Service 認証でのストレージ アカウントの作成または更新をサポートしました</span><span class="sxs-lookup"><span data-stu-id="35cec-333">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="35cec-334">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="35cec-334">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="35cec-335">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="35cec-335">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="35cec-336">ストレージ アカウントの Kerberos キーの新規作成または一覧表示をサポートしました</span><span class="sxs-lookup"><span data-stu-id="35cec-336">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="35cec-337">'New-AzStorageAccountKey'</span><span class="sxs-lookup"><span data-stu-id="35cec-337">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="35cec-338">'Get-AzStorageAccountKey'</span><span class="sxs-lookup"><span data-stu-id="35cec-338">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="35cec-339">ストレージ アカウントのフェールオーバーをサポートしました</span><span class="sxs-lookup"><span data-stu-id="35cec-339">Supported failover Storage account</span></span>
    - <span data-ttu-id="35cec-340">'Invoke-AzStorageAccountFailover'</span><span class="sxs-lookup"><span data-stu-id="35cec-340">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="35cec-341">'Get-AzStorageBlobCopyState' のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-341">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="35cec-342">'Get-AzStorageFileCopyState' と 'Start-AzStorageBlobCopy' のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-342">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="35cec-343">ストレージ クライアント ライブラリ v12 を Queue および File コマンドレットに統合しました</span><span class="sxs-lookup"><span data-stu-id="35cec-343">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="35cec-344">出力の種類を CloudFile から AzureStorageFile に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="35cec-344">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="35cec-345">'Get-AzStorageFile'</span><span class="sxs-lookup"><span data-stu-id="35cec-345">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="35cec-346">'Remove-AzStorageFile'</span><span class="sxs-lookup"><span data-stu-id="35cec-346">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="35cec-347">'Get-AzStorageFileContent'</span><span class="sxs-lookup"><span data-stu-id="35cec-347">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="35cec-348">'Set-AzStorageFileContent'</span><span class="sxs-lookup"><span data-stu-id="35cec-348">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="35cec-349">'Start-AzStorageFileCopy'</span><span class="sxs-lookup"><span data-stu-id="35cec-349">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="35cec-350">出力の種類を CloudFileDirectory から AzureStorageFileDirectory に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="35cec-350">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="35cec-351">'New-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="35cec-351">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="35cec-352">'Remove-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="35cec-352">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="35cec-353">出力の種類を CloudFileShare から AzureStorageFileShare に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="35cec-353">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="35cec-354">'Get-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="35cec-354">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="35cec-355">'New-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="35cec-355">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="35cec-356">'Remove-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="35cec-356">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="35cec-357">出力の種類を FileShareProperties から AzureStorageFileShare に変更しました。元の出力は新しい出力のサブの子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="35cec-357">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="35cec-358">'Set-AzStorageShareQuota'</span><span class="sxs-lookup"><span data-stu-id="35cec-358">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="35cec-359">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="35cec-359">Az.TrafficManager</span></span>
* <span data-ttu-id="35cec-360">'DisableAzureTrafficManagerEndpoint' の詳細出力の間違ったプロファイル名を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-360">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-361">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-361">Az.Websites</span></span>
* <span data-ttu-id="35cec-362">'Update-AzWebAppAccessRestrictionConfig' のヘルプの誤記を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-362">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="35cec-363">3.8.0 - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="35cec-363">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="35cec-364">前回のリリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-364">Highlights since the last release</span></span>
* <span data-ttu-id="35cec-365">Az.Storage でサポートされる PowerShell のバージョンは次のとおりです。Windows PowerShell 5.1、PowerShell Core 6.2.4+、PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="35cec-365">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-366">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-366">Az.Accounts</span></span>
* <span data-ttu-id="35cec-367">'Resolve-AzError' の Azure PowerShell アンケートの URL を更新しました [#11507]</span><span class="sxs-lookup"><span data-stu-id="35cec-367">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-368">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-368">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-369">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-369">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="35cec-370">GroupId パラメーターの指定について 'Set-AzApiManagementGroup' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-370">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-371">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-371">Az.Cdn</span></span>
* <span data-ttu-id="35cec-372">ChinaCDN 関連の価格 SKU の表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-372">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-373">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-373">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-374">ID、暗号化、UserOwnedStorage をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-374">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-375">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-375">Az.Compute</span></span>
* <span data-ttu-id="35cec-376">'Set-AzVmssOrchestrationServiceState' コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-376">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="35cec-377">'Get-AzVmss' に -InstanceView を指定することで、OrchestrationService の状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-377">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-378">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-378">Az.IotHub</span></span>
* <span data-ttu-id="35cec-379">IoT デバイス ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-379">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="35cec-380">'Get-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="35cec-380">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="35cec-381">'Update-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="35cec-381">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="35cec-382">Iot Hub のデバイスでダイレクト メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-382">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="35cec-383">IoT デバイス モジュール ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-383">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="35cec-384">'Get-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="35cec-384">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="35cec-385">'Update-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="35cec-385">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="35cec-386">IoT の自動デバイス管理構成を大規模に管理します。</span><span class="sxs-lookup"><span data-stu-id="35cec-386">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="35cec-387">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-387">New cmdlets are:</span></span>
    - <span data-ttu-id="35cec-388">'Add-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="35cec-388">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="35cec-389">'Get-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="35cec-389">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="35cec-390">'Remove-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="35cec-390">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="35cec-391">'Set-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="35cec-391">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="35cec-392">Iot Hub で edge モジュール メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-392">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-393">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-393">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-394">コンテナーでの論理的な削除と消去保護を有効にできる新しいコマンドレット 'Update-AzKeyVault' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-394">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="35cec-395">Microsoft.PowerShell.SecretManagement へのサポートを追加しました [#11178]</span><span class="sxs-lookup"><span data-stu-id="35cec-395">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="35cec-396">'Remove-AzKeyVaultManagedStorageSasDefinition' の例の誤りを修正しました [#11479]</span><span class="sxs-lookup"><span data-stu-id="35cec-396">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="35cec-397">プライベート エンドポイントへのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-397">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="35cec-398">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="35cec-398">Az.Maintenance</span></span>
* <span data-ttu-id="35cec-399">GA 用のメンテナンス コマンドレットのリリース バージョンを公開しています</span><span class="sxs-lookup"><span data-stu-id="35cec-399">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-400">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-400">Az.Monitor</span></span>
* <span data-ttu-id="35cec-401">プライベート リンク スコープのコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-401">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="35cec-402">'Get-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="35cec-402">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="35cec-403">'Remove-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="35cec-403">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="35cec-404">'New-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="35cec-404">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="35cec-405">'Update-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="35cec-405">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="35cec-406">'Get-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="35cec-406">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="35cec-407">'New-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="35cec-407">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="35cec-408">'Remove-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="35cec-408">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-409">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-409">Az.Network</span></span>
* <span data-ttu-id="35cec-410">仮想ネットワーク ゲートウェイのプライベート IP での接続を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-410">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="35cec-411">'New-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="35cec-411">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="35cec-412">'Set-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="35cec-412">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="35cec-413">'New-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="35cec-413">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="35cec-414">'Set-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="35cec-414">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="35cec-415">FQDN ベースの LocalNetworkGateways と VpnSites を有効にするコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-415">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="35cec-416">'New-AzLocalNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="35cec-416">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="35cec-417">'New-AzVpnSiteLink'</span><span class="sxs-lookup"><span data-stu-id="35cec-417">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="35cec-418">ExpressRouteCircuitConnectionConfig (Global Reach) で IPv6 アドレス ファミリのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-418">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="35cec-419">'Set-AzExpressRouteCircuitConnectionConfig' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-419">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="35cec-420">IPv6CircuitConnectionProperties を含むすべての既存のプロパティを設定できます</span><span class="sxs-lookup"><span data-stu-id="35cec-420">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="35cec-421">'Add-AzExpressRouteCircuitConnectionConfig' を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-421">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="35cec-422">アドレス プレフィックスのアドレス ファミリを指定する、別の省略可能なパラメーター AddressPrefixType を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-422">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="35cec-423">仮想ネットワーク ゲートウェイ接続で DPD タイムアウトの設定を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-423">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="35cec-424">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-424">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="35cec-425">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-425">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-426">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-426">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-427">ポリシー コンプライアンス スキャンをトリガーするための 'Start-AzPolicyComplianceScan' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-427">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="35cec-428">ポリシー定義、セット定義、および割り当てのバージョンを 'Get-AzPolicyState' 出力に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-428">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-429">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-429">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-430">'New-AzServiceFabricCluster' サンプルのコードのフォーマットと使いやすさが向上しています</span><span class="sxs-lookup"><span data-stu-id="35cec-430">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-431">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-431">Az.Sql</span></span>
* <span data-ttu-id="35cec-432">コマンドレット 'Get-AzSqlInstanceOperation' および 'Stop-AzSqlInstanceOperation' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-432">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="35cec-433">VNet のストレージ アカウントに対する監査をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-433">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-434">Az.Storage</span></span>
* <span data-ttu-id="35cec-435">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-435">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="35cec-436">ストレージ アカウントの作成/更新時に新しい SkuName StandardGZRS、StandardRAGZRS をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-436">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="35cec-437">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="35cec-437">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="35cec-438">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="35cec-438">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="35cec-439">Supported DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="35cec-439">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="35cec-440">'New-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="35cec-440">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="35cec-441">'Get-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="35cec-441">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="35cec-442">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="35cec-442">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="35cec-443">'Move-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="35cec-443">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="35cec-444">'Set-AzDataLakeGen2ItemAclObject'</span><span class="sxs-lookup"><span data-stu-id="35cec-444">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="35cec-445">'Update-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="35cec-445">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="35cec-446">'Get-AzDataLakeGen2ItemContent'</span><span class="sxs-lookup"><span data-stu-id="35cec-446">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="35cec-447">'Remove-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="35cec-447">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="35cec-448">0.10.0-preview - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="35cec-448">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="35cec-449">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-449">General</span></span>
* <span data-ttu-id="35cec-450">Az モジュールが Azure Stack Hub のプレビューで使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-450">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="35cec-451">これにより、Linux および macOS とのクロスプラットフォームの互換性が確保されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-451">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="35cec-452">Azure Stack Hub で、Az モジュールを使用した PowerShell Core がサポートされるようになりました。詳細については、[こちら](https://aka.ms/az4AzureStack)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-452">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="35cec-453">Az モジュールでプロファイル 2019-03-01-hybrid がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-453">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="35cec-454">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="35cec-454">Az.Billing</span></span>
  - <span data-ttu-id="35cec-455">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-455">Az.Compute</span></span>
  - <span data-ttu-id="35cec-456">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="35cec-456">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="35cec-457">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-457">Az.EventHub</span></span>
  - <span data-ttu-id="35cec-458">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-458">Az.IotHub</span></span>
  - <span data-ttu-id="35cec-459">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-459">Az.KeyVault</span></span>
  - <span data-ttu-id="35cec-460">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-460">Az.Monitor</span></span>
  - <span data-ttu-id="35cec-461">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-461">Az.Network</span></span>
  - <span data-ttu-id="35cec-462">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-462">Az.Resources</span></span>
  - <span data-ttu-id="35cec-463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-463">Az.Storage</span></span>
  - <span data-ttu-id="35cec-464">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-464">Az.Websites</span></span>
* <span data-ttu-id="35cec-465">Azure Stack Hubで動作する、Az 用の 3 つの新しい PowerShell モジュール (Az.Databox、Az.IotHub、Az.EventHu) が導入されました</span><span class="sxs-lookup"><span data-stu-id="35cec-465">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="35cec-466">コマンドは比較的同じままですが、AzureRM を Az に変更するなどの軽微な変更が加えられています</span><span class="sxs-lookup"><span data-stu-id="35cec-466">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="35cec-467">Azure Stack Hub の PowerShell ドキュメントへのリンクを更新しました。[こちら](https://aka.ms/InstallASHPowerShell)で確認できます</span><span class="sxs-lookup"><span data-stu-id="35cec-467">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="35cec-468">3.7.0 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="35cec-468">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-469">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-469">Az.Accounts</span></span>
* <span data-ttu-id="35cec-470">ログインしていない場合に、'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' が NullReferenceException をスローする問題を修正しました [#10292]</span><span class="sxs-lookup"><span data-stu-id="35cec-470">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-471">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-471">Az.Compute</span></span>
* <span data-ttu-id="35cec-472">'New-AzDiskConfig' コマンドレットに次のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-472">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="35cec-473">DiskIOPSReadOnly、DiskMBpsReadOnly、MaxSharesCount、GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="35cec-473">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="35cec-474">'New-AzGalleryImageVersion' コマンドレットの Target パラメーターで Encryption プロパティを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-474">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="35cec-475">'Set-AzVmss' の -Reimage と 'Invoke-AzVMReimage' コマンドレットの tempDisk の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-475">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="35cec-476">[#11354]</span><span class="sxs-lookup"><span data-stu-id="35cec-476">[#11354]</span></span>
* <span data-ttu-id="35cec-477">新しい SAP 拡張機能の次のコマンドレットに対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-477">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="35cec-478">'Set-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="35cec-478">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="35cec-479">'Get-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="35cec-479">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="35cec-480">'Remove-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="35cec-480">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="35cec-481">'Update-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="35cec-481">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="35cec-482">ヘルプ ドキュメントの例の誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-482">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="35cec-483">VM PowerState の正確な文字列値をテーブル形式で示しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-483">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="35cec-484">'New-AzVmssConfig': SinglePlacementGroup が無効な場合の AutomaticRepairs プロパティのシリアル化を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-484">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="35cec-485">[#11257]</span><span class="sxs-lookup"><span data-stu-id="35cec-485">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-486">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-486">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-487">ADF .Net SDK のバージョンを 4.8.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-487">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="35cec-488">再実行をサポートするために、'Invoke-AzDataFactoryV2Pipeline' コマンドに省略可能なパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-488">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-489">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-489">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-490">'Export-AzDataLakeStoreItem' と 'Import-AzDataLakeStoreItem' に破壊的変更の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-490">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="35cec-491">'New-AzDataLakeStoreItem'、'Add-AzDAtaLakeStoreItemContent'、および 'Get-AzDAtaLakeStoreItemContent' にバイト エンコードのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-491">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-492">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-492">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-493">クラスターの作成時に、最低限サポートされている TLS バージョンの指定をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-493">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-494">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-494">Az.IotHub</span></span>
* <span data-ttu-id="35cec-495">デバイスごとの分散設定の管理のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-495">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="35cec-496">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-496">New Cmdlets are:</span></span>
    - <span data-ttu-id="35cec-497">'Get-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="35cec-497">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="35cec-498">'Set-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="35cec-498">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-499">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-499">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-500">'New-AzKeyVault' に破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-500">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-501">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-501">Az.Monitor</span></span>
* <span data-ttu-id="35cec-502">'New-AzScheduledQueryRuleLogMetricTrigger' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-502">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-503">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-503">Az.Network</span></span>
* <span data-ttu-id="35cec-504">テナント間の VirtualHubVnetConnections を許可するためにコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-504">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="35cec-505">'New-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="35cec-505">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="35cec-506">'Update-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="35cec-506">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="35cec-507">'New-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="35cec-507">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="35cec-508">'Update-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="35cec-508">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="35cec-509">SQL 管理 SDK の依存関係を削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-509">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-510">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-510">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-511">エラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-511">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-512">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-512">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-513">Azure Site Recovery で再保護を行うためのサポートを追加し、Azure Disk Encryption を使用して暗号化されている Virtual Machines の vm プロパティを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-513">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="35cec-514">Azure Site Recovery に VmwareToAzure プロパティの DR 監視を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-514">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="35cec-515">Azure Backup に、失敗した項目の再試行ポリシー更新のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-515">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="35cec-516">Azure Backup に、バックアップおよび復元中のディスク除外設定のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-516">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="35cec-517">Azure Backup に、AzureFileShare で複数ファイル/フォルダーを復元するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-517">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="35cec-518">Azure Backup に、IaasVM ポリシーの更新中にユーザーによって指定された Resourcegroup へのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-518">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-519">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-519">Az.Resources</span></span>
* <span data-ttu-id="35cec-520">既定の apiVersion ではなく、リソースの実際の apiVersion を使用するように 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' を修正しました [#11267]</span><span class="sxs-lookup"><span data-stu-id="35cec-520">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="35cec-521">エラー シナリオでの correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-521">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="35cec-522">'Get-AzResourceLock' のドキュメントをわずかに変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-522">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="35cec-523">例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-523">Added example.</span></span>
* <span data-ttu-id="35cec-524">'Get-AzADUser' のパラメーター値の単一引用符をエスケープしました [#11317]</span><span class="sxs-lookup"><span data-stu-id="35cec-524">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="35cec-525">デプロイ スクリプト ('Get-AzDeploymentScript'、'Get-AzDeploymentScriptLog'、'Save-AzDeploymentScriptLog'、'Remove-AzDeploymentScript') に新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-525">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-526">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-526">Az.Sql</span></span>
* <span data-ttu-id="35cec-527">'Invoke-AzSqlDatabaseFailover' に読み取り可能なセカンダリ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-527">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="35cec-528">コマンドレット 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-528">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="35cec-529">データベース内の列を分類するときの秘密度ランクを保存しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-529">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="35cec-530">Az.Support</span><span class="sxs-lookup"><span data-stu-id="35cec-530">Az.Support</span></span>
* <span data-ttu-id="35cec-531">'Az.Support' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-531">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-532">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-532">Az.Websites</span></span>
* <span data-ttu-id="35cec-533">次の新しいコマンドレットを使用して、webapp トラフィック ルーティング規則を処理するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-533">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="35cec-534">'Get-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="35cec-534">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="35cec-535">'Update-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="35cec-535">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="35cec-536">'Add-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="35cec-536">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="35cec-537">'Remove-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="35cec-537">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="35cec-538">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="35cec-538">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-539">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-539">Az.Accounts</span></span>
* <span data-ttu-id="35cec-540">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="35cec-540">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="35cec-541">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="35cec-541">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="35cec-542">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-542">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-543">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-543">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-544">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="35cec-544">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="35cec-545">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="35cec-545">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="35cec-546">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-546">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="35cec-547">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="35cec-547">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-548">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-548">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-549">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-549">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-550">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-550">Az.IotHub</span></span>
* <span data-ttu-id="35cec-551">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-551">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="35cec-552">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-552">New Cmdlets are:</span></span>
    - <span data-ttu-id="35cec-553">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-553">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-554">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-554">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-555">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-555">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-556">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-556">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="35cec-557">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-557">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="35cec-558">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-558">New Cmdlets are:</span></span>
    - <span data-ttu-id="35cec-559">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="35cec-559">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="35cec-560">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="35cec-560">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="35cec-561">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="35cec-561">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="35cec-562">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="35cec-562">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="35cec-563">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-563">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="35cec-564">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-564">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="35cec-565">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-565">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="35cec-566">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-566">New Cmdlets are:</span></span>
    - <span data-ttu-id="35cec-567">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="35cec-567">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="35cec-568">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="35cec-568">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="35cec-569">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-569">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-570">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-570">Az.Monitor</span></span>
* <span data-ttu-id="35cec-571">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="35cec-571">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-572">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-572">Az.Network</span></span>
* <span data-ttu-id="35cec-573">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-573">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="35cec-574">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-574">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="35cec-575">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="35cec-575">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="35cec-576">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-576">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-577">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-577">Az.Resources</span></span>
* <span data-ttu-id="35cec-578">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-578">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="35cec-579">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="35cec-579">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="35cec-580">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="35cec-580">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="35cec-581">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="35cec-581">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="35cec-582">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-582">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="35cec-583">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-583">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="35cec-584">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-584">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="35cec-585">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="35cec-585">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="35cec-586">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="35cec-586">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="35cec-587">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="35cec-587">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="35cec-588">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="35cec-588">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="35cec-589">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-589">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="35cec-590">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="35cec-590">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="35cec-591">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="35cec-591">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-592">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-592">Az.Sql</span></span>
* <span data-ttu-id="35cec-593">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-593">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="35cec-594">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-594">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="35cec-595">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="35cec-595">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="35cec-596">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-596">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="35cec-597">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-597">Remove an LTR backup</span></span>
    - <span data-ttu-id="35cec-598">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-598">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="35cec-599">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-599">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="35cec-600">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-600">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="35cec-601">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="35cec-601">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-602">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-602">Az.Storage</span></span>
* <span data-ttu-id="35cec-603">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-603">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="35cec-604">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="35cec-604">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="35cec-605">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-605">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="35cec-606">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="35cec-606">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="35cec-607">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="35cec-607">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-608">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-608">Az.Websites</span></span>
* <span data-ttu-id="35cec-609">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-609">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="35cec-610">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="35cec-610">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="35cec-611">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-611">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="35cec-612">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="35cec-612">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="35cec-613">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-613">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="35cec-614">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="35cec-614">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-615">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-615">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-616">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-616">Updated client side telemetry.</span></span>
* <span data-ttu-id="35cec-617">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-617">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="35cec-618">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-618">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-619">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-619">Az.Accounts</span></span>
* <span data-ttu-id="35cec-620">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-620">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-621">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-621">Az.Automation</span></span>
* <span data-ttu-id="35cec-622">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-622">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-623">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-623">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-624">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-624">Updated SDK to 7.0</span></span>
* <span data-ttu-id="35cec-625">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-625">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-626">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-626">Az.Compute</span></span>
* <span data-ttu-id="35cec-627">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-627">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-628">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-628">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-629">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-629">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-630">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-630">Az.IotHub</span></span>
* <span data-ttu-id="35cec-631">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-631">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="35cec-632">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-632">New Cmdlets are:</span></span>
    - <span data-ttu-id="35cec-633">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-633">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-634">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-634">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-635">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-635">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="35cec-636">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="35cec-636">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-637">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-637">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-638">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-638">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-639">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-639">Az.Monitor</span></span>
* <span data-ttu-id="35cec-640">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-640">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="35cec-641">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-641">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="35cec-642">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-642">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-643">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-643">Az.Network</span></span>
* <span data-ttu-id="35cec-644">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-644">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="35cec-645">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-645">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="35cec-646">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-646">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="35cec-647">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-647">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="35cec-648">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="35cec-648">No new cmdlets are added.</span></span> <span data-ttu-id="35cec-649">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="35cec-649">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-650">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-650">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-651">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-651">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-652">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-652">Az.Resources</span></span>
* <span data-ttu-id="35cec-653">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="35cec-653">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="35cec-654">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="35cec-654">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="35cec-655">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="35cec-655">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="35cec-656">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-656">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="35cec-657">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-657">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="35cec-658">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-658">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="35cec-659">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-659">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="35cec-660">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-660">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-661">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-661">Az.Sql</span></span>
* <span data-ttu-id="35cec-662">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-662">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="35cec-663">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-663">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="35cec-664">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="35cec-664">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="35cec-665">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="35cec-665">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="35cec-666">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-666">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="35cec-667">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="35cec-667">Az.StorageSync</span></span>
* <span data-ttu-id="35cec-668">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-668">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="35cec-669">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="35cec-669">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-670">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-670">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-671">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="35cec-671">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="35cec-672">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-672">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-673">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-673">Az.Accounts</span></span>
* <span data-ttu-id="35cec-674">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="35cec-674">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="35cec-675">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-675">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-676">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-676">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-677">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="35cec-677">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="35cec-678">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="35cec-678">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="35cec-679">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-679">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="35cec-680">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-680">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-681">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-681">Az.Compute</span></span>
* <span data-ttu-id="35cec-682">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="35cec-682">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="35cec-683">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-683">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="35cec-684">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-684">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="35cec-685">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-685">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="35cec-686">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-686">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-687">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-687">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-688">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-688">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="35cec-689">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="35cec-689">Az.DeploymentManager</span></span>
* <span data-ttu-id="35cec-690">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-690">Adds LIST operations for resources</span></span>
* <span data-ttu-id="35cec-691">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-691">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-692">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-692">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-693">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-693">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-694">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-694">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-695">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="35cec-695">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-696">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-696">Az.Network</span></span>
* <span data-ttu-id="35cec-697">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-697">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="35cec-698">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="35cec-698">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="35cec-699">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="35cec-699">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="35cec-700">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-700">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="35cec-701">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="35cec-701">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="35cec-702">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-702">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="35cec-703">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-703">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="35cec-704">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-704">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="35cec-705">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-705">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-706">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-706">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="35cec-707">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-707">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="35cec-708">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="35cec-708">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="35cec-709">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-709">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-710">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-710">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-711">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-711">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="35cec-712">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-712">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="35cec-713">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-713">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="35cec-714">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-714">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-715">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-715">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-716">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-716">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="35cec-717">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-717">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-718">Az.Resources</span></span>
* <span data-ttu-id="35cec-719">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="35cec-719">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="35cec-720">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-720">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-721">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-721">Az.Sql</span></span>
<span data-ttu-id="35cec-722">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-722">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-723">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-723">Az.Storage</span></span>
* <span data-ttu-id="35cec-724">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-724">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="35cec-725">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-725">New-AzStorageAccount</span></span>
* <span data-ttu-id="35cec-726">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="35cec-726">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="35cec-727">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-727">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-728">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-728">Az.Websites</span></span>
* <span data-ttu-id="35cec-729">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-729">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="35cec-730">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-730">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="35cec-731">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="35cec-731">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-732">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-732">Az.Accounts</span></span>
* <span data-ttu-id="35cec-733">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-733">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-734">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-734">Az.Cdn</span></span>
* <span data-ttu-id="35cec-735">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="35cec-735">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-736">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-736">Az.Compute</span></span>
* <span data-ttu-id="35cec-737">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-737">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="35cec-738">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-738">Az.ContainerInstance</span></span>
* <span data-ttu-id="35cec-739">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-739">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="35cec-740">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="35cec-740">Az.DataBoxEdge</span></span>
* <span data-ttu-id="35cec-741">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-741">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="35cec-742">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-742">Get the Edge Storage Container</span></span>
* <span data-ttu-id="35cec-743">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-743">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="35cec-744">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-744">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="35cec-745">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-745">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="35cec-746">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-746">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="35cec-747">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-747">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="35cec-748">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="35cec-748">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="35cec-749">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-749">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="35cec-750">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-750">Get the Edge Storage Account</span></span>
* <span data-ttu-id="35cec-751">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-751">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="35cec-752">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-752">Create new Edge Storage Account</span></span>
* <span data-ttu-id="35cec-753">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-753">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="35cec-754">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-754">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="35cec-755">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="35cec-755">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="35cec-756">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="35cec-756">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="35cec-757">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-757">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="35cec-758">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="35cec-758">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-759">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-759">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-760">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-760">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="35cec-761">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-761">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="35cec-762">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="35cec-762">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="35cec-763">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="35cec-763">Az.DevTestLabs</span></span>
* <span data-ttu-id="35cec-764">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-764">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-765">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-765">Az.EventHub</span></span>
* <span data-ttu-id="35cec-766">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-766">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-767">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-767">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-768">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-768">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="35cec-769">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="35cec-769">Az.MachineLearning</span></span>
* <span data-ttu-id="35cec-770">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-770">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="35cec-771">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="35cec-771">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="35cec-772">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="35cec-772">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="35cec-773">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="35cec-773">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="35cec-774">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="35cec-774">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="35cec-775">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="35cec-775">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="35cec-776">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="35cec-776">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="35cec-777">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="35cec-777">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-778">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-778">Az.Network</span></span>
* <span data-ttu-id="35cec-779">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="35cec-779">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-780">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-780">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-781">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="35cec-781">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="35cec-782">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-782">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="35cec-783">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-783">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="35cec-784">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-784">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-785">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-785">Az.Resources</span></span>
* <span data-ttu-id="35cec-786">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-786">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-787">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-787">Az.Sql</span></span>
* <span data-ttu-id="35cec-788">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-788">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="35cec-789">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-789">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="35cec-790">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="35cec-790">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="35cec-791">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-791">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-792">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-792">Az.Storage</span></span>
* <span data-ttu-id="35cec-793">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-793">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="35cec-794">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-794">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="35cec-795">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-795">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="35cec-796">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-796">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="35cec-797">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="35cec-797">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="35cec-798">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-798">General</span></span>
* <span data-ttu-id="35cec-799">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-799">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-800">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-800">Az.Accounts</span></span>
* <span data-ttu-id="35cec-801">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="35cec-801">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="35cec-802">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="35cec-802">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-803">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-803">Az.Batch</span></span>
* <span data-ttu-id="35cec-804">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="35cec-804">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-805">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-805">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-806">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-806">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-807">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-807">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-808">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-808">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="35cec-809">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-809">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="35cec-810">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="35cec-810">Az.HealthcareApis</span></span>
* <span data-ttu-id="35cec-811">例外処理</span><span class="sxs-lookup"><span data-stu-id="35cec-811">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-812">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-812">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-813">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-813">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="35cec-814">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="35cec-814">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="35cec-815">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-815">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-816">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-816">Az.Monitor</span></span>
* <span data-ttu-id="35cec-817">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="35cec-817">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="35cec-818">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="35cec-818">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="35cec-819">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="35cec-819">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-820">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-820">Az.Network</span></span>
* <span data-ttu-id="35cec-821">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-821">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-822">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-822">Az.Resources</span></span>
* <span data-ttu-id="35cec-823">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-823">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="35cec-824">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-824">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-825">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-825">Az.Sql</span></span>
* <span data-ttu-id="35cec-826">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="35cec-826">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-827">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-827">Az.Storage</span></span>
* <span data-ttu-id="35cec-828">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-828">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="35cec-829">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="35cec-829">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="35cec-830">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="35cec-830">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="35cec-831">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="35cec-831">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="35cec-832">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="35cec-832">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="35cec-833">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-833">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="35cec-834">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-834">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="35cec-835">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-835">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="35cec-836">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-836">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="35cec-837">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-837">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="35cec-838">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="35cec-838">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="35cec-839">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-839">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="35cec-840">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="35cec-840">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="35cec-841">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="35cec-841">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-842">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-842">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-843">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="35cec-843">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="35cec-844">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="35cec-844">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-845">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-845">Az.Compute</span></span>
* <span data-ttu-id="35cec-846">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="35cec-846">VM Reapply feature</span></span>
    - <span data-ttu-id="35cec-847">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-847">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="35cec-848">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="35cec-848">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="35cec-849">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="35cec-849">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="35cec-850">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="35cec-850">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="35cec-851">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-851">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="35cec-852">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-852">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="35cec-853">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="35cec-853">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="35cec-854">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-854">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="35cec-855">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-855">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="35cec-856">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-856">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="35cec-857">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="35cec-857">Az.DataBoxEdge</span></span>
* <span data-ttu-id="35cec-858">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-858">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="35cec-859">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-859">Get the Order</span></span>
* <span data-ttu-id="35cec-860">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-860">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="35cec-861">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-861">Create new Order</span></span>
* <span data-ttu-id="35cec-862">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-862">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="35cec-863">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-863">Remove the Order</span></span>
* <span data-ttu-id="35cec-864">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="35cec-864">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="35cec-865">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="35cec-865">Now creates Local Share</span></span>
* <span data-ttu-id="35cec-866">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-866">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="35cec-867">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-867">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="35cec-868">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-868">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="35cec-869">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="35cec-869">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="35cec-870">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-870">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="35cec-871">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-871">Gets the information about Triggers</span></span>
* <span data-ttu-id="35cec-872">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-872">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="35cec-873">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-873">Create new Triggers</span></span>
* <span data-ttu-id="35cec-874">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-874">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="35cec-875">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-875">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-876">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-876">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-877">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-877">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="35cec-878">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-878">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-879">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-879">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-880">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-880">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-881">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-881">Az.EventHub</span></span>
* <span data-ttu-id="35cec-882">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-882">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-883">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-883">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-884">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-884">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="35cec-885">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-885">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="35cec-886">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-886">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="35cec-887">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="35cec-887">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-888">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-888">Az.Network</span></span>
* <span data-ttu-id="35cec-889">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="35cec-889">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="35cec-890">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="35cec-890">Az.PrivateDns</span></span>
* <span data-ttu-id="35cec-891">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-891">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-892">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-892">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-893">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-893">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="35cec-894">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="35cec-894">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="35cec-895">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-895">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="35cec-896">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="35cec-896">Az.RedisCache</span></span>
* <span data-ttu-id="35cec-897">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-897">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="35cec-898">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-898">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="35cec-899">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-899">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-900">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-900">Az.Resources</span></span>
- <span data-ttu-id="35cec-901">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-901">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="35cec-902">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-902">Updated create policy definition help example</span></span>
- <span data-ttu-id="35cec-903">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-903">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="35cec-904">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-904">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="35cec-905">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="35cec-905">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-906">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-906">Az.Sql</span></span>
* <span data-ttu-id="35cec-907">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-907">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="35cec-908">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-908">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="35cec-909">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="35cec-909">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="35cec-910">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-910">General</span></span>
* <span data-ttu-id="35cec-911">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="35cec-911">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-912">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-912">Az.Accounts</span></span>
* <span data-ttu-id="35cec-913">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-913">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="35cec-914">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="35cec-914">Az.Advisor</span></span>
* <span data-ttu-id="35cec-915">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-915">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-916">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-916">Az.Batch</span></span>
* <span data-ttu-id="35cec-917">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-917">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="35cec-918">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="35cec-918">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="35cec-919">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="35cec-919">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="35cec-920">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-920">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="35cec-921">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="35cec-921">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="35cec-922">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-922">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="35cec-923">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-923">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="35cec-924">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-924">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="35cec-925">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-925">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="35cec-926">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-926">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="35cec-927">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-927">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="35cec-928">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="35cec-928">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="35cec-929">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-929">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="35cec-930">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-930">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="35cec-931">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-931">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="35cec-932">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-932">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="35cec-933">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-933">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="35cec-934">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-934">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="35cec-935">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-935">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="35cec-936">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35cec-936">This operation is no longer supported.</span></span>
* <span data-ttu-id="35cec-937">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-937">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="35cec-938">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-938">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="35cec-939">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-939">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="35cec-940">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="35cec-940">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="35cec-941">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="35cec-941">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="35cec-942">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-942">New non-verified images are also now returned.</span></span> <span data-ttu-id="35cec-943">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="35cec-943">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="35cec-944">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-944">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="35cec-945">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-945">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="35cec-946">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="35cec-946">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="35cec-947">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-947">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="35cec-948">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-948">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="35cec-949">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-949">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="35cec-950">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-950">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="35cec-951">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="35cec-951">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="35cec-952">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="35cec-952">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-953">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-953">Az.Cdn</span></span>
* <span data-ttu-id="35cec-954">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-954">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="35cec-955">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-955">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-956">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-956">Az.Compute</span></span>
* <span data-ttu-id="35cec-957">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="35cec-957">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="35cec-958">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="35cec-958">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="35cec-959">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。 Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile、Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="35cec-959">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="35cec-960">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-960">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="35cec-961">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-961">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="35cec-962">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="35cec-962">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="35cec-963">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-963">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="35cec-964">重大な変更</span><span class="sxs-lookup"><span data-stu-id="35cec-964">Breaking changes</span></span>
    - <span data-ttu-id="35cec-965">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="35cec-965">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="35cec-966">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="35cec-966">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-967">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-967">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-968">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-968">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-969">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-969">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-970">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="35cec-970">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="35cec-971">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="35cec-971">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="35cec-972">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="35cec-972">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="35cec-973">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-973">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="35cec-974">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-974">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="35cec-975">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-975">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-976">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-976">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-977">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-977">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-978">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-978">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-979">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-979">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="35cec-980">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="35cec-980">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="35cec-981">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-981">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="35cec-982">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-982">Removed five cmdlets:</span></span>
    - <span data-ttu-id="35cec-983">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="35cec-983">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="35cec-984">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="35cec-984">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="35cec-985">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="35cec-985">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="35cec-986">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="35cec-986">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="35cec-987">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="35cec-987">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="35cec-988">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-988">Added three cmdlets:</span></span>
    - <span data-ttu-id="35cec-989">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="35cec-989">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="35cec-990">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="35cec-990">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="35cec-991">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="35cec-991">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="35cec-992">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-992">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="35cec-993">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-993">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="35cec-994">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-994">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="35cec-995">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="35cec-995">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="35cec-996">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-996">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="35cec-997">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-997">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="35cec-998">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-998">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="35cec-999">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-999">Added some scenario test cases.</span></span>
* <span data-ttu-id="35cec-1000">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="35cec-1000">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-1001">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1001">Az.IotHub</span></span>
* <span data-ttu-id="35cec-1002">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="35cec-1002">Breaking changes:</span></span>
    - <span data-ttu-id="35cec-1003">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1003">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="35cec-1004">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1004">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="35cec-1005">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1005">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="35cec-1006">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1006">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="35cec-1007">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1007">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="35cec-1008">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1008">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="35cec-1009">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1009">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="35cec-1010">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1010">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="35cec-1011">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1011">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="35cec-1012">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1012">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="35cec-1013">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1013">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="35cec-1014">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1014">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1015">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1015">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1016">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1016">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1017">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1017">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="35cec-1018">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1018">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="35cec-1019">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1019">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1020">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1020">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1021">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1021">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1022">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1022">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1023">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1023">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1024">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1024">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1025">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1025">Az.Resources</span></span>
* <span data-ttu-id="35cec-1026">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1026">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1027">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1027">Az.Network</span></span>
* <span data-ttu-id="35cec-1028">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1028">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="35cec-1029">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1029">Updated cmdlet:</span></span>
        - <span data-ttu-id="35cec-1030">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1030">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1031">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1031">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1032">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1032">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1033">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1033">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1034">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1034">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="35cec-1035">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="35cec-1035">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="35cec-1036">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1036">New cmdlet:</span></span>
        - <span data-ttu-id="35cec-1037">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="35cec-1037">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="35cec-1038">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1038">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="35cec-1039">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1039">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="35cec-1040">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1040">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="35cec-1041">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1041">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="35cec-1042">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1042">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="35cec-1043">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1043">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="35cec-1044">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1044">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="35cec-1045">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-1045">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-1046">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="35cec-1046">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="35cec-1047">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-1047">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="35cec-1048">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-1048">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="35cec-1049">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-1049">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="35cec-1050">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1050">Set-AzVirtualHub</span></span>
* <span data-ttu-id="35cec-1051">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1051">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="35cec-1052">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-1052">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="35cec-1053">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1053">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="35cec-1054">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1054">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="35cec-1055">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1055">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="35cec-1056">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1056">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="35cec-1057">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1057">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="35cec-1058">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-1058">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-1059">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1059">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="35cec-1060">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-1060">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="35cec-1061">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1061">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="35cec-1062">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1062">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="35cec-1063">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1063">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="35cec-1064">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1064">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="35cec-1065">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1065">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="35cec-1066">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1066">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="35cec-1067">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-1067">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-1068">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="35cec-1068">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="35cec-1069">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="35cec-1069">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="35cec-1070">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="35cec-1070">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="35cec-1071">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="35cec-1071">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="35cec-1072">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1072">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="35cec-1073">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-1073">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="35cec-1074">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-1074">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="35cec-1075">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1075">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="35cec-1076">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1076">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="35cec-1077">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1077">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="35cec-1078">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1078">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="35cec-1079">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-1079">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="35cec-1080">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1080">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="35cec-1081">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1081">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="35cec-1082">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1082">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="35cec-1083">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1083">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="35cec-1084">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1084">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="35cec-1085">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-1085">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-1086">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1086">New-AzIpGroup</span></span>
        - <span data-ttu-id="35cec-1087">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1087">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="35cec-1088">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1088">Get-AzIpGroup</span></span>
        - <span data-ttu-id="35cec-1089">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1089">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-1090">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1090">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-1091">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="35cec-1091">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1092">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1092">Az.Sql</span></span>
* <span data-ttu-id="35cec-1093">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1093">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="35cec-1094">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1094">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="35cec-1095">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1095">Removed deprecated aliases:</span></span>
* <span data-ttu-id="35cec-1096">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="35cec-1096">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="35cec-1097">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="35cec-1097">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="35cec-1098">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1098">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="35cec-1099">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1099">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="35cec-1100">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="35cec-1100">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="35cec-1101">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1101">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1102">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1102">Az.Storage</span></span>
* <span data-ttu-id="35cec-1103">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-1103">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="35cec-1104">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1104">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="35cec-1105">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1105">Set-AzStorageAccount</span></span>
* <span data-ttu-id="35cec-1106">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="35cec-1106">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="35cec-1107">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="35cec-1107">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="35cec-1108">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="35cec-1108">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="35cec-1109">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1109">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="35cec-1110">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-1110">General</span></span>
* <span data-ttu-id="35cec-1111">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="35cec-1111">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-1112">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1112">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1113">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1113">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-1114">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-1114">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-1115">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1115">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="35cec-1116">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="35cec-1116">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1117">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1117">Az.Automation</span></span>
* <span data-ttu-id="35cec-1118">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1118">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-1119">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-1119">Az.Batch</span></span>
* <span data-ttu-id="35cec-1120">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1120">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1121">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1121">Az.Compute</span></span>
* <span data-ttu-id="35cec-1122">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1122">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="35cec-1123">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1123">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="35cec-1124">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1124">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="35cec-1125">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1125">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1126">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1126">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1127">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="35cec-1127">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="35cec-1128">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="35cec-1128">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="35cec-1129">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1129">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-1130">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-1130">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-1131">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1131">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="35cec-1132">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="35cec-1132">Az.HealthcareApis</span></span>
* <span data-ttu-id="35cec-1133">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1133">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="35cec-1134">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1134">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="35cec-1135">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1135">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="35cec-1136">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1136">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-1137">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1137">Az.IotHub</span></span>
* <span data-ttu-id="35cec-1138">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="35cec-1138">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="35cec-1139">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="35cec-1139">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1140">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1140">Az.Monitor</span></span>
* <span data-ttu-id="35cec-1141">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="35cec-1141">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="35cec-1142">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1142">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="35cec-1143">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="35cec-1143">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="35cec-1144">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1144">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1145">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1145">Az.Network</span></span>
* <span data-ttu-id="35cec-1146">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1146">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="35cec-1147">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1147">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="35cec-1148">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-1148">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-1149">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-1149">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="35cec-1150">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1150">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="35cec-1151">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1151">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="35cec-1152">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1152">Updated cmdlets:</span></span>
        - <span data-ttu-id="35cec-1153">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1153">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="35cec-1154">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1154">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="35cec-1155">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1155">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="35cec-1156">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="35cec-1156">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="35cec-1157">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="35cec-1157">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="35cec-1158">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1158">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="35cec-1159">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1159">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="35cec-1160">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="35cec-1160">Az.RedisCache</span></span>
* <span data-ttu-id="35cec-1161">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1161">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1162">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1162">Az.Sql</span></span>
* <span data-ttu-id="35cec-1163">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1163">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1164">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1164">Az.Storage</span></span>
* <span data-ttu-id="35cec-1165">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="35cec-1165">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="35cec-1166">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="35cec-1166">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="35cec-1167">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="35cec-1167">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="35cec-1168">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="35cec-1168">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="35cec-1169">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1169">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="35cec-1170">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="35cec-1170">Az.StorageSync</span></span>
* <span data-ttu-id="35cec-1171">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1171">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1172">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1172">Az.Websites</span></span>
* <span data-ttu-id="35cec-1173">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="35cec-1173">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="35cec-1174">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1174">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="35cec-1175">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-1175">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-1176">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1176">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="35cec-1177">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1177">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="35cec-1178">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="35cec-1178">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1179">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1179">Az.Automation</span></span>
* <span data-ttu-id="35cec-1180">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1180">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="35cec-1181">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1181">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="35cec-1182">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1182">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1183">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1183">Az.Compute</span></span>
* <span data-ttu-id="35cec-1184">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1184">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="35cec-1185">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1185">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="35cec-1186">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1186">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="35cec-1187">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1187">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="35cec-1188">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1188">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="35cec-1189">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1189">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="35cec-1190">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1190">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="35cec-1191">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1191">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="35cec-1192">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1192">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1193">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1193">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1194">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1194">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="35cec-1195">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1195">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-1196">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-1196">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-1197">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="35cec-1197">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-1198">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1198">Az.IotHub</span></span>
* <span data-ttu-id="35cec-1199">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1199">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="35cec-1200">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1200">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="35cec-1201">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="35cec-1201">New cmdlets are:</span></span>
    - <span data-ttu-id="35cec-1202">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="35cec-1202">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="35cec-1203">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="35cec-1203">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="35cec-1204">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="35cec-1204">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="35cec-1205">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="35cec-1205">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1206">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1206">Az.Monitor</span></span>
* <span data-ttu-id="35cec-1207">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="35cec-1207">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="35cec-1208">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1208">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="35cec-1209">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="35cec-1209">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="35cec-1210">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1210">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="35cec-1211">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1211">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="35cec-1212">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1212">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="35cec-1213">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="35cec-1213">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="35cec-1214">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="35cec-1214">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="35cec-1215">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1215">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="35cec-1216">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1216">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="35cec-1217">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1217">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="35cec-1218">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="35cec-1218">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="35cec-1219">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1219">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="35cec-1220">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1220">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="35cec-1221">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1221">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="35cec-1222">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="35cec-1222">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="35cec-1223">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1223">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="35cec-1224">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1224">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="35cec-1225">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1225">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="35cec-1226">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1226">Overall improved help files</span></span>
* <span data-ttu-id="35cec-1227">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1227">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1228">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1228">Az.Network</span></span>
* <span data-ttu-id="35cec-1229">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1229">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="35cec-1230">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1230">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="35cec-1231">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1231">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="35cec-1232">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1232">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="35cec-1233">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1233">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="35cec-1234">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1234">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="35cec-1235">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1235">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="35cec-1236">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1236">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="35cec-1237">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1237">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="35cec-1238">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1238">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="35cec-1239">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1239">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="35cec-1240">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1240">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="35cec-1241">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1241">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1242">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="35cec-1242">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="35cec-1243">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1243">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="35cec-1244">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1244">Updated cmdlet:</span></span>
        - <span data-ttu-id="35cec-1245">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="35cec-1245">New-VpnSite</span></span>
        - <span data-ttu-id="35cec-1246">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="35cec-1246">Update-VpnSite</span></span>
        - <span data-ttu-id="35cec-1247">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1247">New-VpnConnection</span></span>
        - <span data-ttu-id="35cec-1248">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1248">Update-VpnConnection</span></span>
* <span data-ttu-id="35cec-1249">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1249">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1250">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1250">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1251">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1251">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="35cec-1252">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1252">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1253">Az.Resources</span></span>
* <span data-ttu-id="35cec-1254">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1254">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-1255">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1255">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-1256">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1256">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="35cec-1257">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1257">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="35cec-1258">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="35cec-1258">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="35cec-1259">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="35cec-1259">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="35cec-1260">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="35cec-1260">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="35cec-1261">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="35cec-1261">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="35cec-1262">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="35cec-1262">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="35cec-1263">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="35cec-1263">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="35cec-1264">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="35cec-1264">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="35cec-1265">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="35cec-1265">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="35cec-1266">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="35cec-1266">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="35cec-1267">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="35cec-1267">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="35cec-1268">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="35cec-1268">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="35cec-1269">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="35cec-1269">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="35cec-1270">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="35cec-1270">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="35cec-1271">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1271">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="35cec-1272">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="35cec-1272">Az.SignalR</span></span>
* <span data-ttu-id="35cec-1273">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="35cec-1273">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1274">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1274">Az.Sql</span></span>
* <span data-ttu-id="35cec-1275">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1275">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="35cec-1276">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1276">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="35cec-1277">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1277">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="35cec-1278">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1278">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="35cec-1279">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="35cec-1279">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1280">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1280">Az.Storage</span></span>
* <span data-ttu-id="35cec-1281">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1281">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="35cec-1282">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-1282">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="35cec-1283">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="35cec-1283">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="35cec-1284">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="35cec-1284">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="35cec-1285">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1285">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="35cec-1286">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="35cec-1286">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="35cec-1287">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-1287">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="35cec-1288">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-1288">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="35cec-1289">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-1289">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="35cec-1290">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-1290">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="35cec-1291">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="35cec-1291">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1292">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1292">Az.Websites</span></span>
* <span data-ttu-id="35cec-1293">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1293">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="35cec-1294">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="35cec-1294">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="35cec-1295">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1295">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="35cec-1296">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1296">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="35cec-1297">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-1297">General</span></span>
* <span data-ttu-id="35cec-1298">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1298">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-1299">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1299">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1300">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="35cec-1300">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="35cec-1301">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="35cec-1301">Az.Aks</span></span>
* <span data-ttu-id="35cec-1302">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1302">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="35cec-1303">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="35cec-1303">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-1304">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-1304">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-1305">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="35cec-1305">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="35cec-1306">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="35cec-1306">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="35cec-1307">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1307">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="35cec-1308">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="35cec-1308">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="35cec-1309">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1309">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-1310">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-1310">Az.Batch</span></span>
* <span data-ttu-id="35cec-1311">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1311">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-1312">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-1312">Az.Cdn</span></span>
* <span data-ttu-id="35cec-1313">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1313">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1314">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1314">Az.Compute</span></span>
* <span data-ttu-id="35cec-1315">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1315">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="35cec-1316">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1316">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="35cec-1317">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1317">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="35cec-1318">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1318">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="35cec-1319">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="35cec-1319">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="35cec-1320">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="35cec-1320">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="35cec-1321">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1321">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="35cec-1322">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1322">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1323">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1323">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1324">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1324">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="35cec-1325">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1325">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="35cec-1326">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1326">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="35cec-1327">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1327">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-1328">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-1328">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-1329">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1329">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-1330">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1330">Az.EventHub</span></span>
* <span data-ttu-id="35cec-1331">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="35cec-1331">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="35cec-1332">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="35cec-1332">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="35cec-1333">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1333">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="35cec-1334">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="35cec-1334">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="35cec-1335">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="35cec-1335">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="35cec-1336">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1336">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1337">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1337">Az.Monitor</span></span>
* <span data-ttu-id="35cec-1338">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1338">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1339">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1339">Az.Network</span></span>
* <span data-ttu-id="35cec-1340">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1340">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="35cec-1341">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1341">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="35cec-1342">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1342">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="35cec-1343">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1343">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="35cec-1344">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1344">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="35cec-1345">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1345">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="35cec-1346">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1346">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-1347">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1347">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-1348">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1348">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="35cec-1349">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1349">Added example</span></span>
    - <span data-ttu-id="35cec-1350">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1350">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="35cec-1351">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1351">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="35cec-1352">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1352">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1353">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1353">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1354">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1354">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1355">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1355">Az.Resources</span></span>
* <span data-ttu-id="35cec-1356">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1356">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="35cec-1357">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1357">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="35cec-1358">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="35cec-1358">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="35cec-1359">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1359">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-1360">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-1360">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-1361">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="35cec-1361">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="35cec-1362">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="35cec-1362">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="35cec-1363">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1363">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-1364">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1364">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-1365">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1365">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="35cec-1366">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="35cec-1366">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="35cec-1367">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="35cec-1367">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="35cec-1368">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1368">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="35cec-1369">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="35cec-1369">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="35cec-1370">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1370">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1371">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1371">Az.Sql</span></span>
* <span data-ttu-id="35cec-1372">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1372">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1373">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1373">Az.Storage</span></span>
* <span data-ttu-id="35cec-1374">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1374">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="35cec-1375">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-1375">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="35cec-1376">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="35cec-1376">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="35cec-1377">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="35cec-1377">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="35cec-1378">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-1378">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="35cec-1379">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="35cec-1379">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1380">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1380">Az.Websites</span></span>
* <span data-ttu-id="35cec-1381">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1381">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="35cec-1382">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1382">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-1383">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1383">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1384">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1384">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="35cec-1385">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1385">Az.ApplicationInsights</span></span>
* <span data-ttu-id="35cec-1386">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1386">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1387">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1387">Az.Automation</span></span>
* <span data-ttu-id="35cec-1388">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1388">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-1389">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1389">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-1390">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1390">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1391">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1391">Az.Compute</span></span>
* <span data-ttu-id="35cec-1392">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1392">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="35cec-1393">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="35cec-1393">Az.ContainerRegistry</span></span>
* <span data-ttu-id="35cec-1394">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1394">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="35cec-1395">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="35cec-1395">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1396">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1396">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1397">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1397">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="35cec-1398">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1398">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-1399">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1399">Az.EventHub</span></span>
* <span data-ttu-id="35cec-1400">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="35cec-1400">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="35cec-1401">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1401">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-1402">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-1402">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-1403">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1403">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="35cec-1404">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="35cec-1404">Az.LogicApp</span></span>
* <span data-ttu-id="35cec-1405">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1405">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="35cec-1406">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1406">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="35cec-1407">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1407">Az.ManagedServices</span></span>
* <span data-ttu-id="35cec-1408">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1408">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1409">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1409">Az.Network</span></span>
* <span data-ttu-id="35cec-1410">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1410">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="35cec-1411">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1411">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1412">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="35cec-1412">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="35cec-1413">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="35cec-1413">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="35cec-1414">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1414">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1415">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1415">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1416">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1416">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1417">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1417">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="35cec-1418">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="35cec-1418">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="35cec-1419">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="35cec-1419">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="35cec-1420">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="35cec-1420">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="35cec-1421">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1421">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="35cec-1422">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1422">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="35cec-1423">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1423">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="35cec-1424">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="35cec-1424">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="35cec-1425">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1425">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="35cec-1426">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1426">Updated cmdlets</span></span>
        - <span data-ttu-id="35cec-1427">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1427">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="35cec-1428">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1428">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="35cec-1429">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1429">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="35cec-1430">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1430">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="35cec-1431">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1431">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="35cec-1432">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1432">Updated cmdlet:</span></span>
        - <span data-ttu-id="35cec-1433">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1433">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="35cec-1434">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1434">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="35cec-1435">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1435">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="35cec-1436">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="35cec-1436">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="35cec-1437">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1437">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="35cec-1438">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1438">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-1439">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1439">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-1440">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1440">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="35cec-1441">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1441">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1442">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1442">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1443">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1443">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="35cec-1444">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1444">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="35cec-1445">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1445">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="35cec-1446">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1446">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="35cec-1447">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1447">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="35cec-1448">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1448">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="35cec-1449">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1449">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="35cec-1450">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1450">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="35cec-1451">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1451">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="35cec-1452">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1452">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1453">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1453">Az.Resources</span></span>
- <span data-ttu-id="35cec-1454">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1454">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="35cec-1455">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1455">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-1456">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-1456">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-1457">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="35cec-1457">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="35cec-1458">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1458">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1459">Az.Sql</span></span>
* <span data-ttu-id="35cec-1460">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1460">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="35cec-1461">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1461">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="35cec-1462">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1462">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1463">Az.Storage</span></span>
* <span data-ttu-id="35cec-1464">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1464">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="35cec-1465">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="35cec-1465">Az.StorageSync</span></span>
* <span data-ttu-id="35cec-1466">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1466">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="35cec-1467">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1467">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1468">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1468">Az.Websites</span></span>
* <span data-ttu-id="35cec-1469">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1469">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="35cec-1470">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1470">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="35cec-1471">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1471">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="35cec-1472">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1472">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-1473">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1473">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1474">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1474">Add support for profile cmdlets</span></span>
* <span data-ttu-id="35cec-1475">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1475">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="35cec-1476">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1476">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="35cec-1477">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="35cec-1477">Az.Advisor</span></span>
* <span data-ttu-id="35cec-1478">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="35cec-1478">GA release of Az.Advisor</span></span>
* <span data-ttu-id="35cec-1479">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1479">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="35cec-1480">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-1480">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-1481">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="35cec-1481">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="35cec-1482">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="35cec-1482">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="35cec-1483">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1483">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="35cec-1484">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1484">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="35cec-1485">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1485">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="35cec-1486">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="35cec-1486">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="35cec-1487">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1487">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1488">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1488">Az.Automation</span></span>
* <span data-ttu-id="35cec-1489">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1489">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1490">Az.Compute</span></span>
* <span data-ttu-id="35cec-1491">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1491">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1492">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1492">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1493">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="35cec-1493">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="35cec-1494">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="35cec-1494">Az.EventGrid</span></span>
* <span data-ttu-id="35cec-1495">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1495">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-1496">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1496">Az.IotHub</span></span>
* <span data-ttu-id="35cec-1497">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1497">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1498">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1498">Az.Network</span></span>
* <span data-ttu-id="35cec-1499">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1499">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="35cec-1500">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1500">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-1501">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1501">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-1502">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1502">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="35cec-1503">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="35cec-1503">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-1504">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1504">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-1505">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1505">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1506">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1506">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1507">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1507">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1508">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1508">Az.Resources</span></span>
    - <span data-ttu-id="35cec-1509">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1509">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="35cec-1510">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1510">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="35cec-1511">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1511">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="35cec-1512">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1512">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-1513">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-1513">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-1514">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="35cec-1514">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1515">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1515">Az.Sql</span></span>
* <span data-ttu-id="35cec-1516">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1516">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="35cec-1517">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1517">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="35cec-1518">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1518">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="35cec-1519">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1519">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="35cec-1520">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1520">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="35cec-1521">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1521">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="35cec-1522">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1522">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="35cec-1523">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="35cec-1523">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="35cec-1524">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1524">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1525">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1525">Az.Storage</span></span>
* <span data-ttu-id="35cec-1526">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1526">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="35cec-1527">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="35cec-1527">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="35cec-1528">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1528">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="35cec-1529">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="35cec-1529">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="35cec-1530">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1530">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="35cec-1531">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1531">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="35cec-1532">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1532">Set-AzStorageAccount</span></span>
* <span data-ttu-id="35cec-1533">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-1533">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="35cec-1534">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="35cec-1534">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="35cec-1535">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="35cec-1535">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="35cec-1536">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="35cec-1536">Az.StorageSync</span></span>
* <span data-ttu-id="35cec-1537">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1537">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="35cec-1538">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1538">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-1539">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1539">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1540">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1540">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="35cec-1541">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="35cec-1541">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="35cec-1542">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1542">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="35cec-1543">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="35cec-1543">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="35cec-1544">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="35cec-1544">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1545">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1545">Az.Compute</span></span>
* <span data-ttu-id="35cec-1546">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1546">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="35cec-1547">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1547">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="35cec-1548">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="35cec-1548">Az.Dns</span></span>
* <span data-ttu-id="35cec-1549">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1549">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="35cec-1550">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="35cec-1550">Az.EventGrid</span></span>
* <span data-ttu-id="35cec-1551">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1551">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="35cec-1552">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1552">New cmdlets:</span></span>
    - <span data-ttu-id="35cec-1553">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="35cec-1553">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="35cec-1554">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1554">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="35cec-1555">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="35cec-1555">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="35cec-1556">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1556">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="35cec-1557">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="35cec-1557">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="35cec-1558">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1558">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="35cec-1559">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="35cec-1559">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="35cec-1560">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1560">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="35cec-1561">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="35cec-1561">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="35cec-1562">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1562">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="35cec-1563">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="35cec-1563">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="35cec-1564">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1564">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="35cec-1565">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="35cec-1565">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="35cec-1566">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1566">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="35cec-1567">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="35cec-1567">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="35cec-1568">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1568">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="35cec-1569">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1569">Updated cmdlets:</span></span>
    - <span data-ttu-id="35cec-1570">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="35cec-1570">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="35cec-1571">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1571">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="35cec-1572">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1572">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="35cec-1573">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="35cec-1573">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="35cec-1574">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="35cec-1574">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="35cec-1575">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="35cec-1575">Event subscription expiration date,</span></span>
            - <span data-ttu-id="35cec-1576">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="35cec-1576">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="35cec-1577">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1577">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="35cec-1578">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="35cec-1578">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="35cec-1579">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="35cec-1579">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="35cec-1580">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1580">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="35cec-1581">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="35cec-1581">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="35cec-1582">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1582">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="35cec-1583">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1583">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-1584">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-1584">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-1585">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="35cec-1585">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="35cec-1586">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1586">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="35cec-1587">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="35cec-1587">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="35cec-1588">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1588">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1589">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1589">Az.Network</span></span>
* <span data-ttu-id="35cec-1590">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1590">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="35cec-1591">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1591">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1592">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="35cec-1592">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="35cec-1593">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1593">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="35cec-1594">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1594">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1595">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="35cec-1595">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="35cec-1596">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1596">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="35cec-1597">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1597">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1598">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="35cec-1598">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="35cec-1599">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="35cec-1599">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="35cec-1600">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="35cec-1600">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="35cec-1601">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1601">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="35cec-1602">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1602">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="35cec-1603">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1603">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="35cec-1604">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1604">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1605">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="35cec-1605">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="35cec-1606">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="35cec-1606">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="35cec-1607">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="35cec-1607">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="35cec-1608">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="35cec-1608">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="35cec-1609">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="35cec-1609">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="35cec-1610">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1610">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="35cec-1611">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1611">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="35cec-1612">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1612">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="35cec-1613">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1613">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="35cec-1614">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1614">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="35cec-1615">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1615">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="35cec-1616">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1616">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="35cec-1617">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1617">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="35cec-1618">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1618">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="35cec-1619">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1619">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="35cec-1620">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1620">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="35cec-1621">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1621">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="35cec-1622">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1622">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="35cec-1623">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="35cec-1623">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="35cec-1624">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1624">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="35cec-1625">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1625">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="35cec-1626">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="35cec-1626">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="35cec-1627">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1627">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="35cec-1628">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1628">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="35cec-1629">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1629">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="35cec-1630">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1630">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="35cec-1631">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1631">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-1632">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1632">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-1633">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1633">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1634">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1634">Az.Resources</span></span>
* <span data-ttu-id="35cec-1635">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="35cec-1635">Support for additional Template Export options</span></span>
    - <span data-ttu-id="35cec-1636">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1636">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="35cec-1637">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1637">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="35cec-1638">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1638">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-1639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1639">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-1640">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1640">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1641">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1641">Az.Sql</span></span>
* <span data-ttu-id="35cec-1642">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1642">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="35cec-1643">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1643">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="35cec-1644">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1644">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="35cec-1645">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="35cec-1645">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="35cec-1646">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="35cec-1646">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="35cec-1647">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="35cec-1647">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="35cec-1648">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="35cec-1648">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="35cec-1649">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="35cec-1649">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1650">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1650">Az.Storage</span></span>
* <span data-ttu-id="35cec-1651">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1651">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="35cec-1652">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1652">New-AzStorageAccount</span></span>
* <span data-ttu-id="35cec-1653">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1653">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="35cec-1654">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-1654">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1655">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1655">Az.Websites</span></span>
* <span data-ttu-id="35cec-1656">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1656">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="35cec-1657">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1657">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="35cec-1658">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1658">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="35cec-1659">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-1659">Az.Cdn</span></span>
* <span data-ttu-id="35cec-1660">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1660">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1661">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1661">Az.Compute</span></span>
* <span data-ttu-id="35cec-1662">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1662">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="35cec-1663">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="35cec-1663">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-1664">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1664">Az.EventHub</span></span>
* <span data-ttu-id="35cec-1665">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1665">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="35cec-1666">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1666">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1667">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1667">Az.Network</span></span>
* <span data-ttu-id="35cec-1668">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1668">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="35cec-1669">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1669">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-1670">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1670">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-1671">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1671">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1672">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1672">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1673">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1673">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-1674">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-1674">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-1675">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1675">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-1676">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1676">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-1677">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1677">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="35cec-1678">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1678">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1679">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1679">Az.Sql</span></span>
* <span data-ttu-id="35cec-1680">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1680">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="35cec-1681">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="35cec-1681">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="35cec-1682">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1682">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="35cec-1683">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1683">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1684">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1684">Az.Websites</span></span>
* <span data-ttu-id="35cec-1685">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1685">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="35cec-1686">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1686">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="35cec-1687">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-1687">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-1688">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1688">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="35cec-1689">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-1689">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="35cec-1690">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-1690">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="35cec-1691">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-1691">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="35cec-1692">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1692">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="35cec-1693">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-1693">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="35cec-1694">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1694">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="35cec-1695">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1695">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="35cec-1696">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1696">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="35cec-1697">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-1697">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="35cec-1698">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-1698">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="35cec-1699">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1699">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="35cec-1700">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1700">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="35cec-1701">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1701">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="35cec-1702">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="35cec-1702">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="35cec-1703">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-1703">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="35cec-1704">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="35cec-1704">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="35cec-1705">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="35cec-1705">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="35cec-1706">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1706">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="35cec-1707">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="35cec-1707">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="35cec-1708">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1708">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="35cec-1709">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1709">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="35cec-1710">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="35cec-1710">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="35cec-1711">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1711">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="35cec-1712">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1712">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="35cec-1713">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1713">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="35cec-1714">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1714">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="35cec-1715">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1715">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="35cec-1716">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1716">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="35cec-1717">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1717">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="35cec-1718">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1718">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="35cec-1719">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="35cec-1719">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="35cec-1720">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1720">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="35cec-1721">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1721">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="35cec-1722">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="35cec-1722">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="35cec-1723">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="35cec-1723">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="35cec-1724">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="35cec-1724">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="35cec-1725">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1725">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="35cec-1726">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1726">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="35cec-1727">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1727">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="35cec-1728">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="35cec-1728">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="35cec-1729">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="35cec-1729">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="35cec-1730">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="35cec-1730">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="35cec-1731">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1731">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="35cec-1732">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1732">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="35cec-1733">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="35cec-1733">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="35cec-1734">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="35cec-1734">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="35cec-1735">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1735">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="35cec-1736">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1736">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="35cec-1737">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="35cec-1737">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="35cec-1738">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="35cec-1738">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="35cec-1739">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="35cec-1739">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="35cec-1740">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="35cec-1740">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="35cec-1741">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1741">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="35cec-1742">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="35cec-1742">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="35cec-1743">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="35cec-1743">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="35cec-1744">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1744">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="35cec-1745">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="35cec-1745">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="35cec-1746">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="35cec-1746">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="35cec-1747">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1747">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="35cec-1748">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1748">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="35cec-1749">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="35cec-1749">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="35cec-1750">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="35cec-1750">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="35cec-1751">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1751">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="35cec-1752">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1752">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="35cec-1753">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="35cec-1753">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="35cec-1754">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="35cec-1754">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="35cec-1755">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="35cec-1755">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="35cec-1756">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="35cec-1756">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="35cec-1757">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="35cec-1757">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="35cec-1758">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="35cec-1758">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="35cec-1759">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="35cec-1759">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="35cec-1760">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="35cec-1760">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="35cec-1761">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="35cec-1761">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="35cec-1762">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="35cec-1762">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="35cec-1763">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="35cec-1763">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="35cec-1764">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="35cec-1764">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1765">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1765">Az.Automation</span></span>
* <span data-ttu-id="35cec-1766">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1766">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="35cec-1767">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="35cec-1767">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="35cec-1768">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="35cec-1768">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="35cec-1769">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1769">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="35cec-1770">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="35cec-1770">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="35cec-1771">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1771">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="35cec-1772">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1772">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1773">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1773">Az.Compute</span></span>
* <span data-ttu-id="35cec-1774">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1774">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="35cec-1775">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-1775">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-1776">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-1776">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-1777">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1777">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1778">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1778">Az.Monitor</span></span>
* <span data-ttu-id="35cec-1779">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1779">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1780">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1780">Az.Network</span></span>
* <span data-ttu-id="35cec-1781">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1781">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="35cec-1782">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="35cec-1782">Updated cmdlet:</span></span>
        - <span data-ttu-id="35cec-1783">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-1783">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="35cec-1784">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1784">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1785">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1785">Az.Resources</span></span>
* <span data-ttu-id="35cec-1786">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1786">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1787">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1787">Az.Sql</span></span>
* <span data-ttu-id="35cec-1788">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1788">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="35cec-1789">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1789">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-1790">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1790">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1791">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1791">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-1792">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1792">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-1793">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1793">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="35cec-1794">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1794">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1795">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1795">Az.Compute</span></span>
* <span data-ttu-id="35cec-1796">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="35cec-1796">Proximity placement group feature.</span></span>
    - <span data-ttu-id="35cec-1797">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1797">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="35cec-1798">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-1798">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="35cec-1799">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1799">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="35cec-1800">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1800">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="35cec-1801">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1801">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="35cec-1802">重大な変更</span><span class="sxs-lookup"><span data-stu-id="35cec-1802">Breaking changes</span></span>
    - <span data-ttu-id="35cec-1803">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-1803">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="35cec-1804">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="35cec-1804">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="35cec-1805">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="35cec-1805">Az.DeploymentManager</span></span>
* <span data-ttu-id="35cec-1806">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="35cec-1806">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="35cec-1807">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="35cec-1807">Az.Dns</span></span>
* <span data-ttu-id="35cec-1808">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="35cec-1808">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="35cec-1809">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1809">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="35cec-1810">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1810">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="35cec-1811">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-1811">Az.FrontDoor</span></span>
* <span data-ttu-id="35cec-1812">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="35cec-1812">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="35cec-1813">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="35cec-1813">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="35cec-1814">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-1814">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-1815">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1815">Removed two cmdlets:</span></span>
    - <span data-ttu-id="35cec-1816">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="35cec-1816">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="35cec-1817">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="35cec-1817">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="35cec-1818">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1818">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="35cec-1819">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1819">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="35cec-1820">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="35cec-1820">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="35cec-1821">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="35cec-1821">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1822">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1822">Az.Monitor</span></span>
* <span data-ttu-id="35cec-1823">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="35cec-1823">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="35cec-1824">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="35cec-1824">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="35cec-1825">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="35cec-1825">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="35cec-1826">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="35cec-1826">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="35cec-1827">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="35cec-1827">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="35cec-1828">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="35cec-1828">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="35cec-1829">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="35cec-1829">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="35cec-1830">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1830">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="35cec-1831">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1831">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="35cec-1832">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1832">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="35cec-1833">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1833">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="35cec-1834">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="35cec-1834">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="35cec-1835">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="35cec-1835">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="35cec-1836">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1836">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1837">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1837">Az.Network</span></span>
* <span data-ttu-id="35cec-1838">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1838">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="35cec-1839">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1839">New cmdlets</span></span>
        - <span data-ttu-id="35cec-1840">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="35cec-1840">New-AzNatGateway</span></span>
        - <span data-ttu-id="35cec-1841">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="35cec-1841">Get-AzNatGateway</span></span>
        - <span data-ttu-id="35cec-1842">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="35cec-1842">Set-AzNatGateway</span></span>
        - <span data-ttu-id="35cec-1843">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="35cec-1843">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="35cec-1844">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1844">Updated cmdlets</span></span>
        - <span data-ttu-id="35cec-1845">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="35cec-1845">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="35cec-1846">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="35cec-1846">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="35cec-1847">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="35cec-1847">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="35cec-1848">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1848">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="35cec-1849">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1849">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-1850">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1850">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-1851">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-1851">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="35cec-1852">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1852">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="35cec-1853">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="35cec-1853">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1854">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1854">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1855">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-1855">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="35cec-1856">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="35cec-1856">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="35cec-1857">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="35cec-1857">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="35cec-1858">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="35cec-1858">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="35cec-1859">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="35cec-1859">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="35cec-1860">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="35cec-1860">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="35cec-1861">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="35cec-1861">Az.Relay</span></span>
* <span data-ttu-id="35cec-1862">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1862">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-1863">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-1863">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-1864">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1864">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1865">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1865">Az.Storage</span></span>
* <span data-ttu-id="35cec-1866">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="35cec-1866">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="35cec-1867">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1867">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="35cec-1868">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1868">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="35cec-1869">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1869">New-AzStorageAccount</span></span>
* <span data-ttu-id="35cec-1870">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="35cec-1870">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="35cec-1871">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1871">New-AzStorageAccount</span></span>
    - <span data-ttu-id="35cec-1872">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1872">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="35cec-1873">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="35cec-1873">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1874">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1874">Az.Websites</span></span>
* <span data-ttu-id="35cec-1875">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="35cec-1875">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="35cec-1876">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="35cec-1876">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="35cec-1877">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1877">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-1878">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-1878">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-1879">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-1879">General availability of `Az` module</span></span>
* <span data-ttu-id="35cec-1880">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="35cec-1880">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="35cec-1881">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="35cec-1881">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="35cec-1882">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1882">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="35cec-1883">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1883">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="35cec-1884">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1884">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="35cec-1885">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1885">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-1886">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1886">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1887">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-1887">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="35cec-1888">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-1888">Az.Batch</span></span>
* <span data-ttu-id="35cec-1889">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1889">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-1890">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-1890">Az.Cdn</span></span>
* <span data-ttu-id="35cec-1891">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1891">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-1892">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1892">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-1893">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1893">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1894">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1894">Az.Compute</span></span>
* <span data-ttu-id="35cec-1895">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1895">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="35cec-1896">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1896">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1897">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1897">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1898">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1898">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1899">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1899">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-1900">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-1900">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-1901">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1901">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="35cec-1902">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="35cec-1902">Az.EventGrid</span></span>
* <span data-ttu-id="35cec-1903">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1903">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-1904">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1904">Az.EventHub</span></span>
* <span data-ttu-id="35cec-1905">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1905">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="35cec-1906">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="35cec-1906">Az.HDInsight</span></span>
* <span data-ttu-id="35cec-1907">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1907">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-1908">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-1908">Az.IotHub</span></span>
* <span data-ttu-id="35cec-1909">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1909">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-1910">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-1910">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-1911">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1911">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1912">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1912">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="35cec-1913">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="35cec-1913">Az.MachineLearning</span></span>
* <span data-ttu-id="35cec-1914">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1914">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="35cec-1915">Az.Media</span><span class="sxs-lookup"><span data-stu-id="35cec-1915">Az.Media</span></span>
* <span data-ttu-id="35cec-1916">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1916">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-1917">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-1917">Az.Monitor</span></span>
  * <span data-ttu-id="35cec-1918">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1918">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="35cec-1919">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="35cec-1919">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="35cec-1920">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="35cec-1920">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="35cec-1921">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="35cec-1921">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="35cec-1922">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="35cec-1922">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="35cec-1923">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="35cec-1923">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="35cec-1924">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1924">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-1925">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-1925">Az.Network</span></span>
* <span data-ttu-id="35cec-1926">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1926">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1927">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1927">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="35cec-1928">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="35cec-1928">Az.NotificationHubs</span></span>
* <span data-ttu-id="35cec-1929">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1929">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-1930">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-1930">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-1931">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1931">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="35cec-1932">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="35cec-1932">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="35cec-1933">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1933">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-1934">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1934">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-1935">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1935">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1936">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1936">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="35cec-1937">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1937">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="35cec-1938">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1938">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="35cec-1939">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="35cec-1939">Az.RedisCache</span></span>
* <span data-ttu-id="35cec-1940">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1940">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1941">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1941">Az.Resources</span></span>
* <span data-ttu-id="35cec-1942">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1942">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1943">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1943">Az.Sql</span></span>
* <span data-ttu-id="35cec-1944">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="35cec-1944">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="35cec-1945">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1945">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1946">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1946">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="35cec-1947">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1947">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="35cec-1948">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="35cec-1948">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="35cec-1949">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="35cec-1949">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="35cec-1950">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1950">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-1951">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-1951">Az.Websites</span></span>
* <span data-ttu-id="35cec-1952">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-1952">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="35cec-1953">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1953">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="35cec-1954">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1954">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="35cec-1955">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1955">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="35cec-1956">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="35cec-1956">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-1957">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-1957">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-1958">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-1958">General availability of `Az` module</span></span>
* <span data-ttu-id="35cec-1959">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="35cec-1959">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="35cec-1960">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="35cec-1960">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="35cec-1961">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1961">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="35cec-1962">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1962">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="35cec-1963">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-1963">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="35cec-1964">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-1964">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="35cec-1965">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-1965">Az.Accounts</span></span>
* <span data-ttu-id="35cec-1966">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1966">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="35cec-1967">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="35cec-1967">Az.AnalysisServices</span></span>
* <span data-ttu-id="35cec-1968">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="35cec-1968">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="35cec-1969">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1969">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-1970">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-1970">Az.Automation</span></span>
* <span data-ttu-id="35cec-1971">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1971">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="35cec-1972">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1972">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="35cec-1973">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1973">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-1974">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-1974">Az.Compute</span></span>
* <span data-ttu-id="35cec-1975">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1975">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="35cec-1976">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1976">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="35cec-1977">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-1977">Az.ContainerInstance</span></span>
* <span data-ttu-id="35cec-1978">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1978">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-1979">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-1979">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-1980">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1980">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="35cec-1981">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1981">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-1982">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-1982">Az.Resources</span></span>
* <span data-ttu-id="35cec-1983">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1983">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="35cec-1984">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1984">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="35cec-1985">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="35cec-1985">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="35cec-1986">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="35cec-1986">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="35cec-1987">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-1987">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="35cec-1988">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="35cec-1988">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-1989">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-1989">Az.Sql</span></span>
* <span data-ttu-id="35cec-1990">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-1990">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-1991">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-1991">Az.Storage</span></span>
* <span data-ttu-id="35cec-1992">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="35cec-1992">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="35cec-1993">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="35cec-1993">New-AzStorageContext</span></span>
* <span data-ttu-id="35cec-1994">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="35cec-1994">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="35cec-1995">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="35cec-1995">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="35cec-1996">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="35cec-1996">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="35cec-1997">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-1997">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="35cec-1998">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-1998">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="35cec-1999">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="35cec-1999">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="35cec-2000">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="35cec-2000">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="35cec-2001">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="35cec-2001">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="35cec-2002">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="35cec-2002">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="35cec-2003">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="35cec-2003">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="35cec-2004">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2004">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="35cec-2005">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="35cec-2005">Highlights since the last major release</span></span>
* <span data-ttu-id="35cec-2006">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="35cec-2006">General availability of `Az` module</span></span>
* <span data-ttu-id="35cec-2007">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="35cec-2007">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="35cec-2008">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="35cec-2008">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="35cec-2009">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2009">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="35cec-2010">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2010">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="35cec-2011">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2011">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="35cec-2012">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2012">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-2013">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-2013">Az.Automation</span></span>
* <span data-ttu-id="35cec-2014">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2014">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="35cec-2015">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="35cec-2015">Dynamic grouping</span></span>
    * <span data-ttu-id="35cec-2016">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="35cec-2016">Pre-Post script</span></span>
    * <span data-ttu-id="35cec-2017">再起動設定</span><span class="sxs-lookup"><span data-stu-id="35cec-2017">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2018">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2018">Az.Compute</span></span>
* <span data-ttu-id="35cec-2019">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2019">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="35cec-2020">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2020">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-2021">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-2021">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-2022">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2022">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2023">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2023">Az.Network</span></span>
* <span data-ttu-id="35cec-2024">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2024">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="35cec-2025">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2025">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2026">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2026">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-2027">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2027">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="35cec-2028">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2028">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2029">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2029">Az.Resources</span></span>
* <span data-ttu-id="35cec-2030">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2030">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="35cec-2031">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2031">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2032">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2032">Az.Sql</span></span>
* <span data-ttu-id="35cec-2033">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2033">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-2034">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2034">Az.Storage</span></span>
* <span data-ttu-id="35cec-2035">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-2035">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="35cec-2036">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-2036">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="35cec-2037">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-2037">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="35cec-2038">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="35cec-2038">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="35cec-2039">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="35cec-2039">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="35cec-2040">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="35cec-2040">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="35cec-2041">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="35cec-2041">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-2042">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2042">Az.Websites</span></span>
* <span data-ttu-id="35cec-2043">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2043">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="35cec-2044">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2044">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-2045">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2045">Az.Accounts</span></span>
* <span data-ttu-id="35cec-2046">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2046">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="35cec-2047">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2047">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-2048">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-2048">Az.Automation</span></span>
* <span data-ttu-id="35cec-2049">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2049">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="35cec-2050">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2050">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="35cec-2051">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="35cec-2051">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-2052">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-2052">Az.Cdn</span></span>
* <span data-ttu-id="35cec-2053">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-2053">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2054">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2054">Az.Compute</span></span>
* <span data-ttu-id="35cec-2055">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2055">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-2056">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-2056">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-2057">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2057">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="35cec-2058">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="35cec-2058">Az.LogicApp</span></span>
* <span data-ttu-id="35cec-2059">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2059">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2060">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2060">Az.Network</span></span>
* <span data-ttu-id="35cec-2061">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2061">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2062">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2062">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-2063">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2063">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="35cec-2064">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2064">SDK Update</span></span>
* <span data-ttu-id="35cec-2065">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2065">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="35cec-2066">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2066">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2067">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2067">Az.Resources</span></span>
* <span data-ttu-id="35cec-2068">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2068">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="35cec-2069">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="35cec-2069">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="35cec-2070">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2070">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="35cec-2071">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="35cec-2071">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="35cec-2072">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2072">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="35cec-2073">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="35cec-2073">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2074">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2074">Az.Sql</span></span>
* <span data-ttu-id="35cec-2075">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2075">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="35cec-2076">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2076">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-2077">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2077">Az.Storage</span></span>
* <span data-ttu-id="35cec-2078">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="35cec-2078">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="35cec-2079">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2079">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="35cec-2080">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2080">Az.AnalysisServices</span></span>
* <span data-ttu-id="35cec-2081">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-2081">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-2082">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-2082">Az.Automation</span></span>
* <span data-ttu-id="35cec-2083">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2083">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="35cec-2084">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2084">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="35cec-2085">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2085">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-2086">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2086">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-2087">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2087">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2088">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2088">Az.Compute</span></span>
* <span data-ttu-id="35cec-2089">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2089">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="35cec-2090">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2090">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="35cec-2091">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2091">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="35cec-2092">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-2092">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2093">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2093">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-2094">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2094">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="35cec-2095">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="35cec-2095">Az.EventHub</span></span>
* <span data-ttu-id="35cec-2096">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2096">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-2097">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-2097">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-2098">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2098">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="35cec-2099">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="35cec-2099">Az.LogicApp</span></span>
* <span data-ttu-id="35cec-2100">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2100">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="35cec-2101">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2101">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="35cec-2102">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2102">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="35cec-2103">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="35cec-2103">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="35cec-2104">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="35cec-2104">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="35cec-2105">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="35cec-2105">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="35cec-2106">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="35cec-2106">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="35cec-2107">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2107">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="35cec-2108">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-2108">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="35cec-2109">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-2109">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="35cec-2110">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-2110">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="35cec-2111">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-2111">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="35cec-2112">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2112">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="35cec-2113">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-2113">Az.Monitor</span></span>
* <span data-ttu-id="35cec-2114">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2114">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2115">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2115">Az.Network</span></span>
* <span data-ttu-id="35cec-2116">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2116">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-2117">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-2117">Az.OperationalInsights</span></span>
* <span data-ttu-id="35cec-2118">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2118">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="35cec-2119">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2119">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="35cec-2120">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2120">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2121">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2121">Az.Resources</span></span>
* <span data-ttu-id="35cec-2122">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="35cec-2122">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="35cec-2123">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="35cec-2123">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="35cec-2124">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="35cec-2124">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="35cec-2125">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2125">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2126">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2126">Az.Sql</span></span>
* <span data-ttu-id="35cec-2127">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2127">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="35cec-2128">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2128">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-2129">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2129">Az.Websites</span></span>
* <span data-ttu-id="35cec-2130">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2130">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="35cec-2131">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2131">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-2132">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2132">Az.Accounts</span></span>
* <span data-ttu-id="35cec-2133">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2133">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="35cec-2134">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2134">Az.AnalysisServices</span></span>
<span data-ttu-id="35cec-2135">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-2135">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2136">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2136">Az.Compute</span></span>
* <span data-ttu-id="35cec-2137">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2137">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="35cec-2138">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2138">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="35cec-2139">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2139">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2140">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2140">Az.RecoveryServices</span></span>
<span data-ttu-id="35cec-2141">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-2141">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2142">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2142">Az.Resources</span></span>
* <span data-ttu-id="35cec-2143">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2143">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="35cec-2144">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="35cec-2144">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="35cec-2145">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2145">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="35cec-2146">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="35cec-2146">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2147">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2147">Az.Sql</span></span>
* <span data-ttu-id="35cec-2148">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2148">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="35cec-2149">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2149">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="35cec-2150">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2150">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="35cec-2151">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2151">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-2152">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2152">Az.Accounts</span></span>
* <span data-ttu-id="35cec-2153">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="35cec-2153">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="35cec-2154">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2154">Az.AnalysisServices</span></span>
* <span data-ttu-id="35cec-2155">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="35cec-2155">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2156">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2156">Az.RecoveryServices</span></span>
* <span data-ttu-id="35cec-2157">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="35cec-2157">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="35cec-2158">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2158">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-2159">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2159">Az.Accounts</span></span>
* <span data-ttu-id="35cec-2160">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2160">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="35cec-2161">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2161">Update incorrect online help URLs</span></span>
* <span data-ttu-id="35cec-2162">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2162">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="35cec-2163">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="35cec-2163">Az.Aks</span></span>
* <span data-ttu-id="35cec-2164">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2164">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="35cec-2165">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-2165">Az.Automation</span></span>
* <span data-ttu-id="35cec-2166">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2166">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="35cec-2167">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2167">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="35cec-2168">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="35cec-2168">Az.Cdn</span></span>
* <span data-ttu-id="35cec-2169">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2169">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2170">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2170">Az.Compute</span></span>
* <span data-ttu-id="35cec-2171">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2171">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="35cec-2172">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2172">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="35cec-2173">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2173">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="35cec-2174">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="35cec-2174">Az.ContainerRegistry</span></span>
* <span data-ttu-id="35cec-2175">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2175">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="35cec-2176">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="35cec-2176">Az.DataFactory</span></span>
* <span data-ttu-id="35cec-2177">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2177">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2178">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2178">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-2179">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="35cec-2179">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="35cec-2180">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="35cec-2180">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="35cec-2181">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2181">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-2182">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-2182">Az.IotHub</span></span>
* <span data-ttu-id="35cec-2183">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2183">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="35cec-2184">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-2184">Az.KeyVault</span></span>
* <span data-ttu-id="35cec-2185">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2185">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2186">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2186">Az.Network</span></span>
* <span data-ttu-id="35cec-2187">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2187">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2188">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2188">Az.Resources</span></span>
* <span data-ttu-id="35cec-2189">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2189">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="35cec-2190">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2190">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="35cec-2191">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2191">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="35cec-2192">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="35cec-2192">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="35cec-2193">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="35cec-2193">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="35cec-2194">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2194">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="35cec-2195">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="35cec-2195">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-2196">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-2196">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-2197">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="35cec-2197">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="35cec-2198">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2198">Fix some error messages.</span></span>
* <span data-ttu-id="35cec-2199">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2199">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="35cec-2200">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2200">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="35cec-2201">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="35cec-2201">Az.SignalR</span></span>
* <span data-ttu-id="35cec-2202">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2202">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2203">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2203">Az.Sql</span></span>
* <span data-ttu-id="35cec-2204">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2204">Update incorrect online help URLs</span></span>
* <span data-ttu-id="35cec-2205">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2205">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="35cec-2206">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2206">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="35cec-2207">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-2207">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-2208">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2208">Az.Storage</span></span>
* <span data-ttu-id="35cec-2209">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2209">Update incorrect online help URLs</span></span>
* <span data-ttu-id="35cec-2210">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="35cec-2210">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="35cec-2211">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="35cec-2211">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="35cec-2212">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="35cec-2212">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="35cec-2213">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="35cec-2213">Az.TrafficManager</span></span>
* <span data-ttu-id="35cec-2214">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2214">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-2215">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2215">Az.Websites</span></span>
* <span data-ttu-id="35cec-2216">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2216">Update incorrect online help URLs</span></span>
* <span data-ttu-id="35cec-2217">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2217">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="35cec-2218">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="35cec-2218">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="35cec-2219">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2219">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="35cec-2220">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2220">Az.Accounts</span></span>
* <span data-ttu-id="35cec-2221">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="35cec-2221">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2222">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2222">Az.Compute</span></span>
* <span data-ttu-id="35cec-2223">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2223">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="35cec-2224">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="35cec-2224">Updated the description of ID in help files</span></span>
* <span data-ttu-id="35cec-2225">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2225">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2226">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2226">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-2227">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2227">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="35cec-2228">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2228">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="35cec-2229">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="35cec-2229">Az.EventGrid</span></span>
* <span data-ttu-id="35cec-2230">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2230">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="35cec-2231">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="35cec-2231">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="35cec-2232">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="35cec-2232">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="35cec-2233">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="35cec-2233">Event Time-To-Live,</span></span>
        - <span data-ttu-id="35cec-2234">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="35cec-2234">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="35cec-2235">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="35cec-2235">Dead letter endpoint.</span></span>
    - <span data-ttu-id="35cec-2236">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="35cec-2236">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="35cec-2237">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="35cec-2237">Event Time-To-Live,</span></span>
        - <span data-ttu-id="35cec-2238">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="35cec-2238">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="35cec-2239">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="35cec-2239">Dead letter endpoint.</span></span>
* <span data-ttu-id="35cec-2240">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2240">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="35cec-2241">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2241">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="35cec-2242">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="35cec-2242">Az.IotHub</span></span>
* <span data-ttu-id="35cec-2243">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2243">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="35cec-2244">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="35cec-2244">Az.LogicApp</span></span>
* <span data-ttu-id="35cec-2245">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="35cec-2245">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2246">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2246">Az.Resources</span></span>
* <span data-ttu-id="35cec-2247">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2247">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="35cec-2248">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="35cec-2248">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="35cec-2249">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2249">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="35cec-2250">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2250">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="35cec-2251">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="35cec-2251">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="35cec-2252">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="35cec-2252">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="35cec-2253">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="35cec-2253">Az.SignalR</span></span>
* <span data-ttu-id="35cec-2254">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2254">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2255">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2255">Az.Sql</span></span>
* <span data-ttu-id="35cec-2256">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2256">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="35cec-2257">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2257">Az.Storage</span></span>
* <span data-ttu-id="35cec-2258">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="35cec-2258">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="35cec-2259">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="35cec-2259">New-AzStorageContext</span></span>
* <span data-ttu-id="35cec-2260">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2260">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="35cec-2261">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="35cec-2261">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-2262">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2262">Az.Websites</span></span>
* <span data-ttu-id="35cec-2263">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2263">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="35cec-2264">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2264">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="35cec-2265">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2265">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="35cec-2266">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-2266">General</span></span>

- <span data-ttu-id="35cec-2267">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-2267">General Availability of Az Module</span></span>
- <span data-ttu-id="35cec-2268">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="35cec-2268">Online help for each module</span></span>
- <span data-ttu-id="35cec-2269">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2269">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="35cec-2270">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2270">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="35cec-2271">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="35cec-2271">Az.Accounts</span></span>
- <span data-ttu-id="35cec-2272">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2272">Changed from Az.Profile</span></span>
- <span data-ttu-id="35cec-2273">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2273">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="35cec-2274">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-2274">Az.ApiManagement</span></span>
- <span data-ttu-id="35cec-2275">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35cec-2275">Fixes for #7002</span></span>
- <span data-ttu-id="35cec-2276">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2276">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="35cec-2277">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="35cec-2277">Az.Batch</span></span>
- <span data-ttu-id="35cec-2278">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2278">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="35cec-2279">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2279">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="35cec-2280">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2280">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="35cec-2281">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="35cec-2281">Az.Billing</span></span>
- <span data-ttu-id="35cec-2282">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2282">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="35cec-2283">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2283">Az.CognitivServices</span></span>
- <span data-ttu-id="35cec-2284">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2284">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="35cec-2285">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2285">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="35cec-2286">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2286">Az.ContainerInstance</span></span>
- <span data-ttu-id="35cec-2287">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2287">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="35cec-2288">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="35cec-2288">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="35cec-2289">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2289">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2290">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2290">Az.DataLakeStore</span></span>
- <span data-ttu-id="35cec-2291">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2291">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="35cec-2292">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="35cec-2292">Az.Monitor</span></span>
- <span data-ttu-id="35cec-2293">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2293">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="35cec-2294">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="35cec-2294">Az.KeyVault</span></span>
- <span data-ttu-id="35cec-2295">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2295">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="35cec-2296">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="35cec-2296">Az.MachineLearning</span></span>
- <span data-ttu-id="35cec-2297">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="35cec-2297">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="35cec-2298">Az.Media</span><span class="sxs-lookup"><span data-stu-id="35cec-2298">Az.Media</span></span>
- <span data-ttu-id="35cec-2299">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2299">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="35cec-2300">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2300">Az.Network</span></span>
<span data-ttu-id="35cec-2301">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2301">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="35cec-2302">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-2302">New cmdlets added:</span></span>
        - <span data-ttu-id="35cec-2303">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2303">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2304">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2304">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2305">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2305">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2306">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2306">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2307">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2307">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2308">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="35cec-2308">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="35cec-2309">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="35cec-2309">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="35cec-2310">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="35cec-2310">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="35cec-2311">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2311">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="35cec-2312">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="35cec-2312">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="35cec-2313">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="35cec-2313">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="35cec-2314">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="35cec-2314">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="35cec-2315">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-2315">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="35cec-2316">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-2316">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="35cec-2317">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2317">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="35cec-2318">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2318">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="35cec-2319">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="35cec-2319">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="35cec-2320">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="35cec-2320">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="35cec-2321">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="35cec-2321">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="35cec-2322">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2322">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="35cec-2323">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2323">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="35cec-2324">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-2324">Az.OperationalInsights</span></span>
- <span data-ttu-id="35cec-2325">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2325">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="35cec-2326">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="35cec-2326">Az.Profile</span></span>
- <span data-ttu-id="35cec-2327">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2327">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2328">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2328">Az.RecoveryServices</span></span>
- <span data-ttu-id="35cec-2329">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2329">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="35cec-2330">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2330">Az.Resources</span></span>
- <span data-ttu-id="35cec-2331">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2331">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="35cec-2332">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-2332">Az.ServiceFabric</span></span>
- <span data-ttu-id="35cec-2333">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="35cec-2333">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="35cec-2334">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2334">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="35cec-2335">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="35cec-2335">Az.SIgnalR</span></span>
- <span data-ttu-id="35cec-2336">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="35cec-2336">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="35cec-2337">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2337">Az.Sql</span></span>
- <span data-ttu-id="35cec-2338">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2338">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="35cec-2339">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2339">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="35cec-2340">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2340">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="35cec-2341">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2341">Az.Storage</span></span>
- <span data-ttu-id="35cec-2342">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2342">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="35cec-2343">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2343">Az.Websites</span></span>
- <span data-ttu-id="35cec-2344">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="35cec-2344">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="35cec-2345">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2345">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="35cec-2346">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-2346">General</span></span>

* <span data-ttu-id="35cec-2347">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="35cec-2347">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="35cec-2348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2348">Az.Compute</span></span>

* <span data-ttu-id="35cec-2349">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2349">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2350">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2350">Az.DataLakeStore</span></span>

* <span data-ttu-id="35cec-2351">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2351">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="35cec-2352">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="35cec-2352">Az.FrontDoor</span></span>

* <span data-ttu-id="35cec-2353">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2353">Fixed some broken links</span></span>
    - <span data-ttu-id="35cec-2354">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2354">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="35cec-2355">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2355">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="35cec-2356">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2356">Az.RecoveryServices</span></span>

* <span data-ttu-id="35cec-2357">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2357">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="35cec-2358">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2358">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="35cec-2359">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2359">Az.Resources</span></span>

* <span data-ttu-id="35cec-2360">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2360">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="35cec-2361">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2361">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="35cec-2362">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2362">Az.Sql</span></span>

* <span data-ttu-id="35cec-2363">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="35cec-2363">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="35cec-2364">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2364">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="35cec-2365">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2365">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="35cec-2366">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2366">Az.Storage</span></span>

* <span data-ttu-id="35cec-2367">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2367">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="35cec-2368">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2368">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="35cec-2369">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="35cec-2369">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="35cec-2370">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="35cec-2370">Support Static Website configuration</span></span>
    - <span data-ttu-id="35cec-2371">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="35cec-2371">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="35cec-2372">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="35cec-2372">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="35cec-2373">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2373">Az.Websites</span></span>

* <span data-ttu-id="35cec-2374">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="35cec-2374">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="35cec-2375">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2375">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="35cec-2376">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="35cec-2376">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="35cec-2377">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2377">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="35cec-2378">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="35cec-2378">Az.ApiManagement</span></span>
* <span data-ttu-id="35cec-2379">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2379">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="35cec-2380">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="35cec-2380">Az.Automation</span></span>
* <span data-ttu-id="35cec-2381">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="35cec-2381">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="35cec-2382">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2382">Added Update Management cmdlets</span></span>
* <span data-ttu-id="35cec-2383">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2383">Added Source Control cmdlets</span></span>
* <span data-ttu-id="35cec-2384">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2384">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="35cec-2385">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2385">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="35cec-2386">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2386">Az.Compute</span></span>
* <span data-ttu-id="35cec-2387">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2387">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="35cec-2388">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2388">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="35cec-2389">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2389">Az.ContainerInstance</span></span>
* <span data-ttu-id="35cec-2390">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2390">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="35cec-2391">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="35cec-2391">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="35cec-2392">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2392">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="35cec-2393">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2393">Az.Network</span></span>
* <span data-ttu-id="35cec-2394">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2394">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="35cec-2395">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2395">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="35cec-2396">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2396">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="35cec-2397">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2397">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="35cec-2398">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="35cec-2398">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="35cec-2399">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2399">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="35cec-2400">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2400">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="35cec-2401">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="35cec-2401">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="35cec-2402">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2402">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="35cec-2403">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2403">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="35cec-2404">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="35cec-2404">Az.Relay</span></span>
* <span data-ttu-id="35cec-2405">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="35cec-2405">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="35cec-2406">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2406">Az.Resources</span></span>
* <span data-ttu-id="35cec-2407">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2407">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="35cec-2408">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2408">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="35cec-2409">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="35cec-2409">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="35cec-2410">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-2410">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-2411">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2411">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="35cec-2412">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2412">Az.Sql</span></span>
* <span data-ttu-id="35cec-2413">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2413">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="35cec-2414">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2414">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="35cec-2415">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2415">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="35cec-2416">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2416">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="35cec-2417">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="35cec-2417">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="35cec-2418">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="35cec-2418">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="35cec-2419">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="35cec-2419">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="35cec-2420">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="35cec-2420">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="35cec-2421">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="35cec-2421">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="35cec-2422">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="35cec-2422">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="35cec-2423">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2423">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="35cec-2424">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2424">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="35cec-2425">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="35cec-2425">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="35cec-2426">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="35cec-2426">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="35cec-2427">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="35cec-2427">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="35cec-2428">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="35cec-2428">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="35cec-2429">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2429">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="35cec-2430">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2430">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="35cec-2431">全般</span><span class="sxs-lookup"><span data-stu-id="35cec-2431">General</span></span>
* <span data-ttu-id="35cec-2432">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="35cec-2432">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="35cec-2433">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="35cec-2433">Az.Profile</span></span>
* <span data-ttu-id="35cec-2434">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2434">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="35cec-2435">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2435">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="35cec-2436">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2436">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="35cec-2437">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2437">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="35cec-2438">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2438">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="35cec-2439">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2439">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="35cec-2440">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2440">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-2441">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2441">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-2442">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2442">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2443">Az.Compute</span></span>
* <span data-ttu-id="35cec-2444">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2444">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="35cec-2445">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="35cec-2445">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="35cec-2446">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2446">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2447">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2447">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-2448">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2448">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="35cec-2449">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2449">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="35cec-2450">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="35cec-2450">Az.Insights</span></span>
* <span data-ttu-id="35cec-2451">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2451">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="35cec-2452">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="35cec-2452">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="35cec-2453">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2453">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="35cec-2454">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="35cec-2454">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2455">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2455">Az.Network</span></span>
* <span data-ttu-id="35cec-2456">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="35cec-2456">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="35cec-2457">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-2457">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="35cec-2458">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="35cec-2458">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="35cec-2459">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="35cec-2459">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="35cec-2460">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="35cec-2460">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="35cec-2461">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="35cec-2461">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="35cec-2462">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="35cec-2462">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="35cec-2463">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="35cec-2463">Az.PolicyInsights</span></span>
* <span data-ttu-id="35cec-2464">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2464">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2465">Az.Resources</span></span>
* <span data-ttu-id="35cec-2466">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2466">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="35cec-2467">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2467">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="35cec-2468">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="35cec-2468">Az.ServiceBus</span></span>
* <span data-ttu-id="35cec-2469">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2469">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="35cec-2470">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="35cec-2470">Az.ServiceFabric</span></span>
* <span data-ttu-id="35cec-2471">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2471">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="35cec-2472">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2472">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="35cec-2473">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="35cec-2473">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="35cec-2474">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="35cec-2474">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="35cec-2475">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2475">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="35cec-2476">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2476">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="35cec-2477">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="35cec-2477">Az.Profile</span></span>
* <span data-ttu-id="35cec-2478">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2478">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="35cec-2479">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2479">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2480">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2480">Az.Compute</span></span>
* <span data-ttu-id="35cec-2481">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2481">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="35cec-2482">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2482">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="35cec-2483">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="35cec-2483">Az.DataLakeStore</span></span>
* <span data-ttu-id="35cec-2484">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2484">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="35cec-2485">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2485">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="35cec-2486">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2486">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="35cec-2487">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2487">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="35cec-2488">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="35cec-2488">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2489">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2489">Az.Network</span></span>
* <span data-ttu-id="35cec-2490">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2490">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="35cec-2491">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2491">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2492">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2492">Az.Resources</span></span>
* <span data-ttu-id="35cec-2493">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2493">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="35cec-2494">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2494">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="35cec-2495">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2495">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="35cec-2496">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="35cec-2496">Azure.Storage</span></span>
* <span data-ttu-id="35cec-2497">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2497">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="35cec-2498">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="35cec-2498">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="35cec-2499">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="35cec-2499">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="35cec-2500">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2500">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="35cec-2501">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="35cec-2501">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="35cec-2502">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="35cec-2502">Az.CognitiveServices</span></span>
* <span data-ttu-id="35cec-2503">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2503">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="35cec-2504">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="35cec-2504">Az.Compute</span></span>
* <span data-ttu-id="35cec-2505">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2505">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="35cec-2506">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2506">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="35cec-2507">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2507">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="35cec-2508">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="35cec-2508">Az.DataFactoryV2</span></span>
* <span data-ttu-id="35cec-2509">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2509">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="35cec-2510">Az.Network</span><span class="sxs-lookup"><span data-stu-id="35cec-2510">Az.Network</span></span>
* <span data-ttu-id="35cec-2511">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="35cec-2511">Added NetworkProfile functionality.</span></span> <span data-ttu-id="35cec-2512">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="35cec-2512">new cmdlets added</span></span>
    - <span data-ttu-id="35cec-2513">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="35cec-2513">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="35cec-2514">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="35cec-2514">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="35cec-2515">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="35cec-2515">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="35cec-2516">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="35cec-2516">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="35cec-2517">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-2517">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="35cec-2518">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="35cec-2518">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="35cec-2519">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2519">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="35cec-2520">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2520">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="35cec-2521">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2521">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="35cec-2522">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="35cec-2522">Az.RedisCache</span></span>
* <span data-ttu-id="35cec-2523">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="35cec-2523">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="35cec-2524">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2524">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="35cec-2525">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="35cec-2525">Az.Resources</span></span>
* <span data-ttu-id="35cec-2526">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2526">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="35cec-2527">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2527">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="35cec-2528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="35cec-2528">Az.Sql</span></span>
* <span data-ttu-id="35cec-2529">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="35cec-2529">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="35cec-2530">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="35cec-2530">Az.Websites</span></span>
* <span data-ttu-id="35cec-2531">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="35cec-2531">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="35cec-2532">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="35cec-2532">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="35cec-2533">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="35cec-2533">0.2.0 - September 2018</span></span>
 <span data-ttu-id="35cec-2534">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="35cec-2534">Initial Release</span></span>

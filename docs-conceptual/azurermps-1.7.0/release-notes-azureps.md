---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: c821153db7fb2c337e936abbd8ebb8c848069415
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2018
---
# <a name="release-notes"></a><span data-ttu-id="6f87c-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="6f87c-103">Release notes</span></span>

<span data-ttu-id="6f87c-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="6f87c-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-170"></a><span data-ttu-id="6f87c-105">バージョン 1.7.0</span><span class="sxs-lookup"><span data-stu-id="6f87c-105">Version 1.7.0</span></span>

* <span data-ttu-id="6f87c-106">**全コマンドレットを対象に、-Force、-Confirm、$ConfirmPreference の各パラメーターの動作を変更しました。Microsoft では、PowerShell のガイドラインに合わせてこの実装変更を進めています。これにより、ほとんどのコマンドレットで、Force パラメーターが削除されることになります。ShouldProcess プロンプトをスキップするためには、ユーザーがその PowerShell スクリプトでパラメーター "-Confirm:$false" を追加する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="6f87c-106">**Behavioral change for -Force, –Confirm and $ConfirmPreference parameters for all cmdlets. We are changing this implementation to be in line with PowerShell guidelines. For most cmdlets, this means removing the Force parameter and to skip the ShouldProcess prompt, users will need to include the parameter: ‘-Confirm:$false’ in their PowerShell scripts.**</span></span> <span data-ttu-id="6f87c-107">この変更によって次の問題が解決されます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-107">This changes are addressing following issues:</span></span>
  - <span data-ttu-id="6f87c-108">-WhatIf 機能を正しく実装する。ユーザーは、実際に変更を加えずにコマンドレットまたはスクリプトの影響を確認できます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-108">Correct implementation of –WhatIf functionality, allowing a user to determine the effects of a cmdlet or script without making any actual changes</span></span>
  - <span data-ttu-id="6f87c-109">セッション全体の $ConfirmPreference を使ってプロンプトを制御する。予想される変更の影響 (コマンドレットの ConfirmImpact 設定で指定) に基づいてプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-109">Control over prompting using a session-wide $ConfirmPreference, so that the user is prompted based on the impact of a prospective change (as reported in the ConfirmImpact setting in the cmdlet)</span></span>
  - <span data-ttu-id="6f87c-110">-Confirm パラメーターを使ってコマンドレットごとに確認プロンプトを制御する。</span><span class="sxs-lookup"><span data-stu-id="6f87c-110">Cmdlet-specific control over confirmation prompts using the –Confirm parameter</span></span>
  - <span data-ttu-id="6f87c-111">変更の性格が特殊 (隠しファイルの削除など) であるためにユーザーの確認を必要とするような操作についてのみ ShouldContinue と -Force パラメーターを使用するように全コマンドレットで統一する。</span><span class="sxs-lookup"><span data-stu-id="6f87c-111">Consistent use of ShouldContinue and the –Force parameter across cmdlets, for only those actions that would require prompting from the user due to the special nature of the changes (for example, deleting hidden files)</span></span>
  - <span data-ttu-id="6f87c-112">他のコマンドレットで身に付けた PowerShell スクリプト作成の知識をそのまま Azure PowerShell のコマンドレットに応用できるように他の PowerShell コマンドレットとの一貫性を確保する。</span><span class="sxs-lookup"><span data-stu-id="6f87c-112">Consistency with other PowerShell cmdlets, so that PowerShell scripting knowledge from other cmdlets is immediately applicable to the Azure PowerShell cmdlets.</span></span>

<span data-ttu-id="6f87c-113">**今後、Azure PowerShell コマンドレットで "*すべてのプロンプトをあらゆる状況で自動的にスキップ*" するためには、次の 2 つのパラメーターを指定する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="6f87c-113">**Notice that now to *automatically skip all Prompts in all Circumstances* Azure PowerShell cmdlets require the user to supply two parameters:**</span></span>
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* <span data-ttu-id="6f87c-114">Azure コンピューティング</span><span class="sxs-lookup"><span data-stu-id="6f87c-114">Azure Compute</span></span>
  - <span data-ttu-id="6f87c-115">Set-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="6f87c-115">Set-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="6f87c-116">Get-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="6f87c-116">Get-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="6f87c-117">Restart-AzureVM の -Redeploy パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f87c-117">-Redeploy parameter for Restart-AzureVM</span></span>
  - <span data-ttu-id="6f87c-118">Move-AzureService、Move-AzureStorageAccount、Move-AzureVirtualNetwork の -Validate パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f87c-118">-Validate parameter for Move-AzureService, Move-AzureStorageAccount, and Move-AzureVirtualNetwork</span></span>
  - <span data-ttu-id="6f87c-119">従来と同様、拡張機能のコマンドレットに対する名前とバージョンのパラメーターは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="6f87c-119">Name and version parameters for extension cmdlets are optional as before.</span></span>
  - <span data-ttu-id="6f87c-120">New-AzureVM で VM オブジェクトのライセンス タイプを取得できます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-120">New-AzureVM can get a license type from VM object.</span></span>
* <span data-ttu-id="6f87c-121">Azure Storage</span><span class="sxs-lookup"><span data-stu-id="6f87c-121">Azure Storage</span></span>
  - <span data-ttu-id="6f87c-122">Tags パラメーターを Tag に変更し、パラメーター エイリアスとして Tags を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-122">Change Tags Parameter to Tag, and add parameter alias Tags</span></span>
    + <span data-ttu-id="6f87c-123">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-123">New-AzureRmStorageAccount</span></span>
    + <span data-ttu-id="6f87c-124">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-124">Set-AzureRmStorageAccount</span></span>
* <span data-ttu-id="6f87c-125">Azure ネットワーク</span><span class="sxs-lookup"><span data-stu-id="6f87c-125">Azure Network</span></span>
  - <span data-ttu-id="6f87c-126">仮想ネットワーク ピアリング用の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-126">New cmdlet added for Virtual Network Peering</span></span>
* <span data-ttu-id="6f87c-127">Azure Redis Cache</span><span class="sxs-lookup"><span data-stu-id="6f87c-127">Azure Redis Cache</span></span>
  - <span data-ttu-id="6f87c-128">新しいコマンドレット Reset-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-128">New cmdlet added for Reset-AzureRmRedisCache</span></span>
  - <span data-ttu-id="6f87c-129">新しいコマンドレット Export-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-129">New cmdlet added for Export-AzureRmRedisCache</span></span>
  - <span data-ttu-id="6f87c-130">新しいコマンドレット Import-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-130">New cmdlet added for Import-AzureRmRedisCache</span></span>
  - <span data-ttu-id="6f87c-131">vNet に関するパラメーターの変更を反映するためにコマンドレット New-AzureRmRedisCache を変更しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-131">Modified cmdlet New-AzureRmRedisCache to include parameter change for vNet</span></span>
* <span data-ttu-id="6f87c-132">Azure SQL DB バックアップ/復元</span><span class="sxs-lookup"><span data-stu-id="6f87c-132">Azure SQL DB Backup/Restore</span></span>
  - <span data-ttu-id="6f87c-133">LTR (長期的な保有期間) バックアップ機能のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6f87c-133">Cmdlets for LTR (Long Term Retention) backup feature</span></span>
  - <span data-ttu-id="6f87c-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="6f87c-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="6f87c-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="6f87c-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="6f87c-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="6f87c-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="6f87c-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="6f87c-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="6f87c-138">削除されたデータベースを Restore-AzureRmSqlDatabase で特定の時点まで復元できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-138">Restore-AzureRmSqlDatabase now supports point-in-time restore of a deleted database</span></span>
  - <span data-ttu-id="6f87c-139">Restore-AzureRmSqlDatabase が長期的な保有期間バックアップからの復元に対応しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-139">Restore-AzureRmSqlDatabase now supports restoring from a Long Term Retention backup</span></span>
* <span data-ttu-id="6f87c-140">Azure LogicApp</span><span class="sxs-lookup"><span data-stu-id="6f87c-140">Azure LogicApp</span></span>
  - <span data-ttu-id="6f87c-141">LogicApp 統合アカウントのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-141">Added LogicApp Integration accounts cmdlets.</span></span>
  - <span data-ttu-id="6f87c-142">Get-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="6f87c-142">Get-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="6f87c-143">Get-AzureRmIntegrationAccountCallbackUrl</span><span class="sxs-lookup"><span data-stu-id="6f87c-143">Get-AzureRmIntegrationAccountCallbackUrl</span></span>
  - <span data-ttu-id="6f87c-144">Get-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="6f87c-144">Get-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="6f87c-145">Get-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-145">Get-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="6f87c-146">Get-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="6f87c-146">Get-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="6f87c-147">Get-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="6f87c-147">Get-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="6f87c-148">Get-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="6f87c-148">Get-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="6f87c-149">New-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="6f87c-149">New-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="6f87c-150">New-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="6f87c-150">New-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="6f87c-151">New-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-151">New-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="6f87c-152">New-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="6f87c-152">New-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="6f87c-153">New-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="6f87c-153">New-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="6f87c-154">New-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="6f87c-154">New-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="6f87c-155">Remove-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="6f87c-155">Remove-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="6f87c-156">Remove-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="6f87c-156">Remove-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="6f87c-157">Remove-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-157">Remove-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="6f87c-158">Remove-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="6f87c-158">Remove-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="6f87c-159">Remove-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="6f87c-159">Remove-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="6f87c-160">Remove-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="6f87c-160">Remove-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="6f87c-161">Set-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="6f87c-161">Set-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="6f87c-162">Set-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="6f87c-162">Set-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="6f87c-163">Set-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="6f87c-163">Set-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="6f87c-164">Set-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="6f87c-164">Set-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="6f87c-165">Set-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="6f87c-165">Set-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="6f87c-166">Set-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="6f87c-166">Set-AzureRmIntegrationAccountSchema</span></span>
* <span data-ttu-id="6f87c-167">Azure Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6f87c-167">Azure Data Lake Store</span></span>
  - <span data-ttu-id="6f87c-168">ファイルとフォルダーのアップロードとダウンロードのパフォーマンスが大幅に向上しています。</span><span class="sxs-lookup"><span data-stu-id="6f87c-168">Drastically improve performance of file and folder upload and download.</span></span>
  - <span data-ttu-id="6f87c-169">ダウンロードに関してパラメーター名がわずかに変更されたほか、アップロードに関しては、次のパラメーターが新たに 2 つ追加されました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-169">This includes a slight change to the parameter names for download and inclusion of two new parameters for upload:</span></span>
    + <span data-ttu-id="6f87c-170">NumThreads -> PerFileThreadCount。1 ファイルあたりのスレッド数を指定する目的で使用します。</span><span class="sxs-lookup"><span data-stu-id="6f87c-170">NumThreads -> PerFileThreadCount, used to indicate the number of threads to use in a single file</span></span>
    + <span data-ttu-id="6f87c-171">ConcurrentFileCount。フォルダーのアップロード/ダウンロード時に同時にアップロード/ダウンロードするファイル数を指定する目的で使用します。</span><span class="sxs-lookup"><span data-stu-id="6f87c-171">ConcurrentFileCount, used to indicate the number of files to upload/download in parallel for folder upload/download.</span></span>
  - <span data-ttu-id="6f87c-172">既定のスレッド値。ほとんどのファイル サイズで良好なスループットが得られるように意図された値が指定されています。</span><span class="sxs-lookup"><span data-stu-id="6f87c-172">Default threading values are now designed to give a better all around throughput for most file sizes.</span></span> <span data-ttu-id="6f87c-173">適切なパフォーマンスが得られない場合は、要件を満たすように上記の値を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-173">If performance is not as desired, the values above can be modified to meet requirements.</span></span>
* <span data-ttu-id="6f87c-174">Azure Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6f87c-174">Azure Data Lake Analytics</span></span>
  - <span data-ttu-id="6f87c-175">Get-AzureRMDataLakeAnalyticsDataSource に引数を指定しなかった場合、すべてのデータ ソースが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-175">Get-AzureRMDataLakeAnalyticsDataSource now returns all data sources when called with no arguments.</span></span>
  - <span data-ttu-id="6f87c-176">この変更に伴い、対応するデータ ソース タイプ パラメーターがコマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="6f87c-176">This change also removes the data source type parameter from the cmdlet.</span></span>
  - <span data-ttu-id="6f87c-177">この変更に伴い、次のプロパティを使ったリスト操作で新しいオブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f87c-177">This change results in a new object being returned for the list operation with the following properties:</span></span>
    + <span data-ttu-id="6f87c-178">Type: データ ソースの種類。</span><span class="sxs-lookup"><span data-stu-id="6f87c-178">Type, the type of data source</span></span>
    + <span data-ttu-id="6f87c-179">Name: データ ソースの名前。</span><span class="sxs-lookup"><span data-stu-id="6f87c-179">Name, the name of the data source</span></span>
    + <span data-ttu-id="6f87c-180">IsDefault: アカウントの既定のデータ ソースである場合は true に設定します。</span><span class="sxs-lookup"><span data-stu-id="6f87c-180">IsDefault, set to true if this is the default data source for the account</span></span>
  - <span data-ttu-id="6f87c-181">submittedBefore と submittedAfter を条件としてフィルタリングを行う際の特定の日時オフセット値のリストに関して、Get-AzureRMDataLakeAnalyticsJob を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-181">Get-AzureRMDataLakeAnalyticsJob fixed for list for certain date time offset values when filtering on submittedBefore and submittedAfter.</span></span>
* <span data-ttu-id="6f87c-182">Web Apps</span><span class="sxs-lookup"><span data-stu-id="6f87c-182">Web Apps</span></span>
  - <span data-ttu-id="6f87c-183">通常のスワップとプレビュー付きスワップに対応した Swap-AzureRmWebAppSlot コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-183">Add Swap-AzureRmWebAppSlot cmdlet for regular swap and swap with preview</span></span>
  - <span data-ttu-id="6f87c-184">Set-AzureRmWebAppSlot コマンドレットを拡張し、自動スワップに対応しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-184">Extend Set-AzureRmWebAppSlot cmdlet to support auto swap</span></span>
* <span data-ttu-id="6f87c-185">Azure API Management</span><span class="sxs-lookup"><span data-stu-id="6f87c-185">Azure API Management</span></span>
  - <span data-ttu-id="6f87c-186">AzureChinaCloud の Azure API Management デプロイ コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-186">Fixed Azure Api Management Deployment cmdlets for AzureChinaCloud.</span></span>
  - <span data-ttu-id="6f87c-187">Git アクセスは既定で有効になっているため、Set-AzureRmApiManagementTenantGitAccess コマンドレットは削除しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-187">Removed cmdlet Set-AzureRmApiManagementTenantGitAccess as Git Access is enabled by Default.</span></span>
* <span data-ttu-id="6f87c-188">Azure Recovery Services バックアップ</span><span class="sxs-lookup"><span data-stu-id="6f87c-188">Azure Recovery Services Backup</span></span>
  - <span data-ttu-id="6f87c-189">新たに Azure SQL ワークロードに対応しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-189">Added support for the Azure SQL workload</span></span>
  - <span data-ttu-id="6f87c-190">暗号化された Azure VM のバックアップと復元に新たに対応しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-190">Added support for backing up and restoring encrypted Azure VMs</span></span>
  - <span data-ttu-id="6f87c-191">Backup-AzureRmRecoveryServicesBackupItem - 復旧ポイントに関してオプションの保持期間機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-191">Backup-AzureRmRecoveryServicesBackupItem - Added optional retention time feature for recovery points</span></span>
  - <span data-ttu-id="6f87c-192">Get-AzureRmRecoveryServicesBackupContainer コマンドレットと Get-AzureRmRecoveryServicesBackupItem コマンドレットのフィルターに関連した小さなバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-192">Minor filter-related bug fixes in Get-AzureRmRecoveryServicesBackupContainer and Get-AzureRmRecoveryServicesBackupItem cmdlets</span></span>
* <span data-ttu-id="6f87c-193">Azure Automation</span><span class="sxs-lookup"><span data-stu-id="6f87c-193">Azure Automation</span></span>
  - <span data-ttu-id="6f87c-194">Get-AzureRmAutomationHybridWorkerGroup を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6f87c-194">Added Get-AzureRmAutomationHybridWorkerGroup</span></span>

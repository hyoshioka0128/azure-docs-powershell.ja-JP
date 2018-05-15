---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 0a3f152751fee569d3ac5fba6bcff8c1737f7b8c
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a><span data-ttu-id="a3f4b-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="a3f4b-103">Release notes</span></span>

<span data-ttu-id="a3f4b-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-170"></a><span data-ttu-id="a3f4b-105">バージョン 1.7.0</span><span class="sxs-lookup"><span data-stu-id="a3f4b-105">Version 1.7.0</span></span>

* <span data-ttu-id="a3f4b-106">**全コマンドレットを対象に、-Force、-Confirm、$ConfirmPreference の各パラメーターの動作を変更しました。Microsoft では、PowerShell のガイドラインに合わせてこの実装変更を進めています。これにより、ほとんどのコマンドレットで、Force パラメーターが削除されることになります。ShouldProcess プロンプトをスキップするためには、ユーザーがその PowerShell スクリプトでパラメーター "-Confirm:$false" を追加する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="a3f4b-106">**Behavioral change for -Force, –Confirm and $ConfirmPreference parameters for all cmdlets. We are changing this implementation to be in line with PowerShell guidelines. For most cmdlets, this means removing the Force parameter and to skip the ShouldProcess prompt, users will need to include the parameter: ‘-Confirm:$false’ in their PowerShell scripts.**</span></span> <span data-ttu-id="a3f4b-107">この変更によって次の問題が解決されます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-107">This changes are addressing following issues:</span></span>
  - <span data-ttu-id="a3f4b-108">-WhatIf 機能を正しく実装する。ユーザーは、実際に変更を加えずにコマンドレットまたはスクリプトの影響を確認できます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-108">Correct implementation of –WhatIf functionality, allowing a user to determine the effects of a cmdlet or script without making any actual changes</span></span>
  - <span data-ttu-id="a3f4b-109">セッション全体の $ConfirmPreference を使ってプロンプトを制御する。予想される変更の影響 (コマンドレットの ConfirmImpact 設定で指定) に基づいてプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-109">Control over prompting using a session-wide $ConfirmPreference, so that the user is prompted based on the impact of a prospective change (as reported in the ConfirmImpact setting in the cmdlet)</span></span>
  - <span data-ttu-id="a3f4b-110">-Confirm パラメーターを使ってコマンドレットごとに確認プロンプトを制御する。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-110">Cmdlet-specific control over confirmation prompts using the –Confirm parameter</span></span>
  - <span data-ttu-id="a3f4b-111">変更の性格が特殊 (隠しファイルの削除など) であるためにユーザーの確認を必要とするような操作についてのみ ShouldContinue と -Force パラメーターを使用するように全コマンドレットで統一する。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-111">Consistent use of ShouldContinue and the –Force parameter across cmdlets, for only those actions that would require prompting from the user due to the special nature of the changes (for example, deleting hidden files)</span></span>
  - <span data-ttu-id="a3f4b-112">他のコマンドレットで身に付けた PowerShell スクリプト作成の知識をそのまま Azure PowerShell のコマンドレットに応用できるように他の PowerShell コマンドレットとの一貫性を確保する。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-112">Consistency with other PowerShell cmdlets, so that PowerShell scripting knowledge from other cmdlets is immediately applicable to the Azure PowerShell cmdlets.</span></span>

<span data-ttu-id="a3f4b-113">**今後、Azure PowerShell コマンドレットで "*すべてのプロンプトをあらゆる状況で自動的にスキップ*" するためには、次の 2 つのパラメーターを指定する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="a3f4b-113">**Notice that now to *automatically skip all Prompts in all Circumstances* Azure PowerShell cmdlets require the user to supply two parameters:**</span></span>
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* <span data-ttu-id="a3f4b-114">Azure コンピューティング</span><span class="sxs-lookup"><span data-stu-id="a3f4b-114">Azure Compute</span></span>
  - <span data-ttu-id="a3f4b-115">Set-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="a3f4b-115">Set-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="a3f4b-116">Get-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="a3f4b-116">Get-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="a3f4b-117">Restart-AzureVM の -Redeploy パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3f4b-117">-Redeploy parameter for Restart-AzureVM</span></span>
  - <span data-ttu-id="a3f4b-118">Move-AzureService、Move-AzureStorageAccount、Move-AzureVirtualNetwork の -Validate パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3f4b-118">-Validate parameter for Move-AzureService, Move-AzureStorageAccount, and Move-AzureVirtualNetwork</span></span>
  - <span data-ttu-id="a3f4b-119">従来と同様、拡張機能のコマンドレットに対する名前とバージョンのパラメーターは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-119">Name and version parameters for extension cmdlets are optional as before.</span></span>
  - <span data-ttu-id="a3f4b-120">New-AzureVM で VM オブジェクトのライセンス タイプを取得できます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-120">New-AzureVM can get a license type from VM object.</span></span>
* <span data-ttu-id="a3f4b-121">Azure Storage</span><span class="sxs-lookup"><span data-stu-id="a3f4b-121">Azure Storage</span></span>
  - <span data-ttu-id="a3f4b-122">Tags パラメーターを Tag に変更し、パラメーター エイリアスとして Tags を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-122">Change Tags Parameter to Tag, and add parameter alias Tags</span></span>
    + <span data-ttu-id="a3f4b-123">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-123">New-AzureRmStorageAccount</span></span>
    + <span data-ttu-id="a3f4b-124">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-124">Set-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a3f4b-125">Azure ネットワーク</span><span class="sxs-lookup"><span data-stu-id="a3f4b-125">Azure Network</span></span>
  - <span data-ttu-id="a3f4b-126">仮想ネットワーク ピアリング用の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-126">New cmdlet added for Virtual Network Peering</span></span>
* <span data-ttu-id="a3f4b-127">Azure Redis Cache</span><span class="sxs-lookup"><span data-stu-id="a3f4b-127">Azure Redis Cache</span></span>
  - <span data-ttu-id="a3f4b-128">新しいコマンドレット Reset-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-128">New cmdlet added for Reset-AzureRmRedisCache</span></span>
  - <span data-ttu-id="a3f4b-129">新しいコマンドレット Export-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-129">New cmdlet added for Export-AzureRmRedisCache</span></span>
  - <span data-ttu-id="a3f4b-130">新しいコマンドレット Import-AzureRmRedisCache を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-130">New cmdlet added for Import-AzureRmRedisCache</span></span>
  - <span data-ttu-id="a3f4b-131">vNet に関するパラメーターの変更を反映するためにコマンドレット New-AzureRmRedisCache を変更しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-131">Modified cmdlet New-AzureRmRedisCache to include parameter change for vNet</span></span>
* <span data-ttu-id="a3f4b-132">Azure SQL DB バックアップ/復元</span><span class="sxs-lookup"><span data-stu-id="a3f4b-132">Azure SQL DB Backup/Restore</span></span>
  - <span data-ttu-id="a3f4b-133">LTR (長期的な保有期間) バックアップ機能のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a3f4b-133">Cmdlets for LTR (Long Term Retention) backup feature</span></span>
  - <span data-ttu-id="a3f4b-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="a3f4b-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="a3f4b-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a3f4b-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="a3f4b-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="a3f4b-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="a3f4b-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a3f4b-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="a3f4b-138">削除されたデータベースを Restore-AzureRmSqlDatabase で特定の時点まで復元できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-138">Restore-AzureRmSqlDatabase now supports point-in-time restore of a deleted database</span></span>
  - <span data-ttu-id="a3f4b-139">Restore-AzureRmSqlDatabase が長期的な保有期間バックアップからの復元に対応しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-139">Restore-AzureRmSqlDatabase now supports restoring from a Long Term Retention backup</span></span>
* <span data-ttu-id="a3f4b-140">Azure LogicApp</span><span class="sxs-lookup"><span data-stu-id="a3f4b-140">Azure LogicApp</span></span>
  - <span data-ttu-id="a3f4b-141">LogicApp 統合アカウントのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-141">Added LogicApp Integration accounts cmdlets.</span></span>
  - <span data-ttu-id="a3f4b-142">Get-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="a3f4b-142">Get-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="a3f4b-143">Get-AzureRmIntegrationAccountCallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a3f4b-143">Get-AzureRmIntegrationAccountCallbackUrl</span></span>
  - <span data-ttu-id="a3f4b-144">Get-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="a3f4b-144">Get-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="a3f4b-145">Get-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-145">Get-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="a3f4b-146">Get-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="a3f4b-146">Get-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="a3f4b-147">Get-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="a3f4b-147">Get-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="a3f4b-148">Get-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="a3f4b-148">Get-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="a3f4b-149">New-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="a3f4b-149">New-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="a3f4b-150">New-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="a3f4b-150">New-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="a3f4b-151">New-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-151">New-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="a3f4b-152">New-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="a3f4b-152">New-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="a3f4b-153">New-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="a3f4b-153">New-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="a3f4b-154">New-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="a3f4b-154">New-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="a3f4b-155">Remove-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="a3f4b-155">Remove-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="a3f4b-156">Remove-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="a3f4b-156">Remove-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="a3f4b-157">Remove-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-157">Remove-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="a3f4b-158">Remove-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="a3f4b-158">Remove-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="a3f4b-159">Remove-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="a3f4b-159">Remove-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="a3f4b-160">Remove-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="a3f4b-160">Remove-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="a3f4b-161">Set-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="a3f4b-161">Set-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="a3f4b-162">Set-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="a3f4b-162">Set-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="a3f4b-163">Set-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="a3f4b-163">Set-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="a3f4b-164">Set-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="a3f4b-164">Set-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="a3f4b-165">Set-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="a3f4b-165">Set-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="a3f4b-166">Set-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="a3f4b-166">Set-AzureRmIntegrationAccountSchema</span></span>
* <span data-ttu-id="a3f4b-167">Azure Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a3f4b-167">Azure Data Lake Store</span></span>
  - <span data-ttu-id="a3f4b-168">ファイルとフォルダーのアップロードとダウンロードのパフォーマンスが大幅に向上しています。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-168">Drastically improve performance of file and folder upload and download.</span></span>
  - <span data-ttu-id="a3f4b-169">ダウンロードに関してパラメーター名がわずかに変更されたほか、アップロードに関しては、次のパラメーターが新たに 2 つ追加されました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-169">This includes a slight change to the parameter names for download and inclusion of two new parameters for upload:</span></span>
    + <span data-ttu-id="a3f4b-170">NumThreads -> PerFileThreadCount。1 ファイルあたりのスレッド数を指定する目的で使用します。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-170">NumThreads -> PerFileThreadCount, used to indicate the number of threads to use in a single file</span></span>
    + <span data-ttu-id="a3f4b-171">ConcurrentFileCount。フォルダーのアップロード/ダウンロード時に同時にアップロード/ダウンロードするファイル数を指定する目的で使用します。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-171">ConcurrentFileCount, used to indicate the number of files to upload/download in parallel for folder upload/download.</span></span>
  - <span data-ttu-id="a3f4b-172">既定のスレッド値。ほとんどのファイル サイズで良好なスループットが得られるように意図された値が指定されています。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-172">Default threading values are now designed to give a better all around throughput for most file sizes.</span></span> <span data-ttu-id="a3f4b-173">適切なパフォーマンスが得られない場合は、要件を満たすように上記の値を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-173">If performance is not as desired, the values above can be modified to meet requirements.</span></span>
* <span data-ttu-id="a3f4b-174">Azure Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a3f4b-174">Azure Data Lake Analytics</span></span>
  - <span data-ttu-id="a3f4b-175">Get-AzureRMDataLakeAnalyticsDataSource に引数を指定しなかった場合、すべてのデータ ソースが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-175">Get-AzureRMDataLakeAnalyticsDataSource now returns all data sources when called with no arguments.</span></span>
  - <span data-ttu-id="a3f4b-176">この変更に伴い、対応するデータ ソース タイプ パラメーターがコマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-176">This change also removes the data source type parameter from the cmdlet.</span></span>
  - <span data-ttu-id="a3f4b-177">この変更に伴い、次のプロパティを使ったリスト操作で新しいオブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-177">This change results in a new object being returned for the list operation with the following properties:</span></span>
    + <span data-ttu-id="a3f4b-178">Type: データ ソースの種類。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-178">Type, the type of data source</span></span>
    + <span data-ttu-id="a3f4b-179">Name: データ ソースの名前。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-179">Name, the name of the data source</span></span>
    + <span data-ttu-id="a3f4b-180">IsDefault: アカウントの既定のデータ ソースである場合は true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-180">IsDefault, set to true if this is the default data source for the account</span></span>
  - <span data-ttu-id="a3f4b-181">submittedBefore と submittedAfter を条件としてフィルタリングを行う際の特定の日時オフセット値のリストに関して、Get-AzureRMDataLakeAnalyticsJob を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-181">Get-AzureRMDataLakeAnalyticsJob fixed for list for certain date time offset values when filtering on submittedBefore and submittedAfter.</span></span>
* <span data-ttu-id="a3f4b-182">Web Apps</span><span class="sxs-lookup"><span data-stu-id="a3f4b-182">Web Apps</span></span>
  - <span data-ttu-id="a3f4b-183">通常のスワップとプレビュー付きスワップに対応した Swap-AzureRmWebAppSlot コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-183">Add Swap-AzureRmWebAppSlot cmdlet for regular swap and swap with preview</span></span>
  - <span data-ttu-id="a3f4b-184">Set-AzureRmWebAppSlot コマンドレットを拡張し、自動スワップに対応しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-184">Extend Set-AzureRmWebAppSlot cmdlet to support auto swap</span></span>
* <span data-ttu-id="a3f4b-185">Azure API Management</span><span class="sxs-lookup"><span data-stu-id="a3f4b-185">Azure API Management</span></span>
  - <span data-ttu-id="a3f4b-186">AzureChinaCloud の Azure API Management デプロイ コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-186">Fixed Azure Api Management Deployment cmdlets for AzureChinaCloud.</span></span>
  - <span data-ttu-id="a3f4b-187">Git アクセスは既定で有効になっているため、Set-AzureRmApiManagementTenantGitAccess コマンドレットは削除しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-187">Removed cmdlet Set-AzureRmApiManagementTenantGitAccess as Git Access is enabled by Default.</span></span>
* <span data-ttu-id="a3f4b-188">Azure Recovery Services バックアップ</span><span class="sxs-lookup"><span data-stu-id="a3f4b-188">Azure Recovery Services Backup</span></span>
  - <span data-ttu-id="a3f4b-189">新たに Azure SQL ワークロードに対応しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-189">Added support for the Azure SQL workload</span></span>
  - <span data-ttu-id="a3f4b-190">暗号化された Azure VM のバックアップと復元に新たに対応しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-190">Added support for backing up and restoring encrypted Azure VMs</span></span>
  - <span data-ttu-id="a3f4b-191">Backup-AzureRmRecoveryServicesBackupItem - 復旧ポイントに関してオプションの保持期間機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-191">Backup-AzureRmRecoveryServicesBackupItem - Added optional retention time feature for recovery points</span></span>
  - <span data-ttu-id="a3f4b-192">Get-AzureRmRecoveryServicesBackupContainer コマンドレットと Get-AzureRmRecoveryServicesBackupItem コマンドレットのフィルターに関連した小さなバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-192">Minor filter-related bug fixes in Get-AzureRmRecoveryServicesBackupContainer and Get-AzureRmRecoveryServicesBackupItem cmdlets</span></span>
* <span data-ttu-id="a3f4b-193">Azure Automation</span><span class="sxs-lookup"><span data-stu-id="a3f4b-193">Azure Automation</span></span>
  - <span data-ttu-id="a3f4b-194">Get-AzureRmAutomationHybridWorkerGroup を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a3f4b-194">Added Get-AzureRmAutomationHybridWorkerGroup</span></span>

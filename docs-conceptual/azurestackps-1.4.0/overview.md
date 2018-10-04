---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: 72d147f5bc9c882083dda6b33b1c89663fd2eb34
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/04/2018
ms.locfileid: "47424855"
---
# <a name="azure-stack-module-140"></a><span data-ttu-id="35aaf-103">Azure Stack Module 1.4.0</span><span class="sxs-lookup"><span data-stu-id="35aaf-103">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="35aaf-104">要件:</span><span class="sxs-lookup"><span data-stu-id="35aaf-104">Requirements:</span></span>
<span data-ttu-id="35aaf-105">サポートされている Azure Stack の最小バージョンは 1804 です。</span><span class="sxs-lookup"><span data-stu-id="35aaf-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="35aaf-106">注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="35aaf-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="35aaf-107">既知の問題:</span><span class="sxs-lookup"><span data-stu-id="35aaf-107">Known issues:</span></span>

- <span data-ttu-id="35aaf-108">アラートを閉じるには、Azure Stack バージョン 1803 が必要です。</span><span class="sxs-lookup"><span data-stu-id="35aaf-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="35aaf-109">New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="35aaf-109">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="35aaf-110">状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="35aaf-110">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="35aaf-111">再デプロイせずに IP プールを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="35aaf-111">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="35aaf-112">重大な変更</span><span class="sxs-lookup"><span data-stu-id="35aaf-112">Breaking Changes</span></span>
<span data-ttu-id="35aaf-113">バージョン 1.3.0 からの重大な変更はありません。</span><span class="sxs-lookup"><span data-stu-id="35aaf-113">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="35aaf-114">1.2.11 からの移行に関する重大な変更はすべて https://aka.ms/azspowershellmigration に記載されています。</span><span class="sxs-lookup"><span data-stu-id="35aaf-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="35aaf-115">Install</span><span class="sxs-lookup"><span data-stu-id="35aaf-115">Install</span></span>
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="35aaf-116">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="35aaf-116">Release Notes</span></span>
    * <span data-ttu-id="35aaf-117">Azure Stack 1.4.0 バージョンには、以前のリリース 1.3.0 からの重大な変更はありません</span><span class="sxs-lookup"><span data-stu-id="35aaf-117">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="35aaf-118">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-118">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="35aaf-119">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-119">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-120">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-120">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="35aaf-121">Set-AzsBackupShare コマンドレットに、BackupFrequencyInHours、IsBackupSchedulerEnabled、BackupRetentionPeriodInDays の各パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-121">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="35aaf-122">暗号化キーの作成を容易にするために、New-EncyptionKeyBase64 コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-122">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="35aaf-123">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-124">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-124">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="35aaf-125">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-125">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-126">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-126">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="35aaf-127">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-127">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="35aaf-128">管理者が Azure Stack スタンプに新しいスケール ユニット ノードを追加できるように、Add-AzsScaleUnitNode コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-128">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="35aaf-129">スケール ユニット パラメーター オブジェクトの作成を容易にするために、New-AzsScaleUnitNodeObject コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-129">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="35aaf-130">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-130">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="35aaf-131">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-132">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-132">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="35aaf-133">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-134">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-134">Azs.Network.Admin</span></span>
        - <span data-ttu-id="35aaf-135">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-136">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-136">Azs.Update.Admin</span></span>
        - <span data-ttu-id="35aaf-137">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-138">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="35aaf-138">Azs.Subscriptions</span></span>
        - <span data-ttu-id="35aaf-139">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-139">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="35aaf-140">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="35aaf-140">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="35aaf-141">委任されたプロバイダーのプラン間でサブスクリプションを移動するために、Move-AzsSubscription コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-141">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="35aaf-142">委任されたプロバイダーのプラン間でユーザー サブスクリプションを移動できることを検証するために、Test-AzsMoveSubscription コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="35aaf-142">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="35aaf-143">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="35aaf-143">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="35aaf-144">内容:</span><span class="sxs-lookup"><span data-stu-id="35aaf-144">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="35aaf-145">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="35aaf-145">Azure Bridge</span></span>
<span data-ttu-id="35aaf-146">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-146">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="35aaf-147">Backup</span><span class="sxs-lookup"><span data-stu-id="35aaf-147">Backup</span></span>
<span data-ttu-id="35aaf-148">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-148">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="35aaf-149">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="35aaf-149">Configure where backups are stored</span></span>
- <span data-ttu-id="35aaf-150">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="35aaf-150">Perform backups</span></span>
- <span data-ttu-id="35aaf-151">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="35aaf-151">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="35aaf-152">コマース</span><span class="sxs-lookup"><span data-stu-id="35aaf-152">Commerce</span></span>
<span data-ttu-id="35aaf-153">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-153">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="35aaf-154">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="35aaf-154">Compute</span></span>
<span data-ttu-id="35aaf-155">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="35aaf-155">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="35aaf-156">Fabric</span><span class="sxs-lookup"><span data-stu-id="35aaf-156">Fabric</span></span>
<span data-ttu-id="35aaf-157">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-157">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="35aaf-158">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="35aaf-158">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="35aaf-159">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="35aaf-159">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="35aaf-160">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="35aaf-160">Repair of scale unit nodes</span></span>
- <span data-ttu-id="35aaf-161">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="35aaf-161">Restart of Infrastructure role</span></span>
- <span data-ttu-id="35aaf-162">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="35aaf-162">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="35aaf-163">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="35aaf-163">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="35aaf-164">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="35aaf-164">Gallery</span></span>
<span data-ttu-id="35aaf-165">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="35aaf-165">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="35aaf-166">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="35aaf-166">Infrastructure Insights</span></span>
<span data-ttu-id="35aaf-167">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-167">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="35aaf-168">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-168">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="35aaf-169">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-169">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="35aaf-170">KeyVault</span><span class="sxs-lookup"><span data-stu-id="35aaf-170">KeyVault</span></span>
<span data-ttu-id="35aaf-171">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-171">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="35aaf-172">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="35aaf-172">Network</span></span>
<span data-ttu-id="35aaf-173">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="35aaf-173">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="35aaf-174">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-174">Management of network quotas</span></span>
- <span data-ttu-id="35aaf-175">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-175">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="35aaf-176">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="35aaf-176">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="35aaf-177">Storage</span><span class="sxs-lookup"><span data-stu-id="35aaf-177">Storage</span></span>
<span data-ttu-id="35aaf-178">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="35aaf-178">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="35aaf-179">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="35aaf-179">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="35aaf-180">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-180">Manage storage quotas</span></span>
- <span data-ttu-id="35aaf-181">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="35aaf-181">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="35aaf-182">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="35aaf-182">Restore deleted storage accounts</span></span>
- <span data-ttu-id="35aaf-183">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="35aaf-183">Migrate containers from one share to another</span></span>
- <span data-ttu-id="35aaf-184">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-184">View information about the individual storage components</span></span>
- <span data-ttu-id="35aaf-185">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-185">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="35aaf-186">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-186">Subscription Admin</span></span>
<span data-ttu-id="35aaf-187">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="35aaf-187">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="35aaf-188">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="35aaf-188">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="35aaf-189">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-189">Manage plans and offers</span></span>
- <span data-ttu-id="35aaf-190">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-190">View usage and performance information</span></span>
- <span data-ttu-id="35aaf-191">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="35aaf-191">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="35aaf-192">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="35aaf-192">Subscription</span></span>
<span data-ttu-id="35aaf-193">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="35aaf-193">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="35aaf-194">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="35aaf-194">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="35aaf-195">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="35aaf-195">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="35aaf-196">アップデート</span><span class="sxs-lookup"><span data-stu-id="35aaf-196">Update</span></span>
<span data-ttu-id="35aaf-197">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="35aaf-197">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="35aaf-198">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="35aaf-198">In this module administrators can:</span></span>
- <span data-ttu-id="35aaf-199">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="35aaf-199">List and install available updates</span></span>
- <span data-ttu-id="35aaf-200">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="35aaf-200">Resume interrupted updates</span></span>
- <span data-ttu-id="35aaf-201">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="35aaf-201">View installed updates</span></span>

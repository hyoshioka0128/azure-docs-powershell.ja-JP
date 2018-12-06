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
ms.openlocfilehash: afa83a6258e57e961576b328e67fad634704dddf
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52827311"
---
# <a name="azure-stack-module-150"></a><span data-ttu-id="f3374-103">Azure Stack Module 1.5.0</span><span class="sxs-lookup"><span data-stu-id="f3374-103">Azure Stack Module 1.5.0</span></span>

## <a name="requirements"></a><span data-ttu-id="f3374-104">要件:</span><span class="sxs-lookup"><span data-stu-id="f3374-104">Requirements:</span></span>
<span data-ttu-id="f3374-105">サポートされている Azure Stack の最小バージョンは 1808 です。</span><span class="sxs-lookup"><span data-stu-id="f3374-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="f3374-106">注: 以前のバージョンを使用している場合は、バージョン 1.4.0 をインストールしてください</span><span class="sxs-lookup"><span data-stu-id="f3374-106">Note: If you are using an earlier version install version 1.4.0</span></span>

## <a name="known-issues"></a><span data-ttu-id="f3374-107">既知の問題:</span><span class="sxs-lookup"><span data-stu-id="f3374-107">Known issues:</span></span>

- <span data-ttu-id="f3374-108">New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="f3374-108">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="f3374-109">状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3374-109">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="f3374-110">再デプロイせずに IP プールを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="f3374-110">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="install"></a><span data-ttu-id="f3374-111">Install</span><span class="sxs-lookup"><span data-stu-id="f3374-111">Install</span></span>
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.5.0
```

## <a name="release-notes"></a><span data-ttu-id="f3374-112">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="f3374-112">Release Notes</span></span>
* <span data-ttu-id="f3374-113">AzureRm.Profile モジュールへの同等以上の依存関係が確立されるように、すべての Azure Stack 管理モジュールが更新されました</span><span class="sxs-lookup"><span data-stu-id="f3374-113">All the Azure Stack Admin modules are updated for greater than or equal to dependency on the AzureRm.Profile module</span></span>
* <span data-ttu-id="f3374-114">すべてのモジュール内の入れ子になったリソース名を処理するためのサポート</span><span class="sxs-lookup"><span data-stu-id="f3374-114">Support for handling nested resource names in all the modules</span></span>
* <span data-ttu-id="f3374-115">ErrorActionPreference が上書きされて Stop になる、すべてのモジュールでのバグ修正</span><span class="sxs-lookup"><span data-stu-id="f3374-115">Bug fix in all the modules where ErrorActionPreference is being overridden to be Stop</span></span>
* <span data-ttu-id="f3374-116">Azs.Compute.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="f3374-116">Azs.Compute.Admin Module</span></span>
    * <span data-ttu-id="f3374-117">マネージド ディスクをサポートするために新しいクォータ プロパティが追加されました</span><span class="sxs-lookup"><span data-stu-id="f3374-117">New quota properties added for the support of manged disk</span></span>
    * <span data-ttu-id="f3374-118">ディスク移行関連のコマンドレットの追加</span><span class="sxs-lookup"><span data-stu-id="f3374-118">Addition of disk migration related cmdlets</span></span>
    * <span data-ttu-id="f3374-119">プラットフォーム イメージと VM 拡張機能オブジェクトでの追加のプロパティ</span><span class="sxs-lookup"><span data-stu-id="f3374-119">Additional properties in the Platform Image and VM extesnion objects</span></span>
* <span data-ttu-id="f3374-120">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="f3374-120">Azs.Fabric.Admin</span></span> 
    * <span data-ttu-id="f3374-121">スケール ユニット ノードを追加するための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f3374-121">New cmdlet for adding scale unit node</span></span>
* <span data-ttu-id="f3374-122">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="f3374-122">Azs.Backup.Admin</span></span>
    * <span data-ttu-id="f3374-123">Set-AzsBackupShare が cmdlet Set-AzsBackupConfiguration コマンドレットのエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="f3374-123">Set-AzsBackupShare is an alias now to the cmdlet Set-AzsBackupConfiguration</span></span>
    * <span data-ttu-id="f3374-124">Get-AzsBackupLocation が Get-AzsBackupConfiguration コマンドレットのエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="f3374-124">Get-AzsBackupLocation is an alias now to the cmdlet Get-AzsBackupConfiguration</span></span>
    * <span data-ttu-id="f3374-125">Set-AzsBackupConfiguration、BackupShare パラメーターがパラメーター パスのエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="f3374-125">Set-AzsBackupConfiguration, the parameter BackupShare is an alias now for the parameter path</span></span>
* <span data-ttu-id="f3374-126">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="f3374-126">Azs.Subscriptions</span></span>
    * <span data-ttu-id="f3374-127">Get-AzsDelegatedProviderOffer、OfferName パラメーターが Offer のエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="f3374-127">Get-AzsDelegatedProviderOffer, the parameter OfferName is now an alias for Offer</span></span>
* <span data-ttu-id="f3374-128">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="f3374-128">Azs.Subscriptions.Admin</span></span>
    * <span data-ttu-id="f3374-129">Get-AzsDelegatedProviderOffer、OfferName パラメーターが Offer のエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="f3374-129">Get-AzsDelegatedProviderOffer, the parameter OfferName is now an alias for Offer</span></span>

## <a name="content"></a><span data-ttu-id="f3374-130">内容:</span><span class="sxs-lookup"><span data-stu-id="f3374-130">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="f3374-131">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="f3374-131">Azure Bridge</span></span>
<span data-ttu-id="f3374-132">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="f3374-132">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="f3374-133">バックアップ</span><span class="sxs-lookup"><span data-stu-id="f3374-133">Backup</span></span>
<span data-ttu-id="f3374-134">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f3374-134">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="f3374-135">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="f3374-135">Configure where backups are stored</span></span>
- <span data-ttu-id="f3374-136">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="f3374-136">Perform backups</span></span>
- <span data-ttu-id="f3374-137">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="f3374-137">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="f3374-138">コマース</span><span class="sxs-lookup"><span data-stu-id="f3374-138">Commerce</span></span>
<span data-ttu-id="f3374-139">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="f3374-139">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="f3374-140">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="f3374-140">Compute</span></span>
<span data-ttu-id="f3374-141">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、マネージド ディスク、および仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="f3374-141">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="f3374-142">Fabric</span><span class="sxs-lookup"><span data-stu-id="f3374-142">Fabric</span></span>
<span data-ttu-id="f3374-143">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="f3374-143">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="f3374-144">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="f3374-144">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="f3374-145">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="f3374-145">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="f3374-146">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="f3374-146">Repair of scale unit nodes</span></span>
- <span data-ttu-id="f3374-147">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="f3374-147">Restart of Infrastructure role</span></span>
- <span data-ttu-id="f3374-148">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="f3374-148">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="f3374-149">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="f3374-149">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="f3374-150">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="f3374-150">Gallery</span></span>
<span data-ttu-id="f3374-151">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="f3374-151">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="f3374-152">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="f3374-152">Infrastructure Insights</span></span>
<span data-ttu-id="f3374-153">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f3374-153">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="f3374-154">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="f3374-154">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="f3374-155">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="f3374-155">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="f3374-156">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f3374-156">KeyVault</span></span>
<span data-ttu-id="f3374-157">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="f3374-157">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="f3374-158">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="f3374-158">Network</span></span>
<span data-ttu-id="f3374-159">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="f3374-159">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="f3374-160">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="f3374-160">Management of network quotas</span></span>
- <span data-ttu-id="f3374-161">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="f3374-161">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="f3374-162">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="f3374-162">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="f3374-163">Storage</span><span class="sxs-lookup"><span data-stu-id="f3374-163">Storage</span></span>
<span data-ttu-id="f3374-164">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="f3374-164">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="f3374-165">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="f3374-165">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="f3374-166">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="f3374-166">Manage storage quotas</span></span>
- <span data-ttu-id="f3374-167">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="f3374-167">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="f3374-168">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="f3374-168">Restore deleted storage accounts</span></span>
- <span data-ttu-id="f3374-169">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="f3374-169">Migrate containers from one share to another</span></span>
- <span data-ttu-id="f3374-170">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="f3374-170">View information about the individual storage components</span></span>
- <span data-ttu-id="f3374-171">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="f3374-171">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="f3374-172">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="f3374-172">Subscription Admin</span></span>
<span data-ttu-id="f3374-173">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="f3374-173">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="f3374-174">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="f3374-174">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="f3374-175">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="f3374-175">Manage plans and offers</span></span>
- <span data-ttu-id="f3374-176">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="f3374-176">View usage and performance information</span></span>
- <span data-ttu-id="f3374-177">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="f3374-177">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="f3374-178">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f3374-178">Subscription</span></span>
<span data-ttu-id="f3374-179">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="f3374-179">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="f3374-180">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="f3374-180">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="f3374-181">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="f3374-181">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="f3374-182">アップデート</span><span class="sxs-lookup"><span data-stu-id="f3374-182">Update</span></span>
<span data-ttu-id="f3374-183">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="f3374-183">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="f3374-184">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f3374-184">In this module administrators can:</span></span>
- <span data-ttu-id="f3374-185">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="f3374-185">List and install available updates</span></span>
- <span data-ttu-id="f3374-186">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="f3374-186">Resume interrupted updates</span></span>
- <span data-ttu-id="f3374-187">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="f3374-187">View installed updates</span></span>

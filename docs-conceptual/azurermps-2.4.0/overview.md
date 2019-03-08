---
title: Azure Stack PowerShell の概要 | Microsoft Docs
description: Azure Stack PowerShell の概要と、インストールおよび構成の手順。
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: cd415e862bfaa2b767cce108689ebaf34ef74305
ms.sourcegitcommit: 8c829e03cafd0575ecc594360b6b412cec0d6d71
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57343661"
---
# <a name="azurerm-module-230"></a><span data-ttu-id="8ab46-103">AzureRM モジュール 2.3.0</span><span class="sxs-lookup"><span data-stu-id="8ab46-103">AzureRM Module 2.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="8ab46-104">要件:</span><span class="sxs-lookup"><span data-stu-id="8ab46-104">Requirements:</span></span>
<span data-ttu-id="8ab46-105">サポートされている Azure Stack の最小バージョンは 1808 です。</span><span class="sxs-lookup"><span data-stu-id="8ab46-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="8ab46-106">注:以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください</span><span class="sxs-lookup"><span data-stu-id="8ab46-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="8ab46-107">Install</span><span class="sxs-lookup"><span data-stu-id="8ab46-107">Install</span></span>
```powershell-interactive
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

## <a name="release-notes"></a><span data-ttu-id="8ab46-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="8ab46-108">Release Notes</span></span>
* <span data-ttu-id="8ab46-109">リリース 2.3.0 には破壊的変更の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8ab46-109">The release 2.3.0 comes with a list of breaking changes.</span></span> <span data-ttu-id="8ab46-110">バージョン 1.2.11 からのアップグレードについては、移行ガイドをご用意しました (https://aka.ms/azspowershellmigration)</span><span class="sxs-lookup"><span data-stu-id="8ab46-110">To upgrade from the 1.2.11 version, we have created a migration guide at https://aka.ms/azspowershellmigration</span></span>
* <span data-ttu-id="8ab46-111">このリリースは、AzureStack 固有の API プロファイル 2018-03-01-hybrid に対応しています</span><span class="sxs-lookup"><span data-stu-id="8ab46-111">This release corresponds to the azurestack specific api profile 2018-03-01-hybrid</span></span>
* <span data-ttu-id="8ab46-112">すべてのモジュールで、AzureRm.Profile モジュールへの同等以上の依存関係が確立されます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-112">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="8ab46-113">各モジュールでサポートされている API バージョンが更新されています。</span><span class="sxs-lookup"><span data-stu-id="8ab46-113">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="8ab46-114">コンピューティング - 2017-03-30</span><span class="sxs-lookup"><span data-stu-id="8ab46-114">Compute - 2017-03-30</span></span>
    * <span data-ttu-id="8ab46-115">ネットワーク - 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="8ab46-115">Network - 2017-10-01</span></span>
    * <span data-ttu-id="8ab46-116">ストレージ - 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="8ab46-116">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="8ab46-117">リソース - 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="8ab46-117">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="8ab46-118">Keyvault - 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="8ab46-118">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="8ab46-119">DNS - 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="8ab46-119">Dns - 2016-04-01</span></span>
* <span data-ttu-id="8ab46-120">リソースの種類それぞれに対する詳細な API バージョン マップについては、 https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json をご覧ください</span><span class="sxs-lookup"><span data-stu-id="8ab46-120">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="8ab46-121">内容:</span><span class="sxs-lookup"><span data-stu-id="8ab46-121">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="8ab46-122">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="8ab46-122">Azure Bridge</span></span>
<span data-ttu-id="8ab46-123">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-123">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="8ab46-124">バックアップ</span><span class="sxs-lookup"><span data-stu-id="8ab46-124">Backup</span></span>
<span data-ttu-id="8ab46-125">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-125">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="8ab46-126">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="8ab46-126">Configure where backups are stored</span></span>
- <span data-ttu-id="8ab46-127">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="8ab46-127">Perform backups</span></span>
- <span data-ttu-id="8ab46-128">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="8ab46-128">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="8ab46-129">コマース</span><span class="sxs-lookup"><span data-stu-id="8ab46-129">Commerce</span></span>
<span data-ttu-id="8ab46-130">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-130">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="8ab46-131">Compute</span><span class="sxs-lookup"><span data-stu-id="8ab46-131">Compute</span></span>
<span data-ttu-id="8ab46-132">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、マネージド ディスク、および仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="8ab46-132">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="8ab46-133">Fabric</span><span class="sxs-lookup"><span data-stu-id="8ab46-133">Fabric</span></span>
<span data-ttu-id="8ab46-134">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-134">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="8ab46-135">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="8ab46-135">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="8ab46-136">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="8ab46-136">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="8ab46-137">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="8ab46-137">Repair of scale unit nodes</span></span>
- <span data-ttu-id="8ab46-138">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="8ab46-138">Restart of Infrastructure role</span></span>
- <span data-ttu-id="8ab46-139">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="8ab46-139">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="8ab46-140">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="8ab46-140">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="8ab46-141">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="8ab46-141">Gallery</span></span>
<span data-ttu-id="8ab46-142">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="8ab46-142">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="8ab46-143">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="8ab46-143">Infrastructure Insights</span></span>
<span data-ttu-id="8ab46-144">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-144">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="8ab46-145">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-145">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="8ab46-146">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-146">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="8ab46-147">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ab46-147">KeyVault</span></span>
<span data-ttu-id="8ab46-148">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-148">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="8ab46-149">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="8ab46-149">Network</span></span>
<span data-ttu-id="8ab46-150">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="8ab46-150">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="8ab46-151">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-151">Management of network quotas</span></span>
- <span data-ttu-id="8ab46-152">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-152">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="8ab46-153">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="8ab46-153">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="8ab46-154">Storage</span><span class="sxs-lookup"><span data-stu-id="8ab46-154">Storage</span></span>
<span data-ttu-id="8ab46-155">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="8ab46-155">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="8ab46-156">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="8ab46-156">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="8ab46-157">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-157">Manage storage quotas</span></span>
- <span data-ttu-id="8ab46-158">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="8ab46-158">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="8ab46-159">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="8ab46-159">Restore deleted storage accounts</span></span>
- <span data-ttu-id="8ab46-160">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="8ab46-160">Migrate containers from one share to another</span></span>
- <span data-ttu-id="8ab46-161">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-161">View information about the individual storage components</span></span>
- <span data-ttu-id="8ab46-162">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-162">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="8ab46-163">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-163">Subscription Admin</span></span>
<span data-ttu-id="8ab46-164">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="8ab46-164">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="8ab46-165">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="8ab46-165">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="8ab46-166">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-166">Manage plans and offers</span></span>
- <span data-ttu-id="8ab46-167">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-167">View usage and performance information</span></span>
- <span data-ttu-id="8ab46-168">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="8ab46-168">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="8ab46-169">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="8ab46-169">Subscription</span></span>
<span data-ttu-id="8ab46-170">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="8ab46-170">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="8ab46-171">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="8ab46-171">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="8ab46-172">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="8ab46-172">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="8ab46-173">アップデート</span><span class="sxs-lookup"><span data-stu-id="8ab46-173">Update</span></span>
<span data-ttu-id="8ab46-174">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="8ab46-174">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="8ab46-175">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8ab46-175">In this module administrators can:</span></span>
- <span data-ttu-id="8ab46-176">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="8ab46-176">List and install available updates</span></span>
- <span data-ttu-id="8ab46-177">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="8ab46-177">Resume interrupted updates</span></span>
- <span data-ttu-id="8ab46-178">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="8ab46-178">View installed updates</span></span>

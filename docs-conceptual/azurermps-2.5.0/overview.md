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
ms.openlocfilehash: 55f19ac5e6767df1312e0b531184e8621b60a011
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2019
ms.locfileid: "67038195"
---
# <a name="azurerm-module-250"></a><span data-ttu-id="28031-103">AzureRM モジュール 2.5.0</span><span class="sxs-lookup"><span data-stu-id="28031-103">AzureRM Module 2.5.0</span></span>

## <a name="requirements"></a><span data-ttu-id="28031-104">要件:</span><span class="sxs-lookup"><span data-stu-id="28031-104">Requirements:</span></span>
<span data-ttu-id="28031-105">サポートされている Azure Stack の最小バージョンは 1904 です。</span><span class="sxs-lookup"><span data-stu-id="28031-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="28031-106">注:以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください</span><span class="sxs-lookup"><span data-stu-id="28031-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="28031-107">Install</span><span class="sxs-lookup"><span data-stu-id="28031-107">Install</span></span>
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

## <a name="release-notes"></a><span data-ttu-id="28031-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="28031-108">Release Notes</span></span>
* <span data-ttu-id="28031-109">AzureRm.Resources</span><span class="sxs-lookup"><span data-stu-id="28031-109">AzureRm.Resources</span></span>
    * <span data-ttu-id="28031-110">2019-03-01-hybrid プロファイルで 2018-05-01 API バージョンをサポートしている、新しい Resources モジュール</span><span class="sxs-lookup"><span data-stu-id="28031-110">New Resources module supporting 2018-05-01 api version with 2019-03-01-hybrid profile</span></span>
    * <span data-ttu-id="28031-111">PolicyDefinition(2016-12-01) と PolicyAssisgment(2017-06-01-preview) の操作はまだ古い API バージョン</span><span class="sxs-lookup"><span data-stu-id="28031-111">PolicyDefinition(2016-12-01) and PolicyAssisgment(2017-06-01-preview) operations are still with old api versions</span></span>
* <span data-ttu-id="28031-112">AzureRm.Compute</span><span class="sxs-lookup"><span data-stu-id="28031-112">AzureRm.Compute</span></span>
    * <span data-ttu-id="28031-113">2017-12-01 API バージョンをサポートする新しい Compute モジュール</span><span class="sxs-lookup"><span data-stu-id="28031-113">New compute module supporting 2017-12-01 api version.'</span></span>


* <span data-ttu-id="28031-114">このリリースは、azurestack 固有の API プロファイル 2019-03-01-hybrid に対応しています。</span><span class="sxs-lookup"><span data-stu-id="28031-114">This release corresponds to the azurestack specific api profile 2019-03-01-hybrid</span></span>
* <span data-ttu-id="28031-115">すべてのモジュールで、AzureRm.Profile モジュールへの同等以上の依存関係が確立されます。</span><span class="sxs-lookup"><span data-stu-id="28031-115">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="28031-116">各モジュールでサポートされている API バージョンが更新されています。</span><span class="sxs-lookup"><span data-stu-id="28031-116">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="28031-117">Compute - 2017-12-30</span><span class="sxs-lookup"><span data-stu-id="28031-117">Compute - 2017-12-30</span></span>
    * <span data-ttu-id="28031-118">ネットワーク - 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="28031-118">Network - 2017-10-01</span></span>
    * <span data-ttu-id="28031-119">ストレージ - 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="28031-119">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="28031-120">リソース - 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="28031-120">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="28031-121">Keyvault - 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="28031-121">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="28031-122">DNS - 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="28031-122">Dns - 2016-04-01</span></span>
* <span data-ttu-id="28031-123">リソースの種類それぞれに対する詳細な API バージョン マップについては、 https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json をご覧ください</span><span class="sxs-lookup"><span data-stu-id="28031-123">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="28031-124">内容:</span><span class="sxs-lookup"><span data-stu-id="28031-124">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="28031-125">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="28031-125">Azure Bridge</span></span>
<span data-ttu-id="28031-126">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="28031-126">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="28031-127">バックアップ</span><span class="sxs-lookup"><span data-stu-id="28031-127">Backup</span></span>
<span data-ttu-id="28031-128">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="28031-128">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="28031-129">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="28031-129">Configure where backups are stored</span></span>
- <span data-ttu-id="28031-130">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="28031-130">Perform backups</span></span>
- <span data-ttu-id="28031-131">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="28031-131">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="28031-132">コマース</span><span class="sxs-lookup"><span data-stu-id="28031-132">Commerce</span></span>
<span data-ttu-id="28031-133">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="28031-133">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="28031-134">Compute</span><span class="sxs-lookup"><span data-stu-id="28031-134">Compute</span></span>
<span data-ttu-id="28031-135">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、マネージド ディスク、および仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="28031-135">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="28031-136">Fabric</span><span class="sxs-lookup"><span data-stu-id="28031-136">Fabric</span></span>
<span data-ttu-id="28031-137">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="28031-137">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="28031-138">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="28031-138">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="28031-139">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="28031-139">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="28031-140">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="28031-140">Repair of scale unit nodes</span></span>
- <span data-ttu-id="28031-141">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="28031-141">Restart of Infrastructure role</span></span>
- <span data-ttu-id="28031-142">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="28031-142">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="28031-143">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="28031-143">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="28031-144">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="28031-144">Gallery</span></span>
<span data-ttu-id="28031-145">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="28031-145">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="28031-146">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="28031-146">Infrastructure Insights</span></span>
<span data-ttu-id="28031-147">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="28031-147">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="28031-148">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="28031-148">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="28031-149">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="28031-149">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="28031-150">KeyVault</span><span class="sxs-lookup"><span data-stu-id="28031-150">KeyVault</span></span>
<span data-ttu-id="28031-151">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="28031-151">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="28031-152">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="28031-152">Network</span></span>
<span data-ttu-id="28031-153">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="28031-153">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="28031-154">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="28031-154">Management of network quotas</span></span>
- <span data-ttu-id="28031-155">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="28031-155">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="28031-156">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="28031-156">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="28031-157">Storage</span><span class="sxs-lookup"><span data-stu-id="28031-157">Storage</span></span>
<span data-ttu-id="28031-158">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="28031-158">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="28031-159">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="28031-159">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="28031-160">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="28031-160">Manage storage quotas</span></span>
- <span data-ttu-id="28031-161">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="28031-161">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="28031-162">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="28031-162">Restore deleted storage accounts</span></span>
- <span data-ttu-id="28031-163">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="28031-163">Migrate containers from one share to another</span></span>
- <span data-ttu-id="28031-164">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="28031-164">View information about the individual storage components</span></span>
- <span data-ttu-id="28031-165">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="28031-165">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="28031-166">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="28031-166">Subscription Admin</span></span>
<span data-ttu-id="28031-167">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="28031-167">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="28031-168">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="28031-168">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="28031-169">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="28031-169">Manage plans and offers</span></span>
- <span data-ttu-id="28031-170">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="28031-170">View usage and performance information</span></span>
- <span data-ttu-id="28031-171">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="28031-171">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="28031-172">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="28031-172">Subscription</span></span>
<span data-ttu-id="28031-173">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="28031-173">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="28031-174">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="28031-174">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="28031-175">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="28031-175">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="28031-176">アップデート</span><span class="sxs-lookup"><span data-stu-id="28031-176">Update</span></span>
<span data-ttu-id="28031-177">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="28031-177">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="28031-178">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="28031-178">In this module administrators can:</span></span>
- <span data-ttu-id="28031-179">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="28031-179">List and install available updates</span></span>
- <span data-ttu-id="28031-180">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="28031-180">Resume interrupted updates</span></span>
- <span data-ttu-id="28031-181">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="28031-181">View installed updates</span></span>

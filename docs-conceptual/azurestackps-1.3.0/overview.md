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
ms.openlocfilehash: fb892daeafb1365ea62324392ac806cf9f3d39cf
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882505"
---
# <a name="azure-stack-module-130"></a><span data-ttu-id="7d8f2-103">Azure Stack Module 1.3.0</span><span class="sxs-lookup"><span data-stu-id="7d8f2-103">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="7d8f2-104">要件:</span><span class="sxs-lookup"><span data-stu-id="7d8f2-104">Requirements:</span></span>
<span data-ttu-id="7d8f2-105">サポートされている Azure Stack の最小バージョンは 1804 です。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="7d8f2-106">注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="7d8f2-107">既知の問題:</span><span class="sxs-lookup"><span data-stu-id="7d8f2-107">Known issues:</span></span>

- <span data-ttu-id="7d8f2-108">アラートを閉じるには、Azure Stack バージョン 1803 が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="7d8f2-109">一部の Storage コマンドレットには、Azure Stack バージョン 1804 が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-109">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="7d8f2-110">New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-110">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="7d8f2-111">状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-111">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="7d8f2-112">再デプロイせずに IP プールを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-112">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="7d8f2-113">重大な変更</span><span class="sxs-lookup"><span data-stu-id="7d8f2-113">Breaking Changes</span></span>
<span data-ttu-id="7d8f2-114">1.2.11 からの移行に関する重大な変更はすべて https://aka.ms/azspowershellmigration に記載されています。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="7d8f2-115">Install</span><span class="sxs-lookup"><span data-stu-id="7d8f2-115">Install</span></span>
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a><span data-ttu-id="7d8f2-116">内容:</span><span class="sxs-lookup"><span data-stu-id="7d8f2-116">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="7d8f2-117">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="7d8f2-117">Azure Bridge</span></span>
<span data-ttu-id="7d8f2-118">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-118">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="7d8f2-119">バックアップ</span><span class="sxs-lookup"><span data-stu-id="7d8f2-119">Backup</span></span>
<span data-ttu-id="7d8f2-120">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-120">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="7d8f2-121">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="7d8f2-121">Configure where backups are stored</span></span>
- <span data-ttu-id="7d8f2-122">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="7d8f2-122">Perform backups</span></span>
- <span data-ttu-id="7d8f2-123">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="7d8f2-123">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="7d8f2-124">コマース</span><span class="sxs-lookup"><span data-stu-id="7d8f2-124">Commerce</span></span>
<span data-ttu-id="7d8f2-125">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-125">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="7d8f2-126">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="7d8f2-126">Compute</span></span>
<span data-ttu-id="7d8f2-127">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-127">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="7d8f2-128">Fabric</span><span class="sxs-lookup"><span data-stu-id="7d8f2-128">Fabric</span></span>
<span data-ttu-id="7d8f2-129">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-129">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="7d8f2-130">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="7d8f2-130">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="7d8f2-131">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="7d8f2-131">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="7d8f2-132">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="7d8f2-132">Repair of scale unit nodes</span></span>
- <span data-ttu-id="7d8f2-133">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="7d8f2-133">Restart of Infrastructure role</span></span>
- <span data-ttu-id="7d8f2-134">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="7d8f2-134">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="7d8f2-135">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="7d8f2-135">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="7d8f2-136">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="7d8f2-136">Gallery</span></span>
<span data-ttu-id="7d8f2-137">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-137">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="7d8f2-138">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="7d8f2-138">Infrastructure Insights</span></span>
<span data-ttu-id="7d8f2-139">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-139">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="7d8f2-140">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-140">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="7d8f2-141">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-141">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="7d8f2-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="7d8f2-142">KeyVault</span></span>
<span data-ttu-id="7d8f2-143">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-143">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="7d8f2-144">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="7d8f2-144">Network</span></span>
<span data-ttu-id="7d8f2-145">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-145">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="7d8f2-146">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-146">Management of network quotas</span></span>
- <span data-ttu-id="7d8f2-147">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-147">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="7d8f2-148">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="7d8f2-148">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="7d8f2-149">Storage</span><span class="sxs-lookup"><span data-stu-id="7d8f2-149">Storage</span></span>
<span data-ttu-id="7d8f2-150">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-150">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="7d8f2-151">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-151">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="7d8f2-152">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-152">Manage storage quotas</span></span>
- <span data-ttu-id="7d8f2-153">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="7d8f2-153">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="7d8f2-154">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="7d8f2-154">Restore deleted storage accounts</span></span>
- <span data-ttu-id="7d8f2-155">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="7d8f2-155">Migrate containers from one share to another</span></span>
- <span data-ttu-id="7d8f2-156">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-156">View information about the individual storage components</span></span>
- <span data-ttu-id="7d8f2-157">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-157">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="7d8f2-158">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-158">Subscription Admin</span></span>
<span data-ttu-id="7d8f2-159">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-159">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="7d8f2-160">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-160">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="7d8f2-161">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-161">Manage plans and offers</span></span>
- <span data-ttu-id="7d8f2-162">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-162">View usage and performance information</span></span>
- <span data-ttu-id="7d8f2-163">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="7d8f2-163">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="7d8f2-164">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="7d8f2-164">Subscription</span></span>
<span data-ttu-id="7d8f2-165">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-165">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="7d8f2-166">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-166">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="7d8f2-167">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="7d8f2-167">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="7d8f2-168">アップデート</span><span class="sxs-lookup"><span data-stu-id="7d8f2-168">Update</span></span>
<span data-ttu-id="7d8f2-169">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-169">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="7d8f2-170">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7d8f2-170">In this module administrators can:</span></span>
- <span data-ttu-id="7d8f2-171">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="7d8f2-171">List and install available updates</span></span>
- <span data-ttu-id="7d8f2-172">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="7d8f2-172">Resume interrupted updates</span></span>
- <span data-ttu-id="7d8f2-173">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="7d8f2-173">View installed updates</span></span>

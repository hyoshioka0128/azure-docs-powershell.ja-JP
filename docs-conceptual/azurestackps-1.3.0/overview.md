# <a name="azure-stack-module-130"></a><span data-ttu-id="84df1-101">Azure Stack Module 1.3.0</span><span class="sxs-lookup"><span data-stu-id="84df1-101">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="84df1-102">要件:</span><span class="sxs-lookup"><span data-stu-id="84df1-102">Requirements:</span></span>
<span data-ttu-id="84df1-103">サポートされている Azure Stack の最小バージョンは 1804 です。</span><span class="sxs-lookup"><span data-stu-id="84df1-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="84df1-104">注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="84df1-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="84df1-105">既知の問題:</span><span class="sxs-lookup"><span data-stu-id="84df1-105">Known issues:</span></span>

- <span data-ttu-id="84df1-106">アラートを閉じるには、Azure Stack バージョン 1803 が必要です。</span><span class="sxs-lookup"><span data-stu-id="84df1-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="84df1-107">一部の Storage コマンドレットには、Azure Stack バージョン 1804 が必要です。</span><span class="sxs-lookup"><span data-stu-id="84df1-107">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="84df1-108">New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="84df1-108">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="84df1-109">状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="84df1-109">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="84df1-110">再デプロイせずに IP プールを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="84df1-110">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="84df1-111">重大な変更</span><span class="sxs-lookup"><span data-stu-id="84df1-111">Breaking Changes</span></span>
<span data-ttu-id="84df1-112">1.2.11 からの移行に関する重大な変更はすべて https://aka.ms/azspowershellmigration に記載されています。</span><span class="sxs-lookup"><span data-stu-id="84df1-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="84df1-113">Install</span><span class="sxs-lookup"><span data-stu-id="84df1-113">Install</span></span>
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
## <a name="content"></a><span data-ttu-id="84df1-114">内容:</span><span class="sxs-lookup"><span data-stu-id="84df1-114">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="84df1-115">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="84df1-115">Azure Bridge</span></span>
<span data-ttu-id="84df1-116">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="84df1-116">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="84df1-117">Backup
</span><span class="sxs-lookup"><span data-stu-id="84df1-117">Backup</span></span>
<span data-ttu-id="84df1-118">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="84df1-118">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="84df1-119">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="84df1-119">Configure where backups are stored</span></span>
- <span data-ttu-id="84df1-120">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="84df1-120">Perform backups</span></span>
- <span data-ttu-id="84df1-121">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="84df1-121">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="84df1-122">コマース</span><span class="sxs-lookup"><span data-stu-id="84df1-122">Commerce</span></span>
<span data-ttu-id="84df1-123">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="84df1-123">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="84df1-124">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="84df1-124">Compute</span></span>
<span data-ttu-id="84df1-125">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="84df1-125">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="84df1-126">Fabric</span><span class="sxs-lookup"><span data-stu-id="84df1-126">Fabric</span></span>
<span data-ttu-id="84df1-127">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="84df1-127">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="84df1-128">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="84df1-128">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="84df1-129">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="84df1-129">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="84df1-130">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="84df1-130">Repair of scale unit nodes</span></span>
- <span data-ttu-id="84df1-131">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="84df1-131">Restart of Infrastructure role</span></span>
- <span data-ttu-id="84df1-132">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="84df1-132">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="84df1-133">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="84df1-133">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="84df1-134">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="84df1-134">Gallery</span></span>
<span data-ttu-id="84df1-135">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="84df1-135">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="84df1-136">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="84df1-136">Infrastructure Insights</span></span>
<span data-ttu-id="84df1-137">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="84df1-137">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="84df1-138">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="84df1-138">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="84df1-139">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="84df1-139">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="84df1-140">KeyVault</span><span class="sxs-lookup"><span data-stu-id="84df1-140">KeyVault</span></span>
<span data-ttu-id="84df1-141">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="84df1-141">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="84df1-142">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="84df1-142">Network</span></span>
<span data-ttu-id="84df1-143">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="84df1-143">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="84df1-144">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="84df1-144">Management of network quotas</span></span>
- <span data-ttu-id="84df1-145">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="84df1-145">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="84df1-146">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="84df1-146">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="84df1-147">Storage</span><span class="sxs-lookup"><span data-stu-id="84df1-147">Storage</span></span>
<span data-ttu-id="84df1-148">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="84df1-148">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="84df1-149">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="84df1-149">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="84df1-150">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="84df1-150">Manage storage quotas</span></span>
- <span data-ttu-id="84df1-151">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="84df1-151">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="84df1-152">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="84df1-152">Restore deleted storage accounts</span></span>
- <span data-ttu-id="84df1-153">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="84df1-153">Migrate containers from one share to another</span></span>
- <span data-ttu-id="84df1-154">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="84df1-154">View information about the individual storage components</span></span>
- <span data-ttu-id="84df1-155">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="84df1-155">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="84df1-156">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="84df1-156">Subscription Admin</span></span>
<span data-ttu-id="84df1-157">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="84df1-157">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="84df1-158">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="84df1-158">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="84df1-159">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="84df1-159">Manage plans and offers</span></span>
- <span data-ttu-id="84df1-160">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="84df1-160">View usage and performance information</span></span>
- <span data-ttu-id="84df1-161">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="84df1-161">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="84df1-162">[サブスクリプション]</span><span class="sxs-lookup"><span data-stu-id="84df1-162">Subscription</span></span>
<span data-ttu-id="84df1-163">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="84df1-163">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="84df1-164">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="84df1-164">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="84df1-165">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="84df1-165">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="84df1-166">アップデート</span><span class="sxs-lookup"><span data-stu-id="84df1-166">Update</span></span>
<span data-ttu-id="84df1-167">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="84df1-167">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="84df1-168">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="84df1-168">In this module administrators can:</span></span>
- <span data-ttu-id="84df1-169">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="84df1-169">List and install available updates</span></span>
- <span data-ttu-id="84df1-170">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="84df1-170">Resume interrupted updates</span></span>
- <span data-ttu-id="84df1-171">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="84df1-171">View installed updates</span></span>

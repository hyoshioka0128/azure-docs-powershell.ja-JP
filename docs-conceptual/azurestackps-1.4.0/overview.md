# <a name="azure-stack-module-140"></a><span data-ttu-id="bc47b-101">Azure Stack Module 1.4.0</span><span class="sxs-lookup"><span data-stu-id="bc47b-101">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="bc47b-102">要件:</span><span class="sxs-lookup"><span data-stu-id="bc47b-102">Requirements:</span></span>
<span data-ttu-id="bc47b-103">サポートされている Azure Stack の最小バージョンは 1804 です。</span><span class="sxs-lookup"><span data-stu-id="bc47b-103">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="bc47b-104">注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="bc47b-104">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="bc47b-105">既知の問題:</span><span class="sxs-lookup"><span data-stu-id="bc47b-105">Known issues:</span></span>

- <span data-ttu-id="bc47b-106">アラートを閉じるには、Azure Stack バージョン 1803 が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc47b-106">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="bc47b-107">New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="bc47b-107">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="bc47b-108">状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc47b-108">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="bc47b-109">再デプロイせずに IP プールを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="bc47b-109">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="bc47b-110">重大な変更</span><span class="sxs-lookup"><span data-stu-id="bc47b-110">Breaking Changes</span></span>
<span data-ttu-id="bc47b-111">バージョン 1.3.0 からの重大な変更はありません。</span><span class="sxs-lookup"><span data-stu-id="bc47b-111">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="bc47b-112">1.2.11 からの移行に関する重大な変更はすべて https://aka.ms/azspowershellmigration に記載されています。</span><span class="sxs-lookup"><span data-stu-id="bc47b-112">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="bc47b-113">Install</span><span class="sxs-lookup"><span data-stu-id="bc47b-113">Install</span></span>
```
# 1.4.0 can be installed side by side with 1.3.0
# Remove previous version 1.2.11
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="bc47b-114">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="bc47b-114">Release Notes</span></span>
    * <span data-ttu-id="bc47b-115">Azure Stack 1.4.0 バージョンには、以前のリリース 1.3.0 からの重大な変更はありません</span><span class="sxs-lookup"><span data-stu-id="bc47b-115">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="bc47b-116">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-116">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="bc47b-117">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-117">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-118">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-118">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="bc47b-119">Set-AzsBackupShare コマンドレットに、BackupFrequencyInHours、IsBackupSchedulerEnabled、BackupRetentionPeriodInDays の各パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-119">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="bc47b-120">暗号化キーの作成を容易にするために、New-EncyptionKeyBase64 コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-120">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="bc47b-121">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-121">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-122">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-122">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="bc47b-123">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-124">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-124">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="bc47b-125">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-125">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="bc47b-126">管理者が Azure Stack スタンプに新しいスケール ユニット ノードを追加できるように、Add-AzsScaleUnitNode コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-126">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="bc47b-127">スケール ユニット パラメーター オブジェクトの作成を容易にするために、New-AzsScaleUnitNodeObject コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-127">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="bc47b-128">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-128">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="bc47b-129">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-129">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-130">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-130">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="bc47b-131">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-132">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-132">Azs.Network.Admin</span></span>
        - <span data-ttu-id="bc47b-133">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-134">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-134">Azs.Update.Admin</span></span>
        - <span data-ttu-id="bc47b-135">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-136">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="bc47b-136">Azs.Subscriptions</span></span>
        - <span data-ttu-id="bc47b-137">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="bc47b-138">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="bc47b-138">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="bc47b-139">委任されたプロバイダーのプラン間でサブスクリプションを移動するために、Move-AzsSubscription コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-139">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="bc47b-140">委任されたプロバイダーのプラン間でユーザー サブスクリプションを移動できることを検証するために、Test-AzsMoveSubscription コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bc47b-140">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="bc47b-141">改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム</span><span class="sxs-lookup"><span data-stu-id="bc47b-141">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="bc47b-142">内容:</span><span class="sxs-lookup"><span data-stu-id="bc47b-142">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="bc47b-143">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="bc47b-143">Azure Bridge</span></span>
<span data-ttu-id="bc47b-144">Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-144">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="bc47b-145">Backup</span><span class="sxs-lookup"><span data-stu-id="bc47b-145">Backup</span></span>
<span data-ttu-id="bc47b-146">Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-146">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="bc47b-147">バックアップの保存先の構成</span><span class="sxs-lookup"><span data-stu-id="bc47b-147">Configure where backups are stored</span></span>
- <span data-ttu-id="bc47b-148">バックアップの実行</span><span class="sxs-lookup"><span data-stu-id="bc47b-148">Perform backups</span></span>
- <span data-ttu-id="bc47b-149">完了したバックアップの表示と復元</span><span class="sxs-lookup"><span data-stu-id="bc47b-149">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="bc47b-150">コマース</span><span class="sxs-lookup"><span data-stu-id="bc47b-150">Commerce</span></span>
<span data-ttu-id="bc47b-151">Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-151">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="bc47b-152">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="bc47b-152">Compute</span></span>
<span data-ttu-id="bc47b-153">Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、仮想マシン拡張機能を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bc47b-153">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="bc47b-154">Fabric</span><span class="sxs-lookup"><span data-stu-id="bc47b-154">Fabric</span></span>
<span data-ttu-id="bc47b-155">Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-155">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="bc47b-156">スケール ユニット ノードの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="bc47b-156">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="bc47b-157">FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開</span><span class="sxs-lookup"><span data-stu-id="bc47b-157">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="bc47b-158">スケール ユニット ノードの修復</span><span class="sxs-lookup"><span data-stu-id="bc47b-158">Repair of scale unit nodes</span></span>
- <span data-ttu-id="bc47b-159">インフラストラクチャ ロールの再起動</span><span class="sxs-lookup"><span data-stu-id="bc47b-159">Restart of Infrastructure role</span></span>
- <span data-ttu-id="bc47b-160">インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン</span><span class="sxs-lookup"><span data-stu-id="bc47b-160">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="bc47b-161">新しい IP プールの作成</span><span class="sxs-lookup"><span data-stu-id="bc47b-161">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="bc47b-162">[ギャラリー]</span><span class="sxs-lookup"><span data-stu-id="bc47b-162">Gallery</span></span>
<span data-ttu-id="bc47b-163">Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bc47b-163">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="bc47b-164">Infrastructure Insights</span><span class="sxs-lookup"><span data-stu-id="bc47b-164">Infrastructure Insights</span></span>
<span data-ttu-id="bc47b-165">Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-165">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="bc47b-166">Azure Stack スタンプ リソースの正常性の表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-166">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="bc47b-167">アラートの表示と管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-167">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="bc47b-168">KeyVault</span><span class="sxs-lookup"><span data-stu-id="bc47b-168">KeyVault</span></span>
<span data-ttu-id="bc47b-169">Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-169">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="bc47b-170">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="bc47b-170">Network</span></span>
<span data-ttu-id="bc47b-171">Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="bc47b-171">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="bc47b-172">ネットワーク クォータの管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-172">Management of network quotas</span></span>
- <span data-ttu-id="bc47b-173">割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-173">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="bc47b-174">管理者の概要を表示するコマンドレットの提供</span><span class="sxs-lookup"><span data-stu-id="bc47b-174">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="bc47b-175">Storage</span><span class="sxs-lookup"><span data-stu-id="bc47b-175">Storage</span></span>
<span data-ttu-id="bc47b-176">Azure Stack Storage 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="bc47b-176">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="bc47b-177">このリリースには、次の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="bc47b-177">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="bc47b-178">ストレージ クォータの管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-178">Manage storage quotas</span></span>
- <span data-ttu-id="bc47b-179">削除されたストレージ リソースのガベージ コレクションの実行</span><span class="sxs-lookup"><span data-stu-id="bc47b-179">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="bc47b-180">削除されたストレージ アカウントの復元</span><span class="sxs-lookup"><span data-stu-id="bc47b-180">Restore deleted storage accounts</span></span>
- <span data-ttu-id="bc47b-181">共有間でのコンテナーの移行</span><span class="sxs-lookup"><span data-stu-id="bc47b-181">Migrate containers from one share to another</span></span>
- <span data-ttu-id="bc47b-182">個々のストレージ コンポーネントに関する情報の表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-182">View information about the individual storage components</span></span>
- <span data-ttu-id="bc47b-183">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-183">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="bc47b-184">サブスクリプション管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-184">Subscription Admin</span></span>
<span data-ttu-id="bc47b-185">Azure Stack Subscription 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="bc47b-185">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="bc47b-186">このモジュールは、管理者向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bc47b-186">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="bc47b-187">プランとオファーの管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-187">Manage plans and offers</span></span>
- <span data-ttu-id="bc47b-188">使用状況とパフォーマンスの情報の表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-188">View usage and performance information</span></span>
- <span data-ttu-id="bc47b-189">RBAC の管理</span><span class="sxs-lookup"><span data-stu-id="bc47b-189">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="bc47b-190">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="bc47b-190">Subscription</span></span>
<span data-ttu-id="bc47b-191">Azure Stack Subscription モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="bc47b-191">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="bc47b-192">このモジュールは、ユーザー向けの次の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="bc47b-192">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="bc47b-193">サブスクリプションの作成、削除、更新</span><span class="sxs-lookup"><span data-stu-id="bc47b-193">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="bc47b-194">アップデート</span><span class="sxs-lookup"><span data-stu-id="bc47b-194">Update</span></span>
<span data-ttu-id="bc47b-195">Azure Stack Update 管理者モジュールのプレビュー リリース。</span><span class="sxs-lookup"><span data-stu-id="bc47b-195">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="bc47b-196">このモジュールでは、管理者は以下を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="bc47b-196">In this module administrators can:</span></span>
- <span data-ttu-id="bc47b-197">使用可能な更新プログラムの表示とインストール</span><span class="sxs-lookup"><span data-stu-id="bc47b-197">List and install available updates</span></span>
- <span data-ttu-id="bc47b-198">中断された更新の再開</span><span class="sxs-lookup"><span data-stu-id="bc47b-198">Resume interrupted updates</span></span>
- <span data-ttu-id="bc47b-199">インストール済みの更新プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="bc47b-199">View installed updates</span></span>

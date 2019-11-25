---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: ee3f54e6bc15dbbaeb97cad7463cb1d2e5795e3e
ms.sourcegitcommit: 05431341858d10eb9c345213275c3ccc24c83c9b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/13/2019
ms.locfileid: "74062141"
---
## <a name="300---november-2019"></a><span data-ttu-id="ea6d2-103">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-103">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="ea6d2-104">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-104">General</span></span>
* <span data-ttu-id="ea6d2-105">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-105">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-106">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-107">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-107">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="ea6d2-108">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-108">Az.Advisor</span></span>
* <span data-ttu-id="ea6d2-109">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-109">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ea6d2-110">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ea6d2-110">Az.Batch</span></span>
* <span data-ttu-id="ea6d2-111">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-111">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="ea6d2-112">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-112">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="ea6d2-113">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-113">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="ea6d2-114">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-114">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="ea6d2-115">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-115">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="ea6d2-116">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-116">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="ea6d2-117">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-117">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="ea6d2-118">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-118">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="ea6d2-119">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-119">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="ea6d2-120">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-120">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="ea6d2-121">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-121">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="ea6d2-122">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-122">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="ea6d2-123">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-123">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="ea6d2-124">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-124">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="ea6d2-125">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-125">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="ea6d2-126">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-126">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="ea6d2-127">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-127">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="ea6d2-128">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-128">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="ea6d2-129">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-129">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="ea6d2-130">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-130">This operation is no longer supported.</span></span>
* <span data-ttu-id="ea6d2-131">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-131">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="ea6d2-132">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-132">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="ea6d2-133">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-133">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="ea6d2-134">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-134">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="ea6d2-135">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-135">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="ea6d2-136">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-136">New non-verified images are also now returned.</span></span> <span data-ttu-id="ea6d2-137">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-137">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="ea6d2-138">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-138">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="ea6d2-139">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-139">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="ea6d2-140">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-140">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="ea6d2-141">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-141">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="ea6d2-142">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-142">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="ea6d2-143">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-143">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="ea6d2-144">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-144">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="ea6d2-145">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-145">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="ea6d2-146">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-146">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ea6d2-147">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-147">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-148">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-148">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="ea6d2-149">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-149">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-150">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-150">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-151">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="ea6d2-151">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="ea6d2-152">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-152">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="ea6d2-153">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-153">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="ea6d2-154">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="ea6d2-154">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="ea6d2-155">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-155">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ea6d2-156">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-156">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="ea6d2-157">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-157">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="ea6d2-158">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-158">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="ea6d2-159">重大な変更</span><span class="sxs-lookup"><span data-stu-id="ea6d2-159">Breaking changes</span></span>
    - <span data-ttu-id="ea6d2-160">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-160">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="ea6d2-161">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-161">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-162">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-162">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-163">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-163">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-164">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-164">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-165">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-165">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="ea6d2-166">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-166">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="ea6d2-167">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-167">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="ea6d2-168">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-168">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="ea6d2-169">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-169">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="ea6d2-170">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-170">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ea6d2-171">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-171">Az.FrontDoor</span></span>
* <span data-ttu-id="ea6d2-172">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-172">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="ea6d2-173">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ea6d2-173">Az.HDInsight</span></span>
* <span data-ttu-id="ea6d2-174">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-174">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="ea6d2-175">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-175">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="ea6d2-176">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-176">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="ea6d2-177">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-177">Removed five cmdlets:</span></span>
    - <span data-ttu-id="ea6d2-178">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="ea6d2-178">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="ea6d2-179">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="ea6d2-179">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="ea6d2-180">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="ea6d2-180">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="ea6d2-181">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ea6d2-181">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="ea6d2-182">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ea6d2-182">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="ea6d2-183">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-183">Added three cmdlets:</span></span>
    - <span data-ttu-id="ea6d2-184">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-184">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="ea6d2-185">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-185">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="ea6d2-186">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-186">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="ea6d2-187">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-187">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="ea6d2-188">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-188">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="ea6d2-189">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-189">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="ea6d2-190">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-190">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="ea6d2-191">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-191">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="ea6d2-192">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-192">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="ea6d2-193">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-193">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="ea6d2-194">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-194">Added some scenario test cases.</span></span>
* <span data-ttu-id="ea6d2-195">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-195">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-196">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-197">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-197">Breaking changes:</span></span>
    - <span data-ttu-id="ea6d2-198">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-198">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="ea6d2-199">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-199">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="ea6d2-200">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-200">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="ea6d2-201">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-201">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="ea6d2-202">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-202">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="ea6d2-203">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-203">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="ea6d2-204">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-204">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="ea6d2-205">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-205">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="ea6d2-206">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-206">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="ea6d2-207">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-207">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="ea6d2-208">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-208">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="ea6d2-209">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-209">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-210">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-210">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-211">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-211">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-212">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-212">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="ea6d2-213">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-213">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="ea6d2-214">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-214">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-215">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-215">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-216">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-216">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-217">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-217">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-218">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-218">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-219">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-219">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-220">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-220">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-221">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-221">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-222">Az.Network</span></span>
* <span data-ttu-id="ea6d2-223">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-223">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="ea6d2-224">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-224">Updated cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-225">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-225">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-226">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-226">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-227">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-227">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-228">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-228">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-229">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-229">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="ea6d2-230">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-230">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="ea6d2-231">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-231">New cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-232">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="ea6d2-232">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="ea6d2-233">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-233">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="ea6d2-234">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-234">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="ea6d2-235">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-235">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="ea6d2-236">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-236">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="ea6d2-237">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-237">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="ea6d2-238">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-238">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="ea6d2-239">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-239">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="ea6d2-240">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-240">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-241">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-241">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="ea6d2-242">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-242">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="ea6d2-243">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-243">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="ea6d2-244">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-244">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="ea6d2-245">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-245">Set-AzVirtualHub</span></span>
* <span data-ttu-id="ea6d2-246">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-246">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="ea6d2-247">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-247">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="ea6d2-248">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-248">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="ea6d2-249">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-249">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="ea6d2-250">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-250">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="ea6d2-251">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-251">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="ea6d2-252">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-252">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="ea6d2-253">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-253">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-254">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-254">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="ea6d2-255">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-255">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="ea6d2-256">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-256">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="ea6d2-257">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-257">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="ea6d2-258">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-258">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="ea6d2-259">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-259">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="ea6d2-260">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-260">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="ea6d2-261">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-261">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="ea6d2-262">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-262">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-263">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="ea6d2-263">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="ea6d2-264">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="ea6d2-264">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="ea6d2-265">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="ea6d2-265">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="ea6d2-266">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="ea6d2-266">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="ea6d2-267">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-267">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="ea6d2-268">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-268">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="ea6d2-269">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-269">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="ea6d2-270">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-270">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="ea6d2-271">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-271">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="ea6d2-272">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-272">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="ea6d2-273">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-273">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="ea6d2-274">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-274">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="ea6d2-275">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-275">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="ea6d2-276">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-276">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="ea6d2-277">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-277">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="ea6d2-278">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-278">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="ea6d2-279">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-279">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="ea6d2-280">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-280">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-281">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-281">New-AzIpGroup</span></span>
        - <span data-ttu-id="ea6d2-282">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-282">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="ea6d2-283">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-283">Get-AzIpGroup</span></span>
        - <span data-ttu-id="ea6d2-284">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-284">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-285">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-285">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-286">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-286">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-287">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-288">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-288">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="ea6d2-289">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-289">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="ea6d2-290">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-290">Removed deprecated aliases:</span></span>
* <span data-ttu-id="ea6d2-291">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-291">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="ea6d2-292">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-292">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="ea6d2-293">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-293">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="ea6d2-294">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-294">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="ea6d2-295">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-295">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="ea6d2-296">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-296">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-297">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-297">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-298">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-298">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="ea6d2-299">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-299">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="ea6d2-300">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-300">Set-AzStorageAccount</span></span>
* <span data-ttu-id="ea6d2-301">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-301">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="ea6d2-302">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ea6d2-302">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="ea6d2-303">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ea6d2-303">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="ea6d2-304">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-304">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="ea6d2-305">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-305">General</span></span>
* <span data-ttu-id="ea6d2-306">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-306">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-307">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-307">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-308">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-308">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-309">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-309">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-310">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-310">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="ea6d2-311">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="ea6d2-311">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-312">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-312">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-313">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-313">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="ea6d2-314">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ea6d2-314">Az.Batch</span></span>
* <span data-ttu-id="ea6d2-315">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-315">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-316">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-317">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-317">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="ea6d2-318">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-318">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="ea6d2-319">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-319">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="ea6d2-320">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-320">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-321">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-322">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-322">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="ea6d2-323">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-323">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="ea6d2-324">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-324">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-325">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-325">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-326">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-326">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="ea6d2-327">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="ea6d2-327">Az.HealthcareApis</span></span>
* <span data-ttu-id="ea6d2-328">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-328">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="ea6d2-329">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-329">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="ea6d2-330">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-330">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="ea6d2-331">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-331">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-332">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-332">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-333">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="ea6d2-333">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="ea6d2-334">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="ea6d2-334">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-335">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-335">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-336">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="ea6d2-336">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="ea6d2-337">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-337">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="ea6d2-338">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="ea6d2-338">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="ea6d2-339">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-339">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-340">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-340">Az.Network</span></span>
* <span data-ttu-id="ea6d2-341">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-341">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="ea6d2-342">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-342">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="ea6d2-343">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-343">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-344">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-344">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="ea6d2-345">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-345">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ea6d2-346">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-346">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="ea6d2-347">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-347">Updated cmdlets:</span></span>
        - <span data-ttu-id="ea6d2-348">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-348">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ea6d2-349">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-349">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ea6d2-350">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-350">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ea6d2-351">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-351">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="ea6d2-352">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="ea6d2-352">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="ea6d2-353">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-353">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="ea6d2-354">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-354">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ea6d2-355">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ea6d2-355">Az.RedisCache</span></span>
* <span data-ttu-id="ea6d2-356">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-356">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-357">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-357">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-358">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-358">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-359">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-359">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-360">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-360">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="ea6d2-361">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-361">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ea6d2-362">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="ea6d2-362">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="ea6d2-363">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-363">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ea6d2-364">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-364">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ea6d2-365">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ea6d2-365">Az.StorageSync</span></span>
* <span data-ttu-id="ea6d2-366">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-366">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-367">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-367">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-368">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-368">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="ea6d2-369">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-369">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-370">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-370">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-371">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-371">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="ea6d2-372">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-372">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="ea6d2-373">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-373">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-374">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-374">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-375">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-375">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="ea6d2-376">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-376">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="ea6d2-377">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-377">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-378">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-378">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-379">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-379">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="ea6d2-380">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-380">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ea6d2-381">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-381">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="ea6d2-382">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-382">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="ea6d2-383">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-383">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="ea6d2-384">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-384">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="ea6d2-385">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-385">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="ea6d2-386">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-386">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="ea6d2-387">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-387">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-388">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-388">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-389">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-389">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="ea6d2-390">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-390">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="ea6d2-391">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ea6d2-391">Az.HDInsight</span></span>
* <span data-ttu-id="ea6d2-392">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-392">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-393">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-393">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-394">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-394">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="ea6d2-395">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-395">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="ea6d2-396">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-396">New cmdlets are:</span></span>
    - <span data-ttu-id="ea6d2-397">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ea6d2-397">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ea6d2-398">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ea6d2-398">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ea6d2-399">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ea6d2-399">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ea6d2-400">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ea6d2-400">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-401">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-401">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-402">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="ea6d2-402">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="ea6d2-403">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-403">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="ea6d2-404">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-404">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="ea6d2-405">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-405">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="ea6d2-406">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-406">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="ea6d2-407">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-407">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="ea6d2-408">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-408">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="ea6d2-409">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-409">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="ea6d2-410">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-410">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ea6d2-411">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-411">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="ea6d2-412">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-412">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ea6d2-413">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-413">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="ea6d2-414">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-414">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="ea6d2-415">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-415">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="ea6d2-416">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-416">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="ea6d2-417">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="ea6d2-417">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="ea6d2-418">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-418">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="ea6d2-419">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-419">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="ea6d2-420">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-420">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="ea6d2-421">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-421">Overall improved help files</span></span>
* <span data-ttu-id="ea6d2-422">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-422">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-423">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-423">Az.Network</span></span>
* <span data-ttu-id="ea6d2-424">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-424">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="ea6d2-425">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-425">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="ea6d2-426">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-426">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="ea6d2-427">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-427">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="ea6d2-428">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-428">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="ea6d2-429">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-429">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="ea6d2-430">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-430">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="ea6d2-431">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-431">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="ea6d2-432">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-432">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="ea6d2-433">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-433">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="ea6d2-434">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-434">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="ea6d2-435">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-435">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="ea6d2-436">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-436">New cmdlets</span></span>
        - <span data-ttu-id="ea6d2-437">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="ea6d2-437">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="ea6d2-438">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-438">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="ea6d2-439">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-439">Updated cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-440">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ea6d2-440">New-VpnSite</span></span>
        - <span data-ttu-id="ea6d2-441">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ea6d2-441">Update-VpnSite</span></span>
        - <span data-ttu-id="ea6d2-442">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-442">New-VpnConnection</span></span>
        - <span data-ttu-id="ea6d2-443">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-443">Update-VpnConnection</span></span>
* <span data-ttu-id="ea6d2-444">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-444">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-445">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-445">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-446">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-446">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="ea6d2-447">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-447">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-448">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-448">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-449">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-449">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-450">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-450">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-451">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-451">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="ea6d2-452">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-452">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="ea6d2-453">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ea6d2-453">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ea6d2-454">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ea6d2-454">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ea6d2-455">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ea6d2-455">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ea6d2-456">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-456">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="ea6d2-457">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ea6d2-457">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ea6d2-458">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ea6d2-458">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ea6d2-459">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ea6d2-459">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ea6d2-460">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ea6d2-460">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ea6d2-461">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-461">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="ea6d2-462">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ea6d2-462">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ea6d2-463">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ea6d2-463">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ea6d2-464">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ea6d2-464">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ea6d2-465">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="ea6d2-465">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="ea6d2-466">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-466">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ea6d2-467">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ea6d2-467">Az.SignalR</span></span>
* <span data-ttu-id="ea6d2-468">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-468">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-469">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-470">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-470">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="ea6d2-471">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-471">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="ea6d2-472">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-472">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="ea6d2-473">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-473">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="ea6d2-474">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-474">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-475">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-475">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-476">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-476">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="ea6d2-477">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-477">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="ea6d2-478">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-478">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="ea6d2-479">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-479">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="ea6d2-480">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-480">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="ea6d2-481">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-481">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="ea6d2-482">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-482">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="ea6d2-483">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ea6d2-483">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ea6d2-484">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ea6d2-484">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ea6d2-485">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ea6d2-485">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ea6d2-486">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ea6d2-486">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-487">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-487">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-488">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-488">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="ea6d2-489">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-489">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="ea6d2-490">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-490">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="ea6d2-491">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-491">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="ea6d2-492">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-492">General</span></span>
* <span data-ttu-id="ea6d2-493">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-493">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-494">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-494">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-495">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-495">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="ea6d2-496">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ea6d2-496">Az.Aks</span></span>
* <span data-ttu-id="ea6d2-497">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-497">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="ea6d2-498">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="ea6d2-498">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-499">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-499">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-500">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="ea6d2-500">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="ea6d2-501">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-501">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="ea6d2-502">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-502">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="ea6d2-503">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="ea6d2-503">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="ea6d2-504">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-504">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ea6d2-505">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ea6d2-505">Az.Batch</span></span>
* <span data-ttu-id="ea6d2-506">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-506">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ea6d2-507">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-507">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-508">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-508">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-509">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-509">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-510">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-510">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="ea6d2-511">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-511">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="ea6d2-512">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-512">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="ea6d2-513">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-513">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="ea6d2-514">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="ea6d2-514">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="ea6d2-515">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-515">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="ea6d2-516">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-516">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="ea6d2-517">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-517">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-518">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-518">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-519">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-519">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="ea6d2-520">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-520">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="ea6d2-521">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-521">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="ea6d2-522">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-522">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-523">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-523">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-524">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-524">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ea6d2-525">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-525">Az.EventHub</span></span>
* <span data-ttu-id="ea6d2-526">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="ea6d2-526">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="ea6d2-527">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="ea6d2-527">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="ea6d2-528">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-528">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="ea6d2-529">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="ea6d2-529">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="ea6d2-530">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ea6d2-530">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ea6d2-531">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-531">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-532">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-532">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-533">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-533">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-534">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-534">Az.Network</span></span>
* <span data-ttu-id="ea6d2-535">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-535">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="ea6d2-536">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-536">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="ea6d2-537">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-537">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="ea6d2-538">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-538">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="ea6d2-539">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-539">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="ea6d2-540">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-540">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="ea6d2-541">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-541">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-542">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-542">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-543">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-543">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="ea6d2-544">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-544">Added example</span></span>
    - <span data-ttu-id="ea6d2-545">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-545">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="ea6d2-546">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-546">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="ea6d2-547">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-547">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-548">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-548">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-549">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-549">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-550">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-550">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-551">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-551">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="ea6d2-552">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-552">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="ea6d2-553">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-553">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="ea6d2-554">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-554">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-555">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-555">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-556">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="ea6d2-556">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="ea6d2-557">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="ea6d2-557">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="ea6d2-558">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-558">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-559">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-559">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-560">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-560">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="ea6d2-561">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-561">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="ea6d2-562">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="ea6d2-562">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="ea6d2-563">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-563">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="ea6d2-564">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="ea6d2-564">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="ea6d2-565">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-565">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-566">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-566">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-567">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-567">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-568">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-569">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-569">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="ea6d2-570">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-570">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="ea6d2-571">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-571">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="ea6d2-572">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-572">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="ea6d2-573">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-573">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="ea6d2-574">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-574">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-575">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-575">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-576">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-576">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="ea6d2-577">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-577">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-578">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-578">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-579">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-579">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="ea6d2-580">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-580">Az.ApplicationInsights</span></span>
* <span data-ttu-id="ea6d2-581">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-581">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-582">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-582">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-583">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-583">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-584">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-584">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-585">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-585">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-586">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-587">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-587">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ea6d2-588">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ea6d2-588">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ea6d2-589">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-589">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="ea6d2-590">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="ea6d2-590">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-591">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-591">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-592">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-592">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="ea6d2-593">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-593">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ea6d2-594">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-594">Az.EventHub</span></span>
* <span data-ttu-id="ea6d2-595">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ea6d2-595">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ea6d2-596">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-596">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-597">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-597">Az.KeyVault</span></span>
* <span data-ttu-id="ea6d2-598">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-598">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ea6d2-599">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ea6d2-599">Az.LogicApp</span></span>
* <span data-ttu-id="ea6d2-600">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-600">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="ea6d2-601">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-601">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="ea6d2-602">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-602">Az.ManagedServices</span></span>
* <span data-ttu-id="ea6d2-603">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-603">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-604">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-604">Az.Network</span></span>
* <span data-ttu-id="ea6d2-605">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-605">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="ea6d2-606">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-606">New cmdlets</span></span>
        - <span data-ttu-id="ea6d2-607">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ea6d2-607">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ea6d2-608">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-608">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ea6d2-609">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-609">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-610">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-610">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-611">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-611">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-612">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-612">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ea6d2-613">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="ea6d2-613">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="ea6d2-614">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-614">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="ea6d2-615">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="ea6d2-615">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="ea6d2-616">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-616">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="ea6d2-617">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-617">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="ea6d2-618">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-618">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="ea6d2-619">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-619">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="ea6d2-620">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-620">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="ea6d2-621">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-621">Updated cmdlets</span></span>
        - <span data-ttu-id="ea6d2-622">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-622">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ea6d2-623">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-623">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ea6d2-624">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-624">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ea6d2-625">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-625">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ea6d2-626">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-626">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="ea6d2-627">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-627">Updated cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-628">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-628">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ea6d2-629">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-629">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ea6d2-630">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-630">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="ea6d2-631">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-631">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="ea6d2-632">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-632">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="ea6d2-633">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-633">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-634">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-634">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-635">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-635">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="ea6d2-636">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-636">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-637">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-637">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-638">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-638">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ea6d2-639">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-639">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="ea6d2-640">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-640">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="ea6d2-641">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-641">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ea6d2-642">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-642">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="ea6d2-643">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-643">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ea6d2-644">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-644">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="ea6d2-645">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-645">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ea6d2-646">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-646">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="ea6d2-647">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-647">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-648">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-648">Az.Resources</span></span>
- <span data-ttu-id="ea6d2-649">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-649">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="ea6d2-650">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-650">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-651">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-651">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-652">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ea6d2-652">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ea6d2-653">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-653">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-654">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-654">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-655">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-655">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="ea6d2-656">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-656">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="ea6d2-657">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-657">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-658">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-658">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-659">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-659">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ea6d2-660">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ea6d2-660">Az.StorageSync</span></span>
* <span data-ttu-id="ea6d2-661">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-661">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="ea6d2-662">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-662">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-663">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-663">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-664">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-664">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="ea6d2-665">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-665">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="ea6d2-666">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-666">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="ea6d2-667">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-667">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-668">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-668">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-669">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-669">Add support for profile cmdlets</span></span>
* <span data-ttu-id="ea6d2-670">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-670">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="ea6d2-671">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-671">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="ea6d2-672">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-672">Az.Advisor</span></span>
* <span data-ttu-id="ea6d2-673">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-673">GA release of Az.Advisor</span></span>
* <span data-ttu-id="ea6d2-674">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-674">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-675">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-675">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-676">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="ea6d2-676">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="ea6d2-677">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="ea6d2-677">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="ea6d2-678">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-678">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="ea6d2-679">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-679">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="ea6d2-680">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-680">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="ea6d2-681">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ea6d2-681">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="ea6d2-682">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-682">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-683">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-683">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-684">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-684">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-685">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-685">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-686">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-686">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-687">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-687">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-688">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-688">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ea6d2-689">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ea6d2-689">Az.EventGrid</span></span>
* <span data-ttu-id="ea6d2-690">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-690">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-691">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-691">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-692">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-692">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-693">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-693">Az.Network</span></span>
* <span data-ttu-id="ea6d2-694">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-694">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="ea6d2-695">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-695">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ea6d2-696">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-696">Az.PolicyInsights</span></span>
* <span data-ttu-id="ea6d2-697">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-697">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="ea6d2-698">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="ea6d2-698">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-699">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-699">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-700">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-700">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-701">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-701">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-702">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-702">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-703">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-703">Az.Resources</span></span>
    - <span data-ttu-id="ea6d2-704">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-704">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="ea6d2-705">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-705">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="ea6d2-706">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-706">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="ea6d2-707">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-707">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-708">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-708">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-709">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="ea6d2-709">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-710">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-710">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-711">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-711">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="ea6d2-712">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-712">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="ea6d2-713">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-713">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ea6d2-714">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-714">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ea6d2-715">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-715">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ea6d2-716">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-716">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ea6d2-717">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-717">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ea6d2-718">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ea6d2-718">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="ea6d2-719">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-719">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-720">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-720">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-721">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-721">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="ea6d2-722">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ea6d2-722">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="ea6d2-723">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-723">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="ea6d2-724">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="ea6d2-724">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="ea6d2-725">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-725">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="ea6d2-726">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-726">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="ea6d2-727">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-727">Set-AzStorageAccount</span></span>
* <span data-ttu-id="ea6d2-728">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-728">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="ea6d2-729">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ea6d2-729">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="ea6d2-730">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ea6d2-730">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ea6d2-731">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ea6d2-731">Az.StorageSync</span></span>
* <span data-ttu-id="ea6d2-732">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-732">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="ea6d2-733">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-733">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-734">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-734">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-735">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-735">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="ea6d2-736">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="ea6d2-736">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="ea6d2-737">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-737">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="ea6d2-738">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="ea6d2-738">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="ea6d2-739">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="ea6d2-739">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-740">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-740">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-741">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-741">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="ea6d2-742">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-742">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="ea6d2-743">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ea6d2-743">Az.Dns</span></span>
* <span data-ttu-id="ea6d2-744">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-744">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ea6d2-745">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ea6d2-745">Az.EventGrid</span></span>
* <span data-ttu-id="ea6d2-746">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-746">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="ea6d2-747">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-747">New cmdlets:</span></span>
    - <span data-ttu-id="ea6d2-748">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ea6d2-748">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ea6d2-749">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-749">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ea6d2-750">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ea6d2-750">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ea6d2-751">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-751">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="ea6d2-752">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ea6d2-752">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ea6d2-753">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-753">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ea6d2-754">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ea6d2-754">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ea6d2-755">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-755">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ea6d2-756">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ea6d2-756">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ea6d2-757">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-757">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="ea6d2-758">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-758">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ea6d2-759">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-759">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="ea6d2-760">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="ea6d2-760">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="ea6d2-761">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-761">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="ea6d2-762">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-762">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ea6d2-763">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-763">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="ea6d2-764">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-764">Updated cmdlets:</span></span>
    - <span data-ttu-id="ea6d2-765">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-765">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="ea6d2-766">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-766">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ea6d2-767">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-767">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ea6d2-768">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-768">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="ea6d2-769">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-769">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="ea6d2-770">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="ea6d2-770">Event subscription expiration date,</span></span>
            - <span data-ttu-id="ea6d2-771">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="ea6d2-771">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="ea6d2-772">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-772">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="ea6d2-773">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-773">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="ea6d2-774">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-774">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="ea6d2-775">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-775">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="ea6d2-776">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="ea6d2-776">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="ea6d2-777">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-777">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="ea6d2-778">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-778">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ea6d2-779">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-779">Az.FrontDoor</span></span>
* <span data-ttu-id="ea6d2-780">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="ea6d2-780">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="ea6d2-781">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-781">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="ea6d2-782">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="ea6d2-782">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="ea6d2-783">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-783">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-784">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-784">Az.Network</span></span>
* <span data-ttu-id="ea6d2-785">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-785">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="ea6d2-786">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-786">New cmdlets</span></span>
        - <span data-ttu-id="ea6d2-787">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="ea6d2-787">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="ea6d2-788">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-788">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="ea6d2-789">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-789">New cmdlets</span></span> 
        - <span data-ttu-id="ea6d2-790">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="ea6d2-790">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="ea6d2-791">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-791">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="ea6d2-792">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-792">New cmdlets</span></span> 
        - <span data-ttu-id="ea6d2-793">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-793">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="ea6d2-794">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-794">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ea6d2-795">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ea6d2-795">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ea6d2-796">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-796">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="ea6d2-797">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-797">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="ea6d2-798">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-798">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="ea6d2-799">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-799">New cmdlets</span></span>
        - <span data-ttu-id="ea6d2-800">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ea6d2-800">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ea6d2-801">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ea6d2-801">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ea6d2-802">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ea6d2-802">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ea6d2-803">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-803">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="ea6d2-804">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="ea6d2-804">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="ea6d2-805">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-805">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="ea6d2-806">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-806">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="ea6d2-807">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-807">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="ea6d2-808">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-808">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="ea6d2-809">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-809">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="ea6d2-810">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-810">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="ea6d2-811">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-811">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="ea6d2-812">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-812">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="ea6d2-813">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-813">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="ea6d2-814">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-814">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="ea6d2-815">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-815">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="ea6d2-816">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-816">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="ea6d2-817">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-817">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="ea6d2-818">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-818">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-819">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-819">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="ea6d2-820">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-820">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="ea6d2-821">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-821">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="ea6d2-822">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-822">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="ea6d2-823">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-823">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="ea6d2-824">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-824">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ea6d2-825">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-825">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ea6d2-826">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-826">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-827">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-827">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-828">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-828">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-829">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-829">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-830">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-830">Support for additional Template Export options</span></span>
    - <span data-ttu-id="ea6d2-831">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-831">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ea6d2-832">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-832">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ea6d2-833">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-833">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-834">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-834">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-835">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-835">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-836">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-836">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-837">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-837">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="ea6d2-838">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-838">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="ea6d2-839">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-839">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="ea6d2-840">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ea6d2-840">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ea6d2-841">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ea6d2-841">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ea6d2-842">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ea6d2-842">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ea6d2-843">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ea6d2-843">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="ea6d2-844">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ea6d2-844">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-845">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-845">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-846">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-846">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="ea6d2-847">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-847">New-AzStorageAccount</span></span>
* <span data-ttu-id="ea6d2-848">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-848">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="ea6d2-849">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-849">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-850">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-850">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-851">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-851">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="ea6d2-852">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-852">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="ea6d2-853">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-853">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="ea6d2-854">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-854">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-855">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-855">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-856">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-856">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-857">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-857">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="ea6d2-858">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="ea6d2-858">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ea6d2-859">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-859">Az.EventHub</span></span>
* <span data-ttu-id="ea6d2-860">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-860">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="ea6d2-861">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-861">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-862">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-862">Az.Network</span></span>
* <span data-ttu-id="ea6d2-863">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-863">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="ea6d2-864">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-864">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ea6d2-865">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-865">Az.PolicyInsights</span></span>
* <span data-ttu-id="ea6d2-866">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-866">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-867">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-867">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-868">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-868">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-869">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-869">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-870">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-870">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-871">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-871">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-872">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-872">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="ea6d2-873">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-873">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-874">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-874">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-875">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-875">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="ea6d2-876">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="ea6d2-876">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="ea6d2-877">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-877">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="ea6d2-878">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-878">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-879">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-879">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-880">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-880">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="ea6d2-881">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-881">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-882">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-882">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-883">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-883">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="ea6d2-884">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-884">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="ea6d2-885">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-885">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="ea6d2-886">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-886">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="ea6d2-887">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-887">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="ea6d2-888">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-888">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="ea6d2-889">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-889">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="ea6d2-890">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-890">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="ea6d2-891">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-891">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="ea6d2-892">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-892">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="ea6d2-893">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-893">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="ea6d2-894">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-894">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="ea6d2-895">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-895">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="ea6d2-896">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-896">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="ea6d2-897">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-897">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="ea6d2-898">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-898">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="ea6d2-899">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-899">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="ea6d2-900">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-900">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="ea6d2-901">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-901">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="ea6d2-902">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="ea6d2-902">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="ea6d2-903">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-903">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="ea6d2-904">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-904">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="ea6d2-905">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-905">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="ea6d2-906">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-906">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="ea6d2-907">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-907">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="ea6d2-908">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-908">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="ea6d2-909">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-909">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="ea6d2-910">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-910">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="ea6d2-911">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-911">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="ea6d2-912">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-912">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="ea6d2-913">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-913">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="ea6d2-914">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="ea6d2-914">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="ea6d2-915">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-915">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="ea6d2-916">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-916">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ea6d2-917">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="ea6d2-917">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="ea6d2-918">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-918">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="ea6d2-919">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-919">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="ea6d2-920">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-920">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="ea6d2-921">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-921">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="ea6d2-922">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-922">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="ea6d2-923">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-923">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ea6d2-924">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-924">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="ea6d2-925">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-925">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="ea6d2-926">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-926">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ea6d2-927">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-927">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ea6d2-928">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-928">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ea6d2-929">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-929">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="ea6d2-930">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-930">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ea6d2-931">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-931">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="ea6d2-932">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-932">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="ea6d2-933">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-933">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="ea6d2-934">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-934">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="ea6d2-935">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-935">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="ea6d2-936">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-936">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="ea6d2-937">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-937">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="ea6d2-938">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-938">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="ea6d2-939">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-939">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ea6d2-940">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-940">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ea6d2-941">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-941">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ea6d2-942">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-942">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ea6d2-943">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-943">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ea6d2-944">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-944">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ea6d2-945">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="ea6d2-945">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ea6d2-946">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-946">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ea6d2-947">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-947">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="ea6d2-948">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-948">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="ea6d2-949">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="ea6d2-949">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="ea6d2-950">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-950">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="ea6d2-951">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="ea6d2-951">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="ea6d2-952">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-952">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="ea6d2-953">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="ea6d2-953">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="ea6d2-954">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-954">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="ea6d2-955">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-955">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="ea6d2-956">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-956">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="ea6d2-957">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-957">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="ea6d2-958">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-958">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="ea6d2-959">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="ea6d2-959">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-960">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-960">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-961">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-961">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="ea6d2-962">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="ea6d2-962">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="ea6d2-963">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="ea6d2-963">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="ea6d2-964">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-964">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="ea6d2-965">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="ea6d2-965">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="ea6d2-966">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-966">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="ea6d2-967">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-967">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-968">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-969">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-969">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="ea6d2-970">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-970">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-971">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-971">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-972">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-972">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-973">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-973">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-974">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-974">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-975">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-975">Az.Network</span></span>
* <span data-ttu-id="ea6d2-976">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-976">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="ea6d2-977">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-977">Updated cmdlet:</span></span>
        - <span data-ttu-id="ea6d2-978">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-978">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="ea6d2-979">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-979">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-980">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-980">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-981">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-981">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-982">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-982">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-983">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-983">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="ea6d2-984">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-984">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-985">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-985">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-986">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-986">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-987">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-987">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-988">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-988">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="ea6d2-989">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-989">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-990">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-990">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-991">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-991">Proximity placement group feature.</span></span>
    - <span data-ttu-id="ea6d2-992">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-992">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="ea6d2-993">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-993">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="ea6d2-994">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-994">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="ea6d2-995">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-995">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="ea6d2-996">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-996">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="ea6d2-997">重大な変更</span><span class="sxs-lookup"><span data-stu-id="ea6d2-997">Breaking changes</span></span>
    - <span data-ttu-id="ea6d2-998">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-998">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="ea6d2-999">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-999">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="ea6d2-1000">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1000">Az.DeploymentManager</span></span>
* <span data-ttu-id="ea6d2-1001">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1001">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="ea6d2-1002">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1002">Az.Dns</span></span>
* <span data-ttu-id="ea6d2-1003">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1003">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="ea6d2-1004">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1004">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="ea6d2-1005">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1005">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ea6d2-1006">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1006">Az.FrontDoor</span></span>
* <span data-ttu-id="ea6d2-1007">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1007">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="ea6d2-1008">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1008">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="ea6d2-1009">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1009">Az.HDInsight</span></span>
* <span data-ttu-id="ea6d2-1010">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1010">Removed two cmdlets:</span></span>
    - <span data-ttu-id="ea6d2-1011">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1011">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="ea6d2-1012">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1012">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ea6d2-1013">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1013">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ea6d2-1014">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1014">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="ea6d2-1015">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1015">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="ea6d2-1016">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1016">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-1017">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1017">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-1018">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1018">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="ea6d2-1019">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1019">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="ea6d2-1020">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1020">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="ea6d2-1021">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1021">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="ea6d2-1022">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1022">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="ea6d2-1023">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1023">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="ea6d2-1024">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1024">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="ea6d2-1025">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1025">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ea6d2-1026">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1026">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ea6d2-1027">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1027">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ea6d2-1028">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1028">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ea6d2-1029">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1029">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ea6d2-1030">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1030">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="ea6d2-1031">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1031">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1032">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1032">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1033">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1033">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="ea6d2-1034">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1034">New cmdlets</span></span>
        - <span data-ttu-id="ea6d2-1035">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1035">New-AzNatGateway</span></span>
        - <span data-ttu-id="ea6d2-1036">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1036">Get-AzNatGateway</span></span>
        - <span data-ttu-id="ea6d2-1037">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1037">Set-AzNatGateway</span></span>
        - <span data-ttu-id="ea6d2-1038">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1038">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="ea6d2-1039">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1039">Updated cmdlets</span></span>
        - <span data-ttu-id="ea6d2-1040">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1040">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="ea6d2-1041">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1041">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="ea6d2-1042">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1042">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="ea6d2-1043">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1043">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="ea6d2-1044">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1044">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ea6d2-1045">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1045">Az.PolicyInsights</span></span>
* <span data-ttu-id="ea6d2-1046">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1046">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="ea6d2-1047">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1047">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="ea6d2-1048">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1048">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1049">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1049">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-1050">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1050">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="ea6d2-1051">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1051">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="ea6d2-1052">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1052">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="ea6d2-1053">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1053">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="ea6d2-1054">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1054">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="ea6d2-1055">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1055">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="ea6d2-1056">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1056">Az.Relay</span></span>
* <span data-ttu-id="ea6d2-1057">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1057">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-1058">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1058">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-1059">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1059">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1060">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1061">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1061">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="ea6d2-1062">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1062">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="ea6d2-1063">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1063">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="ea6d2-1064">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1064">New-AzStorageAccount</span></span>
* <span data-ttu-id="ea6d2-1065">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1065">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="ea6d2-1066">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1066">New-AzStorageAccount</span></span>
    - <span data-ttu-id="ea6d2-1067">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1067">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="ea6d2-1068">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1068">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1069">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1069">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1070">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1070">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="ea6d2-1071">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1071">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="ea6d2-1072">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1072">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ea6d2-1073">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1073">Highlights since the last major release</span></span>
* <span data-ttu-id="ea6d2-1074">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1074">General availability of `Az` module</span></span>
* <span data-ttu-id="ea6d2-1075">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1075">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ea6d2-1076">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1076">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ea6d2-1077">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1077">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ea6d2-1078">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1078">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ea6d2-1079">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1079">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1080">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1080">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1081">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1081">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1082">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1082">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ea6d2-1083">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1083">Az.Batch</span></span>
* <span data-ttu-id="ea6d2-1084">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1084">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ea6d2-1085">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1085">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-1086">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1086">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-1087">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1087">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-1088">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1088">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1089">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1089">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1090">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1090">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="ea6d2-1091">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1091">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1092">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1092">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-1093">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1093">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-1094">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1094">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1095">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1095">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1096">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1096">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ea6d2-1097">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1097">Az.EventGrid</span></span>
* <span data-ttu-id="ea6d2-1098">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1098">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ea6d2-1099">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1099">Az.EventHub</span></span>
* <span data-ttu-id="ea6d2-1100">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1100">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="ea6d2-1101">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1101">Az.HDInsight</span></span>
* <span data-ttu-id="ea6d2-1102">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1102">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-1103">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1103">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-1104">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1104">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-1105">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1105">Az.KeyVault</span></span>
* <span data-ttu-id="ea6d2-1106">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1106">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1107">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1107">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="ea6d2-1108">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1108">Az.MachineLearning</span></span>
* <span data-ttu-id="ea6d2-1109">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1109">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="ea6d2-1110">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1110">Az.Media</span></span>
* <span data-ttu-id="ea6d2-1111">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1111">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-1112">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1112">Az.Monitor</span></span>
  * <span data-ttu-id="ea6d2-1113">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1113">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="ea6d2-1114">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1114">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="ea6d2-1115">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1115">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="ea6d2-1116">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1116">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ea6d2-1117">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1117">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ea6d2-1118">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1118">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="ea6d2-1119">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1119">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1120">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1120">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1121">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1121">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1122">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1122">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="ea6d2-1123">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1123">Az.NotificationHubs</span></span>
* <span data-ttu-id="ea6d2-1124">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1124">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-1125">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1125">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-1126">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1126">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="ea6d2-1127">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1127">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="ea6d2-1128">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1128">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1129">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1129">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-1130">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1130">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1131">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1131">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="ea6d2-1132">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1132">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="ea6d2-1133">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1133">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ea6d2-1134">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1134">Az.RedisCache</span></span>
* <span data-ttu-id="ea6d2-1135">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1136">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1136">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1137">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1137">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1138">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1138">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1139">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1139">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="ea6d2-1140">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1141">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1141">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="ea6d2-1142">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1142">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="ea6d2-1143">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1143">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="ea6d2-1144">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1144">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="ea6d2-1145">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1145">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1146">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1146">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1147">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1147">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="ea6d2-1148">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1148">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ea6d2-1149">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1149">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="ea6d2-1150">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1150">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="ea6d2-1151">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1151">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ea6d2-1152">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1152">Highlights since the last major release</span></span>
* <span data-ttu-id="ea6d2-1153">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1153">General availability of `Az` module</span></span>
* <span data-ttu-id="ea6d2-1154">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1154">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ea6d2-1155">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1155">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ea6d2-1156">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1156">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ea6d2-1157">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1157">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ea6d2-1158">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1158">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1159">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1159">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1160">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1160">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1161">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1161">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ea6d2-1162">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1162">Az.AnalysisServices</span></span>
* <span data-ttu-id="ea6d2-1163">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1163">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="ea6d2-1164">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1164">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-1165">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1165">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1166">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1166">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="ea6d2-1167">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1167">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="ea6d2-1168">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1168">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1169">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1169">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1170">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1170">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ea6d2-1171">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1171">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="ea6d2-1172">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1172">Az.ContainerInstance</span></span>
* <span data-ttu-id="ea6d2-1173">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1173">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-1174">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1174">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-1175">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1175">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="ea6d2-1176">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1176">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1177">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1177">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1178">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1178">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="ea6d2-1179">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1179">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="ea6d2-1180">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1180">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="ea6d2-1181">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1181">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="ea6d2-1182">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1182">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="ea6d2-1183">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1183">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1184">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1184">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1185">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1185">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1186">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1186">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1187">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1187">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="ea6d2-1188">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1188">New-AzStorageContext</span></span>
* <span data-ttu-id="ea6d2-1189">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1189">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="ea6d2-1190">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1190">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ea6d2-1191">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1191">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ea6d2-1192">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1192">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="ea6d2-1193">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1193">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="ea6d2-1194">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1194">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="ea6d2-1195">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1195">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ea6d2-1196">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1196">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ea6d2-1197">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1197">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="ea6d2-1198">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1198">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="ea6d2-1199">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1199">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ea6d2-1200">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1200">Highlights since the last major release</span></span>
* <span data-ttu-id="ea6d2-1201">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1201">General availability of `Az` module</span></span>
* <span data-ttu-id="ea6d2-1202">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1202">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ea6d2-1203">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1203">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ea6d2-1204">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1204">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ea6d2-1205">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1205">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ea6d2-1206">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1206">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1207">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1207">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-1208">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1208">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1209">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1209">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="ea6d2-1210">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1210">Dynamic grouping</span></span>
    * <span data-ttu-id="ea6d2-1211">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1211">Pre-Post script</span></span>
    * <span data-ttu-id="ea6d2-1212">再起動設定</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1212">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1213">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1213">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1214">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1214">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="ea6d2-1215">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1215">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-1216">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1216">Az.KeyVault</span></span>
* <span data-ttu-id="ea6d2-1217">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1217">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1218">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1218">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1219">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1219">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="ea6d2-1220">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1220">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1221">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1221">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-1222">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1222">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="ea6d2-1223">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1223">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1224">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1224">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1225">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1225">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="ea6d2-1226">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1226">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1227">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1228">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1228">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1229">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1229">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1230">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1230">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="ea6d2-1231">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1231">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ea6d2-1232">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1232">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ea6d2-1233">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1233">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ea6d2-1234">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1234">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="ea6d2-1235">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1235">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="ea6d2-1236">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1236">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1237">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1237">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1238">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1238">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="ea6d2-1239">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1239">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1240">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1240">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1241">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1241">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="ea6d2-1242">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1242">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-1243">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1243">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1244">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1244">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="ea6d2-1245">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1245">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="ea6d2-1246">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1246">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ea6d2-1247">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1247">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-1248">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1248">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1249">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1249">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1250">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1250">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-1251">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1251">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-1252">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1252">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ea6d2-1253">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1253">Az.LogicApp</span></span>
* <span data-ttu-id="ea6d2-1254">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1254">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1255">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1255">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1256">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1256">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1257">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1257">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-1258">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1258">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="ea6d2-1259">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1259">SDK Update</span></span>
* <span data-ttu-id="ea6d2-1260">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1260">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="ea6d2-1261">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1261">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1262">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1262">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1263">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1263">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="ea6d2-1264">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1264">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="ea6d2-1265">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1265">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="ea6d2-1266">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1266">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="ea6d2-1267">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1267">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="ea6d2-1268">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1268">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1269">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1269">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1270">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1270">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="ea6d2-1271">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1271">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1272">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1272">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1273">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1273">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="ea6d2-1274">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1274">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="ea6d2-1275">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1275">Az.AnalysisServices</span></span>
* <span data-ttu-id="ea6d2-1276">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1276">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-1277">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1277">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1278">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1278">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="ea6d2-1279">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1279">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="ea6d2-1280">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1280">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-1281">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1281">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-1282">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1282">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1283">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1283">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1284">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1284">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="ea6d2-1285">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1285">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="ea6d2-1286">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1286">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="ea6d2-1287">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1287">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1288">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1288">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1289">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1289">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ea6d2-1290">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1290">Az.EventHub</span></span>
* <span data-ttu-id="ea6d2-1291">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1291">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-1292">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1292">Az.KeyVault</span></span>
* <span data-ttu-id="ea6d2-1293">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1293">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ea6d2-1294">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1294">Az.LogicApp</span></span>
* <span data-ttu-id="ea6d2-1295">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1295">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="ea6d2-1296">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1296">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="ea6d2-1297">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1297">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="ea6d2-1298">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1298">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ea6d2-1299">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1299">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ea6d2-1300">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1300">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ea6d2-1301">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1301">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="ea6d2-1302">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1302">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="ea6d2-1303">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1303">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ea6d2-1304">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1304">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ea6d2-1305">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1305">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ea6d2-1306">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1306">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="ea6d2-1307">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1307">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ea6d2-1308">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1308">Az.Monitor</span></span>
* <span data-ttu-id="ea6d2-1309">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1309">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1310">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1310">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1311">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1311">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-1312">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1312">Az.OperationalInsights</span></span>
* <span data-ttu-id="ea6d2-1313">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1313">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="ea6d2-1314">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1314">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="ea6d2-1315">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1315">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1316">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1316">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1317">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1317">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ea6d2-1318">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1318">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="ea6d2-1319">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1319">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="ea6d2-1320">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1320">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1321">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1321">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1322">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1322">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="ea6d2-1323">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1323">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1324">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1324">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1325">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1325">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="ea6d2-1326">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1326">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1327">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1327">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1328">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1328">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ea6d2-1329">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1329">Az.AnalysisServices</span></span>
<span data-ttu-id="ea6d2-1330">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1330">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1331">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1331">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1332">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1332">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="ea6d2-1333">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1333">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="ea6d2-1334">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1334">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1335">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1335">Az.RecoveryServices</span></span>
<span data-ttu-id="ea6d2-1336">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1336">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1337">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1337">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1338">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1338">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="ea6d2-1339">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1339">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ea6d2-1340">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1340">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="ea6d2-1341">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1341">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1342">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1342">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1343">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1343">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="ea6d2-1344">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1344">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="ea6d2-1345">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1345">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="ea6d2-1346">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1346">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1347">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1347">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1348">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1348">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ea6d2-1349">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1349">Az.AnalysisServices</span></span>
* <span data-ttu-id="ea6d2-1350">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1350">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1351">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1351">Az.RecoveryServices</span></span>
* <span data-ttu-id="ea6d2-1352">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1352">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="ea6d2-1353">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1353">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1354">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1354">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1355">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1355">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ea6d2-1356">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1356">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ea6d2-1357">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1357">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="ea6d2-1358">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1358">Az.Aks</span></span>
* <span data-ttu-id="ea6d2-1359">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1359">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ea6d2-1360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1360">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1361">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1361">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="ea6d2-1362">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1362">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ea6d2-1363">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1363">Az.Cdn</span></span>
* <span data-ttu-id="ea6d2-1364">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1364">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1365">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1365">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1366">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1366">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="ea6d2-1367">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1367">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="ea6d2-1368">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1368">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ea6d2-1369">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1369">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ea6d2-1370">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1370">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ea6d2-1371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1371">Az.DataFactory</span></span>
* <span data-ttu-id="ea6d2-1372">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1372">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1373">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1373">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1374">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1374">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="ea6d2-1375">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1375">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="ea6d2-1376">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1376">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-1377">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1377">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-1378">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1378">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-1379">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1379">Az.KeyVault</span></span>
* <span data-ttu-id="ea6d2-1380">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1380">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1381">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1381">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1382">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1382">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1383">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1383">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1384">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1384">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="ea6d2-1385">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1385">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="ea6d2-1386">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1386">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="ea6d2-1387">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1387">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="ea6d2-1388">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1388">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="ea6d2-1389">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1389">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="ea6d2-1390">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1390">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-1391">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1391">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-1392">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1392">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="ea6d2-1393">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1393">Fix some error messages.</span></span>
* <span data-ttu-id="ea6d2-1394">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1394">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="ea6d2-1395">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1395">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ea6d2-1396">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1396">Az.SignalR</span></span>
* <span data-ttu-id="ea6d2-1397">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1397">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1398">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1399">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1399">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ea6d2-1400">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1400">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="ea6d2-1401">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1401">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="ea6d2-1402">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1402">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1403">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1403">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1404">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1404">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ea6d2-1405">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1405">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="ea6d2-1406">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1406">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="ea6d2-1407">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1407">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="ea6d2-1408">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1408">Az.TrafficManager</span></span>
* <span data-ttu-id="ea6d2-1409">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1409">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1410">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1410">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1411">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1411">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ea6d2-1412">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1412">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="ea6d2-1413">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1413">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="ea6d2-1414">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1414">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1415">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1415">Az.Accounts</span></span>
* <span data-ttu-id="ea6d2-1416">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1416">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1417">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1418">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1418">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="ea6d2-1419">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1419">Updated the description of ID in help files</span></span>
* <span data-ttu-id="ea6d2-1420">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1420">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1421">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1421">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1422">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1422">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="ea6d2-1423">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1423">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ea6d2-1424">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1424">Az.EventGrid</span></span>
* <span data-ttu-id="ea6d2-1425">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1425">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="ea6d2-1426">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1426">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="ea6d2-1427">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1427">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ea6d2-1428">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1428">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ea6d2-1429">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1429">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ea6d2-1430">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1430">Dead letter endpoint.</span></span>
    - <span data-ttu-id="ea6d2-1431">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1431">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ea6d2-1432">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1432">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ea6d2-1433">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1433">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ea6d2-1434">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1434">Dead letter endpoint.</span></span>
* <span data-ttu-id="ea6d2-1435">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1435">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="ea6d2-1436">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1436">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ea6d2-1437">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1437">Az.IotHub</span></span>
* <span data-ttu-id="ea6d2-1438">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1438">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ea6d2-1439">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1439">Az.LogicApp</span></span>
* <span data-ttu-id="ea6d2-1440">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1440">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1441">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1441">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1442">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1442">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="ea6d2-1443">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1443">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="ea6d2-1444">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1444">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ea6d2-1445">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1445">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="ea6d2-1446">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1446">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="ea6d2-1447">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1447">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ea6d2-1448">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1448">Az.SignalR</span></span>
* <span data-ttu-id="ea6d2-1449">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1449">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1450">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1450">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1451">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1451">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ea6d2-1452">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1452">Az.Storage</span></span>
* <span data-ttu-id="ea6d2-1453">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1453">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="ea6d2-1454">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1454">New-AzStorageContext</span></span>
* <span data-ttu-id="ea6d2-1455">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1455">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="ea6d2-1456">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1456">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1457">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1457">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1458">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1458">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="ea6d2-1459">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1459">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="ea6d2-1460">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1460">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="ea6d2-1461">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1461">General</span></span>

- <span data-ttu-id="ea6d2-1462">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1462">General Availability of Az Module</span></span>
- <span data-ttu-id="ea6d2-1463">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1463">Online help for each module</span></span>
- <span data-ttu-id="ea6d2-1464">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1464">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="ea6d2-1465">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1465">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="ea6d2-1466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1466">Az.Accounts</span></span>
- <span data-ttu-id="ea6d2-1467">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1467">Changed from Az.Profile</span></span>
- <span data-ttu-id="ea6d2-1468">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1468">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-1469">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1469">Az.ApiManagement</span></span>
- <span data-ttu-id="ea6d2-1470">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1470">Fixes for #7002</span></span>
- <span data-ttu-id="ea6d2-1471">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1471">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="ea6d2-1472">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1472">Az.Batch</span></span>
- <span data-ttu-id="ea6d2-1473">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1473">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="ea6d2-1474">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1474">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="ea6d2-1475">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1475">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="ea6d2-1476">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1476">Az.Billing</span></span>
- <span data-ttu-id="ea6d2-1477">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1477">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="ea6d2-1478">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1478">Az.CognitivServices</span></span>
- <span data-ttu-id="ea6d2-1479">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1479">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="ea6d2-1480">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1480">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ea6d2-1481">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1481">Az.ContainerInstance</span></span>
- <span data-ttu-id="ea6d2-1482">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1482">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="ea6d2-1483">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1483">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="ea6d2-1484">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1484">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1485">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1485">Az.DataLakeStore</span></span>
- <span data-ttu-id="ea6d2-1486">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1486">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="ea6d2-1487">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1487">Az.Monitor</span></span>
- <span data-ttu-id="ea6d2-1488">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1488">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="ea6d2-1489">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1489">Az.KeyVault</span></span>
- <span data-ttu-id="ea6d2-1490">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1490">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="ea6d2-1491">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1491">Az.MachineLearning</span></span>
- <span data-ttu-id="ea6d2-1492">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1492">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="ea6d2-1493">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1493">Az.Media</span></span>
- <span data-ttu-id="ea6d2-1494">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1494">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1495">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1495">Az.Network</span></span>
<span data-ttu-id="ea6d2-1496">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1496">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="ea6d2-1497">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1497">New cmdlets added:</span></span>
        - <span data-ttu-id="ea6d2-1498">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1498">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1499">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1499">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1500">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1500">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1501">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1501">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1502">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1502">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1503">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1503">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="ea6d2-1504">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1504">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="ea6d2-1505">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1505">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="ea6d2-1506">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1506">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="ea6d2-1507">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1507">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="ea6d2-1508">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1508">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ea6d2-1509">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1509">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ea6d2-1510">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1510">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="ea6d2-1511">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1511">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="ea6d2-1512">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1512">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="ea6d2-1513">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1513">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="ea6d2-1514">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1514">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ea6d2-1515">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1515">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ea6d2-1516">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1516">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="ea6d2-1517">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1517">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="ea6d2-1518">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1518">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="ea6d2-1519">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1519">Az.OperationalInsights</span></span>
- <span data-ttu-id="ea6d2-1520">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1520">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="ea6d2-1521">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1521">Az.Profile</span></span>
- <span data-ttu-id="ea6d2-1522">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1522">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1523">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1523">Az.RecoveryServices</span></span>
- <span data-ttu-id="ea6d2-1524">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1524">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="ea6d2-1525">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1525">Az.Resources</span></span>
- <span data-ttu-id="ea6d2-1526">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1526">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-1527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1527">Az.ServiceFabric</span></span>
- <span data-ttu-id="ea6d2-1528">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1528">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="ea6d2-1529">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1529">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="ea6d2-1530">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1530">Az.SIgnalR</span></span>
- <span data-ttu-id="ea6d2-1531">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1531">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="ea6d2-1532">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1532">Az.Sql</span></span>
- <span data-ttu-id="ea6d2-1533">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1533">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="ea6d2-1534">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1534">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="ea6d2-1535">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1535">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="ea6d2-1536">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1536">Az.Storage</span></span>
- <span data-ttu-id="ea6d2-1537">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1537">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1538">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1538">Az.Websites</span></span>
- <span data-ttu-id="ea6d2-1539">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1539">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="ea6d2-1540">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1540">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="ea6d2-1541">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1541">General</span></span>

* <span data-ttu-id="ea6d2-1542">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1542">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="ea6d2-1543">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1543">Az.Compute</span></span>

* <span data-ttu-id="ea6d2-1544">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1544">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1545">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1545">Az.DataLakeStore</span></span>

* <span data-ttu-id="ea6d2-1546">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1546">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="ea6d2-1547">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1547">Az.FrontDoor</span></span>

* <span data-ttu-id="ea6d2-1548">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1548">Fixed some broken links</span></span>
    - <span data-ttu-id="ea6d2-1549">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1549">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="ea6d2-1550">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1550">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ea6d2-1551">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1551">Az.RecoveryServices</span></span>

* <span data-ttu-id="ea6d2-1552">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1552">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="ea6d2-1553">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1553">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="ea6d2-1554">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1554">Az.Resources</span></span>

* <span data-ttu-id="ea6d2-1555">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1555">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="ea6d2-1556">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1556">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="ea6d2-1557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1557">Az.Sql</span></span>

* <span data-ttu-id="ea6d2-1558">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1558">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="ea6d2-1559">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1559">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="ea6d2-1560">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1560">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="ea6d2-1561">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1561">Az.Storage</span></span>

* <span data-ttu-id="ea6d2-1562">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1562">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="ea6d2-1563">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1563">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="ea6d2-1564">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1564">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ea6d2-1565">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1565">Support Static Website configuration</span></span>
    - <span data-ttu-id="ea6d2-1566">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1566">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="ea6d2-1567">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1567">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1568">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1568">Az.Websites</span></span>

* <span data-ttu-id="ea6d2-1569">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1569">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="ea6d2-1570">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1570">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="ea6d2-1571">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1571">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="ea6d2-1572">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1572">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ea6d2-1573">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1573">Az.ApiManagement</span></span>
* <span data-ttu-id="ea6d2-1574">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1574">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="ea6d2-1575">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1575">Az.Automation</span></span>
* <span data-ttu-id="ea6d2-1576">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1576">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="ea6d2-1577">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1577">Added Update Management cmdlets</span></span>
* <span data-ttu-id="ea6d2-1578">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1578">Added Source Control cmdlets</span></span>
* <span data-ttu-id="ea6d2-1579">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1579">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="ea6d2-1580">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1580">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="ea6d2-1581">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1581">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1582">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1582">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="ea6d2-1583">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1583">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ea6d2-1584">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1584">Az.ContainerInstance</span></span>
* <span data-ttu-id="ea6d2-1585">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1585">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="ea6d2-1586">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1586">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ea6d2-1587">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1587">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1588">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1588">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1589">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1589">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="ea6d2-1590">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1590">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="ea6d2-1591">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1591">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="ea6d2-1592">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1592">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="ea6d2-1593">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1593">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ea6d2-1594">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1594">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="ea6d2-1595">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1595">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="ea6d2-1596">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1596">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="ea6d2-1597">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1597">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="ea6d2-1598">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1598">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="ea6d2-1599">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1599">Az.Relay</span></span>
* <span data-ttu-id="ea6d2-1600">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1600">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="ea6d2-1601">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1601">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1602">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1602">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="ea6d2-1603">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1603">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="ea6d2-1604">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1604">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-1605">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1605">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-1606">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1606">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="ea6d2-1607">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1607">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1608">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1608">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="ea6d2-1609">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1609">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ea6d2-1610">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1610">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ea6d2-1611">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1611">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ea6d2-1612">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1612">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ea6d2-1613">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1613">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ea6d2-1614">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1614">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ea6d2-1615">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1615">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ea6d2-1616">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1616">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="ea6d2-1617">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1617">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="ea6d2-1618">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1618">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="ea6d2-1619">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1619">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="ea6d2-1620">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1620">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ea6d2-1621">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1621">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ea6d2-1622">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1622">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="ea6d2-1623">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1623">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="ea6d2-1624">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1624">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="ea6d2-1625">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1625">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ea6d2-1626">全般</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1626">General</span></span>
* <span data-ttu-id="ea6d2-1627">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1627">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="ea6d2-1628">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1628">Az.Profile</span></span>
* <span data-ttu-id="ea6d2-1629">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1629">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="ea6d2-1630">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1630">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="ea6d2-1631">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1631">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="ea6d2-1632">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1632">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="ea6d2-1633">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1633">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="ea6d2-1634">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1634">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="ea6d2-1635">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1635">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-1636">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1636">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-1637">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1637">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1638">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1638">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1639">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1639">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="ea6d2-1640">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1640">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="ea6d2-1641">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1641">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1642">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1642">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1643">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1643">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="ea6d2-1644">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1644">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="ea6d2-1645">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1645">Az.Insights</span></span>
* <span data-ttu-id="ea6d2-1646">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1646">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="ea6d2-1647">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1647">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="ea6d2-1648">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1648">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="ea6d2-1649">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1649">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1650">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1650">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1651">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1651">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="ea6d2-1652">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1652">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="ea6d2-1653">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1653">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="ea6d2-1654">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1654">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="ea6d2-1655">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1655">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="ea6d2-1656">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1656">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="ea6d2-1657">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1657">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ea6d2-1658">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1658">Az.PolicyInsights</span></span>
* <span data-ttu-id="ea6d2-1659">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1659">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1660">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1661">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1661">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="ea6d2-1662">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1662">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ea6d2-1663">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1663">Az.ServiceBus</span></span>
* <span data-ttu-id="ea6d2-1664">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1664">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ea6d2-1665">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1665">Az.ServiceFabric</span></span>
* <span data-ttu-id="ea6d2-1666">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1666">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="ea6d2-1667">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1667">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="ea6d2-1668">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1668">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="ea6d2-1669">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1669">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="ea6d2-1670">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1670">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="ea6d2-1671">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1671">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="ea6d2-1672">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1672">Az.Profile</span></span>
* <span data-ttu-id="ea6d2-1673">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1673">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="ea6d2-1674">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1674">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1675">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1675">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1676">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1676">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="ea6d2-1677">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1677">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ea6d2-1678">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1678">Az.DataLakeStore</span></span>
* <span data-ttu-id="ea6d2-1679">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1679">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="ea6d2-1680">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1680">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="ea6d2-1681">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1681">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ea6d2-1682">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1682">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ea6d2-1683">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1683">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1684">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1684">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1685">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1685">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="ea6d2-1686">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1686">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1687">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1687">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1688">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1688">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="ea6d2-1689">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1689">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="ea6d2-1690">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1690">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="ea6d2-1691">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1691">Azure.Storage</span></span>
* <span data-ttu-id="ea6d2-1692">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1692">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="ea6d2-1693">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1693">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="ea6d2-1694">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1694">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ea6d2-1695">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1695">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="ea6d2-1696">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1696">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="ea6d2-1697">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1697">Az.CognitiveServices</span></span>
* <span data-ttu-id="ea6d2-1698">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1698">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ea6d2-1699">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1699">Az.Compute</span></span>
* <span data-ttu-id="ea6d2-1700">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1700">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="ea6d2-1701">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1701">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="ea6d2-1702">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1702">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="ea6d2-1703">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1703">Az.DataFactoryV2</span></span>
* <span data-ttu-id="ea6d2-1704">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1704">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ea6d2-1705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1705">Az.Network</span></span>
* <span data-ttu-id="ea6d2-1706">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1706">Added NetworkProfile functionality.</span></span> <span data-ttu-id="ea6d2-1707">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1707">new cmdlets added</span></span>
    - <span data-ttu-id="ea6d2-1708">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1708">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="ea6d2-1709">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1709">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="ea6d2-1710">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1710">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="ea6d2-1711">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1711">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="ea6d2-1712">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1712">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="ea6d2-1713">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1713">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="ea6d2-1714">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1714">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="ea6d2-1715">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1715">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="ea6d2-1716">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1716">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ea6d2-1717">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1717">Az.RedisCache</span></span>
* <span data-ttu-id="ea6d2-1718">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1718">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="ea6d2-1719">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1719">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="ea6d2-1720">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1720">Az.Resources</span></span>
* <span data-ttu-id="ea6d2-1721">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1721">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ea6d2-1722">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1722">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="ea6d2-1723">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1723">Az.Sql</span></span>
* <span data-ttu-id="ea6d2-1724">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1724">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ea6d2-1725">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1725">Az.Websites</span></span>
* <span data-ttu-id="ea6d2-1726">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1726">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="ea6d2-1727">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1727">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="ea6d2-1728">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1728">0.2.0 - September 2018</span></span>
 <span data-ttu-id="ea6d2-1729">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="ea6d2-1729">Initial Release</span></span>

---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 60827fe7b4f8c351655046e3711660cdf7ce0513
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "83631066"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="c78ba-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="c78ba-103">Azure PowerShell release notes</span></span>

## <a name="410---may-2020"></a><span data-ttu-id="c78ba-104">4.1.0 - 2020 年 5 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-104">4.1.0 - May 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c78ba-105">前回のリリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-105">Highlights since the last release</span></span>
* <span data-ttu-id="c78ba-106">次の PowerShell バージョンをサポートしました。Windows PowerShell 5.1、PowerShell Core 6.2.4+、PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c78ba-106">Supported PowerShell versions: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>
* <span data-ttu-id="c78ba-107">Az.Functions の一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-107">General availability of Az.Functions</span></span> 
* <span data-ttu-id="c78ba-108">Az.ApiManagement、Az.Batch、Az.Compute、Az.KeyVault、Az.Monitor、Az.Network、Az.OperationalInsights、Az.Resources、Az.Storage にメジャー リリースがあります</span><span class="sxs-lookup"><span data-stu-id="c78ba-108">Az.ApiManagement, Az.Batch, Az.Compute, Az.KeyVault, Az.Monitor, Az.Network, Az.OperationalInsights, Az.Resources, and Az.Storage have major release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-109">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-110">パラメーター 'AzureSynapseAnalyticsEndpointResourceId' および 'AzureSynapseAnalyticsEndpointSuffix' を受け入れるように 'Add-AzEnvironment' と 'Set-AzEnvironment' を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-110">Updated 'Add-AzEnvironment' and 'Set-AzEnvironment' to accept parameters 'AzureSynapseAnalyticsEndpointResourceId' and 'AzureSynapseAnalyticsEndpointSuffix'</span></span>
* <span data-ttu-id="c78ba-111">Azure.Core 関連アセンブリを Az.Accounts に追加しました。サポートされている PowerShell プラットフォームには、Windows PowerShell 5.1、PowerShell Core 6.2.4、PowerShell 7 以降が含まれます</span><span class="sxs-lookup"><span data-stu-id="c78ba-111">Added Azure.Core related assemblies into Az.Accounts, supported PowerShell platforms include Windows PowerShell 5.1, PowerShell Core 6.2.4, PowerShell 7+</span></span>

#### <a name="azaks"></a><span data-ttu-id="c78ba-112">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c78ba-112">Az.Aks</span></span>
* <span data-ttu-id="c78ba-113">API バージョンを 2019-10-01 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-113">Upgraded API Version to 2019-10-01</span></span>
* <span data-ttu-id="c78ba-114">Windows コンテナーを使用した AKS の作成をサポートしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-114">Supported to create AKS using Windows container</span></span>
* <span data-ttu-id="c78ba-115">次の新しいコマンドレットを提供しました。'New-AzAksNodePool'、'Update-AzAksNodePool'、'Remove-AzAksNodePool'、'Get-AzAksNodePool'、'Install-AzAksKubectl'、'Get-AzAksVersion'</span><span class="sxs-lookup"><span data-stu-id="c78ba-115">Provided new cmdlets: 'New-AzAksNodePool', 'Update-AzAksNodePool', 'Remove-AzAksNodePool',        'Get-AzAksNodePool', 'Install-AzAksKubectl', 'Get-AzAksVersion'</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-116">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-116">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-117">'New-AzApiManagement' と 'Set-AzApiManagement': [-AssignIdentity] パラメーターの名前を [-SystemAssignedIdentity] に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-117">'New-AzApiManagement' and 'Set-AzApiManagement': [-AssignIdentity] parameter renamed as [-SystemAssignedIdentity]</span></span>
* <span data-ttu-id="c78ba-118">'New-AzApiManagement' と 'Set-AzApiManagement':新しいパラメーター [-UserAssignedIdentity <String[]>] を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-118">'New-AzApiManagement' and 'Set-AzApiManagement': New parameter added: [-UserAssignedIdentity <String[]>]</span></span>
* <span data-ttu-id="c78ba-119">'Get-AzApiManagementProperty': 名前を 'Get-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-119">'Get-AzApiManagementProperty': renamed as 'Get-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c78ba-120">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-120">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c78ba-121">'New-AzApiManagementProperty': 名前を 'New-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-121">'New-AzApiManagementProperty': renamed as 'New-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c78ba-122">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-122">PropertyId parameter renamed as NamedValueId.</span></span> 
* <span data-ttu-id="c78ba-123">'Set-AzApiManagementProperty': 名前を 'Set-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-123">'Set-AzApiManagementProperty': renamed as 'Set-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c78ba-124">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-124">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c78ba-125">'Remove-AzApiManagementProperty': 名前を 'Remove-AzApiManagementNamedValue' に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-125">'Remove-AzApiManagementProperty': renamed as 'Remove-AzApiManagementNamedValue'.</span></span> <span data-ttu-id="c78ba-126">PropertyId パラメーターの名前を NamedValueId に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-126">PropertyId parameter renamed as NamedValueId.</span></span>
* <span data-ttu-id="c78ba-127">新しい 'Get-AzApiManagementAuthorizationServerClientSecret' コマンドレットを追加しました。'Get-AzApiManagementAuthorizationServer' ではクライアント シークレットは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-127">Added new 'Get-AzApiManagementAuthorizationServerClientSecret' cmdlet and 'Get-AzApiManagementAuthorizationServer' will not return client secret anymore.</span></span>
* <span data-ttu-id="c78ba-128">新しい 'Get-AzApiManagementNamedValueSecretValue' コマンドレットを追加しました。'Get-AzApiManagementNamedValue' ではシークレット値は返されません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-128">Added new 'Get-AzApiManagementNamedValueSecretValue' cmdlet and 'Get-AzApiManagementNamedValue' will not return secret value.</span></span>
* <span data-ttu-id="c78ba-129">新しい 'Get-AzApiManagementOpenIdConnectProviderClientSecret' コマンドレットを追加しました。'Get-AzApiManagementOpenIdConnectProvider' ではクライアント シークレットは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-129">Added new 'Get-AzApiManagementOpenIdConnectProviderClientSecret' cmdlet and 'Get-AzApiManagementOpenIdConnectProvider' will not return client secret anymore.</span></span>
* <span data-ttu-id="c78ba-130">新しい 'Get-AzApiManagementSubscriptionKey' コマンドレットを追加しました。'Get-AzApiManagementSubscription' ではサブスクリプション キーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-130">Added new 'Get-AzApiManagementSubscriptionKey' cmdlet and 'Get-AzApiManagementSubscription' will not return subscription keys anymore.</span></span>
* <span data-ttu-id="c78ba-131">新しい 'Get-AzApiManagementTenantAccessSecret' コマンドレットを追加しました。'Get-AzApiManagementTenantAccess' ではキーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-131">Added new 'Get-AzApiManagementTenantAccessSecret' cmdlet and 'Get-AzApiManagementTenantAccess' will not return keys anymore.</span></span>
* <span data-ttu-id="c78ba-132">新しい 'Get-AzApiManagementTenantGitAccessSecret' コマンドレットを追加しました。'Get-AzApiManagementTenantGitAccess' ではキーは返されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-132">Added new 'Get-AzApiManagementTenantGitAccessSecret' cmdlet and 'Get-AzApiManagementTenantGitAccess' will not return keys anymore.</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c78ba-133">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-133">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c78ba-134">次のパラメーターを追加しました。'New-AzApplicationInsights' 用の 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery'</span><span class="sxs-lookup"><span data-stu-id="c78ba-134">Added Parameters: 'RetentionInDays' 'PublicNetworkAccessForIngestion' 'PublicNetworkAccessForQuery' for 'New-AzApplicationInsights'</span></span>
* <span data-ttu-id="c78ba-135">コマンドレット 'Update-AzApplicationInsights' を作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-135">Created cmdlet 'Update-AzApplicationInsights'</span></span>
* <span data-ttu-id="c78ba-136">リンクされているストレージ アカウント用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-136">Created cmdlets for Linked Storage Account</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-137">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-137">Az.Batch</span></span>
* <span data-ttu-id="c78ba-138">'Microsoft.Azure.Batch' SDK バージョン 13.0.0 と 'Microsoft.Azure.Management.Batch' SDK バージョン 9.0.0 を使用するように Az.Batch を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-138">Updated Az.Batch to use 'Microsoft.Azure.Batch' SDK version 13.0.0 and 'Microsoft.Azure.Management.Batch' SDK version 9.0.0.</span></span>
* <span data-ttu-id="c78ba-139">新しい '-CertificateKind' パラメーターを使用して追加する証明書の種類を選択する機能を 'New-AzBatchCertificate' に追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-139">Added the ability to select the kind of certificate being added using the new '-CertificateKind' parameter to 'New-AzBatchCertificate'.</span></span>
* <span data-ttu-id="c78ba-140">以前は常に '' であった 'PSApplication' から 'ApplicationPackages' プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-140">Removed 'ApplicationPackages' property from 'PSApplication' which was previously always ''.</span></span>
  - <span data-ttu-id="c78ba-141">アプリケーション内の特定のパッケージは 'Get-AzBatchApplicationPackage' を使用して取得できるようになっています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-141">The specific packages inside of an application now can be retrieved using 'Get-AzBatchApplicationPackage'.</span></span> <span data-ttu-id="c78ba-142">次に例を示します。'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'</span><span class="sxs-lookup"><span data-stu-id="c78ba-142">For example: 'Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication'.</span></span>
* <span data-ttu-id="c78ba-143">'New-AzBatchPool' を使用してプールを作成する場合に、'PSImageReference' の 'VirtualMachineImageId' プロパティが Shared Image Gallery のイメージのみを参照できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-143">When creating a pool using 'New-AzBatchPool', the 'VirtualMachineImageId' property of 'PSImageReference' can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="c78ba-144">'New-AzBatchPool' を使用してプールを作成する場合に、'PSNetworkConfiguration' の新しい 'PublicIPAddressConfiguration' プロパティを使用して、そのプールをパブリック IP なしでプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-144">When creating a pool using 'New-AzBatchPool', the pool can be provisioned without a public IP using the new 'PublicIPAddressConfiguration' property of 'PSNetworkConfiguration'.</span></span>
  - <span data-ttu-id="c78ba-145">'PSNetworkConfiguration' の 'PublicIPs' プロパティも 'PSPublicIPAddressConfiguration' に移動しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-145">The 'PublicIPs' property of 'PSNetworkConfiguration' has moved in to 'PSPublicIPAddressConfiguration' as well.</span></span> <span data-ttu-id="c78ba-146">このプロパティは、'IPAddressProvisioningType ' が 'UserManaged' の場合にのみ指定できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-146">This property can only be specified if 'IPAddressProvisioningType' is 'UserManaged'.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-147">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-147">Az.Compute</span></span>
* <span data-ttu-id="c78ba-148">'Update-AzVM' コマンドレットに HostId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-148">Added HostId parameter to 'Update-AzVM' cmdlet</span></span>
* <span data-ttu-id="c78ba-149">'New-AzVMConfig'、'New-AzVmssConfig'、'Update-AzVmss'、'Set-AzVMOperatingSystem'、'Set-AzVmssOsProfile' コマンドレットのヘルプ ドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-149">Updated Help documents for 'New-AzVMConfig', 'New-AzVmssConfig', 'Update-AzVmss', 'Set-AzVMOperatingSystem' and 'Set-AzVmssOsProfile' cmdlets.</span></span>
* <span data-ttu-id="c78ba-150">重大な変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-150">Breaking changes</span></span>
    - <span data-ttu-id="c78ba-151">FilterExpression パラメーターが 'Get-AzVMImage' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-151">FilterExpression parameter is removed from 'Get-AzVMImage' cmdlet.</span></span>
    - <span data-ttu-id="c78ba-152">AssignIdentity パラメーターが 'New-AzVmssConfig'、'New-AzVMConfig'、'Update-AzVM' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-152">AssignIdentity parameter is removed from 'New-AzVmssConfig', 'New-AzVMConfig' and 'Update-AzVM' cmdlets.</span></span>
    - <span data-ttu-id="c78ba-153">AutomaticRepairMaxInstanceRepairsPercent が 'New-AzVmssConfig' と 'Update-AzVmss' コマンドレットから削除されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-153">AutomaticRepairMaxInstanceRepairsPercent is removed from 'New-AzVmssConfig' and 'Update-AzVmss' cmdlets.</span></span>
    - <span data-ttu-id="c78ba-154">AvailabilitySetsColocationStatus、VirtualMachinesColocationStatus、VirtualMachineScaleSetsColocationStatus プロパティが ProximityPlacementGroup から削除されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-154">AvailabilitySetsColocationStatus, VirtualMachinesColocationStatus and VirtualMachineScaleSetsColocationStatus properties are removed from ProximityPlacementGroup.</span></span>
    - <span data-ttu-id="c78ba-155">MaxInstanceRepairsPercent プロパティが AutomaticRepairsPolicy から削除されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-155">MaxInstanceRepairsPercent property is removed from AutomaticRepairsPolicy.</span></span>
    - <span data-ttu-id="c78ba-156">AvailabilitySets、VirtualMachines、VirtualMachineScaleSets の種類が IList<SubResource> から IList<SubResourceWithColocationStatus> に変更されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-156">The types of AvailabilitySets, VirtualMachines and VirtualMachineScaleSets are changed from IList<SubResource> to IList<SubResourceWithColocationStatus>.</span></span>
* <span data-ttu-id="c78ba-157">'Get-AzVM' コマンドレットの説明を、わかりやすくするために更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-157">Description for 'Get-AzVM' cmdlet has been updated to better describe it.</span></span> 

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-158">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-158">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-159">Managed IR でデータ フロー ランタイム プロパティの CRUD をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-159">Supported CRUD of data flow runtime properties in Managed IR.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-160">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-160">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-161">Front Door ルール エンジン オブジェクトを作成、更新、取得、削除するための新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-161">Added new cmdlets for creation, update, retreival, and deletion of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c78ba-162">Front Door ルール エンジン オブジェクトを構築するためのヘルパー コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-162">Added helper cmdlets for construction of Front Door Rules Engine object</span></span>
* <span data-ttu-id="c78ba-163">Front Door ルーティング規則オブジェクトにルール エンジン参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-163">Added Rules Engine reference to Front Door Routing Rule object.</span></span>
* <span data-ttu-id="c78ba-164">Front Door バックエンド オブジェクトにプライベート リンク パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-164">Added Private Link parameters to Front Door Backend object</span></span>

#### <a name="azfunctions"></a><span data-ttu-id="c78ba-165">Az.Functions</span><span class="sxs-lookup"><span data-stu-id="c78ba-165">Az.Functions</span></span>
* <span data-ttu-id="c78ba-166">''Az.Functions'' モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-166">General availability of ''Az.Functions'' module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-167">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-167">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-168">お客様が管理するキー ディスクの暗号化をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-168">Supported Customer-managed key disk encryption.</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c78ba-169">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c78ba-169">Az.HealthcareApis</span></span>
* <span data-ttu-id="c78ba-170">アクセス ポリシーの既定値が現在のプリンシパルではなくなりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-170">Access policies are no longer defaulted to the current principal</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-171">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-172">SQL に似た言語を使用して情報を取得するために、IoT ハブ内でクエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-172">Added cmdlet to invoke a query in an IoT hub to retrieve information using a SQL-like language.</span></span>
* <span data-ttu-id="c78ba-173">'Add-AzIotHubDevice' が子デバイスなしで Edge 対応デバイスを作成できない問題を修正しました [#11597]</span><span class="sxs-lookup"><span data-stu-id="c78ba-173">Fix issue that 'Add-AzIotHubDevice' fails to create Edge Enabled Device without child devices [#11597]</span></span>
* <span data-ttu-id="c78ba-174">Iot Hub、デバイス、またはモジュールの SAS トークンを生成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-174">Added cmdlet to generate SAS token for Iot Hub, device or module.</span></span>
* <span data-ttu-id="c78ba-175">構成メトリック クエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-175">Added cmdlet to invoke configuration metrics query.</span></span>
* <span data-ttu-id="c78ba-176">大規模な IoT Edge 自動デプロイを管理します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-176">Manage IoT Edge automatic deployment at scale.</span></span> <span data-ttu-id="c78ba-177">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-177">New cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-178">'Add-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-178">'Add-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c78ba-179">'Get-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-179">'Get-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c78ba-180">'Remove-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-180">'Remove-AzIotHubDeployment'</span></span>
    - <span data-ttu-id="c78ba-181">'Set-AzIotHubDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-181">'Set-AzIotHubDeployment'</span></span>
* <span data-ttu-id="c78ba-182">IoT Edge デプロイ メトリック クエリを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-182">Added cmdlet to invoke an IoT Edge deployment metrics query.</span></span>
* <span data-ttu-id="c78ba-183">指定されたエッジ デバイスに構成内容を適用するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-183">Added cmdlet to apply the configuration content to the specified edge device.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-184">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-184">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-185">次の 2 つの別名を削除しました。'New-AzKeyVaultCertificateAdministratorDetails' と 'New-AzKeyVaultCertificateOrganizationDetails'</span><span class="sxs-lookup"><span data-stu-id="c78ba-185">Removed two aliases: 'New-AzKeyVaultCertificateAdministratorDetails' and 'New-AzKeyVaultCertificateOrganizationDetails'</span></span>
* <span data-ttu-id="c78ba-186">キー コンテナーを作成するときに、論理的な削除を既定で有効にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-186">Enabled soft delete by default when creating a key vault</span></span>
* <span data-ttu-id="c78ba-187">キー コンテナーを作成するときに、特定のネットワークの場所からのアクセスを管理するようにネットワーク ルールを設定できます</span><span class="sxs-lookup"><span data-stu-id="c78ba-187">Network rules can be set to govern the accessibility from specific network locations when creating a key vault</span></span>
* <span data-ttu-id="c78ba-188">Bring Your Own Key (BYOK) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-188">Added support to bring your own key (BYOK)</span></span>
    - <span data-ttu-id="c78ba-189">'Add-AzKeyVaultKey' で、キー交換キーの生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-189">'Add-AzKeyVaultKey' supports generating a key exchange key</span></span>
    - <span data-ttu-id="c78ba-190">'Get-AzKeyVaultKey' で、PEM 形式の公開キーのダウンロードをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-190">'Get-AzKeyVaultKey' supports downloading a public key in PEM format</span></span>
* <span data-ttu-id="c78ba-191">'Add-AzKeyVaultKey' のヘルプ ドキュメントの 'KeyOps' 部分を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-191">Updated the 'KeyOps' part of the help document of 'Add-AzKeyVaultKey'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-192">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-192">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-193">保持ポリシーがすべてのカテゴリに適用されないという 'Set-AzDiagnosticSettings' のバグを修正しました [#11589]</span><span class="sxs-lookup"><span data-stu-id="c78ba-193">Fixed bug for 'Set-AzDiagnosticSettings', retention policy won't apply to all categories [#11589]</span></span>
* <span data-ttu-id="c78ba-194">メトリック アラート V2 の WebTest 可用性基準をサポートしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-194">Supported WebTest availability criteria for metric alert V2</span></span>
    - <span data-ttu-id="c78ba-195">'New-AzMetricAlertRuleV2Criteria': WebTest 可用性基準を作成するためのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-195">'New-AzMetricAlertRuleV2Criteria': an option to create webtest availability criteria was added</span></span>
    - <span data-ttu-id="c78ba-196">'Add-AzMetricAlertRuleV2': 新しい WebTest 可用性基準をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-196">'Add-AzMetricAlertRuleV2': supports the new webtest availability criteria</span></span>
* <span data-ttu-id="c78ba-197">PSLogProfile 内の RetentionPolicy の冗長な定義を削除しました [#7608]</span><span class="sxs-lookup"><span data-stu-id="c78ba-197">Removed redundant definition for RetentionPolicy in PSLogProfile [#7608]</span></span>
* <span data-ttu-id="c78ba-198">PSEventData で定義された冗長なプロパティを削除しました [#11353]</span><span class="sxs-lookup"><span data-stu-id="c78ba-198">Removed redundant properties difined in PSEventData [#11353]</span></span>
* <span data-ttu-id="c78ba-199">'Get-AzLog' の名前を 'Get-AzActivityLog' に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-199">Renamed 'Get-AzLog' to 'Get-AzActivityLog'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-200">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-200">Az.Network</span></span>
* <span data-ttu-id="c78ba-201">ゾーンの既定の動作が変更されることを通知するための、破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-201">Added breaking change attribute to notify that Zone default behaviour will be changed</span></span>
    - <span data-ttu-id="c78ba-202">'New-AzPublicIpAddress'</span><span class="sxs-lookup"><span data-stu-id="c78ba-202">'New-AzPublicIpAddress'</span></span>
    - <span data-ttu-id="c78ba-203">'New-AzPublicIpPrefix'</span><span class="sxs-lookup"><span data-stu-id="c78ba-203">'New-AzPublicIpPrefix'</span></span>
    - <span data-ttu-id="c78ba-204">'New-AzLoadBalancerFrontendIpConfig'</span><span class="sxs-lookup"><span data-stu-id="c78ba-204">'New-AzLoadBalancerFrontendIpConfig'</span></span>
* <span data-ttu-id="c78ba-205">新しい最上位リソース SecurityPartnerProvider のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-205">Added support for a new top level resource SecurityPartnerProvider</span></span>
    - <span data-ttu-id="c78ba-206">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-206">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-207">New-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c78ba-207">New-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c78ba-208">Remove-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c78ba-208">Remove-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c78ba-209">Get-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c78ba-209">Get-AzSecurityPartnerProvider</span></span>
        - <span data-ttu-id="c78ba-210">Set-AzSecurityPartnerProvider</span><span class="sxs-lookup"><span data-stu-id="c78ba-210">Set-AzSecurityPartnerProvider</span></span>
* <span data-ttu-id="c78ba-211">'RequiredZoneNames' を 'PSPrivateLinkResource' に、'GroupId' を 'PSPrivateEndpointConnection' に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-211">Added 'RequiredZoneNames' on 'PSPrivateLinkResource' and 'GroupId' on 'PSPrivateEndpointConnection'</span></span>
* <span data-ttu-id="c78ba-212">New-AzNetworkWatcherConnectionMonitorTestConfigurationObject の SuccessThresholdRoundTripTimeMs パラメーターの誤った種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-212">Fixed incorrect type of SuccessThresholdRoundTripTimeMs parameter for New-AzNetworkWatcherConnectionMonitorTestConfigurationObject</span></span>
* <span data-ttu-id="c78ba-213">AllowVnetToVnetTraffic 引数の既定値を True に設定するように VirtualWan コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-213">Updated VirtualWan cmdlets to set default value of AllowVnetToVnetTraffic argument to True.</span></span>
    - <span data-ttu-id="c78ba-214">'New-AzVirtualWan'</span><span class="sxs-lookup"><span data-stu-id="c78ba-214">'New-AzVirtualWan'</span></span>
    - <span data-ttu-id="c78ba-215">'Update-AzVirtualWan'</span><span class="sxs-lookup"><span data-stu-id="c78ba-215">'Update-AzVirtualWan'</span></span>
* <span data-ttu-id="c78ba-216">プライベート エンドポイントの DNS ゾーン グループをサポートする新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-216">Added new cmdlets to support DNS zone group for private endpoint</span></span>
    - <span data-ttu-id="c78ba-217">'New-AzPrivateDnsZoneConfig'</span><span class="sxs-lookup"><span data-stu-id="c78ba-217">'New-AzPrivateDnsZoneConfig'</span></span>
    - <span data-ttu-id="c78ba-218">'Get-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="c78ba-218">'Get-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c78ba-219">'New-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="c78ba-219">'New-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c78ba-220">'Set-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="c78ba-220">'Set-AzPrivateDnsZoneGroup'</span></span>
    - <span data-ttu-id="c78ba-221">'Remove-AzPrivateDnsZoneGroup'</span><span class="sxs-lookup"><span data-stu-id="c78ba-221">'Remove-AzPrivateDnsZoneGroup'</span></span>
* <span data-ttu-id="c78ba-222">'DNSEnableProxy'、'DNSRequireProxyForNetworkRules'、'DNSServers' パラメーターを 'AzureFirewall' に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-222">Added 'DNSEnableProxy', 'DNSRequireProxyForNetworkRules' and 'DNSServers' parameters to 'AzureFirewall'</span></span>
* <span data-ttu-id="c78ba-223">'EnableDnsProxy'、'DnsProxyNotRequiredForNetworkRule'、'DnsServer' パラメーターを 'AzureFirewall' に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-223">Added 'EnableDnsProxy', 'DnsProxyNotRequiredForNetworkRule' and 'DnsServer' parameters to 'AzureFirewall'</span></span>
    - <span data-ttu-id="c78ba-224">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-224">Updated cmdlet:</span></span>
        - <span data-ttu-id="c78ba-225">New-AzFirewall</span><span class="sxs-lookup"><span data-stu-id="c78ba-225">New-AzFirewall</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-226">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-226">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-227">生成された新しい SDK を適用するようにレガシ コードを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-227">Updated legacy code to apply new generated SDK</span></span>
* <span data-ttu-id="c78ba-228">非推奨になった API が原因でコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-228">Deleted cmdlets due to deprecated APIs</span></span>
    - <span data-ttu-id="c78ba-229">'Get-AzOperationalInsightsSavedSearchResult' (別名 'Get-AzOperationalInsightsSavedSearchResults')</span><span class="sxs-lookup"><span data-stu-id="c78ba-229">'Get-AzOperationalInsightsSavedSearchResult' (alias 'Get-AzOperationalInsightsSavedSearchResults')</span></span>
    - <span data-ttu-id="c78ba-230">'Get-AzOperationalInsightsSearchResult' (別名 'Get-AzOperationalInsightsSearchResults')</span><span class="sxs-lookup"><span data-stu-id="c78ba-230">'Get-AzOperationalInsightsSearchResult' (alias 'Get-AzOperationalInsightsSearchResults')</span></span>
    - <span data-ttu-id="c78ba-231">'Get-AzOperationalInsightsLinkTarget' (別名 'Get-AzOperationalInsightsLinkTargets')</span><span class="sxs-lookup"><span data-stu-id="c78ba-231">'Get-AzOperationalInsightsLinkTarget' (alias 'Get-AzOperationalInsightsLinkTargets')</span></span>
* <span data-ttu-id="c78ba-232">'Set-AzOperationalInsightsWorkspace' と 'New-AzOperationalInsightsWorkspace' のパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-232">Added parameters for 'Set-AzOperationalInsightsWorkspace' and 'New-AzOperationalInsightsWorkspace'</span></span>
* <span data-ttu-id="c78ba-233">リンクされているストレージ アカウント用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-233">Created cmdlets for Linked Stoarge Account</span></span>
* <span data-ttu-id="c78ba-234">クラスターおよびリンクされたサービス用のコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-234">Created cmdlets for Clusters and Linked Service</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-235">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-235">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-236">Azure Site Recovery で、Azure to Azure プロバイダーの近接配置グループ仮想マシンを保護するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-236">Azure Site Recovery added support for protecting proximity placement group virtual machines for Azure to Azure provider.</span></span>
* <span data-ttu-id="c78ba-237">Azure Site Recovery でゾーン間レプリケーションのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-237">Azure Site Recovery added support for zone to zone replication.</span></span>
* <span data-ttu-id="c78ba-238">Azure Backup で、Azure FileShare 回復ポイントの長期保持サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-238">Azure Backup Added Long term retention support for Azure FileShare Recovery Points.</span></span>
* <span data-ttu-id="c78ba-239">Azure Backup で、'Get-AzRecoveryServicesBackupItem' コマンドレット出力にディスク除外プロパティを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-239">Azure Backup Added disk exclusion properties to 'Get-AzRecoveryServicesBackupItem' cmdlet output.</span></span>
* <span data-ttu-id="c78ba-240">Site Recovery サービスのコンテナー資格情報ファイルのプライベート エンドポイントを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-240">Added private endpoint for Vault credential file for site recovery service.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-241">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-241">Az.Resources</span></span>
* <span data-ttu-id="c78ba-242">新しいロール定義を作成するときの表示遅延に関するメッセージ警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-242">Added message warning about view delay when creating a new Role Definition</span></span>
* <span data-ttu-id="c78ba-243">厳密に型指定されたオブジェクトを出力するようにポリシー コマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-243">Changed policy cmdlets to output strongly-typed objects</span></span>
* <span data-ttu-id="c78ba-244">'Get-AzResourceLock' コマンドレットで使用されていた '-TenantLevel' パラメーターを削除しました [#11335]</span><span class="sxs-lookup"><span data-stu-id="c78ba-244">Removed '-TenantLevel' parameter used for on the 'Get-AzResourceLock' cmdlet [#11335]</span></span>
* <span data-ttu-id="c78ba-245">'Remove-AzResourceGroup -Id ResourceId' を修正しました [#9882]</span><span class="sxs-lookup"><span data-stu-id="c78ba-245">Fixed 'Remove-AzResourceGroup -Id ResourceId'[#9882]</span></span>
* <span data-ttu-id="c78ba-246">リソース グループ スコープで ARM テンプレートの What-If 結果を取得するための新しいコマンドレット 'Get-AzDeploymentResourceGroupWhatIfResult' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-246">Added new cmdlet for getting ARM template What-If results at resource group scope: 'Get-AzDeploymentResourceGroupWhatIfResult'</span></span>
* <span data-ttu-id="c78ba-247">サブスクリプション スコープで ARM テンプレートの What-If 結果を取得するための新しいコマンドレット 'Get-AzDeploymentWhatIfResult' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-247">Added new cmdlet for getting ARM template What-If results at subscription scope: 'Get-AzDeploymentWhatIfResult'</span></span>
   - <span data-ttu-id="c78ba-248">エイリアス:'Get-AzSubscriptionDeploymentWhatIf'</span><span class="sxs-lookup"><span data-stu-id="c78ba-248">Alias: 'Get-AzSubscriptionDeploymentWhatIf'</span></span>
* <span data-ttu-id="c78ba-249">ARM テンプレートの What-If 結果を使用するために、'New-AzDeployment' と 'New-AzResourceGroupDeployment' の '-WhatIf' と '-Confirm' パラメーターをオーバーライドしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-249">Overrode '-WhatIf' and '-Confirm' parameters for 'New-AzDeployment' and 'New-AzResourceGroupDeployment' to use ARM template What-If results</span></span>
* <span data-ttu-id="c78ba-250">デプロイ コマンドレットの 'ApiVersion' パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-250">Added deprecation message for 'ApiVersion' parameter in deployment cmdlets</span></span>
* <span data-ttu-id="c78ba-251">デプロイの失敗に対する改善されたエラー メッセージを表示する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-251">Added capability to show improved error messages for deployment failures</span></span>
* <span data-ttu-id="c78ba-252">デプロイの失敗に対する correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-252">Added correlationId logging for deployment failures</span></span>
* <span data-ttu-id="c78ba-253">デプロイ スクリプトの出力に 'error' プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-253">Added 'error' property to the deployment script output</span></span>
* <span data-ttu-id="c78ba-254">nuget Microsoft.Azure.Management.ResourceManager を '3.7.1-preview' に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-254">Updated nuget Microsoft.Azure.Management.ResourceManager to '3.7.1-preview'</span></span>
* <span data-ttu-id="c78ba-255">DeploymentValidateResult の Error プロパティがnuget 3.7.1-preview から読み取り専用に変更されたため、特定のテスト ケースを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-255">Removed specific test cases as Error property in DeploymentValidateResult has changed to readonly from nuget 3.7.1-preview</span></span>
* <span data-ttu-id="c78ba-256">SDK ResourceManager 3.7.1-preview から GenericResourceExpanded を取得しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-256">Brought GenericResourceExpanded from SDK ResourceManager 3.7.1-preview</span></span>
* <span data-ttu-id="c78ba-257">デプロイ用のすべての Get コマンドレットおよび以下に対するタグ サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-257">Added tag support for all Get cmdlets for deployment, as well as</span></span>
    - <span data-ttu-id="c78ba-258">'New-AzDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-258">'New-AzDeployment'</span></span>
    - <span data-ttu-id="c78ba-259">'New-AzManagementGroupDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-259">'New-AzManagementGroupDeployment'</span></span>
    - <span data-ttu-id="c78ba-260">'New-AzResourceGroupDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-260">'New-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c78ba-261">'New-AzTenantDeployment'</span><span class="sxs-lookup"><span data-stu-id="c78ba-261">'New-AzTenantDeployment'</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-262">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-262">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-263">--SecretIdentifier を使用した証明書の追加で、誤った証明書の拇印を取得していたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-263">Fixed bug in add certificate using --SecretIdentifier that was getting the wrong certificate thumbprint</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-264">Az.Sql</span></span>
* <span data-ttu-id="c78ba-265">以下のパフォーマンスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-265">Enhance performance of:</span></span>
    - <span data-ttu-id="c78ba-266">'Set-AzSqlDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="c78ba-266">'Set-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c78ba-267">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="c78ba-267">'Set-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c78ba-268">'Remove-AzSqlDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="c78ba-268">'Remove-AzSqlDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c78ba-269">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span><span class="sxs-lookup"><span data-stu-id="c78ba-269">'Remove-AzSqlInstanceDatabaseSensitivityClassification'</span></span>
    - <span data-ttu-id="c78ba-270">'Enable-AzSqlDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="c78ba-270">'Enable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c78ba-271">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="c78ba-271">'Enable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c78ba-272">'Disable-AzSqlDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="c78ba-272">'Disable-AzSqlDatabaseSensitivityRecommendation'</span></span>
    - <span data-ttu-id="c78ba-273">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span><span class="sxs-lookup"><span data-stu-id="c78ba-273">'Disable-AzSqlInstanceDatabaseSensitivityRecommendation'</span></span>
* <span data-ttu-id="c78ba-274">コマンドレット 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy' から 'RetentionDays' パラメーターのクライアント側の検証を削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-274">Removed client-side validation of 'RetentionDays' parameter from cmdlet 'Set-AzSqlDatabaseBackupShortTermRetentionPolicy'</span></span>
* <span data-ttu-id="c78ba-275">Vnet のストレージ アカウントを監査し、Storage Blob Data Contributor ロールの作成時のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-275">Auditing to a storage account in Vnet, fixing a bug when creating a Storage Blob Data Contributor role.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-276">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-276">Az.Storage</span></span>
* <span data-ttu-id="c78ba-277">コマンドレット 'Get-AzStorageAccount' でアカウントを取得/一覧表示するために '-AsJob' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-277">Added '-AsJob' to get/list account cmdlet 'Get-AzStorageAccount'</span></span>
* <span data-ttu-id="c78ba-278">KeyvaultEncryption を使用してストレージ アカウントを更新するときに KeyVersion をオプションにして、キーの自動ローテーションをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-278">Make KeyVersion to optional when update Storage account with KeyvaultEncryption, to support key auto-rotation</span></span>
    - <span data-ttu-id="c78ba-279">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="c78ba-279">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c78ba-280">Azure File Directory の削除がパイプラインで失敗することを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-280">Fixed remove Azure File Directory fail with pipeline</span></span>
    - <span data-ttu-id="c78ba-281">'Remove-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="c78ba-281">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c78ba-282">[#9880] を修正しました。swagger に合わせて NetWorkRule DefaultAction 値の定義を変更しています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-282">Fixed [#9880]: Change NetWorkRule DefaultAction value defination to align with swagger.</span></span>
    - <span data-ttu-id="c78ba-283">'Update-AzStorageAccountNetworkRuleSet'</span><span class="sxs-lookup"><span data-stu-id="c78ba-283">'Update-AzStorageAccountNetworkRuleSet'</span></span>
    - <span data-ttu-id="c78ba-284">'Get-AzStorageAccountNetworkRuleSet'</span><span class="sxs-lookup"><span data-stu-id="c78ba-284">'Get-AzStorageAccountNetworkRuleSet'</span></span>
* <span data-ttu-id="c78ba-285">[#11624] を修正しました。サーバー障害を回避するため、NetworkRules の追加時に重複するルールをスキップします</span><span class="sxs-lookup"><span data-stu-id="c78ba-285">Fixed [#11624]: Skip duplicated rules when add NetworkRules, to avoid server failure</span></span>
    - <span data-ttu-id="c78ba-286">'Add-AzStorageAccountNetworkRule'</span><span class="sxs-lookup"><span data-stu-id="c78ba-286">'Add-AzStorageAccountNetworkRule'</span></span>
* <span data-ttu-id="c78ba-287">Microsoft.Azure.Cosmos.Table SDK を 1.0.7 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-287">Upgraded Microsoft.Azure.Cosmos.Table SDK to 1.0.7</span></span>
* <span data-ttu-id="c78ba-288">DataLake Gen2 項目の一覧表示で一部の項目のみが返されたときに、ContinuationToken を使用して再度一覧表示するようにユーザーに促す警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-288">Added a warning message to remind user to list again with ContinuationToken when only part items are returned in list DataLake Gen2 Items,</span></span>
    - <span data-ttu-id="c78ba-289">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="c78ba-289">'Get-AzDataLakeGen2ChildItem'</span></span>
* <span data-ttu-id="c78ba-290">Azure Files Active Directory Domain Service 認証でのストレージ アカウントの作成または更新をサポートしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-290">Supported to create or update Storage account with Azure Files Active Directory Domain Service Authentication</span></span>
    -  <span data-ttu-id="c78ba-291">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="c78ba-291">'New-AzStorageAccount'</span></span>
    -  <span data-ttu-id="c78ba-292">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="c78ba-292">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c78ba-293">ストレージ アカウントの Kerberos キーの新規作成または一覧表示をサポートしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-293">Supported to new or list Kerberos keys of Storage account</span></span>
    -  <span data-ttu-id="c78ba-294">'New-AzStorageAccountKey'</span><span class="sxs-lookup"><span data-stu-id="c78ba-294">'New-AzStorageAccountKey'</span></span>
    -  <span data-ttu-id="c78ba-295">'Get-AzStorageAccountKey'</span><span class="sxs-lookup"><span data-stu-id="c78ba-295">'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c78ba-296">ストレージ アカウントのフェールオーバーをサポートしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-296">Supported failover Storage account</span></span>
    - <span data-ttu-id="c78ba-297">'Invoke-AzStorageAccountFailover'</span><span class="sxs-lookup"><span data-stu-id="c78ba-297">'Invoke-AzStorageAccountFailover'</span></span>
* <span data-ttu-id="c78ba-298">'Get-AzStorageBlobCopyState' のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-298">Updated help of 'Get-AzStorageBlobCopyState'</span></span>
* <span data-ttu-id="c78ba-299">'Get-AzStorageFileCopyState' と 'Start-AzStorageBlobCopy' のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-299">Updated help of 'Get-AzStorageFileCopyState' and 'Start-AzStorageBlobCopy'</span></span>
* <span data-ttu-id="c78ba-300">ストレージ クライアント ライブラリ v12 を Queue および File コマンドレットに統合しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-300">Integrated Storage client library v12 to Queue and File cmdlets</span></span>
* <span data-ttu-id="c78ba-301">出力の種類を CloudFile から AzureStorageFile に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-301">Changed output type from CloudFile to AzureStorageFile, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c78ba-302">'Get-AzStorageFile'</span><span class="sxs-lookup"><span data-stu-id="c78ba-302">'Get-AzStorageFile'</span></span>
    - <span data-ttu-id="c78ba-303">'Remove-AzStorageFile'</span><span class="sxs-lookup"><span data-stu-id="c78ba-303">'Remove-AzStorageFile'</span></span>
    - <span data-ttu-id="c78ba-304">'Get-AzStorageFileContent'</span><span class="sxs-lookup"><span data-stu-id="c78ba-304">'Get-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c78ba-305">'Set-AzStorageFileContent'</span><span class="sxs-lookup"><span data-stu-id="c78ba-305">'Set-AzStorageFileContent'</span></span>
    - <span data-ttu-id="c78ba-306">'Start-AzStorageFileCopy'</span><span class="sxs-lookup"><span data-stu-id="c78ba-306">'Start-AzStorageFileCopy'</span></span>
* <span data-ttu-id="c78ba-307">出力の種類を CloudFileDirectory から AzureStorageFileDirectory に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-307">Changed output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c78ba-308">'New-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="c78ba-308">'New-AzStorageDirectory'</span></span>
    - <span data-ttu-id="c78ba-309">'Remove-AzStorageDirectory'</span><span class="sxs-lookup"><span data-stu-id="c78ba-309">'Remove-AzStorageDirectory'</span></span>
* <span data-ttu-id="c78ba-310">出力の種類を CloudFileShare から AzureStorageFileShare に変更しました。元の出力は新しい出力の子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-310">Changed output type from CloudFileShare to AzureStorageFileShare, the original output will become a child property of the new output</span></span>
    - <span data-ttu-id="c78ba-311">'Get-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="c78ba-311">'Get-AzStorageShare'</span></span>
    - <span data-ttu-id="c78ba-312">'New-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="c78ba-312">'New-AzStorageShare'</span></span>
    - <span data-ttu-id="c78ba-313">'Remove-AzStorageShare'</span><span class="sxs-lookup"><span data-stu-id="c78ba-313">'Remove-AzStorageShare'</span></span>
* <span data-ttu-id="c78ba-314">出力の種類を FileShareProperties から AzureStorageFileShare に変更しました。元の出力は新しい出力のサブの子プロパティになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-314">Changed output type from FileShareProperties to AzureStorageFileShare, the original output will become a sub child property of the new output</span></span>
    - <span data-ttu-id="c78ba-315">'Set-AzStorageShareQuota'</span><span class="sxs-lookup"><span data-stu-id="c78ba-315">'Set-AzStorageShareQuota'</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c78ba-316">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78ba-316">Az.TrafficManager</span></span>
* <span data-ttu-id="c78ba-317">'DisableAzureTrafficManagerEndpoint' の詳細出力の間違ったプロファイル名を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-317">Fixed incorrect profile name in 'DisableAzureTrafficManagerEndpoint' verbose output</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-318">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-318">Az.Websites</span></span>
* <span data-ttu-id="c78ba-319">'Update-AzWebAppAccessRestrictionConfig' のヘルプの誤記を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-319">Fixed typo on help of 'Update-AzWebAppAccessRestrictionConfig'.</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="c78ba-320">3.8.0 - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-320">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="c78ba-321">前回のリリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-321">Highlights since the last release</span></span>
* <span data-ttu-id="c78ba-322">Az.Storage でサポートされる PowerShell のバージョンは次のとおりです。Windows PowerShell 5.1、PowerShell Core 6.2.4+、PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="c78ba-322">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-323">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-323">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-324">'Resolve-AzError' の Azure PowerShell アンケートの URL を更新しました [#11507]</span><span class="sxs-lookup"><span data-stu-id="c78ba-324">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-325">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-325">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-326">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-326">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c78ba-327">GroupId パラメーターの指定について 'Set-AzApiManagementGroup' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-327">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-328">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-328">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-329">ChinaCDN 関連の価格 SKU の表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-329">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-330">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-330">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-331">ID、暗号化、UserOwnedStorage をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-331">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-332">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-332">Az.Compute</span></span>
* <span data-ttu-id="c78ba-333">'Set-AzVmssOrchestrationServiceState' コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-333">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="c78ba-334">'Get-AzVmss' に -InstanceView を指定することで、OrchestrationService の状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-334">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-335">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-335">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-336">IoT デバイス ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-336">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-337">'Get-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="c78ba-337">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="c78ba-338">'Update-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="c78ba-338">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="c78ba-339">Iot Hub のデバイスでダイレクト メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-339">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="c78ba-340">IoT デバイス モジュール ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-340">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-341">'Get-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="c78ba-341">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="c78ba-342">'Update-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="c78ba-342">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="c78ba-343">IoT の自動デバイス管理構成を大規模に管理します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-343">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="c78ba-344">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-344">New cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-345">'Add-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="c78ba-345">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c78ba-346">'Get-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="c78ba-346">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c78ba-347">'Remove-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="c78ba-347">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="c78ba-348">'Set-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="c78ba-348">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="c78ba-349">Iot Hub で edge モジュール メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-349">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-350">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-350">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-351">コンテナーでの論理的な削除と消去保護を有効にできる新しいコマンドレット 'Update-AzKeyVault' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-351">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="c78ba-352">Microsoft.PowerShell.SecretManagement へのサポートを追加しました [#11178]</span><span class="sxs-lookup"><span data-stu-id="c78ba-352">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="c78ba-353">'Remove-AzKeyVaultManagedStorageSasDefinition' の例の誤りを修正しました [#11479]</span><span class="sxs-lookup"><span data-stu-id="c78ba-353">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="c78ba-354">プライベート エンドポイントへのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-354">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="c78ba-355">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="c78ba-355">Az.Maintenance</span></span>
* <span data-ttu-id="c78ba-356">GA 用のメンテナンス コマンドレットのリリース バージョンを公開しています</span><span class="sxs-lookup"><span data-stu-id="c78ba-356">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-357">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-357">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-358">プライベート リンク スコープのコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-358">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="c78ba-359">'Get-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="c78ba-359">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c78ba-360">'Remove-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="c78ba-360">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c78ba-361">'New-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="c78ba-361">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c78ba-362">'Update-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="c78ba-362">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="c78ba-363">'Get-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="c78ba-363">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c78ba-364">'New-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="c78ba-364">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="c78ba-365">'Remove-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="c78ba-365">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-366">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-366">Az.Network</span></span>
* <span data-ttu-id="c78ba-367">仮想ネットワーク ゲートウェイのプライベート IP での接続を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-367">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="c78ba-368">'New-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="c78ba-368">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c78ba-369">'Set-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="c78ba-369">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="c78ba-370">'New-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="c78ba-370">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="c78ba-371">'Set-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="c78ba-371">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="c78ba-372">FQDN ベースの LocalNetworkGateways と VpnSites を有効にするコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-372">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="c78ba-373">'New-AzLocalNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="c78ba-373">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="c78ba-374">'New-AzVpnSiteLink'</span><span class="sxs-lookup"><span data-stu-id="c78ba-374">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="c78ba-375">ExpressRouteCircuitConnectionConfig (Global Reach) で IPv6 アドレス ファミリのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-375">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="c78ba-376">'Set-AzExpressRouteCircuitConnectionConfig' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-376">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c78ba-377">IPv6CircuitConnectionProperties を含むすべての既存のプロパティを設定できます</span><span class="sxs-lookup"><span data-stu-id="c78ba-377">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="c78ba-378">'Add-AzExpressRouteCircuitConnectionConfig' を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-378">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="c78ba-379">アドレス プレフィックスのアドレス ファミリを指定する、別の省略可能なパラメーター AddressPrefixType を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-379">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="c78ba-380">仮想ネットワーク ゲートウェイ接続で DPD タイムアウトの設定を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-380">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="c78ba-381">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-381">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="c78ba-382">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-382">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-383">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-383">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-384">ポリシー コンプライアンス スキャンをトリガーするための 'Start-AzPolicyComplianceScan' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-384">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="c78ba-385">ポリシー定義、セット定義、および割り当てのバージョンを 'Get-AzPolicyState' 出力に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-385">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-386">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-386">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-387">'New-AzServiceFabricCluster' サンプルのコードのフォーマットと使いやすさが向上しています</span><span class="sxs-lookup"><span data-stu-id="c78ba-387">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-388">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-388">Az.Sql</span></span>
* <span data-ttu-id="c78ba-389">コマンドレット 'Get-AzSqlInstanceOperation' および 'Stop-AzSqlInstanceOperation' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-389">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="c78ba-390">VNet のストレージ アカウントに対する監査をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-390">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-391">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-391">Az.Storage</span></span>
* <span data-ttu-id="c78ba-392">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-392">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="c78ba-393">ストレージ アカウントの作成/更新時に新しい SkuName StandardGZRS、StandardRAGZRS をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-393">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="c78ba-394">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="c78ba-394">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="c78ba-395">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="c78ba-395">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="c78ba-396">Supported DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="c78ba-396">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="c78ba-397">'New-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="c78ba-397">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c78ba-398">'Get-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="c78ba-398">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c78ba-399">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="c78ba-399">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="c78ba-400">'Move-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="c78ba-400">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c78ba-401">'Set-AzDataLakeGen2ItemAclObject'</span><span class="sxs-lookup"><span data-stu-id="c78ba-401">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="c78ba-402">'Update-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="c78ba-402">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="c78ba-403">'Get-AzDataLakeGen2ItemContent'</span><span class="sxs-lookup"><span data-stu-id="c78ba-403">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="c78ba-404">'Remove-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="c78ba-404">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="c78ba-405">0.10.0-preview - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-405">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="c78ba-406">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-406">General</span></span>
* <span data-ttu-id="c78ba-407">Az モジュールが Azure Stack Hub のプレビューで使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-407">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="c78ba-408">これにより、Linux および macOS とのクロスプラットフォームの互換性が確保されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-408">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="c78ba-409">Azure Stack Hub で、Az モジュールを使用した PowerShell Core がサポートされるようになりました。詳細については、[こちら](https://aka.ms/az4AzureStack)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-409">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="c78ba-410">Az モジュールでプロファイル 2019-03-01-hybrid がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-410">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="c78ba-411">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c78ba-411">Az.Billing</span></span>
  - <span data-ttu-id="c78ba-412">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-412">Az.Compute</span></span>
  - <span data-ttu-id="c78ba-413">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c78ba-413">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="c78ba-414">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-414">Az.EventHub</span></span>
  - <span data-ttu-id="c78ba-415">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-415">Az.IotHub</span></span>
  - <span data-ttu-id="c78ba-416">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-416">Az.KeyVault</span></span>
  - <span data-ttu-id="c78ba-417">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-417">Az.Monitor</span></span>
  - <span data-ttu-id="c78ba-418">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-418">Az.Network</span></span>
  - <span data-ttu-id="c78ba-419">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-419">Az.Resources</span></span>
  - <span data-ttu-id="c78ba-420">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-420">Az.Storage</span></span>
  - <span data-ttu-id="c78ba-421">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-421">Az.Websites</span></span>
* <span data-ttu-id="c78ba-422">Azure Stack Hubで動作する、Az 用の 3 つの新しい PowerShell モジュール (Az.Databox、Az.IotHub、Az.EventHu) が導入されました</span><span class="sxs-lookup"><span data-stu-id="c78ba-422">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="c78ba-423">コマンドは比較的同じままですが、AzureRM を Az に変更するなどの軽微な変更が加えられています</span><span class="sxs-lookup"><span data-stu-id="c78ba-423">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="c78ba-424">Azure Stack Hub の PowerShell ドキュメントへのリンクを更新しました。[こちら](https://aka.ms/InstallASHPowerShell)で確認できます</span><span class="sxs-lookup"><span data-stu-id="c78ba-424">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="c78ba-425">3.7.0 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-425">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-426">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-426">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-427">ログインしていない場合に、'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' が NullReferenceException をスローする問題を修正しました [#10292]</span><span class="sxs-lookup"><span data-stu-id="c78ba-427">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-428">Az.Compute</span></span>
* <span data-ttu-id="c78ba-429">'New-AzDiskConfig' コマンドレットに次のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-429">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="c78ba-430">DiskIOPSReadOnly、DiskMBpsReadOnly、MaxSharesCount、GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="c78ba-430">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="c78ba-431">'New-AzGalleryImageVersion' コマンドレットの Target パラメーターで Encryption プロパティを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-431">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="c78ba-432">'Set-AzVmss' の -Reimage と 'Invoke-AzVMReimage' コマンドレットの tempDisk の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-432">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="c78ba-433">[#11354]</span><span class="sxs-lookup"><span data-stu-id="c78ba-433">[#11354]</span></span>
* <span data-ttu-id="c78ba-434">新しい SAP 拡張機能の次のコマンドレットに対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-434">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="c78ba-435">'Set-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="c78ba-435">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c78ba-436">'Get-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="c78ba-436">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c78ba-437">'Remove-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="c78ba-437">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="c78ba-438">'Update-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="c78ba-438">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="c78ba-439">ヘルプ ドキュメントの例の誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-439">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="c78ba-440">VM PowerState の正確な文字列値をテーブル形式で示しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-440">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="c78ba-441">'New-AzVmssConfig': SinglePlacementGroup が無効な場合の AutomaticRepairs プロパティのシリアル化を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-441">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="c78ba-442">[#11257]</span><span class="sxs-lookup"><span data-stu-id="c78ba-442">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-443">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-443">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-444">ADF .Net SDK のバージョンを 4.8.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-444">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="c78ba-445">再実行をサポートするために、'Invoke-AzDataFactoryV2Pipeline' コマンドに省略可能なパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-445">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-446">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-446">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-447">'Export-AzDataLakeStoreItem' と 'Import-AzDataLakeStoreItem' に破壊的変更の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-447">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="c78ba-448">'New-AzDataLakeStoreItem'、'Add-AzDAtaLakeStoreItemContent'、および 'Get-AzDAtaLakeStoreItemContent' にバイト エンコードのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-448">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-449">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-449">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-450">クラスターの作成時に、最低限サポートされている TLS バージョンの指定をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-450">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-451">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-451">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-452">デバイスごとの分散設定の管理のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-452">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="c78ba-453">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-453">New Cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-454">'Get-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="c78ba-454">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="c78ba-455">'Set-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="c78ba-455">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-456">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-456">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-457">'New-AzKeyVault' に破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-457">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-458">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-458">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-459">'New-AzScheduledQueryRuleLogMetricTrigger' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-459">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-460">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-460">Az.Network</span></span>
* <span data-ttu-id="c78ba-461">テナント間の VirtualHubVnetConnections を許可するためにコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-461">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="c78ba-462">'New-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="c78ba-462">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c78ba-463">'Update-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="c78ba-463">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="c78ba-464">'New-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="c78ba-464">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="c78ba-465">'Update-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="c78ba-465">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="c78ba-466">SQL 管理 SDK の依存関係を削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-466">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-467">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-467">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-468">エラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-468">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-469">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-470">Azure Site Recovery で再保護を行うためのサポートを追加し、Azure Disk Encryption を使用して暗号化されている Virtual Machines の vm プロパティを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-470">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="c78ba-471">Azure Site Recovery に VmwareToAzure プロパティの DR 監視を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-471">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="c78ba-472">Azure Backup に、失敗した項目の再試行ポリシー更新のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-472">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="c78ba-473">Azure Backup に、バックアップおよび復元中のディスク除外設定のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-473">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="c78ba-474">Azure Backup に、AzureFileShare で複数ファイル/フォルダーを復元するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-474">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="c78ba-475">Azure Backup に、IaasVM ポリシーの更新中にユーザーによって指定された Resourcegroup へのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-475">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-476">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-476">Az.Resources</span></span>
* <span data-ttu-id="c78ba-477">既定の apiVersion ではなく、リソースの実際の apiVersion を使用するように 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' を修正しました [#11267]</span><span class="sxs-lookup"><span data-stu-id="c78ba-477">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="c78ba-478">エラー シナリオでの correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-478">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="c78ba-479">'Get-AzResourceLock' のドキュメントをわずかに変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-479">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="c78ba-480">例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-480">Added example.</span></span>
* <span data-ttu-id="c78ba-481">'Get-AzADUser' のパラメーター値の単一引用符をエスケープしました [#11317]</span><span class="sxs-lookup"><span data-stu-id="c78ba-481">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="c78ba-482">デプロイ スクリプト ('Get-AzDeploymentScript'、'Get-AzDeploymentScriptLog'、'Save-AzDeploymentScriptLog'、'Remove-AzDeploymentScript') に新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-482">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-483">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-483">Az.Sql</span></span>
* <span data-ttu-id="c78ba-484">'Invoke-AzSqlDatabaseFailover' に読み取り可能なセカンダリ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-484">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="c78ba-485">コマンドレット 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-485">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="c78ba-486">データベース内の列を分類するときの秘密度ランクを保存しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-486">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="c78ba-487">Az.Support</span><span class="sxs-lookup"><span data-stu-id="c78ba-487">Az.Support</span></span>
* <span data-ttu-id="c78ba-488">'Az.Support' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="c78ba-488">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-489">Az.Websites</span></span>
* <span data-ttu-id="c78ba-490">次の新しいコマンドレットを使用して、webapp トラフィック ルーティング規則を処理するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-490">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="c78ba-491">'Get-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="c78ba-491">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c78ba-492">'Update-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="c78ba-492">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c78ba-493">'Add-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="c78ba-493">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="c78ba-494">'Remove-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="c78ba-494">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="c78ba-495">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-495">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-496">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-496">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-497">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="c78ba-497">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="c78ba-498">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="c78ba-498">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="c78ba-499">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-499">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-500">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-500">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-501">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="c78ba-501">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="c78ba-502">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="c78ba-502">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="c78ba-503">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-503">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="c78ba-504">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="c78ba-504">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-505">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-505">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-506">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-506">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-507">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-507">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-508">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-508">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c78ba-509">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-509">New Cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-510">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-510">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-511">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-511">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-512">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-512">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-513">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-513">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="c78ba-514">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-514">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="c78ba-515">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-515">New Cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-516">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="c78ba-516">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="c78ba-517">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="c78ba-517">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="c78ba-518">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="c78ba-518">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="c78ba-519">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="c78ba-519">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="c78ba-520">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-520">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c78ba-521">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-521">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="c78ba-522">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-522">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="c78ba-523">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-523">New Cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-524">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="c78ba-524">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="c78ba-525">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="c78ba-525">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="c78ba-526">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-526">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-527">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-527">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-528">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="c78ba-528">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-529">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-529">Az.Network</span></span>
* <span data-ttu-id="c78ba-530">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-530">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="c78ba-531">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-531">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="c78ba-532">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-532">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="c78ba-533">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-533">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-534">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-534">Az.Resources</span></span>
* <span data-ttu-id="c78ba-535">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-535">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="c78ba-536">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="c78ba-536">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="c78ba-537">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="c78ba-537">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="c78ba-538">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="c78ba-538">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="c78ba-539">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-539">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="c78ba-540">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-540">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="c78ba-541">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-541">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="c78ba-542">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-542">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="c78ba-543">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c78ba-543">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c78ba-544">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c78ba-544">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="c78ba-545">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c78ba-545">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="c78ba-546">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-546">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="c78ba-547">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="c78ba-547">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="c78ba-548">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-548">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-549">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-549">Az.Sql</span></span>
* <span data-ttu-id="c78ba-550">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-550">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="c78ba-551">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-551">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="c78ba-552">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="c78ba-552">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="c78ba-553">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-553">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="c78ba-554">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-554">Remove an LTR backup</span></span>
    - <span data-ttu-id="c78ba-555">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-555">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="c78ba-556">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-556">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="c78ba-557">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-557">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="c78ba-558">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="c78ba-558">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-559">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-559">Az.Storage</span></span>
* <span data-ttu-id="c78ba-560">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-560">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="c78ba-561">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="c78ba-561">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="c78ba-562">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-562">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="c78ba-563">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="c78ba-563">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="c78ba-564">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="c78ba-564">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-565">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-565">Az.Websites</span></span>
* <span data-ttu-id="c78ba-566">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-566">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="c78ba-567">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="c78ba-567">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="c78ba-568">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-568">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="c78ba-569">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-569">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="c78ba-570">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-570">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="c78ba-571">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-571">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-572">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-572">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-573">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-573">Updated client side telemetry.</span></span>
* <span data-ttu-id="c78ba-574">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-574">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="c78ba-575">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-575">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-576">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-576">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-577">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-577">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-578">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-578">Az.Automation</span></span>
* <span data-ttu-id="c78ba-579">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-579">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-580">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-580">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-581">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-581">Updated SDK to 7.0</span></span>
* <span data-ttu-id="c78ba-582">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-582">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-583">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-583">Az.Compute</span></span>
* <span data-ttu-id="c78ba-584">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-584">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-585">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-585">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-586">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-586">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-587">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-587">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-588">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-588">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="c78ba-589">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-589">New Cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-590">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-590">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-591">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-591">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-592">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-592">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="c78ba-593">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="c78ba-593">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-594">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-594">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-595">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-595">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-596">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-596">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-597">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-597">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="c78ba-598">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-598">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="c78ba-599">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-599">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-600">Az.Network</span></span>
* <span data-ttu-id="c78ba-601">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-601">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="c78ba-602">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-602">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c78ba-603">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-603">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="c78ba-604">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-604">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="c78ba-605">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-605">No new cmdlets are added.</span></span> <span data-ttu-id="c78ba-606">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="c78ba-606">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-607">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-607">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-608">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-608">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-609">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-609">Az.Resources</span></span>
* <span data-ttu-id="c78ba-610">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-610">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="c78ba-611">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="c78ba-611">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="c78ba-612">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="c78ba-612">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="c78ba-613">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-613">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="c78ba-614">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-614">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="c78ba-615">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-615">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="c78ba-616">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-616">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="c78ba-617">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-617">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-618">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-618">Az.Sql</span></span>
* <span data-ttu-id="c78ba-619">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-619">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="c78ba-620">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-620">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="c78ba-621">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="c78ba-621">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c78ba-622">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c78ba-622">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c78ba-623">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-623">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c78ba-624">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c78ba-624">Az.StorageSync</span></span>
* <span data-ttu-id="c78ba-625">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-625">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="c78ba-626">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-626">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-627">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-627">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-628">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-628">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="c78ba-629">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-629">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-630">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-630">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-631">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="c78ba-631">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="c78ba-632">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-632">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-633">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-633">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-634">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="c78ba-634">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="c78ba-635">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="c78ba-635">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="c78ba-636">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-636">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="c78ba-637">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-637">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-638">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-638">Az.Compute</span></span>
* <span data-ttu-id="c78ba-639">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-639">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="c78ba-640">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-640">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="c78ba-641">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-641">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="c78ba-642">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-642">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="c78ba-643">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-643">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-644">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-644">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-645">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-645">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c78ba-646">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c78ba-646">Az.DeploymentManager</span></span>
* <span data-ttu-id="c78ba-647">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-647">Adds LIST operations for resources</span></span>
* <span data-ttu-id="c78ba-648">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-648">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-649">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-649">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-650">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-650">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-651">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-651">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-652">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-652">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-653">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-653">Az.Network</span></span>
* <span data-ttu-id="c78ba-654">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-654">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="c78ba-655">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="c78ba-655">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="c78ba-656">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="c78ba-656">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c78ba-657">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-657">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="c78ba-658">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="c78ba-658">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="c78ba-659">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-659">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="c78ba-660">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-660">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="c78ba-661">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-661">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="c78ba-662">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-662">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-663">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-663">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="c78ba-664">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-664">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="c78ba-665">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-665">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="c78ba-666">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-666">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-667">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-667">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-668">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-668">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="c78ba-669">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-669">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="c78ba-670">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-670">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="c78ba-671">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-671">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-672">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-672">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-673">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-673">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="c78ba-674">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-674">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-675">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-675">Az.Resources</span></span>
* <span data-ttu-id="c78ba-676">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="c78ba-676">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="c78ba-677">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-677">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-678">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-678">Az.Sql</span></span>
<span data-ttu-id="c78ba-679">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-679">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-680">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-680">Az.Storage</span></span>
* <span data-ttu-id="c78ba-681">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-681">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="c78ba-682">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-682">New-AzStorageAccount</span></span>
* <span data-ttu-id="c78ba-683">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="c78ba-683">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="c78ba-684">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-684">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-685">Az.Websites</span></span>
* <span data-ttu-id="c78ba-686">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-686">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="c78ba-687">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-687">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="c78ba-688">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-688">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-689">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-689">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-690">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-690">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-691">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-691">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-692">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="c78ba-692">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-693">Az.Compute</span></span>
* <span data-ttu-id="c78ba-694">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-694">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c78ba-695">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-695">Az.ContainerInstance</span></span>
* <span data-ttu-id="c78ba-696">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-696">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c78ba-697">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c78ba-697">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c78ba-698">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-698">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c78ba-699">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-699">Get the Edge Storage Container</span></span>
* <span data-ttu-id="c78ba-700">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-700">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c78ba-701">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-701">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="c78ba-702">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-702">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c78ba-703">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-703">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="c78ba-704">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-704">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="c78ba-705">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="c78ba-705">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="c78ba-706">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-706">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c78ba-707">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-707">Get the Edge Storage Account</span></span>
* <span data-ttu-id="c78ba-708">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-708">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c78ba-709">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-709">Create new Edge Storage Account</span></span>
* <span data-ttu-id="c78ba-710">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-710">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="c78ba-711">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-711">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="c78ba-712">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="c78ba-712">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="c78ba-713">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="c78ba-713">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="c78ba-714">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-714">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="c78ba-715">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="c78ba-715">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-716">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-716">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-717">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-717">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="c78ba-718">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-718">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="c78ba-719">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-719">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="c78ba-720">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="c78ba-720">Az.DevTestLabs</span></span>
* <span data-ttu-id="c78ba-721">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-721">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-722">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-722">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-723">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-723">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-724">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-724">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-725">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-725">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c78ba-726">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c78ba-726">Az.MachineLearning</span></span>
* <span data-ttu-id="c78ba-727">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-727">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="c78ba-728">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c78ba-728">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="c78ba-729">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-729">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="c78ba-730">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c78ba-730">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="c78ba-731">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c78ba-731">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="c78ba-732">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="c78ba-732">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="c78ba-733">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="c78ba-733">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="c78ba-734">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="c78ba-734">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-735">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-735">Az.Network</span></span>
* <span data-ttu-id="c78ba-736">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="c78ba-736">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-737">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-737">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-738">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-738">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="c78ba-739">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-739">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c78ba-740">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-740">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="c78ba-741">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-741">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-742">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-742">Az.Resources</span></span>
* <span data-ttu-id="c78ba-743">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-743">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-744">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-744">Az.Sql</span></span>
* <span data-ttu-id="c78ba-745">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-745">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="c78ba-746">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-746">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="c78ba-747">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="c78ba-747">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="c78ba-748">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-748">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-749">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-749">Az.Storage</span></span>
* <span data-ttu-id="c78ba-750">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-750">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="c78ba-751">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-751">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="c78ba-752">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-752">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="c78ba-753">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-753">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="c78ba-754">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-754">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="c78ba-755">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-755">General</span></span>
* <span data-ttu-id="c78ba-756">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-756">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-757">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-757">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-758">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="c78ba-758">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="c78ba-759">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="c78ba-759">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-760">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-760">Az.Batch</span></span>
* <span data-ttu-id="c78ba-761">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-761">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-762">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-762">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-763">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-763">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-764">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-764">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-765">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-765">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="c78ba-766">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-766">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c78ba-767">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c78ba-767">Az.HealthcareApis</span></span>
* <span data-ttu-id="c78ba-768">例外処理</span><span class="sxs-lookup"><span data-stu-id="c78ba-768">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-769">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-769">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-770">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-770">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="c78ba-771">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="c78ba-771">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="c78ba-772">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-772">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-773">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-774">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-774">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="c78ba-775">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="c78ba-775">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="c78ba-776">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="c78ba-776">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-777">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-777">Az.Network</span></span>
* <span data-ttu-id="c78ba-778">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-778">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-779">Az.Resources</span></span>
* <span data-ttu-id="c78ba-780">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-780">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="c78ba-781">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-781">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-782">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-782">Az.Sql</span></span>
* <span data-ttu-id="c78ba-783">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-783">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-784">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-784">Az.Storage</span></span>
* <span data-ttu-id="c78ba-785">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-785">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="c78ba-786">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="c78ba-786">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="c78ba-787">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c78ba-787">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="c78ba-788">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-788">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="c78ba-789">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="c78ba-789">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="c78ba-790">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-790">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="c78ba-791">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-791">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="c78ba-792">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-792">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="c78ba-793">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-793">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="c78ba-794">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-794">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="c78ba-795">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="c78ba-795">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="c78ba-796">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-796">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="c78ba-797">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="c78ba-797">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="c78ba-798">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-798">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-799">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-799">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-800">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-800">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="c78ba-801">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-801">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-802">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-802">Az.Compute</span></span>
* <span data-ttu-id="c78ba-803">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="c78ba-803">VM Reapply feature</span></span>
    - <span data-ttu-id="c78ba-804">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-804">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="c78ba-805">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="c78ba-805">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="c78ba-806">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="c78ba-806">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="c78ba-807">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-807">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="c78ba-808">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-808">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c78ba-809">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-809">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="c78ba-810">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="c78ba-810">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="c78ba-811">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-811">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="c78ba-812">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-812">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="c78ba-813">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-813">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="c78ba-814">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="c78ba-814">Az.DataBoxEdge</span></span>
* <span data-ttu-id="c78ba-815">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-815">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c78ba-816">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-816">Get the Order</span></span>
* <span data-ttu-id="c78ba-817">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-817">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c78ba-818">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-818">Create new Order</span></span>
* <span data-ttu-id="c78ba-819">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-819">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="c78ba-820">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-820">Remove the Order</span></span>
* <span data-ttu-id="c78ba-821">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-821">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="c78ba-822">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-822">Now creates Local Share</span></span>
* <span data-ttu-id="c78ba-823">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-823">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="c78ba-824">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-824">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="c78ba-825">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-825">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="c78ba-826">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="c78ba-826">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="c78ba-827">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-827">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c78ba-828">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-828">Gets the information about Triggers</span></span>
* <span data-ttu-id="c78ba-829">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-829">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c78ba-830">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-830">Create new Triggers</span></span>
* <span data-ttu-id="c78ba-831">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-831">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="c78ba-832">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-832">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-833">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-833">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-834">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-834">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="c78ba-835">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-835">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-836">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-836">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-837">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-837">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-838">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-838">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-839">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-839">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-840">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-840">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-841">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-841">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="c78ba-842">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-842">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="c78ba-843">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-843">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="c78ba-844">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="c78ba-844">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-845">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-845">Az.Network</span></span>
* <span data-ttu-id="c78ba-846">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-846">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="c78ba-847">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="c78ba-847">Az.PrivateDns</span></span>
* <span data-ttu-id="c78ba-848">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-848">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-849">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-849">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-850">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-850">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="c78ba-851">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="c78ba-851">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="c78ba-852">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-852">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c78ba-853">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78ba-853">Az.RedisCache</span></span>
* <span data-ttu-id="c78ba-854">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-854">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="c78ba-855">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-855">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="c78ba-856">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-856">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-857">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-857">Az.Resources</span></span>
- <span data-ttu-id="c78ba-858">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-858">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="c78ba-859">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-859">Updated create policy definition help example</span></span>
- <span data-ttu-id="c78ba-860">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-860">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="c78ba-861">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-861">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="c78ba-862">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-862">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-863">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-863">Az.Sql</span></span>
* <span data-ttu-id="c78ba-864">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-864">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="c78ba-865">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-865">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="c78ba-866">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-866">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="c78ba-867">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-867">General</span></span>
* <span data-ttu-id="c78ba-868">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-868">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-869">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-869">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-870">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-870">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c78ba-871">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c78ba-871">Az.Advisor</span></span>
* <span data-ttu-id="c78ba-872">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-872">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-873">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-873">Az.Batch</span></span>
* <span data-ttu-id="c78ba-874">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-874">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="c78ba-875">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-875">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="c78ba-876">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-876">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="c78ba-877">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-877">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="c78ba-878">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="c78ba-878">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="c78ba-879">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-879">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="c78ba-880">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-880">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="c78ba-881">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-881">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="c78ba-882">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-882">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="c78ba-883">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-883">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c78ba-884">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-884">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="c78ba-885">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-885">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="c78ba-886">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-886">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="c78ba-887">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-887">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="c78ba-888">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-888">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="c78ba-889">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-889">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="c78ba-890">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-890">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="c78ba-891">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-891">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="c78ba-892">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-892">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="c78ba-893">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-893">This operation is no longer supported.</span></span>
* <span data-ttu-id="c78ba-894">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-894">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c78ba-895">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-895">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="c78ba-896">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-896">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="c78ba-897">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-897">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="c78ba-898">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-898">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="c78ba-899">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-899">New non-verified images are also now returned.</span></span> <span data-ttu-id="c78ba-900">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-900">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="c78ba-901">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-901">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="c78ba-902">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-902">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="c78ba-903">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-903">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="c78ba-904">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-904">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="c78ba-905">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-905">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="c78ba-906">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-906">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="c78ba-907">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-907">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="c78ba-908">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-908">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="c78ba-909">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-909">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-910">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-910">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-911">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-911">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="c78ba-912">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-912">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-913">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-913">Az.Compute</span></span>
* <span data-ttu-id="c78ba-914">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="c78ba-914">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="c78ba-915">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-915">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="c78ba-916">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。 Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile、Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="c78ba-916">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="c78ba-917">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-917">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c78ba-918">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-918">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="c78ba-919">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="c78ba-919">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="c78ba-920">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-920">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="c78ba-921">重大な変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-921">Breaking changes</span></span>
    - <span data-ttu-id="c78ba-922">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-922">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="c78ba-923">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="c78ba-923">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-924">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-924">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-925">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-925">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-926">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-927">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="c78ba-927">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="c78ba-928">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-928">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="c78ba-929">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="c78ba-929">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="c78ba-930">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-930">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="c78ba-931">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-931">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="c78ba-932">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-932">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-933">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-933">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-934">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-934">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-935">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-935">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-936">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-936">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="c78ba-937">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-937">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="c78ba-938">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-938">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="c78ba-939">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-939">Removed five cmdlets:</span></span>
    - <span data-ttu-id="c78ba-940">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c78ba-940">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c78ba-941">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c78ba-941">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c78ba-942">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="c78ba-942">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="c78ba-943">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c78ba-943">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="c78ba-944">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c78ba-944">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="c78ba-945">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-945">Added three cmdlets:</span></span>
    - <span data-ttu-id="c78ba-946">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-946">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c78ba-947">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-947">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="c78ba-948">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-948">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="c78ba-949">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-949">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="c78ba-950">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-950">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="c78ba-951">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-951">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="c78ba-952">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="c78ba-952">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="c78ba-953">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-953">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="c78ba-954">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-954">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="c78ba-955">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-955">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="c78ba-956">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-956">Added some scenario test cases.</span></span>
* <span data-ttu-id="c78ba-957">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="c78ba-957">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-958">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-958">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-959">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="c78ba-959">Breaking changes:</span></span>
    - <span data-ttu-id="c78ba-960">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-960">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c78ba-961">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-961">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c78ba-962">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-962">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c78ba-963">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-963">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c78ba-964">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-964">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="c78ba-965">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-965">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="c78ba-966">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-966">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="c78ba-967">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-967">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="c78ba-968">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-968">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c78ba-969">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-969">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="c78ba-970">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-970">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="c78ba-971">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-971">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-972">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-972">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-973">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-973">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-974">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-974">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="c78ba-975">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-975">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="c78ba-976">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-976">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-977">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-977">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-978">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-978">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-979">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-979">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-980">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-980">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-981">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-981">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-982">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-982">Az.Resources</span></span>
* <span data-ttu-id="c78ba-983">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-983">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-984">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-984">Az.Network</span></span>
* <span data-ttu-id="c78ba-985">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-985">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="c78ba-986">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-986">Updated cmdlet:</span></span>
        - <span data-ttu-id="c78ba-987">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-987">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-988">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-988">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-989">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-989">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-990">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-990">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-991">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-991">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c78ba-992">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c78ba-992">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="c78ba-993">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-993">New cmdlet:</span></span>
        - <span data-ttu-id="c78ba-994">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="c78ba-994">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="c78ba-995">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-995">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="c78ba-996">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-996">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="c78ba-997">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-997">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="c78ba-998">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-998">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="c78ba-999">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-999">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="c78ba-1000">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1000">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="c78ba-1001">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1001">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="c78ba-1002">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-1002">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-1003">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1003">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="c78ba-1004">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-1004">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c78ba-1005">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-1005">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c78ba-1006">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-1006">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="c78ba-1007">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1007">Set-AzVirtualHub</span></span>
* <span data-ttu-id="c78ba-1008">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1008">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="c78ba-1009">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1009">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c78ba-1010">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1010">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c78ba-1011">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1011">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="c78ba-1012">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1012">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="c78ba-1013">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1013">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="c78ba-1014">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1014">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="c78ba-1015">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-1015">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-1016">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1016">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="c78ba-1017">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1017">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c78ba-1018">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1018">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c78ba-1019">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1019">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c78ba-1020">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1020">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c78ba-1021">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1021">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="c78ba-1022">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1022">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="c78ba-1023">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1023">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="c78ba-1024">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-1024">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-1025">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="c78ba-1025">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="c78ba-1026">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="c78ba-1026">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="c78ba-1027">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="c78ba-1027">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="c78ba-1028">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="c78ba-1028">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="c78ba-1029">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1029">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="c78ba-1030">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-1030">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="c78ba-1031">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1031">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c78ba-1032">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1032">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="c78ba-1033">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1033">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="c78ba-1034">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1034">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="c78ba-1035">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1035">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="c78ba-1036">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1036">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="c78ba-1037">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1037">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="c78ba-1038">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1038">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="c78ba-1039">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1039">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="c78ba-1040">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1040">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="c78ba-1041">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1041">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="c78ba-1042">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-1042">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-1043">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1043">New-AzIpGroup</span></span>
        - <span data-ttu-id="c78ba-1044">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1044">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="c78ba-1045">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1045">Get-AzIpGroup</span></span>
        - <span data-ttu-id="c78ba-1046">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1046">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-1047">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1047">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-1048">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1048">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1049">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1049">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1050">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1050">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="c78ba-1051">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1051">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="c78ba-1052">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1052">Removed deprecated aliases:</span></span>
* <span data-ttu-id="c78ba-1053">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1053">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="c78ba-1054">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1054">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="c78ba-1055">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1055">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c78ba-1056">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1056">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="c78ba-1057">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1057">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="c78ba-1058">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1058">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1059">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1059">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1060">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1060">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="c78ba-1061">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1061">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c78ba-1062">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1062">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c78ba-1063">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1063">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="c78ba-1064">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c78ba-1064">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="c78ba-1065">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c78ba-1065">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="c78ba-1066">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1066">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="c78ba-1067">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-1067">General</span></span>
* <span data-ttu-id="c78ba-1068">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-1068">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1069">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1069">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1070">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1070">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-1071">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-1071">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-1072">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1072">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="c78ba-1073">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="c78ba-1073">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1074">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1074">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1075">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1075">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-1076">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-1076">Az.Batch</span></span>
* <span data-ttu-id="c78ba-1077">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1077">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1078">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1078">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1079">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1079">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="c78ba-1080">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1080">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="c78ba-1081">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1081">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="c78ba-1082">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1082">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1083">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1083">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1084">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1084">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="c78ba-1085">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1085">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="c78ba-1086">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1086">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-1087">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-1087">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-1088">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1088">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="c78ba-1089">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="c78ba-1089">Az.HealthcareApis</span></span>
* <span data-ttu-id="c78ba-1090">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1090">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="c78ba-1091">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1091">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="c78ba-1092">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1092">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="c78ba-1093">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1093">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-1094">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1094">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-1095">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="c78ba-1095">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="c78ba-1096">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="c78ba-1096">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1097">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1097">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-1098">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="c78ba-1098">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="c78ba-1099">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1099">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="c78ba-1100">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="c78ba-1100">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="c78ba-1101">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1101">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1102">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1102">Az.Network</span></span>
* <span data-ttu-id="c78ba-1103">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1103">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="c78ba-1104">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1104">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="c78ba-1105">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-1105">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-1106">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1106">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="c78ba-1107">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1107">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c78ba-1108">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1108">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="c78ba-1109">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1109">Updated cmdlets:</span></span>
        - <span data-ttu-id="c78ba-1110">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1110">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c78ba-1111">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1111">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c78ba-1112">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1112">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c78ba-1113">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1113">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="c78ba-1114">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="c78ba-1114">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="c78ba-1115">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1115">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="c78ba-1116">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1116">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c78ba-1117">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78ba-1117">Az.RedisCache</span></span>
* <span data-ttu-id="c78ba-1118">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1118">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1119">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1119">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1120">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1120">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1121">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1121">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1122">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1122">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="c78ba-1123">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1123">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c78ba-1124">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="c78ba-1124">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="c78ba-1125">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1125">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="c78ba-1126">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1126">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c78ba-1127">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c78ba-1127">Az.StorageSync</span></span>
* <span data-ttu-id="c78ba-1128">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1128">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1129">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1129">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1130">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1130">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="c78ba-1131">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1131">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-1132">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-1132">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-1133">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1133">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="c78ba-1134">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1134">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="c78ba-1135">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1135">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1136">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1136">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1137">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1137">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="c78ba-1138">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1138">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="c78ba-1139">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1139">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1140">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1141">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1141">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="c78ba-1142">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1142">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c78ba-1143">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1143">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="c78ba-1144">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1144">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="c78ba-1145">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1145">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="c78ba-1146">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1146">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="c78ba-1147">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1147">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="c78ba-1148">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1148">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="c78ba-1149">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1149">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1150">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1150">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1151">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1151">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="c78ba-1152">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1152">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-1153">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-1153">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-1154">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1154">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-1155">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1155">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-1156">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1156">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="c78ba-1157">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1157">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="c78ba-1158">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1158">New cmdlets are:</span></span>
    - <span data-ttu-id="c78ba-1159">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c78ba-1159">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c78ba-1160">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c78ba-1160">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c78ba-1161">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c78ba-1161">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="c78ba-1162">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="c78ba-1162">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1163">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1163">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-1164">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="c78ba-1164">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="c78ba-1165">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1165">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="c78ba-1166">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1166">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="c78ba-1167">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1167">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="c78ba-1168">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1168">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="c78ba-1169">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1169">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="c78ba-1170">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1170">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="c78ba-1171">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1171">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="c78ba-1172">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1172">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c78ba-1173">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1173">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="c78ba-1174">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1174">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="c78ba-1175">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1175">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="c78ba-1176">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1176">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="c78ba-1177">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1177">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="c78ba-1178">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1178">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="c78ba-1179">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="c78ba-1179">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="c78ba-1180">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1180">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="c78ba-1181">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1181">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="c78ba-1182">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1182">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="c78ba-1183">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1183">Overall improved help files</span></span>
* <span data-ttu-id="c78ba-1184">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1184">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1185">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1185">Az.Network</span></span>
* <span data-ttu-id="c78ba-1186">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1186">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="c78ba-1187">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1187">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="c78ba-1188">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1188">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="c78ba-1189">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1189">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="c78ba-1190">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1190">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="c78ba-1191">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1191">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="c78ba-1192">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1192">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="c78ba-1193">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1193">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="c78ba-1194">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1194">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="c78ba-1195">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1195">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="c78ba-1196">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1196">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="c78ba-1197">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1197">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="c78ba-1198">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1198">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1199">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="c78ba-1199">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="c78ba-1200">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1200">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="c78ba-1201">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1201">Updated cmdlet:</span></span>
        - <span data-ttu-id="c78ba-1202">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c78ba-1202">New-VpnSite</span></span>
        - <span data-ttu-id="c78ba-1203">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="c78ba-1203">Update-VpnSite</span></span>
        - <span data-ttu-id="c78ba-1204">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1204">New-VpnConnection</span></span>
        - <span data-ttu-id="c78ba-1205">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1205">Update-VpnConnection</span></span>
* <span data-ttu-id="c78ba-1206">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1206">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1207">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1208">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1208">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="c78ba-1209">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1209">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1210">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1210">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1211">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1211">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-1212">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1212">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-1213">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1213">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="c78ba-1214">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1214">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="c78ba-1215">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c78ba-1215">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c78ba-1216">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c78ba-1216">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c78ba-1217">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c78ba-1217">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c78ba-1218">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1218">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="c78ba-1219">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c78ba-1219">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c78ba-1220">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c78ba-1220">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c78ba-1221">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c78ba-1221">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c78ba-1222">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c78ba-1222">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c78ba-1223">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1223">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="c78ba-1224">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="c78ba-1224">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="c78ba-1225">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="c78ba-1225">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="c78ba-1226">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="c78ba-1226">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="c78ba-1227">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="c78ba-1227">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="c78ba-1228">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1228">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c78ba-1229">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c78ba-1229">Az.SignalR</span></span>
* <span data-ttu-id="c78ba-1230">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1230">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1231">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1231">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1232">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1232">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="c78ba-1233">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1233">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="c78ba-1234">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1234">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="c78ba-1235">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1235">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="c78ba-1236">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1236">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1237">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1237">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1238">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1238">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="c78ba-1239">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1239">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="c78ba-1240">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1240">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="c78ba-1241">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1241">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="c78ba-1242">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1242">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="c78ba-1243">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1243">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="c78ba-1244">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1244">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="c78ba-1245">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-1245">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c78ba-1246">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-1246">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c78ba-1247">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-1247">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="c78ba-1248">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="c78ba-1248">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1249">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1250">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1250">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="c78ba-1251">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1251">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="c78ba-1252">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1252">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="c78ba-1253">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1253">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="c78ba-1254">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-1254">General</span></span>
* <span data-ttu-id="c78ba-1255">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1255">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1256">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1256">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1257">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1257">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="c78ba-1258">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c78ba-1258">Az.Aks</span></span>
* <span data-ttu-id="c78ba-1259">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1259">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="c78ba-1260">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="c78ba-1260">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-1261">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-1261">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-1262">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="c78ba-1262">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="c78ba-1263">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1263">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="c78ba-1264">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1264">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="c78ba-1265">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="c78ba-1265">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="c78ba-1266">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1266">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-1267">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-1267">Az.Batch</span></span>
* <span data-ttu-id="c78ba-1268">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1268">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-1269">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-1269">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-1270">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1270">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1271">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1271">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1272">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1272">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="c78ba-1273">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1273">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="c78ba-1274">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1274">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="c78ba-1275">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1275">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="c78ba-1276">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="c78ba-1276">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="c78ba-1277">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1277">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="c78ba-1278">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1278">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="c78ba-1279">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1279">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1280">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1280">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1281">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1281">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="c78ba-1282">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1282">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="c78ba-1283">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1283">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="c78ba-1284">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1284">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-1285">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-1285">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-1286">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1286">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-1287">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1287">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-1288">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="c78ba-1288">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="c78ba-1289">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="c78ba-1289">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="c78ba-1290">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1290">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="c78ba-1291">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="c78ba-1291">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="c78ba-1292">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c78ba-1292">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c78ba-1293">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1293">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1294">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1294">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-1295">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1295">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1296">Az.Network</span></span>
* <span data-ttu-id="c78ba-1297">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1297">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="c78ba-1298">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1298">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="c78ba-1299">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1299">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="c78ba-1300">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1300">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="c78ba-1301">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1301">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="c78ba-1302">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1302">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="c78ba-1303">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1303">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-1304">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1304">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-1305">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1305">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="c78ba-1306">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1306">Added example</span></span>
    - <span data-ttu-id="c78ba-1307">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1307">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="c78ba-1308">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1308">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="c78ba-1309">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1309">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1310">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1310">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1311">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1311">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1312">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1312">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1313">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1313">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="c78ba-1314">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1314">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="c78ba-1315">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-1315">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="c78ba-1316">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1316">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-1317">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-1317">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-1318">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="c78ba-1318">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="c78ba-1319">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="c78ba-1319">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="c78ba-1320">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1320">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-1321">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1321">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-1322">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1322">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="c78ba-1323">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1323">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="c78ba-1324">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="c78ba-1324">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="c78ba-1325">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1325">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="c78ba-1326">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="c78ba-1326">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="c78ba-1327">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1327">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1328">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1328">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1329">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1329">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1330">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1330">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1331">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1331">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="c78ba-1332">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1332">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="c78ba-1333">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1333">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="c78ba-1334">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1334">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="c78ba-1335">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-1335">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="c78ba-1336">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1336">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1337">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1337">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1338">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1338">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="c78ba-1339">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1339">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1340">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1340">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1341">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1341">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="c78ba-1342">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1342">Az.ApplicationInsights</span></span>
* <span data-ttu-id="c78ba-1343">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1343">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1344">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1344">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1345">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1345">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-1346">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1346">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-1347">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1347">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1348">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1349">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1349">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c78ba-1350">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c78ba-1350">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c78ba-1351">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1351">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="c78ba-1352">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="c78ba-1352">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1353">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1353">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1354">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1354">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="c78ba-1355">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1355">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-1356">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1356">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-1357">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c78ba-1357">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c78ba-1358">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1358">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-1359">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-1359">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-1360">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1360">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c78ba-1361">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78ba-1361">Az.LogicApp</span></span>
* <span data-ttu-id="c78ba-1362">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1362">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="c78ba-1363">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1363">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="c78ba-1364">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1364">Az.ManagedServices</span></span>
* <span data-ttu-id="c78ba-1365">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1365">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1366">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1366">Az.Network</span></span>
* <span data-ttu-id="c78ba-1367">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1367">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="c78ba-1368">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1368">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1369">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c78ba-1369">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c78ba-1370">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1370">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c78ba-1371">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1371">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-1372">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1372">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-1373">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1373">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-1374">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1374">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="c78ba-1375">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="c78ba-1375">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="c78ba-1376">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1376">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="c78ba-1377">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="c78ba-1377">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="c78ba-1378">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1378">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="c78ba-1379">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1379">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="c78ba-1380">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1380">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="c78ba-1381">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1381">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="c78ba-1382">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1382">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="c78ba-1383">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1383">Updated cmdlets</span></span>
        - <span data-ttu-id="c78ba-1384">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1384">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c78ba-1385">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1385">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="c78ba-1386">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1386">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="c78ba-1387">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1387">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="c78ba-1388">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1388">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="c78ba-1389">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1389">Updated cmdlet:</span></span>
        - <span data-ttu-id="c78ba-1390">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1390">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c78ba-1391">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1391">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="c78ba-1392">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1392">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="c78ba-1393">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-1393">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="c78ba-1394">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1394">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="c78ba-1395">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1395">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-1396">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1396">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-1397">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1397">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="c78ba-1398">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1398">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1399">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1399">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1400">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1400">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c78ba-1401">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1401">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="c78ba-1402">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1402">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="c78ba-1403">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1403">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="c78ba-1404">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1404">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="c78ba-1405">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1405">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c78ba-1406">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1406">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="c78ba-1407">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1407">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="c78ba-1408">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1408">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="c78ba-1409">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1409">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1410">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1410">Az.Resources</span></span>
- <span data-ttu-id="c78ba-1411">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1411">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="c78ba-1412">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1412">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-1413">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-1413">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-1414">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="c78ba-1414">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="c78ba-1415">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1415">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1416">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1416">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1417">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1417">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="c78ba-1418">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1418">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="c78ba-1419">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1419">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1420">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1420">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1421">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1421">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c78ba-1422">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c78ba-1422">Az.StorageSync</span></span>
* <span data-ttu-id="c78ba-1423">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1423">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="c78ba-1424">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1424">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1425">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1425">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1426">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1426">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="c78ba-1427">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1427">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="c78ba-1428">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1428">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="c78ba-1429">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1429">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1430">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1430">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1431">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1431">Add support for profile cmdlets</span></span>
* <span data-ttu-id="c78ba-1432">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1432">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="c78ba-1433">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1433">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="c78ba-1434">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1434">Az.Advisor</span></span>
* <span data-ttu-id="c78ba-1435">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-1435">GA release of Az.Advisor</span></span>
* <span data-ttu-id="c78ba-1436">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1436">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-1437">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-1437">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-1438">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="c78ba-1438">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="c78ba-1439">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="c78ba-1439">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="c78ba-1440">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1440">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="c78ba-1441">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1441">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="c78ba-1442">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1442">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="c78ba-1443">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="c78ba-1443">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="c78ba-1444">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1444">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1445">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1445">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1446">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1446">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1447">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1447">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1448">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1448">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1449">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1449">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1450">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-1450">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c78ba-1451">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78ba-1451">Az.EventGrid</span></span>
* <span data-ttu-id="c78ba-1452">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1452">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-1453">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1453">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-1454">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1454">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1455">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1455">Az.Network</span></span>
* <span data-ttu-id="c78ba-1456">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1456">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="c78ba-1457">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1457">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-1458">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1458">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-1459">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1459">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="c78ba-1460">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="c78ba-1460">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-1461">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1461">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-1462">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1462">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1463">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1463">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1464">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1464">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1465">Az.Resources</span></span>
    - <span data-ttu-id="c78ba-1466">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1466">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="c78ba-1467">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1467">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="c78ba-1468">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1468">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="c78ba-1469">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1469">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-1470">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-1470">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-1471">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="c78ba-1471">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1472">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1473">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1473">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="c78ba-1474">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1474">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="c78ba-1475">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1475">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c78ba-1476">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1476">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c78ba-1477">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1477">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="c78ba-1478">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1478">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c78ba-1479">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1479">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="c78ba-1480">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="c78ba-1480">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="c78ba-1481">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1481">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1482">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1482">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1483">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1483">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="c78ba-1484">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c78ba-1484">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="c78ba-1485">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1485">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="c78ba-1486">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="c78ba-1486">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="c78ba-1487">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1487">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="c78ba-1488">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1488">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="c78ba-1489">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1489">Set-AzStorageAccount</span></span>
* <span data-ttu-id="c78ba-1490">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1490">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="c78ba-1491">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c78ba-1491">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="c78ba-1492">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="c78ba-1492">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="c78ba-1493">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="c78ba-1493">Az.StorageSync</span></span>
* <span data-ttu-id="c78ba-1494">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1494">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="c78ba-1495">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1495">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1496">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1496">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1497">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1497">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="c78ba-1498">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="c78ba-1498">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="c78ba-1499">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1499">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="c78ba-1500">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="c78ba-1500">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="c78ba-1501">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="c78ba-1501">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1502">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1502">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1503">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1503">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="c78ba-1504">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1504">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="c78ba-1505">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c78ba-1505">Az.Dns</span></span>
* <span data-ttu-id="c78ba-1506">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1506">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c78ba-1507">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78ba-1507">Az.EventGrid</span></span>
* <span data-ttu-id="c78ba-1508">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1508">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="c78ba-1509">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1509">New cmdlets:</span></span>
    - <span data-ttu-id="c78ba-1510">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c78ba-1510">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c78ba-1511">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1511">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c78ba-1512">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c78ba-1512">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c78ba-1513">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1513">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="c78ba-1514">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="c78ba-1514">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="c78ba-1515">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1515">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c78ba-1516">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-1516">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c78ba-1517">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1517">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="c78ba-1518">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-1518">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="c78ba-1519">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1519">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="c78ba-1520">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1520">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c78ba-1521">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1521">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="c78ba-1522">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="c78ba-1522">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="c78ba-1523">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1523">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="c78ba-1524">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1524">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="c78ba-1525">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1525">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="c78ba-1526">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1526">Updated cmdlets:</span></span>
    - <span data-ttu-id="c78ba-1527">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1527">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="c78ba-1528">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1528">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c78ba-1529">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1529">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="c78ba-1530">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1530">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="c78ba-1531">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1531">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="c78ba-1532">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="c78ba-1532">Event subscription expiration date,</span></span>
            - <span data-ttu-id="c78ba-1533">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="c78ba-1533">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="c78ba-1534">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1534">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="c78ba-1535">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1535">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="c78ba-1536">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1536">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="c78ba-1537">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1537">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="c78ba-1538">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="c78ba-1538">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="c78ba-1539">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1539">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="c78ba-1540">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1540">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-1541">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1541">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-1542">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="c78ba-1542">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="c78ba-1543">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1543">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="c78ba-1544">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="c78ba-1544">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="c78ba-1545">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1545">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1546">Az.Network</span></span>
* <span data-ttu-id="c78ba-1547">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1547">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="c78ba-1548">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1548">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1549">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="c78ba-1549">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="c78ba-1550">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1550">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="c78ba-1551">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1551">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1552">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="c78ba-1552">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="c78ba-1553">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1553">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="c78ba-1554">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1554">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1555">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1555">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c78ba-1556">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1556">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c78ba-1557">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="c78ba-1557">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="c78ba-1558">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1558">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="c78ba-1559">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1559">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="c78ba-1560">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1560">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="c78ba-1561">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1561">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1562">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c78ba-1562">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c78ba-1563">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c78ba-1563">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c78ba-1564">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="c78ba-1564">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="c78ba-1565">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1565">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="c78ba-1566">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="c78ba-1566">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="c78ba-1567">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1567">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="c78ba-1568">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1568">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="c78ba-1569">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1569">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="c78ba-1570">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1570">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="c78ba-1571">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1571">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="c78ba-1572">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1572">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="c78ba-1573">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1573">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="c78ba-1574">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1574">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="c78ba-1575">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1575">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="c78ba-1576">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1576">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="c78ba-1577">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1577">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="c78ba-1578">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1578">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="c78ba-1579">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1579">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="c78ba-1580">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1580">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="c78ba-1581">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1581">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="c78ba-1582">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1582">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="c78ba-1583">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1583">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="c78ba-1584">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1584">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="c78ba-1585">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1585">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="c78ba-1586">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1586">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c78ba-1587">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1587">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="c78ba-1588">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1588">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-1589">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1589">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-1590">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1590">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1591">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1591">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1592">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1592">Support for additional Template Export options</span></span>
    - <span data-ttu-id="c78ba-1593">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1593">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c78ba-1594">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1594">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="c78ba-1595">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1595">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-1596">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1596">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-1597">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1597">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1598">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1599">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1599">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="c78ba-1600">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1600">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="c78ba-1601">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1601">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="c78ba-1602">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-1602">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c78ba-1603">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-1603">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c78ba-1604">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="c78ba-1604">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="c78ba-1605">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c78ba-1605">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="c78ba-1606">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="c78ba-1606">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1607">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1607">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1608">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1608">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="c78ba-1609">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1609">New-AzStorageAccount</span></span>
* <span data-ttu-id="c78ba-1610">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1610">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="c78ba-1611">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1611">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1612">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1612">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1613">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1613">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="c78ba-1614">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1614">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="c78ba-1615">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1615">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="c78ba-1616">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-1616">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-1617">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1617">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1618">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1618">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1619">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1619">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="c78ba-1620">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="c78ba-1620">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-1621">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1621">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-1622">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1622">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="c78ba-1623">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1623">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1624">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1624">Az.Network</span></span>
* <span data-ttu-id="c78ba-1625">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1625">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="c78ba-1626">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1626">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-1627">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1627">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-1628">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1628">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1629">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1629">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1630">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1630">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-1631">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-1631">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-1632">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1632">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-1633">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1633">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-1634">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1634">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="c78ba-1635">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1635">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1636">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1636">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1637">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1637">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="c78ba-1638">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="c78ba-1638">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="c78ba-1639">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1639">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="c78ba-1640">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1640">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1641">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1641">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1642">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1642">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="c78ba-1643">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1643">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="c78ba-1644">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-1644">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-1645">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1645">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="c78ba-1646">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1646">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="c78ba-1647">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1647">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="c78ba-1648">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1648">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="c78ba-1649">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1649">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="c78ba-1650">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1650">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="c78ba-1651">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1651">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="c78ba-1652">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1652">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="c78ba-1653">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1653">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="c78ba-1654">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1654">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="c78ba-1655">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1655">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="c78ba-1656">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1656">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="c78ba-1657">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1657">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="c78ba-1658">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1658">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="c78ba-1659">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1659">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="c78ba-1660">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1660">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="c78ba-1661">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1661">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="c78ba-1662">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="c78ba-1662">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="c78ba-1663">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1663">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="c78ba-1664">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="c78ba-1664">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="c78ba-1665">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1665">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="c78ba-1666">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1666">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="c78ba-1667">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1667">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="c78ba-1668">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1668">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="c78ba-1669">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1669">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="c78ba-1670">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1670">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="c78ba-1671">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1671">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="c78ba-1672">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1672">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="c78ba-1673">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1673">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="c78ba-1674">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1674">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="c78ba-1675">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1675">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="c78ba-1676">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="c78ba-1676">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="c78ba-1677">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1677">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="c78ba-1678">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1678">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c78ba-1679">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="c78ba-1679">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="c78ba-1680">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1680">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="c78ba-1681">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1681">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="c78ba-1682">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1682">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="c78ba-1683">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1683">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="c78ba-1684">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1684">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c78ba-1685">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1685">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c78ba-1686">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1686">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c78ba-1687">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1687">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="c78ba-1688">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1688">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c78ba-1689">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1689">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="c78ba-1690">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1690">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="c78ba-1691">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1691">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="c78ba-1692">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1692">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="c78ba-1693">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1693">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="c78ba-1694">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1694">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="c78ba-1695">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1695">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="c78ba-1696">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1696">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="c78ba-1697">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1697">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="c78ba-1698">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1698">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="c78ba-1699">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1699">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="c78ba-1700">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1700">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="c78ba-1701">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1701">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c78ba-1702">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1702">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c78ba-1703">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1703">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c78ba-1704">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1704">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c78ba-1705">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1705">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="c78ba-1706">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1706">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="c78ba-1707">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="c78ba-1707">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="c78ba-1708">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1708">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="c78ba-1709">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1709">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="c78ba-1710">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1710">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="c78ba-1711">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="c78ba-1711">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="c78ba-1712">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1712">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="c78ba-1713">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="c78ba-1713">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="c78ba-1714">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1714">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="c78ba-1715">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="c78ba-1715">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="c78ba-1716">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1716">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="c78ba-1717">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1717">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="c78ba-1718">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-1718">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="c78ba-1719">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1719">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="c78ba-1720">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1720">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="c78ba-1721">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="c78ba-1721">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1722">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1722">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1723">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1723">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="c78ba-1724">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="c78ba-1724">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="c78ba-1725">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="c78ba-1725">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="c78ba-1726">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1726">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="c78ba-1727">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="c78ba-1727">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="c78ba-1728">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1728">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="c78ba-1729">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1729">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1730">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1730">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1731">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1731">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="c78ba-1732">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1732">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-1733">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-1733">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-1734">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1734">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1735">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1735">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-1736">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1736">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1737">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1737">Az.Network</span></span>
* <span data-ttu-id="c78ba-1738">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1738">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="c78ba-1739">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="c78ba-1739">Updated cmdlet:</span></span>
        - <span data-ttu-id="c78ba-1740">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-1740">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="c78ba-1741">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1741">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1742">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1742">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1743">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1743">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1744">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1744">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1745">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1745">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="c78ba-1746">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1746">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1747">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1747">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1748">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1748">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-1749">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1749">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-1750">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1750">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="c78ba-1751">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1751">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1752">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1752">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1753">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1753">Proximity placement group feature.</span></span>
    - <span data-ttu-id="c78ba-1754">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1754">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="c78ba-1755">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-1755">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="c78ba-1756">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1756">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="c78ba-1757">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1757">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="c78ba-1758">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1758">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="c78ba-1759">重大な変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-1759">Breaking changes</span></span>
    - <span data-ttu-id="c78ba-1760">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1760">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="c78ba-1761">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1761">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c78ba-1762">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c78ba-1762">Az.DeploymentManager</span></span>
* <span data-ttu-id="c78ba-1763">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-1763">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="c78ba-1764">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c78ba-1764">Az.Dns</span></span>
* <span data-ttu-id="c78ba-1765">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="c78ba-1765">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="c78ba-1766">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1766">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="c78ba-1767">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1767">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-1768">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1768">Az.FrontDoor</span></span>
* <span data-ttu-id="c78ba-1769">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-1769">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="c78ba-1770">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1770">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-1771">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-1771">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-1772">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1772">Removed two cmdlets:</span></span>
    - <span data-ttu-id="c78ba-1773">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c78ba-1773">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="c78ba-1774">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c78ba-1774">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c78ba-1775">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1775">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c78ba-1776">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1776">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="c78ba-1777">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1777">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="c78ba-1778">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1778">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1779">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1779">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-1780">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1780">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="c78ba-1781">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="c78ba-1781">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="c78ba-1782">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="c78ba-1782">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="c78ba-1783">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="c78ba-1783">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="c78ba-1784">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1784">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="c78ba-1785">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="c78ba-1785">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="c78ba-1786">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="c78ba-1786">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="c78ba-1787">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1787">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c78ba-1788">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1788">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c78ba-1789">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1789">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c78ba-1790">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1790">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c78ba-1791">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1791">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c78ba-1792">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="c78ba-1792">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="c78ba-1793">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1793">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1794">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1794">Az.Network</span></span>
* <span data-ttu-id="c78ba-1795">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1795">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="c78ba-1796">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1796">New cmdlets</span></span>
        - <span data-ttu-id="c78ba-1797">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c78ba-1797">New-AzNatGateway</span></span>
        - <span data-ttu-id="c78ba-1798">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c78ba-1798">Get-AzNatGateway</span></span>
        - <span data-ttu-id="c78ba-1799">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c78ba-1799">Set-AzNatGateway</span></span>
        - <span data-ttu-id="c78ba-1800">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c78ba-1800">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="c78ba-1801">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1801">Updated cmdlets</span></span>
        - <span data-ttu-id="c78ba-1802">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c78ba-1802">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="c78ba-1803">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c78ba-1803">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="c78ba-1804">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1804">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="c78ba-1805">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1805">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="c78ba-1806">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1806">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-1807">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1807">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-1808">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1808">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="c78ba-1809">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1809">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="c78ba-1810">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1810">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1811">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1811">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1812">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1812">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="c78ba-1813">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1813">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="c78ba-1814">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1814">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="c78ba-1815">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1815">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="c78ba-1816">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1816">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="c78ba-1817">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1817">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="c78ba-1818">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c78ba-1818">Az.Relay</span></span>
* <span data-ttu-id="c78ba-1819">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1819">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-1820">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-1820">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-1821">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1821">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1822">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1822">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1823">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1823">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="c78ba-1824">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1824">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="c78ba-1825">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1825">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="c78ba-1826">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1826">New-AzStorageAccount</span></span>
* <span data-ttu-id="c78ba-1827">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="c78ba-1827">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="c78ba-1828">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1828">New-AzStorageAccount</span></span>
    - <span data-ttu-id="c78ba-1829">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1829">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="c78ba-1830">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c78ba-1830">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1831">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1831">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1832">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-1832">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="c78ba-1833">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1833">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="c78ba-1834">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1834">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-1835">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-1835">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-1836">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="c78ba-1836">General availability of `Az` module</span></span>
* <span data-ttu-id="c78ba-1837">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c78ba-1837">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c78ba-1838">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c78ba-1838">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c78ba-1839">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1839">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c78ba-1840">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1840">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c78ba-1841">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1841">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c78ba-1842">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1842">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1843">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1843">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1844">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-1844">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c78ba-1845">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-1845">Az.Batch</span></span>
* <span data-ttu-id="c78ba-1846">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1846">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-1847">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-1847">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-1848">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1848">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-1849">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1849">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-1850">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1850">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1851">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1852">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1852">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="c78ba-1853">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1853">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1854">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1854">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1855">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1855">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1856">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1856">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-1857">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-1858">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c78ba-1859">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78ba-1859">Az.EventGrid</span></span>
* <span data-ttu-id="c78ba-1860">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1860">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-1861">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1861">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-1862">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1862">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="c78ba-1863">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c78ba-1863">Az.HDInsight</span></span>
* <span data-ttu-id="c78ba-1864">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1864">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-1865">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-1865">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-1866">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1866">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-1867">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-1867">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-1868">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1868">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1869">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1869">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c78ba-1870">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c78ba-1870">Az.MachineLearning</span></span>
* <span data-ttu-id="c78ba-1871">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1871">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="c78ba-1872">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c78ba-1872">Az.Media</span></span>
* <span data-ttu-id="c78ba-1873">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1873">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-1874">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-1874">Az.Monitor</span></span>
  * <span data-ttu-id="c78ba-1875">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1875">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="c78ba-1876">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="c78ba-1876">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="c78ba-1877">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="c78ba-1877">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="c78ba-1878">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c78ba-1878">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c78ba-1879">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c78ba-1879">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c78ba-1880">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c78ba-1880">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="c78ba-1881">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1881">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1882">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1882">Az.Network</span></span>
* <span data-ttu-id="c78ba-1883">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1883">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1884">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1884">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="c78ba-1885">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c78ba-1885">Az.NotificationHubs</span></span>
* <span data-ttu-id="c78ba-1886">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1886">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-1887">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-1887">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-1888">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1888">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c78ba-1889">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c78ba-1889">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c78ba-1890">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1891">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1891">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1892">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1892">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1893">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1893">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="c78ba-1894">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1894">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="c78ba-1895">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1895">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c78ba-1896">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78ba-1896">Az.RedisCache</span></span>
* <span data-ttu-id="c78ba-1897">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1897">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1898">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1898">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1899">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1899">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1900">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1900">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1901">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="c78ba-1901">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="c78ba-1902">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1902">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1903">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1903">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="c78ba-1904">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1904">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="c78ba-1905">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1905">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="c78ba-1906">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1906">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="c78ba-1907">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1907">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1908">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1908">Az.Websites</span></span>
* <span data-ttu-id="c78ba-1909">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-1909">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="c78ba-1910">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c78ba-1911">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1911">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="c78ba-1912">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1912">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="c78ba-1913">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1913">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-1914">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-1914">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-1915">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="c78ba-1915">General availability of `Az` module</span></span>
* <span data-ttu-id="c78ba-1916">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c78ba-1916">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c78ba-1917">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c78ba-1917">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c78ba-1918">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1918">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c78ba-1919">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1919">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c78ba-1920">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1920">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c78ba-1921">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1921">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c78ba-1922">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-1922">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-1923">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1923">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c78ba-1924">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1924">Az.AnalysisServices</span></span>
* <span data-ttu-id="c78ba-1925">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="c78ba-1925">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="c78ba-1926">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1926">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1927">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1927">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1928">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1928">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="c78ba-1929">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1929">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="c78ba-1930">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1930">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1931">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1931">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1932">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1932">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c78ba-1933">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1933">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="c78ba-1934">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-1934">Az.ContainerInstance</span></span>
* <span data-ttu-id="c78ba-1935">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1935">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-1936">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-1936">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-1937">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1937">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="c78ba-1938">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1938">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1939">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1939">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1940">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1940">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="c78ba-1941">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1941">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c78ba-1942">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1942">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="c78ba-1943">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c78ba-1943">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="c78ba-1944">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1944">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="c78ba-1945">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="c78ba-1945">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1946">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1946">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1947">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1947">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1948">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1948">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1949">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-1949">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="c78ba-1950">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c78ba-1950">New-AzStorageContext</span></span>
* <span data-ttu-id="c78ba-1951">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1951">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="c78ba-1952">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c78ba-1952">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c78ba-1953">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c78ba-1953">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c78ba-1954">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1954">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="c78ba-1955">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1955">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="c78ba-1956">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1956">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="c78ba-1957">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1957">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c78ba-1958">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1958">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c78ba-1959">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1959">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="c78ba-1960">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c78ba-1960">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="c78ba-1961">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-1961">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c78ba-1962">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="c78ba-1962">Highlights since the last major release</span></span>
* <span data-ttu-id="c78ba-1963">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="c78ba-1963">General availability of `Az` module</span></span>
* <span data-ttu-id="c78ba-1964">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="c78ba-1964">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c78ba-1965">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="c78ba-1965">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c78ba-1966">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1966">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c78ba-1967">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1967">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c78ba-1968">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-1968">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c78ba-1969">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-1969">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-1970">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-1970">Az.Automation</span></span>
* <span data-ttu-id="c78ba-1971">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1971">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="c78ba-1972">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="c78ba-1972">Dynamic grouping</span></span>
    * <span data-ttu-id="c78ba-1973">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="c78ba-1973">Pre-Post script</span></span>
    * <span data-ttu-id="c78ba-1974">再起動設定</span><span class="sxs-lookup"><span data-stu-id="c78ba-1974">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-1975">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-1975">Az.Compute</span></span>
* <span data-ttu-id="c78ba-1976">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1976">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="c78ba-1977">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1977">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-1978">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-1978">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-1979">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1979">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-1980">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-1980">Az.Network</span></span>
* <span data-ttu-id="c78ba-1981">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1981">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="c78ba-1982">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1982">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-1983">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-1983">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-1984">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1984">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="c78ba-1985">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-1985">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-1986">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-1986">Az.Resources</span></span>
* <span data-ttu-id="c78ba-1987">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-1987">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="c78ba-1988">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-1988">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-1989">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-1989">Az.Sql</span></span>
* <span data-ttu-id="c78ba-1990">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-1990">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-1991">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-1991">Az.Storage</span></span>
* <span data-ttu-id="c78ba-1992">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-1992">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="c78ba-1993">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1993">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c78ba-1994">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1994">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c78ba-1995">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c78ba-1995">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c78ba-1996">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="c78ba-1996">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="c78ba-1997">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="c78ba-1997">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="c78ba-1998">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-1998">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-1999">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-1999">Az.Websites</span></span>
* <span data-ttu-id="c78ba-2000">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2000">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="c78ba-2001">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2001">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-2002">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2002">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-2003">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2003">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="c78ba-2004">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2004">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-2005">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-2005">Az.Automation</span></span>
* <span data-ttu-id="c78ba-2006">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2006">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="c78ba-2007">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2007">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="c78ba-2008">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2008">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-2009">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-2009">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-2010">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2010">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2011">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2011">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2012">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2012">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-2013">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-2013">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-2014">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2014">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c78ba-2015">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78ba-2015">Az.LogicApp</span></span>
* <span data-ttu-id="c78ba-2016">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2016">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2017">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2017">Az.Network</span></span>
* <span data-ttu-id="c78ba-2018">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2018">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-2019">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2019">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-2020">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2020">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="c78ba-2021">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2021">SDK Update</span></span>
* <span data-ttu-id="c78ba-2022">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2022">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="c78ba-2023">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2023">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2024">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2024">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2025">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2025">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="c78ba-2026">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="c78ba-2026">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="c78ba-2027">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2027">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="c78ba-2028">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="c78ba-2028">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="c78ba-2029">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2029">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="c78ba-2030">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="c78ba-2030">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2031">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2031">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2032">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2032">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="c78ba-2033">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2033">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-2034">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2034">Az.Storage</span></span>
* <span data-ttu-id="c78ba-2035">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2035">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="c78ba-2036">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2036">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="c78ba-2037">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2037">Az.AnalysisServices</span></span>
* <span data-ttu-id="c78ba-2038">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2038">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-2039">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-2039">Az.Automation</span></span>
* <span data-ttu-id="c78ba-2040">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2040">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="c78ba-2041">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2041">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="c78ba-2042">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2042">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-2043">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2043">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-2044">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2044">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2045">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2045">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2046">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2046">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="c78ba-2047">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2047">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="c78ba-2048">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2048">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="c78ba-2049">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2049">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2050">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2050">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-2051">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2051">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c78ba-2052">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-2052">Az.EventHub</span></span>
* <span data-ttu-id="c78ba-2053">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2053">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-2054">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-2054">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-2055">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2055">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c78ba-2056">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78ba-2056">Az.LogicApp</span></span>
* <span data-ttu-id="c78ba-2057">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2057">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="c78ba-2058">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2058">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="c78ba-2059">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2059">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="c78ba-2060">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c78ba-2060">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c78ba-2061">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c78ba-2061">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c78ba-2062">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c78ba-2062">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c78ba-2063">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c78ba-2063">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="c78ba-2064">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2064">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="c78ba-2065">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-2065">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c78ba-2066">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-2066">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c78ba-2067">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-2067">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c78ba-2068">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-2068">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="c78ba-2069">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2069">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c78ba-2070">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-2070">Az.Monitor</span></span>
* <span data-ttu-id="c78ba-2071">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2071">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2072">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2072">Az.Network</span></span>
* <span data-ttu-id="c78ba-2073">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2073">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-2074">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-2074">Az.OperationalInsights</span></span>
* <span data-ttu-id="c78ba-2075">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2075">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="c78ba-2076">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2076">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="c78ba-2077">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2077">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2078">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2079">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c78ba-2079">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c78ba-2080">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c78ba-2080">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="c78ba-2081">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="c78ba-2081">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="c78ba-2082">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2082">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2083">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2083">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2084">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2084">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="c78ba-2085">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2085">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-2086">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2086">Az.Websites</span></span>
* <span data-ttu-id="c78ba-2087">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2087">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="c78ba-2088">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2088">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-2089">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2089">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-2090">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2090">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c78ba-2091">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2091">Az.AnalysisServices</span></span>
<span data-ttu-id="c78ba-2092">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-2092">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2093">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2093">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2094">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2094">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="c78ba-2095">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2095">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="c78ba-2096">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2096">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-2097">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2097">Az.RecoveryServices</span></span>
<span data-ttu-id="c78ba-2098">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-2098">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2099">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2099">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2100">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2100">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="c78ba-2101">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="c78ba-2101">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c78ba-2102">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2102">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="c78ba-2103">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="c78ba-2103">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2104">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2104">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2105">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2105">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="c78ba-2106">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2106">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="c78ba-2107">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2107">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="c78ba-2108">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2108">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-2109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2109">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-2110">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-2110">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c78ba-2111">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2111">Az.AnalysisServices</span></span>
* <span data-ttu-id="c78ba-2112">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-2112">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-2113">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2113">Az.RecoveryServices</span></span>
* <span data-ttu-id="c78ba-2114">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-2114">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="c78ba-2115">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2115">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-2116">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2116">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-2117">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2117">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c78ba-2118">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2118">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c78ba-2119">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2119">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="c78ba-2120">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c78ba-2120">Az.Aks</span></span>
* <span data-ttu-id="c78ba-2121">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2121">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c78ba-2122">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-2122">Az.Automation</span></span>
* <span data-ttu-id="c78ba-2123">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2123">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="c78ba-2124">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2124">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c78ba-2125">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c78ba-2125">Az.Cdn</span></span>
* <span data-ttu-id="c78ba-2126">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2126">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2127">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2127">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2128">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2128">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="c78ba-2129">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2129">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="c78ba-2130">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2130">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c78ba-2131">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c78ba-2131">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c78ba-2132">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2132">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c78ba-2133">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c78ba-2133">Az.DataFactory</span></span>
* <span data-ttu-id="c78ba-2134">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2134">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2135">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2135">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-2136">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="c78ba-2136">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="c78ba-2137">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="c78ba-2137">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="c78ba-2138">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2138">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-2139">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-2139">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-2140">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2140">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c78ba-2141">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-2141">Az.KeyVault</span></span>
* <span data-ttu-id="c78ba-2142">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2142">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2143">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2143">Az.Network</span></span>
* <span data-ttu-id="c78ba-2144">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2144">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2145">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2145">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2146">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2146">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="c78ba-2147">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2147">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="c78ba-2148">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2148">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="c78ba-2149">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="c78ba-2149">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="c78ba-2150">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="c78ba-2150">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="c78ba-2151">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2151">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="c78ba-2152">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="c78ba-2152">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-2153">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-2153">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-2154">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="c78ba-2154">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="c78ba-2155">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2155">Fix some error messages.</span></span>
* <span data-ttu-id="c78ba-2156">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2156">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="c78ba-2157">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2157">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c78ba-2158">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c78ba-2158">Az.SignalR</span></span>
* <span data-ttu-id="c78ba-2159">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2159">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2160">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2160">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2161">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2161">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c78ba-2162">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2162">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="c78ba-2163">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2163">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="c78ba-2164">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-2164">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-2165">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2165">Az.Storage</span></span>
* <span data-ttu-id="c78ba-2166">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2166">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c78ba-2167">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="c78ba-2167">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="c78ba-2168">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="c78ba-2168">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="c78ba-2169">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="c78ba-2169">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c78ba-2170">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c78ba-2170">Az.TrafficManager</span></span>
* <span data-ttu-id="c78ba-2171">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2171">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-2172">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2172">Az.Websites</span></span>
* <span data-ttu-id="c78ba-2173">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2173">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c78ba-2174">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2174">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="c78ba-2175">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="c78ba-2175">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="c78ba-2176">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2176">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c78ba-2177">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2177">Az.Accounts</span></span>
* <span data-ttu-id="c78ba-2178">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="c78ba-2178">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2179">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2179">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2180">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2180">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="c78ba-2181">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2181">Updated the description of ID in help files</span></span>
* <span data-ttu-id="c78ba-2182">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2182">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2183">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2183">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-2184">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2184">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="c78ba-2185">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2185">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c78ba-2186">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c78ba-2186">Az.EventGrid</span></span>
* <span data-ttu-id="c78ba-2187">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2187">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="c78ba-2188">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="c78ba-2188">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="c78ba-2189">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="c78ba-2189">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c78ba-2190">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="c78ba-2190">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c78ba-2191">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="c78ba-2191">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c78ba-2192">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="c78ba-2192">Dead letter endpoint.</span></span>
    - <span data-ttu-id="c78ba-2193">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="c78ba-2193">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c78ba-2194">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="c78ba-2194">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c78ba-2195">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="c78ba-2195">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c78ba-2196">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="c78ba-2196">Dead letter endpoint.</span></span>
* <span data-ttu-id="c78ba-2197">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2197">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="c78ba-2198">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2198">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c78ba-2199">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c78ba-2199">Az.IotHub</span></span>
* <span data-ttu-id="c78ba-2200">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2200">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c78ba-2201">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c78ba-2201">Az.LogicApp</span></span>
* <span data-ttu-id="c78ba-2202">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-2202">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2203">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2203">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2204">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2204">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="c78ba-2205">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="c78ba-2205">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="c78ba-2206">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2206">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c78ba-2207">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2207">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="c78ba-2208">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2208">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="c78ba-2209">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="c78ba-2209">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c78ba-2210">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c78ba-2210">Az.SignalR</span></span>
* <span data-ttu-id="c78ba-2211">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2211">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2212">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2212">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2213">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2213">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c78ba-2214">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2214">Az.Storage</span></span>
* <span data-ttu-id="c78ba-2215">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="c78ba-2215">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="c78ba-2216">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c78ba-2216">New-AzStorageContext</span></span>
* <span data-ttu-id="c78ba-2217">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2217">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="c78ba-2218">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c78ba-2218">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-2219">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2219">Az.Websites</span></span>
* <span data-ttu-id="c78ba-2220">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2220">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c78ba-2221">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2221">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="c78ba-2222">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2222">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="c78ba-2223">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-2223">General</span></span>

- <span data-ttu-id="c78ba-2224">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-2224">General Availability of Az Module</span></span>
- <span data-ttu-id="c78ba-2225">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="c78ba-2225">Online help for each module</span></span>
- <span data-ttu-id="c78ba-2226">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2226">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="c78ba-2227">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2227">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="c78ba-2228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c78ba-2228">Az.Accounts</span></span>
- <span data-ttu-id="c78ba-2229">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2229">Changed from Az.Profile</span></span>
- <span data-ttu-id="c78ba-2230">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2230">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c78ba-2231">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-2231">Az.ApiManagement</span></span>
- <span data-ttu-id="c78ba-2232">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="c78ba-2232">Fixes for #7002</span></span>
- <span data-ttu-id="c78ba-2233">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2233">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="c78ba-2234">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c78ba-2234">Az.Batch</span></span>
- <span data-ttu-id="c78ba-2235">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2235">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="c78ba-2236">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2236">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="c78ba-2237">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2237">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="c78ba-2238">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c78ba-2238">Az.Billing</span></span>
- <span data-ttu-id="c78ba-2239">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2239">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="c78ba-2240">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2240">Az.CognitivServices</span></span>
- <span data-ttu-id="c78ba-2241">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2241">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="c78ba-2242">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2242">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c78ba-2243">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2243">Az.ContainerInstance</span></span>
- <span data-ttu-id="c78ba-2244">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2244">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="c78ba-2245">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c78ba-2245">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="c78ba-2246">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2246">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2247">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2247">Az.DataLakeStore</span></span>
- <span data-ttu-id="c78ba-2248">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2248">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="c78ba-2249">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c78ba-2249">Az.Monitor</span></span>
- <span data-ttu-id="c78ba-2250">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2250">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="c78ba-2251">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c78ba-2251">Az.KeyVault</span></span>
- <span data-ttu-id="c78ba-2252">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2252">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="c78ba-2253">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c78ba-2253">Az.MachineLearning</span></span>
- <span data-ttu-id="c78ba-2254">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2254">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="c78ba-2255">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c78ba-2255">Az.Media</span></span>
- <span data-ttu-id="c78ba-2256">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2256">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c78ba-2257">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2257">Az.Network</span></span>
<span data-ttu-id="c78ba-2258">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2258">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="c78ba-2259">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-2259">New cmdlets added:</span></span>
        - <span data-ttu-id="c78ba-2260">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2260">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2261">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2261">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2262">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2262">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2263">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2263">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2264">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2264">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2265">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-2265">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="c78ba-2266">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c78ba-2266">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="c78ba-2267">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="c78ba-2267">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="c78ba-2268">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2268">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="c78ba-2269">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c78ba-2269">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="c78ba-2270">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-2270">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c78ba-2271">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c78ba-2271">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c78ba-2272">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-2272">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="c78ba-2273">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-2273">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="c78ba-2274">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2274">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="c78ba-2275">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2275">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="c78ba-2276">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c78ba-2276">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c78ba-2277">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c78ba-2277">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c78ba-2278">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c78ba-2278">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="c78ba-2279">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2279">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="c78ba-2280">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2280">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="c78ba-2281">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-2281">Az.OperationalInsights</span></span>
- <span data-ttu-id="c78ba-2282">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2282">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="c78ba-2283">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2283">Az.Profile</span></span>
- <span data-ttu-id="c78ba-2284">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2284">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-2285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2285">Az.RecoveryServices</span></span>
- <span data-ttu-id="c78ba-2286">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2286">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="c78ba-2287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2287">Az.Resources</span></span>
- <span data-ttu-id="c78ba-2288">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2288">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c78ba-2289">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-2289">Az.ServiceFabric</span></span>
- <span data-ttu-id="c78ba-2290">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="c78ba-2290">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="c78ba-2291">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2291">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="c78ba-2292">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="c78ba-2292">Az.SIgnalR</span></span>
- <span data-ttu-id="c78ba-2293">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="c78ba-2293">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="c78ba-2294">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2294">Az.Sql</span></span>
- <span data-ttu-id="c78ba-2295">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2295">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="c78ba-2296">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2296">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="c78ba-2297">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2297">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="c78ba-2298">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2298">Az.Storage</span></span>
- <span data-ttu-id="c78ba-2299">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2299">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c78ba-2300">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2300">Az.Websites</span></span>
- <span data-ttu-id="c78ba-2301">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="c78ba-2301">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="c78ba-2302">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2302">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="c78ba-2303">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-2303">General</span></span>

* <span data-ttu-id="c78ba-2304">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-2304">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="c78ba-2305">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2305">Az.Compute</span></span>

* <span data-ttu-id="c78ba-2306">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2306">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2307">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2307">Az.DataLakeStore</span></span>

* <span data-ttu-id="c78ba-2308">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2308">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="c78ba-2309">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c78ba-2309">Az.FrontDoor</span></span>

* <span data-ttu-id="c78ba-2310">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2310">Fixed some broken links</span></span>
    - <span data-ttu-id="c78ba-2311">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2311">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="c78ba-2312">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2312">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c78ba-2313">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2313">Az.RecoveryServices</span></span>

* <span data-ttu-id="c78ba-2314">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2314">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="c78ba-2315">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2315">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="c78ba-2316">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2316">Az.Resources</span></span>

* <span data-ttu-id="c78ba-2317">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2317">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="c78ba-2318">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2318">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="c78ba-2319">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2319">Az.Sql</span></span>

* <span data-ttu-id="c78ba-2320">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="c78ba-2320">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="c78ba-2321">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2321">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="c78ba-2322">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2322">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="c78ba-2323">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2323">Az.Storage</span></span>

* <span data-ttu-id="c78ba-2324">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2324">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="c78ba-2325">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2325">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="c78ba-2326">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c78ba-2326">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c78ba-2327">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="c78ba-2327">Support Static Website configuration</span></span>
    - <span data-ttu-id="c78ba-2328">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c78ba-2328">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="c78ba-2329">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c78ba-2329">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c78ba-2330">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2330">Az.Websites</span></span>

* <span data-ttu-id="c78ba-2331">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c78ba-2331">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="c78ba-2332">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2332">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="c78ba-2333">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="c78ba-2333">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="c78ba-2334">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2334">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c78ba-2335">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c78ba-2335">Az.ApiManagement</span></span>
* <span data-ttu-id="c78ba-2336">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2336">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="c78ba-2337">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c78ba-2337">Az.Automation</span></span>
* <span data-ttu-id="c78ba-2338">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="c78ba-2338">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="c78ba-2339">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2339">Added Update Management cmdlets</span></span>
* <span data-ttu-id="c78ba-2340">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2340">Added Source Control cmdlets</span></span>
* <span data-ttu-id="c78ba-2341">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2341">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="c78ba-2342">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2342">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="c78ba-2343">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2343">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2344">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2344">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="c78ba-2345">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2345">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c78ba-2346">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2346">Az.ContainerInstance</span></span>
* <span data-ttu-id="c78ba-2347">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2347">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="c78ba-2348">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c78ba-2348">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c78ba-2349">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2349">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c78ba-2350">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2350">Az.Network</span></span>
* <span data-ttu-id="c78ba-2351">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2351">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="c78ba-2352">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2352">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="c78ba-2353">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2353">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="c78ba-2354">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2354">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="c78ba-2355">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c78ba-2355">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c78ba-2356">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2356">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="c78ba-2357">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2357">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="c78ba-2358">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c78ba-2358">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c78ba-2359">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2359">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="c78ba-2360">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2360">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="c78ba-2361">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c78ba-2361">Az.Relay</span></span>
* <span data-ttu-id="c78ba-2362">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-2362">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="c78ba-2363">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2363">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2364">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2364">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="c78ba-2365">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2365">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="c78ba-2366">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="c78ba-2366">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c78ba-2367">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-2367">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-2368">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2368">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="c78ba-2369">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2369">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2370">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2370">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="c78ba-2371">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2371">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c78ba-2372">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2372">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c78ba-2373">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2373">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c78ba-2374">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c78ba-2374">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c78ba-2375">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c78ba-2375">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c78ba-2376">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c78ba-2376">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c78ba-2377">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c78ba-2377">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c78ba-2378">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c78ba-2378">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="c78ba-2379">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2379">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="c78ba-2380">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2380">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="c78ba-2381">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2381">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="c78ba-2382">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="c78ba-2382">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c78ba-2383">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="c78ba-2383">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c78ba-2384">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="c78ba-2384">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="c78ba-2385">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="c78ba-2385">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="c78ba-2386">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2386">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="c78ba-2387">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2387">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c78ba-2388">全般</span><span class="sxs-lookup"><span data-stu-id="c78ba-2388">General</span></span>
* <span data-ttu-id="c78ba-2389">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="c78ba-2389">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="c78ba-2390">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2390">Az.Profile</span></span>
* <span data-ttu-id="c78ba-2391">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2391">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="c78ba-2392">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2392">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="c78ba-2393">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2393">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="c78ba-2394">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2394">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="c78ba-2395">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2395">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="c78ba-2396">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2396">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="c78ba-2397">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2397">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-2398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2398">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-2399">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2399">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2400">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2401">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2401">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="c78ba-2402">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="c78ba-2402">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="c78ba-2403">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2403">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2404">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2404">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-2405">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2405">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="c78ba-2406">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2406">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="c78ba-2407">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="c78ba-2407">Az.Insights</span></span>
* <span data-ttu-id="c78ba-2408">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2408">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="c78ba-2409">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2409">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="c78ba-2410">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2410">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="c78ba-2411">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="c78ba-2411">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2412">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2412">Az.Network</span></span>
* <span data-ttu-id="c78ba-2413">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="c78ba-2413">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="c78ba-2414">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-2414">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="c78ba-2415">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-2415">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="c78ba-2416">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c78ba-2416">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="c78ba-2417">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-2417">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c78ba-2418">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="c78ba-2418">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c78ba-2419">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c78ba-2419">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c78ba-2420">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c78ba-2420">Az.PolicyInsights</span></span>
* <span data-ttu-id="c78ba-2421">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2421">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2422">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2422">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2423">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2423">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="c78ba-2424">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2424">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c78ba-2425">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c78ba-2425">Az.ServiceBus</span></span>
* <span data-ttu-id="c78ba-2426">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2426">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c78ba-2427">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c78ba-2427">Az.ServiceFabric</span></span>
* <span data-ttu-id="c78ba-2428">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2428">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="c78ba-2429">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2429">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="c78ba-2430">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2430">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="c78ba-2431">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2431">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="c78ba-2432">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2432">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="c78ba-2433">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2433">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="c78ba-2434">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2434">Az.Profile</span></span>
* <span data-ttu-id="c78ba-2435">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2435">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="c78ba-2436">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2436">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2437">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2437">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2438">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2438">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="c78ba-2439">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2439">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c78ba-2440">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c78ba-2440">Az.DataLakeStore</span></span>
* <span data-ttu-id="c78ba-2441">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2441">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="c78ba-2442">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2442">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="c78ba-2443">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2443">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c78ba-2444">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2444">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c78ba-2445">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2445">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2446">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2446">Az.Network</span></span>
* <span data-ttu-id="c78ba-2447">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2447">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="c78ba-2448">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2448">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2449">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2449">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2450">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2450">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="c78ba-2451">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2451">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="c78ba-2452">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2452">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="c78ba-2453">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2453">Azure.Storage</span></span>
* <span data-ttu-id="c78ba-2454">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2454">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="c78ba-2455">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c78ba-2455">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="c78ba-2456">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c78ba-2456">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c78ba-2457">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2457">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="c78ba-2458">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="c78ba-2458">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c78ba-2459">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c78ba-2459">Az.CognitiveServices</span></span>
* <span data-ttu-id="c78ba-2460">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2460">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c78ba-2461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c78ba-2461">Az.Compute</span></span>
* <span data-ttu-id="c78ba-2462">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2462">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="c78ba-2463">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2463">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="c78ba-2464">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2464">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="c78ba-2465">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c78ba-2465">Az.DataFactoryV2</span></span>
* <span data-ttu-id="c78ba-2466">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2466">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c78ba-2467">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c78ba-2467">Az.Network</span></span>
* <span data-ttu-id="c78ba-2468">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2468">Added NetworkProfile functionality.</span></span> <span data-ttu-id="c78ba-2469">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="c78ba-2469">new cmdlets added</span></span>
    - <span data-ttu-id="c78ba-2470">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2470">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="c78ba-2471">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2471">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="c78ba-2472">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2472">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="c78ba-2473">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c78ba-2473">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="c78ba-2474">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-2474">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="c78ba-2475">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="c78ba-2475">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="c78ba-2476">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2476">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="c78ba-2477">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2477">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="c78ba-2478">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2478">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c78ba-2479">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c78ba-2479">Az.RedisCache</span></span>
* <span data-ttu-id="c78ba-2480">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="c78ba-2480">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="c78ba-2481">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2481">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="c78ba-2482">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c78ba-2482">Az.Resources</span></span>
* <span data-ttu-id="c78ba-2483">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2483">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c78ba-2484">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2484">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="c78ba-2485">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c78ba-2485">Az.Sql</span></span>
* <span data-ttu-id="c78ba-2486">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="c78ba-2486">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c78ba-2487">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c78ba-2487">Az.Websites</span></span>
* <span data-ttu-id="c78ba-2488">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="c78ba-2488">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="c78ba-2489">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="c78ba-2489">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="c78ba-2490">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="c78ba-2490">0.2.0 - September 2018</span></span>
 <span data-ttu-id="c78ba-2491">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="c78ba-2491">Initial Release</span></span>

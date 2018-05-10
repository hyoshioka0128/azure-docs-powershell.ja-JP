# <a name="table-of-contents"></a><span data-ttu-id="e2de5-101">目次</span><span class="sxs-lookup"><span data-stu-id="e2de5-101">Table of Contents</span></span>
1. [<span data-ttu-id="e2de5-102">Force パラメーターの削除</span><span class="sxs-lookup"><span data-stu-id="e2de5-102">Removal of Force parameters</span></span>](#removal-of-force-parameters)
2. [<span data-ttu-id="e2de5-103">Tag パラメーターの変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-103">Change of Tag parameters</span></span>](#change-of-tag-parameters)
3. [<span data-ttu-id="e2de5-104">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-104">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
4. [<span data-ttu-id="e2de5-105">AD コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-105">Breaking changes to AD cmdlets</span></span>](#breaking-changes-to-ad-cmdlets)

## <a name="removal-of-force-parameters"></a><span data-ttu-id="e2de5-106">Force パラメーターの削除</span><span class="sxs-lookup"><span data-stu-id="e2de5-106">Removal of Force parameters</span></span>

<span data-ttu-id="e2de5-107">このリリースでは、コマンドレットから古い `Force` パラメーターがすべて削除されました。また、将来のリリースでこのパラメーターが削除されることを示す対応する警告も削除されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-107">This release, we removed all Obsolete `Force` parameters from cmdlets and the corresponding warnings that the parameter would be removed in a future release.</span></span>

<span data-ttu-id="e2de5-108">この変更の影響を受けるコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e2de5-108">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="e2de5-109">**ApiManagement**</span><span class="sxs-lookup"><span data-stu-id="e2de5-109">**ApiManagement**</span></span>
- <span data-ttu-id="e2de5-110">Remove-AzureRmApiManagement</span><span class="sxs-lookup"><span data-stu-id="e2de5-110">Remove-AzureRmApiManagement</span></span>
- <span data-ttu-id="e2de5-111">Remove-AzureRmApiManagementApi</span><span class="sxs-lookup"><span data-stu-id="e2de5-111">Remove-AzureRmApiManagementApi</span></span>
- <span data-ttu-id="e2de5-112">Remove-AzureRmApiManagementGroup</span><span class="sxs-lookup"><span data-stu-id="e2de5-112">Remove-AzureRmApiManagementGroup</span></span>
- <span data-ttu-id="e2de5-113">Remove-AzureRmApiManagementLogger</span><span class="sxs-lookup"><span data-stu-id="e2de5-113">Remove-AzureRmApiManagementLogger</span></span>
- <span data-ttu-id="e2de5-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="e2de5-114">Remove-AzureRmApiManagementOpenIdConnectProvider</span></span>
- <span data-ttu-id="e2de5-115">Remove-AzureRmApiManagementOperation</span><span class="sxs-lookup"><span data-stu-id="e2de5-115">Remove-AzureRmApiManagementOperation</span></span>
- <span data-ttu-id="e2de5-116">Remove-AzureRmApiManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="e2de5-116">Remove-AzureRmApiManagementPolicy</span></span>
- <span data-ttu-id="e2de5-117">Remove-AzureRmApiManagementProduct</span><span class="sxs-lookup"><span data-stu-id="e2de5-117">Remove-AzureRmApiManagementProduct</span></span>
- <span data-ttu-id="e2de5-118">Remove-AzureRmApiManagementProperty</span><span class="sxs-lookup"><span data-stu-id="e2de5-118">Remove-AzureRmApiManagementProperty</span></span>
- <span data-ttu-id="e2de5-119">Remove-AzureRmApiManagementSubscription</span><span class="sxs-lookup"><span data-stu-id="e2de5-119">Remove-AzureRmApiManagementSubscription</span></span>
- <span data-ttu-id="e2de5-120">Remove-AzureRmApiManagementUser</span><span class="sxs-lookup"><span data-stu-id="e2de5-120">Remove-AzureRmApiManagementUser</span></span>

<span data-ttu-id="e2de5-121">**Automation**</span><span class="sxs-lookup"><span data-stu-id="e2de5-121">**Automation**</span></span>
- <span data-ttu-id="e2de5-122">Remove-AzureRmAutomationCertificate</span><span class="sxs-lookup"><span data-stu-id="e2de5-122">Remove-AzureRmAutomationCertificate</span></span>
- <span data-ttu-id="e2de5-123">Remove-AzureRmAutomationCredential</span><span class="sxs-lookup"><span data-stu-id="e2de5-123">Remove-AzureRmAutomationCredential</span></span>
- <span data-ttu-id="e2de5-124">Remove-AzureRmAutomationVariable</span><span class="sxs-lookup"><span data-stu-id="e2de5-124">Remove-AzureRmAutomationVariable</span></span>
- <span data-ttu-id="e2de5-125">Remove-AzureRmAutomationWebhook</span><span class="sxs-lookup"><span data-stu-id="e2de5-125">Remove-AzureRmAutomationWebhook</span></span>

<span data-ttu-id="e2de5-126">**Batch**</span><span class="sxs-lookup"><span data-stu-id="e2de5-126">**Batch**</span></span>
- <span data-ttu-id="e2de5-127">Remove-AzureBatchCertificate</span><span class="sxs-lookup"><span data-stu-id="e2de5-127">Remove-AzureBatchCertificate</span></span>
- <span data-ttu-id="e2de5-128">Remove-AzureBatchComputeNode</span><span class="sxs-lookup"><span data-stu-id="e2de5-128">Remove-AzureBatchComputeNode</span></span>
- <span data-ttu-id="e2de5-129">Remove-AzureBatchComputeNodeUser</span><span class="sxs-lookup"><span data-stu-id="e2de5-129">Remove-AzureBatchComputeNodeUser</span></span>

<span data-ttu-id="e2de5-130">**DataFactories**</span><span class="sxs-lookup"><span data-stu-id="e2de5-130">**DataFactories**</span></span>
- <span data-ttu-id="e2de5-131">Resume-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="e2de5-131">Resume-AzureRmDataFactoryPipeline</span></span>
- <span data-ttu-id="e2de5-132">Set-AzureRmDataFactoryPipelineActivePeriod</span><span class="sxs-lookup"><span data-stu-id="e2de5-132">Set-AzureRmDataFactoryPipelineActivePeriod</span></span>
- <span data-ttu-id="e2de5-133">Suspend-AzureRmDataFactoryPipeline</span><span class="sxs-lookup"><span data-stu-id="e2de5-133">Suspend-AzureRmDataFactoryPipeline</span></span>

<span data-ttu-id="e2de5-134">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="e2de5-134">**DataLakeStore**</span></span>
- <span data-ttu-id="e2de5-135">Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e2de5-135">Remove-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="e2de5-136">Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="e2de5-136">Set-AzureRmDataLakeStoreItemAcl</span></span>
- <span data-ttu-id="e2de5-137">Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="e2de5-137">Set-AzureRmDataLakeStoreItemAclEntry</span></span>
- <span data-ttu-id="e2de5-138">Set-AzureRmDataLakeStoreItemOwner</span><span class="sxs-lookup"><span data-stu-id="e2de5-138">Set-AzureRmDataLakeStoreItemOwner</span></span>

<span data-ttu-id="e2de5-139">**OperationalInsights**</span><span class="sxs-lookup"><span data-stu-id="e2de5-139">**OperationalInsights**</span></span>
- <span data-ttu-id="e2de5-140">Remove-AzureRmOperationalInsightsSavedSearch</span><span class="sxs-lookup"><span data-stu-id="e2de5-140">Remove-AzureRmOperationalInsightsSavedSearch</span></span>

<span data-ttu-id="e2de5-141">**プロファイル**</span><span class="sxs-lookup"><span data-stu-id="e2de5-141">**Profile**</span></span>
- <span data-ttu-id="e2de5-142">Remove-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="e2de5-142">Remove-AzureRmEnvironment</span></span>

<span data-ttu-id="e2de5-143">**RedisCache**</span><span class="sxs-lookup"><span data-stu-id="e2de5-143">**RedisCache**</span></span>
- <span data-ttu-id="e2de5-144">Remove-AzureRmRedisCacheDiagnostics</span><span class="sxs-lookup"><span data-stu-id="e2de5-144">Remove-AzureRmRedisCacheDiagnostics</span></span>

<span data-ttu-id="e2de5-145">**リソース**</span><span class="sxs-lookup"><span data-stu-id="e2de5-145">**Resources**</span></span>
- <span data-ttu-id="e2de5-146">Register-AzureRmProviderFeature</span><span class="sxs-lookup"><span data-stu-id="e2de5-146">Register-AzureRmProviderFeature</span></span>
- <span data-ttu-id="e2de5-147">Register-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="e2de5-147">Register-AzureRmResourceProvider</span></span>
- <span data-ttu-id="e2de5-148">Remove-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e2de5-148">Remove-AzureRmADServicePrincipal</span></span>
- <span data-ttu-id="e2de5-149">Remove-AzureRmPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e2de5-149">Remove-AzureRmPolicyAssignment</span></span>
- <span data-ttu-id="e2de5-150">Remove-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="e2de5-150">Remove-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="e2de5-151">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e2de5-151">Remove-AzureRmRoleAssignment</span></span>
- <span data-ttu-id="e2de5-152">Stop-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="e2de5-152">Stop-AzureRmResourceGroupDeployment</span></span>
- <span data-ttu-id="e2de5-153">Unregister-AzureRmResourceProvider</span><span class="sxs-lookup"><span data-stu-id="e2de5-153">Unregister-AzureRmResourceProvider</span></span>

<span data-ttu-id="e2de5-154">**Storage**</span><span class="sxs-lookup"><span data-stu-id="e2de5-154">**Storage**</span></span>
- <span data-ttu-id="e2de5-155">Remove-AzureStorageContainerStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e2de5-155">Remove-AzureStorageContainerStoredAccessPolicy</span></span>
- <span data-ttu-id="e2de5-156">Remove-AzureStorageQueueStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e2de5-156">Remove-AzureStorageQueueStoredAccessPolicy</span></span>
- <span data-ttu-id="e2de5-157">Remove-AzureStorageShareStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e2de5-157">Remove-AzureStorageShareStoredAccessPolicy</span></span>
- <span data-ttu-id="e2de5-158">Remove-AzureStorageTableStoredAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e2de5-158">Remove-AzureStorageTableStoredAccessPolicy</span></span>

<span data-ttu-id="e2de5-159">**StreamAnalytics**</span><span class="sxs-lookup"><span data-stu-id="e2de5-159">**StreamAnalytics**</span></span>
- <span data-ttu-id="e2de5-160">Remove-AzureRmStreamAnalyticsFunction</span><span class="sxs-lookup"><span data-stu-id="e2de5-160">Remove-AzureRmStreamAnalyticsFunction</span></span>
- <span data-ttu-id="e2de5-161">Remove-AzureRmStreamAnalyticsInput</span><span class="sxs-lookup"><span data-stu-id="e2de5-161">Remove-AzureRmStreamAnalyticsInput</span></span>
- <span data-ttu-id="e2de5-162">Remove-AzureRmStreamAnalyticsJob</span><span class="sxs-lookup"><span data-stu-id="e2de5-162">Remove-AzureRmStreamAnalyticsJob</span></span>
- <span data-ttu-id="e2de5-163">Remove-AzureRmStreamAnalyticsOutput</span><span class="sxs-lookup"><span data-stu-id="e2de5-163">Remove-AzureRmStreamAnalyticsOutput</span></span>

<span data-ttu-id="e2de5-164">**Tag**</span><span class="sxs-lookup"><span data-stu-id="e2de5-164">**Tag**</span></span>
- <span data-ttu-id="e2de5-165">Remove-AzureRmTag</span><span class="sxs-lookup"><span data-stu-id="e2de5-165">Remove-AzureRmTag</span></span>

<br>

<span data-ttu-id="e2de5-166">上記のコマンドレットのいずれかを使用するスクリプトがある場合は、`Force` パラメーターを削除するだけで重大な変更に対処できます。</span><span class="sxs-lookup"><span data-stu-id="e2de5-166">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by simply removing the `Force` parameter.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location
```

<br>

## <a name="change-of-tag-parameters"></a><span data-ttu-id="e2de5-167">Tag パラメーターの変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-167">Change of Tag parameters</span></span>

<span data-ttu-id="e2de5-168">このリリースでは、`Tags` パラメーターの名前が `Tag` に変更されました。また、型が `Hashtable[]` から `Hashtable` に変更され、キーと値のペアの形式が変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-168">This release, the `Tags` parameter name was changed to `Tag`, and the type was changed from `Hashtable[]` to `Hashtable`, changing the format of the key-value pairings.</span></span>

<span data-ttu-id="e2de5-169">これまで、`Hashtable[]` 内の各エントリは 1 つのキーと値のペアを表していました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-169">Previously, each entry in the `Hashtable[]` represented a single key-value pairing:</span></span>

```powershell
$tags = @{ Name = "test1"; Value = "testval1" }, @{ Name = "test2", Value = "testval2" }
$tags[0].Name  # Key for the first entry, "test1"
$tags[0].Value # Value for the first entry, "testval1"
$tags[1].Name  # Key for the second entry, "test2"
$tags[1].Value # Value for the second entry, "testval2"
```

<span data-ttu-id="e2de5-170">現在、`Name` と `Value` が不要になり、`Hashtable` で `Key = "Value"` を割り当てることで、キーと値のペアを作成できます。</span><span class="sxs-lookup"><span data-stu-id="e2de5-170">Now, `Name` and `Value` are no longer necessary, allowing for key-value pairings to be created by assigning `Key = "Value"` in the `Hashtable`:</span></span>

```powershell
$tag = @{ test1 = "testval1"; test2 = "testval2" }
$tag["test1"] # Gets the value associated with the key "test1"
$tag["test2"] # Gets the value associated with the key "test2"
```

<span data-ttu-id="e2de5-171">この変更の影響を受けるコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e2de5-171">The following cmdlets are affected by this change:</span></span>

<span data-ttu-id="e2de5-172">**Batch**</span><span class="sxs-lookup"><span data-stu-id="e2de5-172">**Batch**</span></span>
- <span data-ttu-id="e2de5-173">Get-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-173">Get-AzureRmBatchAccount</span></span>
- <span data-ttu-id="e2de5-174">New-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-174">New-AzureRmBatchAccount</span></span>
- <span data-ttu-id="e2de5-175">Set-AzureRmBatchAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-175">Set-AzureRmBatchAccount</span></span>

<span data-ttu-id="e2de5-176">**Compute**</span><span class="sxs-lookup"><span data-stu-id="e2de5-176">**Compute**</span></span>
- <span data-ttu-id="e2de5-177">New-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="e2de5-177">New-AzureRmVM</span></span>
- <span data-ttu-id="e2de5-178">Update-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="e2de5-178">Update-AzureRmVM</span></span>

<span data-ttu-id="e2de5-179">**DataLakeAnalytics**</span><span class="sxs-lookup"><span data-stu-id="e2de5-179">**DataLakeAnalytics**</span></span>
- <span data-ttu-id="e2de5-180">New-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-180">New-AzureRmDataLakeAnalyticsAccount</span></span>
- <span data-ttu-id="e2de5-181">Set-AzureRmDataLakeAnalyticsAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-181">Set-AzureRmDataLakeAnalyticsAccount</span></span>

<span data-ttu-id="e2de5-182">**DataLakeStore**</span><span class="sxs-lookup"><span data-stu-id="e2de5-182">**DataLakeStore**</span></span>
- <span data-ttu-id="e2de5-183">New-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-183">New-AzureRmDataLakeStoreAccount</span></span>
- <span data-ttu-id="e2de5-184">Set-AzureRmDataLakeStoreAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-184">Set-AzureRmDataLakeStoreAccount</span></span>

<span data-ttu-id="e2de5-185">**Dns**</span><span class="sxs-lookup"><span data-stu-id="e2de5-185">**Dns**</span></span>
- <span data-ttu-id="e2de5-186">New-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="e2de5-186">New-AzureRmDnsZone</span></span>
- <span data-ttu-id="e2de5-187">Set-AzureRmDnsZone</span><span class="sxs-lookup"><span data-stu-id="e2de5-187">Set-AzureRmDnsZone</span></span>

<span data-ttu-id="e2de5-188">**KeyVault**</span><span class="sxs-lookup"><span data-stu-id="e2de5-188">**KeyVault**</span></span>
- <span data-ttu-id="e2de5-189">Get-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="e2de5-189">Get-AzureRmKeyVault</span></span>
- <span data-ttu-id="e2de5-190">New-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="e2de5-190">New-AzureRmKeyVault</span></span>

<span data-ttu-id="e2de5-191">**ネットワーク**</span><span class="sxs-lookup"><span data-stu-id="e2de5-191">**Network**</span></span>
- <span data-ttu-id="e2de5-192">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="e2de5-192">New-AzureRmApplicationGateway</span></span>
- <span data-ttu-id="e2de5-193">New-AzureRmExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="e2de5-193">New-AzureRmExpressRouteCircuit</span></span>
- <span data-ttu-id="e2de5-194">New-AzureRmLoadBalancer</span><span class="sxs-lookup"><span data-stu-id="e2de5-194">New-AzureRmLoadBalancer</span></span>
- <span data-ttu-id="e2de5-195">New-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="e2de5-195">New-AzureRmLocalNetworkGateway</span></span>
- <span data-ttu-id="e2de5-196">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="e2de5-196">New-AzureRmNetworkInterface</span></span>
- <span data-ttu-id="e2de5-197">New-AzureRmNetworkSecurityGroup</span><span class="sxs-lookup"><span data-stu-id="e2de5-197">New-AzureRmNetworkSecurityGroup</span></span>
- <span data-ttu-id="e2de5-198">New-AzureRmPublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="e2de5-198">New-AzureRmPublicIpAddress</span></span>
- <span data-ttu-id="e2de5-199">New-AzureRmRouteTable</span><span class="sxs-lookup"><span data-stu-id="e2de5-199">New-AzureRmRouteTable</span></span>
- <span data-ttu-id="e2de5-200">New-AzureRmVirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="e2de5-200">New-AzureRmVirtualNetwork</span></span>
- <span data-ttu-id="e2de5-201">New-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="e2de5-201">New-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="e2de5-202">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e2de5-202">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="e2de5-203">New-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="e2de5-203">New-AzureRmVirtualNetworkPeering</span></span>

<span data-ttu-id="e2de5-204">**リソース**</span><span class="sxs-lookup"><span data-stu-id="e2de5-204">**Resources**</span></span>
- <span data-ttu-id="e2de5-205">Find-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e2de5-205">Find-AzureRmResource</span></span>
- <span data-ttu-id="e2de5-206">Find-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e2de5-206">Find-AzureRmResourceGroup</span></span>
- <span data-ttu-id="e2de5-207">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e2de5-207">New-AzureRmResource</span></span>
- <span data-ttu-id="e2de5-208">New-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e2de5-208">New-AzureRmResourceGroup</span></span>
- <span data-ttu-id="e2de5-209">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="e2de5-209">Set-AzureRmResource</span></span>
- <span data-ttu-id="e2de5-210">Set-AzureRmResourceGroup</span><span class="sxs-lookup"><span data-stu-id="e2de5-210">Set-AzureRmResourceGroup</span></span>

<span data-ttu-id="e2de5-211">**SQL**</span><span class="sxs-lookup"><span data-stu-id="e2de5-211">**SQL**</span></span>
- <span data-ttu-id="e2de5-212">New-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e2de5-212">New-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="e2de5-213">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="e2de5-213">New-AzureRmSqlDatabaseCopy</span></span>
- <span data-ttu-id="e2de5-214">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="e2de5-214">New-AzureRmSqlDatabaseSecondary</span></span>
- <span data-ttu-id="e2de5-215">New-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="e2de5-215">New-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="e2de5-216">New-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="e2de5-216">New-AzureRmSqlServer</span></span>
- <span data-ttu-id="e2de5-217">Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="e2de5-217">Set-AzureRmSqlDatabase</span></span>
- <span data-ttu-id="e2de5-218">Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="e2de5-218">Set-AzureRmSqlElasticPool</span></span>
- <span data-ttu-id="e2de5-219">Set-AzureRmSqlServer</span><span class="sxs-lookup"><span data-stu-id="e2de5-219">Set-AzureRmSqlServer</span></span>

<span data-ttu-id="e2de5-220">**Storage**</span><span class="sxs-lookup"><span data-stu-id="e2de5-220">**Storage**</span></span>
- <span data-ttu-id="e2de5-221">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-221">New-AzureRmStorageAccount</span></span>
- <span data-ttu-id="e2de5-222">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="e2de5-222">Set-AzureRmStorageAccount</span></span>

<span data-ttu-id="e2de5-223">**TrafficManager**</span><span class="sxs-lookup"><span data-stu-id="e2de5-223">**TrafficManager**</span></span>
- <span data-ttu-id="e2de5-224">New-AzureRmTrafficManagerProfile</span><span class="sxs-lookup"><span data-stu-id="e2de5-224">New-AzureRmTrafficManagerProfile</span></span>

<br>

<span data-ttu-id="e2de5-225">上記のコマンドレットのいずれかを使用するスクリプトがある場合は、`Tags` パラメーターを `Tag` に変更し、`Tag` を新しい形式に変更することで、重大な変更に対処できます。</span><span class="sxs-lookup"><span data-stu-id="e2de5-225">If you have a script that uses any of the above cmdlets, the breaking change can be fixed by changing the `Tags` parameter to `Tag`, as well as changing the `Tag` to the new format.</span></span>

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tags @{ Name = "testtag"; Value = "testval" }

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tag @{ testtag = "testval" }
```

<br>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="e2de5-226">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-226">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="e2de5-227">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e2de5-227">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="e2de5-228">**Get-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="e2de5-228">**Get-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="e2de5-229">このコマンドレットは、各キーのプロパティを含むオブジェクトではなく、キーのリストを返すようになりました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-229">The cmdlet now returns a list of keys, rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Key1

# New
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName)[0].Value
```

<span data-ttu-id="e2de5-230">**New-AzureRmStorageAccountKey**</span><span class="sxs-lookup"><span data-stu-id="e2de5-230">**New-AzureRmStorageAccountKey**</span></span>
- <span data-ttu-id="e2de5-231">このコマンドレットの出力の `StorageAccountRegenerateKeyResponse` フィールドの名前が `StorageAccountListKeysResults` に変更され、各キーのプロパティを含むオブジェクトではなく、キーのリストになりました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-231">`StorageAccountRegenerateKeyResponse` field in output of this cmdlet is renamed to `StorageAccountListKeysResults`, which is now a list of keys rather than an object with properties for each key</span></span>

```powershell
# Old
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).StorageAccountKeys.Key1

# New
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Keys[0].Value
```

<span data-ttu-id="e2de5-232">**New/Get/Set-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="e2de5-232">**New/Get/Set-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="e2de5-233">このコマンドレットの出力の `AccountType` フィールドの名前が `Sku.Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-233">`AccountType` field in output of this cmdlet is renamed to `Sku.Name`</span></span>
- <span data-ttu-id="e2de5-234">PrimaryEndpoints/Secondary endpoints blob/table/queue/file の出力の型が `Uri` から `String` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-234">Output type for PrimaryEndpoints/Secondary endpoints blob/table/queue/file changed from `Uri` to `String`</span></span>

```powershell
# Old
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).AccountType

# New
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).Sku.Name
```

```powershell
# Old 
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.AbsolutePath

# New
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob
```

<br>

## <a name="breaking-changes-to-ad-cmdlets"></a><span data-ttu-id="e2de5-235">AD コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e2de5-235">Breaking changes to AD cmdlets</span></span>

<span data-ttu-id="e2de5-236">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e2de5-236">The following cmdlets were affected this release:</span></span>

<span data-ttu-id="e2de5-237">**Get-AzureRMADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="e2de5-237">**Get-AzureRMADServicePrincipal**</span></span>
- <span data-ttu-id="e2de5-238">このコマンドレットの出力の `ServicePrincipalName` フィールドの名前が `ServicePrincipalNames` に変更され、コレクションになりました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-238">`ServicePrincipalName` field in output of this cmdlet is renamed to `ServicePrincipalNames` and is now a collection.</span></span> <span data-ttu-id="e2de5-239">identifierUri に加え、SPN の 1 つとして `ApplicationId` も表示されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-239">It now displays `ApplicationId` also as one of the SPN, along with the identifierUri.</span></span>

```powershell
# Old
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalName

# New
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalNames[0]
```

<span data-ttu-id="e2de5-240">**Get-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e2de5-240">**Get-AzureRmADApplication**</span></span>
- <span data-ttu-id="e2de5-241">`ApplicationObjectId` パラメーターの名前が `ObjectId` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-241">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="e2de5-242">このコマンドレットの出力の `ApplicationObjectId` の名前が `ObjectId` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-242">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Get-AzureRmADApplication -ApplicationObjectId $applicationObjectId
$objectId = $app.ApplicationObjectId

# New
$app = Get-AzureRmADApplication -ObjectId $objectId
$objectId = $app.ObjectId
```

<span data-ttu-id="e2de5-243">**Remove-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e2de5-243">**Remove-AzureRmADApplication**</span></span>
- <span data-ttu-id="e2de5-244">`ApplicationObjectId` パラメーターの名前が `ObjectId` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-244">Parameter `ApplicationObjectId` is renamed to `ObjectId`.</span></span>

```powershell
# Old
$app = Remove-AzureRmADApplication -ApplicationObjectId $applicationObjectId -Force

# New
$app = Remove-AzureRmADApplication -ObjectId $objectId -Force
```

<span data-ttu-id="e2de5-245">**New-AzureRmADApplication**</span><span class="sxs-lookup"><span data-stu-id="e2de5-245">**New-AzureRmADApplication**</span></span>
- <span data-ttu-id="e2de5-246">このコマンドレットの出力の `ApplicationObjectId` の名前が `ObjectId` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-246">In output of this cmdlet, `ApplicationObjectId` is renamed to `ObjectId`.</span></span>
- <span data-ttu-id="e2de5-247">`KeyValue`、`KeyUsage`、`KeyType` の各パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-247">`KeyValue`, `KeyUsage`, `KeyType` parameters are removed.</span></span>

```powershell
# Old
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris -KeyValue $kv -KeyType $kt -KeyUsage $ku
$id = $app.ApplicationObjectId

# New
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris
$id = $app.ObjectId
New-AzureRmADAppCredential -ObjectId $id -Password $kv
```

<span data-ttu-id="e2de5-248">**Get-AzureRmADGroup**</span><span class="sxs-lookup"><span data-stu-id="e2de5-248">**Get-AzureRmADGroup**</span></span>
- <span data-ttu-id="e2de5-249">出力から `Mail` フィールドが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-249">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="e2de5-250">**Get-AzureRmADUser**</span><span class="sxs-lookup"><span data-stu-id="e2de5-250">**Get-AzureRmADUser**</span></span>
- <span data-ttu-id="e2de5-251">出力から `Mail` フィールドが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-251">`Mail` field is removed from the output.</span></span>

<span data-ttu-id="e2de5-252">**New-AzureRmADServicePrincipal**</span><span class="sxs-lookup"><span data-stu-id="e2de5-252">**New-AzureRmADServicePrincipal**</span></span>
- <span data-ttu-id="e2de5-253">`DisableAccount` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e2de5-253">Removed `DisableAccount` parameter.</span></span>

```powershell
# Old
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password -DisableAccount true

# New
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password
Remove-AzureRmADServicePrincipal -ObjectId $servicePrincipal.ObjectId
```
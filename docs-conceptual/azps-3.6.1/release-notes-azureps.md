---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: f24e5ef66f9c49976c550c9847903bd0608c5123
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2020
ms.locfileid: "79111030"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="83262-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="83262-103">Azure PowerShell release notes</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="83262-104">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="83262-104">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-105">Az.Accounts</span></span>
* <span data-ttu-id="83262-106">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="83262-106">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="83262-107">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="83262-107">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="83262-108">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-108">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="83262-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-109">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-110">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="83262-110">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="83262-111">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="83262-111">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="83262-112">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-112">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="83262-113">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="83262-113">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-114">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-114">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-115">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-115">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-116">Az.IotHub</span></span>
* <span data-ttu-id="83262-117">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-117">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="83262-118">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-118">New Cmdlets are:</span></span>
    - <span data-ttu-id="83262-119">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-119">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-120">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-120">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-121">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-121">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-122">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-122">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="83262-123">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-123">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="83262-124">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-124">New Cmdlets are:</span></span>
    - <span data-ttu-id="83262-125">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="83262-125">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="83262-126">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="83262-126">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="83262-127">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="83262-127">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="83262-128">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="83262-128">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="83262-129">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-129">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="83262-130">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-130">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="83262-131">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-131">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="83262-132">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-132">New Cmdlets are:</span></span>
    - <span data-ttu-id="83262-133">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="83262-133">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="83262-134">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="83262-134">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="83262-135">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-135">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-136">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-136">Az.Monitor</span></span>
* <span data-ttu-id="83262-137">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="83262-137">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-138">Az.Network</span></span>
* <span data-ttu-id="83262-139">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-139">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="83262-140">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-140">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="83262-141">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="83262-141">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="83262-142">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-142">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-143">Az.Resources</span></span>
* <span data-ttu-id="83262-144">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-144">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="83262-145">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="83262-145">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="83262-146">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="83262-146">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="83262-147">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="83262-147">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="83262-148">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-148">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="83262-149">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-149">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="83262-150">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-150">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="83262-151">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="83262-151">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="83262-152">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="83262-152">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="83262-153">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="83262-153">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="83262-154">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="83262-154">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="83262-155">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-155">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="83262-156">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="83262-156">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="83262-157">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="83262-157">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-158">Az.Sql</span></span>
* <span data-ttu-id="83262-159">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-159">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="83262-160">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-160">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="83262-161">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="83262-161">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="83262-162">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="83262-162">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="83262-163">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-163">Remove an LTR backup</span></span>
    - <span data-ttu-id="83262-164">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-164">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="83262-165">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-165">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="83262-166">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-166">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="83262-167">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="83262-167">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-168">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-168">Az.Storage</span></span>
* <span data-ttu-id="83262-169">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-169">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="83262-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="83262-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="83262-171">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-171">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="83262-172">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="83262-172">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="83262-173">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="83262-173">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-174">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-174">Az.Websites</span></span>
* <span data-ttu-id="83262-175">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-175">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="83262-176">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="83262-176">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="83262-177">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-177">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="83262-178">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="83262-178">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="83262-179">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-179">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="83262-180">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="83262-180">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-181">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-181">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-182">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-182">Updated client side telemetry.</span></span>
* <span data-ttu-id="83262-183">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-183">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="83262-184">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-184">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-185">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-185">Az.Accounts</span></span>
* <span data-ttu-id="83262-186">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-186">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-187">Az.Automation</span></span>
* <span data-ttu-id="83262-188">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-188">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-189">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-189">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-190">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-190">Updated SDK to 7.0</span></span>
* <span data-ttu-id="83262-191">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-191">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-192">Az.Compute</span></span>
* <span data-ttu-id="83262-193">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-193">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-194">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-194">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-195">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-195">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-196">Az.IotHub</span></span>
* <span data-ttu-id="83262-197">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-197">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="83262-198">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-198">New Cmdlets are:</span></span>
    - <span data-ttu-id="83262-199">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-199">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-200">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-200">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-201">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-201">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="83262-202">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="83262-202">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-203">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-203">Az.KeyVault</span></span>
* <span data-ttu-id="83262-204">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-204">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-205">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-205">Az.Monitor</span></span>
* <span data-ttu-id="83262-206">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-206">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="83262-207">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-207">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="83262-208">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="83262-208">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-209">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-209">Az.Network</span></span>
* <span data-ttu-id="83262-210">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-210">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="83262-211">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-211">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="83262-212">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-212">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="83262-213">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-213">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="83262-214">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="83262-214">No new cmdlets are added.</span></span> <span data-ttu-id="83262-215">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="83262-215">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-216">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-216">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-217">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-217">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-218">Az.Resources</span></span>
* <span data-ttu-id="83262-219">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="83262-219">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="83262-220">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="83262-220">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="83262-221">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="83262-221">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="83262-222">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-222">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="83262-223">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="83262-223">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="83262-224">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-224">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="83262-225">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-225">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="83262-226">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="83262-226">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-227">Az.Sql</span></span>
* <span data-ttu-id="83262-228">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-228">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="83262-229">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-229">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="83262-230">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="83262-230">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="83262-231">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="83262-231">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="83262-232">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-232">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="83262-233">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="83262-233">Az.StorageSync</span></span>
* <span data-ttu-id="83262-234">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-234">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="83262-235">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="83262-235">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-236">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-236">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-237">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="83262-237">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="83262-238">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-238">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-239">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-239">Az.Accounts</span></span>
* <span data-ttu-id="83262-240">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="83262-240">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="83262-241">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-241">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="83262-242">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-242">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-243">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="83262-243">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="83262-244">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="83262-244">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="83262-245">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-245">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="83262-246">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-246">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-247">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-247">Az.Compute</span></span>
* <span data-ttu-id="83262-248">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="83262-248">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="83262-249">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-249">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="83262-250">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-250">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="83262-251">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="83262-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="83262-252">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-252">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-253">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-253">Az.DataFactory</span></span>
* <span data-ttu-id="83262-254">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-254">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="83262-255">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="83262-255">Az.DeploymentManager</span></span>
* <span data-ttu-id="83262-256">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-256">Adds LIST operations for resources</span></span>
* <span data-ttu-id="83262-257">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-257">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="83262-258">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-258">Az.HDInsight</span></span>
* <span data-ttu-id="83262-259">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-259">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-260">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-260">Az.KeyVault</span></span>
* <span data-ttu-id="83262-261">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="83262-261">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-262">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-262">Az.Network</span></span>
* <span data-ttu-id="83262-263">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-263">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="83262-264">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="83262-264">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="83262-265">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="83262-265">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="83262-266">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-266">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="83262-267">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="83262-267">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="83262-268">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-268">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="83262-269">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-269">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="83262-270">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-270">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="83262-271">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-271">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="83262-273">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-273">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="83262-274">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="83262-274">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="83262-275">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-275">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="83262-276">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="83262-276">Az.PolicyInsights</span></span>
* <span data-ttu-id="83262-277">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-277">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="83262-278">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="83262-278">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="83262-279">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-279">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="83262-280">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-280">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-281">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-281">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-282">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-282">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="83262-283">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-283">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-284">Az.Resources</span></span>
* <span data-ttu-id="83262-285">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="83262-285">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="83262-286">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-286">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-287">Az.Sql</span></span>
<span data-ttu-id="83262-288">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-288">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-289">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-289">Az.Storage</span></span>
* <span data-ttu-id="83262-290">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-290">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="83262-291">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-291">New-AzStorageAccount</span></span>
* <span data-ttu-id="83262-292">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="83262-292">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="83262-293">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-293">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-294">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-294">Az.Websites</span></span>
* <span data-ttu-id="83262-295">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-295">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="83262-296">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-296">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="83262-297">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="83262-297">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-298">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-298">Az.Accounts</span></span>
* <span data-ttu-id="83262-299">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-299">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-300">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-300">Az.Cdn</span></span>
* <span data-ttu-id="83262-301">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="83262-301">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-302">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-302">Az.Compute</span></span>
* <span data-ttu-id="83262-303">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-303">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="83262-304">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="83262-304">Az.ContainerInstance</span></span>
* <span data-ttu-id="83262-305">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-305">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="83262-306">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="83262-306">Az.DataBoxEdge</span></span>
* <span data-ttu-id="83262-307">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-307">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="83262-308">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="83262-308">Get the Edge Storage Container</span></span>
* <span data-ttu-id="83262-309">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-309">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="83262-310">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-310">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="83262-311">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-311">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="83262-312">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-312">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="83262-313">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-313">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="83262-314">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="83262-314">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="83262-315">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-315">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="83262-316">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="83262-316">Get the Edge Storage Account</span></span>
* <span data-ttu-id="83262-317">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-317">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="83262-318">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-318">Create new Edge Storage Account</span></span>
* <span data-ttu-id="83262-319">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-319">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="83262-320">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-320">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="83262-321">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="83262-321">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="83262-322">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="83262-322">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="83262-323">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-323">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="83262-324">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="83262-324">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-325">Az.DataFactory</span></span>
* <span data-ttu-id="83262-326">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-326">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="83262-327">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-327">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="83262-328">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="83262-328">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="83262-329">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="83262-329">Az.DevTestLabs</span></span>
* <span data-ttu-id="83262-330">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-330">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-331">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-331">Az.EventHub</span></span>
* <span data-ttu-id="83262-332">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-332">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="83262-333">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-333">Az.HDInsight</span></span>
* <span data-ttu-id="83262-334">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-334">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="83262-335">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="83262-335">Az.MachineLearning</span></span>
* <span data-ttu-id="83262-336">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-336">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="83262-337">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="83262-337">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="83262-338">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="83262-338">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="83262-339">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="83262-339">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="83262-340">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="83262-340">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="83262-341">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="83262-341">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="83262-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="83262-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="83262-343">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="83262-343">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-344">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-344">Az.Network</span></span>
* <span data-ttu-id="83262-345">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="83262-345">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-346">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-346">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-347">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="83262-347">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="83262-348">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-348">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="83262-349">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-349">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="83262-350">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-350">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-351">Az.Resources</span></span>
* <span data-ttu-id="83262-352">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-352">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-353">Az.Sql</span></span>
* <span data-ttu-id="83262-354">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-354">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="83262-355">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-355">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="83262-356">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="83262-356">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="83262-357">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-357">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-358">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-358">Az.Storage</span></span>
* <span data-ttu-id="83262-359">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-359">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="83262-360">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-360">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="83262-361">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-361">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="83262-362">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-362">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="83262-363">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="83262-363">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="83262-364">全般</span><span class="sxs-lookup"><span data-stu-id="83262-364">General</span></span>
* <span data-ttu-id="83262-365">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="83262-365">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-366">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-366">Az.Accounts</span></span>
* <span data-ttu-id="83262-367">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="83262-367">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="83262-368">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="83262-368">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="83262-369">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-369">Az.Batch</span></span>
* <span data-ttu-id="83262-370">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="83262-370">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-371">Az.DataFactory</span></span>
* <span data-ttu-id="83262-372">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-372">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-373">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-374">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-374">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="83262-375">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="83262-375">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="83262-376">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="83262-376">Az.HealthcareApis</span></span>
* <span data-ttu-id="83262-377">例外処理</span><span class="sxs-lookup"><span data-stu-id="83262-377">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-378">Az.KeyVault</span></span>
* <span data-ttu-id="83262-379">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-379">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="83262-380">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="83262-380">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="83262-381">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-381">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-382">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-382">Az.Monitor</span></span>
* <span data-ttu-id="83262-383">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="83262-383">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="83262-384">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="83262-384">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="83262-385">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="83262-385">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-386">Az.Network</span></span>
* <span data-ttu-id="83262-387">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-387">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-388">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-388">Az.Resources</span></span>
* <span data-ttu-id="83262-389">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-389">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="83262-390">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-390">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-391">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-391">Az.Sql</span></span>
* <span data-ttu-id="83262-392">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="83262-392">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-393">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-393">Az.Storage</span></span>
* <span data-ttu-id="83262-394">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-394">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="83262-395">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="83262-395">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="83262-396">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="83262-396">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="83262-397">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="83262-397">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="83262-398">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="83262-398">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="83262-399">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="83262-399">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="83262-400">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-400">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="83262-401">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-401">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="83262-402">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-402">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="83262-403">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="83262-403">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="83262-404">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="83262-404">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="83262-405">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-405">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="83262-406">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="83262-406">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="83262-407">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="83262-407">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-408">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-408">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-409">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="83262-409">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="83262-410">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="83262-410">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-411">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-411">Az.Compute</span></span>
* <span data-ttu-id="83262-412">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="83262-412">VM Reapply feature</span></span>
    - <span data-ttu-id="83262-413">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-413">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="83262-414">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="83262-414">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="83262-415">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="83262-415">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="83262-416">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="83262-416">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="83262-417">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-417">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="83262-418">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-418">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="83262-419">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="83262-419">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="83262-420">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-420">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="83262-421">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-421">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="83262-422">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-422">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="83262-423">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="83262-423">Az.DataBoxEdge</span></span>
* <span data-ttu-id="83262-424">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-424">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="83262-425">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="83262-425">Get the Order</span></span>
* <span data-ttu-id="83262-426">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-426">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="83262-427">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="83262-427">Create new Order</span></span>
* <span data-ttu-id="83262-428">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-428">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="83262-429">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="83262-429">Remove the Order</span></span>
* <span data-ttu-id="83262-430">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="83262-430">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="83262-431">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="83262-431">Now creates Local Share</span></span>
* <span data-ttu-id="83262-432">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-432">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="83262-433">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-433">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="83262-434">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-434">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="83262-435">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="83262-435">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="83262-436">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-436">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="83262-437">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="83262-437">Gets the information about Triggers</span></span>
* <span data-ttu-id="83262-438">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-438">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="83262-439">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-439">Create new Triggers</span></span>
* <span data-ttu-id="83262-440">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-440">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="83262-441">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-441">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-442">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-442">Az.DataFactory</span></span>
* <span data-ttu-id="83262-443">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-443">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="83262-444">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-444">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-445">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-445">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-446">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="83262-446">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-447">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-447">Az.EventHub</span></span>
* <span data-ttu-id="83262-448">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-448">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-449">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-450">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-450">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="83262-451">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-451">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="83262-452">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-452">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="83262-453">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="83262-453">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-454">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-454">Az.Network</span></span>
* <span data-ttu-id="83262-455">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="83262-455">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="83262-456">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="83262-456">Az.PrivateDns</span></span>
* <span data-ttu-id="83262-457">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-457">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-458">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-458">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-459">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-459">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="83262-460">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="83262-460">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="83262-461">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-461">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="83262-462">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="83262-462">Az.RedisCache</span></span>
* <span data-ttu-id="83262-463">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-463">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="83262-464">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-464">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="83262-465">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-465">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-466">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-466">Az.Resources</span></span>
- <span data-ttu-id="83262-467">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-467">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="83262-468">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-468">Updated create policy definition help example</span></span>
- <span data-ttu-id="83262-469">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-469">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="83262-470">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-470">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="83262-471">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="83262-471">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-472">Az.Sql</span></span>
* <span data-ttu-id="83262-473">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-473">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="83262-474">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-474">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="83262-475">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="83262-475">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="83262-476">全般</span><span class="sxs-lookup"><span data-stu-id="83262-476">General</span></span>
* <span data-ttu-id="83262-477">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="83262-477">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-478">Az.Accounts</span></span>
* <span data-ttu-id="83262-479">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-479">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="83262-480">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="83262-480">Az.Advisor</span></span>
* <span data-ttu-id="83262-481">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-481">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="83262-482">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-482">Az.Batch</span></span>
* <span data-ttu-id="83262-483">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-483">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="83262-484">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="83262-484">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="83262-485">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="83262-485">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="83262-486">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="83262-486">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="83262-487">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="83262-487">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="83262-488">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="83262-488">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="83262-489">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="83262-489">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="83262-490">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="83262-490">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="83262-491">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="83262-491">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="83262-492">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-492">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="83262-493">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="83262-493">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="83262-494">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="83262-494">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="83262-495">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-495">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="83262-496">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-496">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="83262-497">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-497">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="83262-498">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-498">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="83262-499">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-499">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="83262-500">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-500">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="83262-501">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-501">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="83262-502">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83262-502">This operation is no longer supported.</span></span>
* <span data-ttu-id="83262-503">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-503">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="83262-504">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-504">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="83262-505">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-505">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="83262-506">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="83262-506">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="83262-507">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="83262-507">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="83262-508">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-508">New non-verified images are also now returned.</span></span> <span data-ttu-id="83262-509">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="83262-509">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="83262-510">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-510">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="83262-511">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-511">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="83262-512">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="83262-512">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="83262-513">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-513">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="83262-514">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="83262-514">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="83262-515">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-515">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="83262-516">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="83262-516">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="83262-517">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="83262-517">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="83262-518">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="83262-518">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-519">Az.Cdn</span></span>
* <span data-ttu-id="83262-520">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="83262-520">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="83262-521">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-521">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-522">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-522">Az.Compute</span></span>
* <span data-ttu-id="83262-523">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="83262-523">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="83262-524">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="83262-524">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="83262-525">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。 Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile、Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="83262-525">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="83262-526">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="83262-526">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="83262-527">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="83262-527">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="83262-528">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="83262-528">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="83262-529">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="83262-529">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="83262-530">重大な変更</span><span class="sxs-lookup"><span data-stu-id="83262-530">Breaking changes</span></span>
    - <span data-ttu-id="83262-531">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="83262-531">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="83262-532">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="83262-532">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-533">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-533">Az.DataFactory</span></span>
* <span data-ttu-id="83262-534">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-534">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-535">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-535">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-536">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="83262-536">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="83262-537">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="83262-537">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="83262-538">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="83262-538">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="83262-539">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-539">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="83262-540">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-540">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="83262-541">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-541">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-542">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-542">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-543">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-543">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="83262-544">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-544">Az.HDInsight</span></span>
* <span data-ttu-id="83262-545">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-545">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="83262-546">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="83262-546">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="83262-547">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-547">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="83262-548">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-548">Removed five cmdlets:</span></span>
    - <span data-ttu-id="83262-549">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="83262-549">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="83262-550">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="83262-550">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="83262-551">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="83262-551">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="83262-552">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="83262-552">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="83262-553">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="83262-553">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="83262-554">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-554">Added three cmdlets:</span></span>
    - <span data-ttu-id="83262-555">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="83262-555">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="83262-556">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="83262-556">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="83262-557">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="83262-557">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="83262-558">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-558">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="83262-559">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-559">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="83262-560">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-560">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="83262-561">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="83262-561">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="83262-562">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-562">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="83262-563">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-563">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="83262-564">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-564">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="83262-565">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-565">Added some scenario test cases.</span></span>
* <span data-ttu-id="83262-566">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="83262-566">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-567">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-567">Az.IotHub</span></span>
* <span data-ttu-id="83262-568">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="83262-568">Breaking changes:</span></span>
    - <span data-ttu-id="83262-569">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-569">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="83262-570">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-570">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="83262-571">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-571">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="83262-572">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-572">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="83262-573">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-573">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="83262-574">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-574">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="83262-575">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="83262-575">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="83262-576">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="83262-576">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="83262-577">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-577">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="83262-578">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-578">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="83262-579">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-579">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="83262-580">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="83262-580">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-581">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-581">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-582">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-582">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="83262-583">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-583">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="83262-584">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-584">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="83262-585">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-585">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="83262-586">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-586">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="83262-587">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-587">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="83262-588">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-588">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="83262-589">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-589">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="83262-590">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-590">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-591">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-591">Az.Resources</span></span>
* <span data-ttu-id="83262-592">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-592">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-593">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-593">Az.Network</span></span>
* <span data-ttu-id="83262-594">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="83262-594">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="83262-595">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-595">Updated cmdlet:</span></span>
        - <span data-ttu-id="83262-596">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-596">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-597">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-597">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-598">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-598">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-599">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-599">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-600">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-600">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="83262-601">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="83262-601">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="83262-602">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-602">New cmdlet:</span></span>
        - <span data-ttu-id="83262-603">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="83262-603">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="83262-604">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-604">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="83262-605">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-605">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="83262-606">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-606">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="83262-607">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-607">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="83262-608">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-608">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="83262-609">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-609">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="83262-610">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-610">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="83262-611">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-611">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-612">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="83262-612">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="83262-613">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-613">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="83262-614">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-614">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="83262-615">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-615">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="83262-616">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="83262-616">Set-AzVirtualHub</span></span>
* <span data-ttu-id="83262-617">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-617">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="83262-618">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-618">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="83262-619">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-619">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="83262-620">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-620">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="83262-621">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-621">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="83262-622">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-622">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="83262-623">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-623">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="83262-624">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-624">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-625">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="83262-625">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="83262-626">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-626">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="83262-627">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-627">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="83262-628">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-628">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="83262-629">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-629">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="83262-630">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-630">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="83262-631">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-631">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="83262-632">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-632">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="83262-633">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-633">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-634">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="83262-634">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="83262-635">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="83262-635">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="83262-636">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="83262-636">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="83262-637">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="83262-637">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="83262-638">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="83262-638">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="83262-639">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-639">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="83262-640">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-640">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="83262-641">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-641">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="83262-642">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-642">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="83262-643">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-643">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="83262-644">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-644">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="83262-645">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-645">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="83262-646">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-646">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="83262-647">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-647">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="83262-648">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="83262-648">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="83262-649">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="83262-649">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="83262-650">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-650">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="83262-651">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-651">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-652">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="83262-652">New-AzIpGroup</span></span>
        - <span data-ttu-id="83262-653">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="83262-653">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="83262-654">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="83262-654">Get-AzIpGroup</span></span>
        - <span data-ttu-id="83262-655">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="83262-655">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-656">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-656">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-657">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="83262-657">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-658">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-658">Az.Sql</span></span>
* <span data-ttu-id="83262-659">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-659">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="83262-660">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="83262-660">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="83262-661">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-661">Removed deprecated aliases:</span></span>
* <span data-ttu-id="83262-662">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="83262-662">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="83262-663">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="83262-663">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="83262-664">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-664">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="83262-665">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="83262-665">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="83262-666">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="83262-666">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="83262-667">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-667">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-668">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-668">Az.Storage</span></span>
* <span data-ttu-id="83262-669">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-669">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="83262-670">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-670">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="83262-671">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-671">Set-AzStorageAccount</span></span>
* <span data-ttu-id="83262-672">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="83262-672">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="83262-673">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="83262-673">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="83262-674">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="83262-674">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="83262-675">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="83262-675">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="83262-676">全般</span><span class="sxs-lookup"><span data-stu-id="83262-676">General</span></span>
* <span data-ttu-id="83262-677">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="83262-677">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-678">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-678">Az.Accounts</span></span>
* <span data-ttu-id="83262-679">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-679">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="83262-680">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-680">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-681">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-681">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="83262-682">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="83262-682">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-683">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-683">Az.Automation</span></span>
* <span data-ttu-id="83262-684">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-684">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="83262-685">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-685">Az.Batch</span></span>
* <span data-ttu-id="83262-686">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="83262-686">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-687">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-687">Az.Compute</span></span>
* <span data-ttu-id="83262-688">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-688">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="83262-689">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-689">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="83262-690">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-690">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="83262-691">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-691">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-692">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-692">Az.DataFactory</span></span>
* <span data-ttu-id="83262-693">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="83262-693">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="83262-694">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="83262-694">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="83262-695">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="83262-695">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-696">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-696">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-697">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-697">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="83262-698">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="83262-698">Az.HealthcareApis</span></span>
* <span data-ttu-id="83262-699">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-699">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="83262-700">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-700">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="83262-701">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="83262-701">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="83262-702">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-702">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-703">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-703">Az.IotHub</span></span>
* <span data-ttu-id="83262-704">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="83262-704">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="83262-705">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="83262-705">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-706">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-706">Az.Monitor</span></span>
* <span data-ttu-id="83262-707">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="83262-707">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="83262-708">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="83262-708">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="83262-709">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="83262-709">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="83262-710">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-710">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-711">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-711">Az.Network</span></span>
* <span data-ttu-id="83262-712">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-712">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="83262-713">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-713">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="83262-714">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-714">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-715">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-715">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="83262-716">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="83262-716">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="83262-717">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-717">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="83262-718">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-718">Updated cmdlets:</span></span>
        - <span data-ttu-id="83262-719">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-719">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="83262-720">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-720">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="83262-721">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-721">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="83262-722">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="83262-722">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="83262-723">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="83262-723">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="83262-724">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="83262-724">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="83262-725">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="83262-725">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="83262-726">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="83262-726">Az.RedisCache</span></span>
* <span data-ttu-id="83262-727">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-727">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-728">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-728">Az.Sql</span></span>
* <span data-ttu-id="83262-729">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-729">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-730">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-730">Az.Storage</span></span>
* <span data-ttu-id="83262-731">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="83262-731">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="83262-732">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83262-732">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="83262-733">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="83262-733">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="83262-734">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83262-734">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="83262-735">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-735">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="83262-736">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="83262-736">Az.StorageSync</span></span>
* <span data-ttu-id="83262-737">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-737">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-738">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-738">Az.Websites</span></span>
* <span data-ttu-id="83262-739">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="83262-739">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="83262-740">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="83262-740">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="83262-741">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-741">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-742">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-742">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="83262-743">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-743">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="83262-744">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="83262-744">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-745">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-745">Az.Automation</span></span>
* <span data-ttu-id="83262-746">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-746">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="83262-747">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-747">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="83262-748">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-748">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-749">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-749">Az.Compute</span></span>
* <span data-ttu-id="83262-750">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="83262-750">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="83262-751">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="83262-751">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="83262-752">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-752">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="83262-753">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="83262-753">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="83262-754">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="83262-754">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="83262-755">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-755">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="83262-756">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-756">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="83262-757">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-757">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="83262-758">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-758">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-759">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-759">Az.DataFactory</span></span>
* <span data-ttu-id="83262-760">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-760">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="83262-761">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-761">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="83262-762">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-762">Az.HDInsight</span></span>
* <span data-ttu-id="83262-763">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="83262-763">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-764">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-764">Az.IotHub</span></span>
* <span data-ttu-id="83262-765">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-765">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="83262-766">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-766">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="83262-767">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83262-767">New cmdlets are:</span></span>
    - <span data-ttu-id="83262-768">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="83262-768">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="83262-769">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="83262-769">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="83262-770">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="83262-770">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="83262-771">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="83262-771">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-772">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-772">Az.Monitor</span></span>
* <span data-ttu-id="83262-773">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="83262-773">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="83262-774">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="83262-774">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="83262-775">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="83262-775">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="83262-776">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="83262-776">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="83262-777">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="83262-777">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="83262-778">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="83262-778">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="83262-779">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="83262-779">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="83262-780">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="83262-780">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="83262-781">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-781">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="83262-782">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-782">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="83262-783">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-783">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="83262-784">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="83262-784">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="83262-785">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="83262-785">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="83262-786">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-786">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="83262-787">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-787">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="83262-788">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="83262-788">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="83262-789">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="83262-789">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="83262-790">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="83262-790">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="83262-791">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-791">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="83262-792">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-792">Overall improved help files</span></span>
* <span data-ttu-id="83262-793">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="83262-793">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-794">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-794">Az.Network</span></span>
* <span data-ttu-id="83262-795">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-795">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="83262-796">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="83262-796">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="83262-797">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="83262-797">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="83262-798">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-798">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="83262-799">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-799">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="83262-800">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-800">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="83262-801">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-801">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="83262-802">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-802">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="83262-803">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-803">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="83262-804">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-804">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="83262-805">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-805">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="83262-806">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="83262-806">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="83262-807">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-807">New cmdlets</span></span>
        - <span data-ttu-id="83262-808">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="83262-808">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="83262-809">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="83262-809">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="83262-810">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-810">Updated cmdlet:</span></span>
        - <span data-ttu-id="83262-811">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="83262-811">New-VpnSite</span></span>
        - <span data-ttu-id="83262-812">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="83262-812">Update-VpnSite</span></span>
        - <span data-ttu-id="83262-813">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="83262-813">New-VpnConnection</span></span>
        - <span data-ttu-id="83262-814">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="83262-814">Update-VpnConnection</span></span>
* <span data-ttu-id="83262-815">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-815">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-816">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-816">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-817">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-817">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="83262-818">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-818">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-819">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-819">Az.Resources</span></span>
* <span data-ttu-id="83262-820">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-820">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-821">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-821">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-822">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-822">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="83262-823">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-823">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="83262-824">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="83262-824">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="83262-825">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="83262-825">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="83262-826">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="83262-826">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="83262-827">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="83262-827">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="83262-828">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="83262-828">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="83262-829">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="83262-829">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="83262-830">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="83262-830">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="83262-831">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="83262-831">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="83262-832">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="83262-832">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="83262-833">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="83262-833">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="83262-834">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="83262-834">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="83262-835">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="83262-835">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="83262-836">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="83262-836">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="83262-837">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="83262-837">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="83262-838">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="83262-838">Az.SignalR</span></span>
* <span data-ttu-id="83262-839">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="83262-839">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-840">Az.Sql</span></span>
* <span data-ttu-id="83262-841">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="83262-841">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="83262-842">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-842">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="83262-843">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="83262-843">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="83262-844">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-844">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="83262-845">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="83262-845">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-846">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-846">Az.Storage</span></span>
* <span data-ttu-id="83262-847">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-847">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="83262-848">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-848">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="83262-849">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="83262-849">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="83262-850">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="83262-850">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="83262-851">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="83262-851">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="83262-852">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="83262-852">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="83262-853">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-853">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="83262-854">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-854">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="83262-855">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-855">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="83262-856">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-856">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="83262-857">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="83262-857">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-858">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-858">Az.Websites</span></span>
* <span data-ttu-id="83262-859">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-859">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="83262-860">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="83262-860">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="83262-861">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="83262-861">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="83262-862">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="83262-862">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="83262-863">全般</span><span class="sxs-lookup"><span data-stu-id="83262-863">General</span></span>
* <span data-ttu-id="83262-864">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-864">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-865">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-865">Az.Accounts</span></span>
* <span data-ttu-id="83262-866">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="83262-866">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="83262-867">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="83262-867">Az.Aks</span></span>
* <span data-ttu-id="83262-868">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-868">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="83262-869">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="83262-869">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="83262-870">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-870">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-871">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="83262-871">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="83262-872">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="83262-872">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="83262-873">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-873">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="83262-874">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="83262-874">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="83262-875">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-875">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="83262-876">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-876">Az.Batch</span></span>
* <span data-ttu-id="83262-877">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="83262-877">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-878">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-878">Az.Cdn</span></span>
* <span data-ttu-id="83262-879">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-879">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-880">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-880">Az.Compute</span></span>
* <span data-ttu-id="83262-881">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-881">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="83262-882">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-882">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="83262-883">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-883">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="83262-884">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-884">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="83262-885">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="83262-885">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="83262-886">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="83262-886">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="83262-887">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-887">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="83262-888">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-888">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-889">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-889">Az.DataFactory</span></span>
* <span data-ttu-id="83262-890">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-890">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="83262-891">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-891">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="83262-892">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-892">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="83262-893">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-893">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-894">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-894">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-895">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-895">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-896">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-896">Az.EventHub</span></span>
* <span data-ttu-id="83262-897">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="83262-897">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="83262-898">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="83262-898">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="83262-899">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-899">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="83262-900">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="83262-900">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="83262-901">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="83262-901">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="83262-902">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-902">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-903">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-903">Az.Monitor</span></span>
* <span data-ttu-id="83262-904">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-904">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-905">Az.Network</span></span>
* <span data-ttu-id="83262-906">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-906">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="83262-907">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="83262-907">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="83262-908">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-908">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="83262-909">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-909">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="83262-910">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="83262-910">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="83262-911">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-911">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="83262-912">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-912">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-913">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-913">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-914">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-914">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="83262-915">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-915">Added example</span></span>
    - <span data-ttu-id="83262-916">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-916">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="83262-917">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-917">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="83262-918">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-918">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-919">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-919">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-920">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-920">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-921">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-921">Az.Resources</span></span>
* <span data-ttu-id="83262-922">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-922">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="83262-923">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-923">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="83262-924">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="83262-924">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="83262-925">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-925">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-926">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-926">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-927">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="83262-927">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="83262-928">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="83262-928">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="83262-929">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-929">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-930">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-930">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-931">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-931">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="83262-932">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="83262-932">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="83262-933">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="83262-933">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="83262-934">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-934">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="83262-935">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="83262-935">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="83262-936">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="83262-936">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-937">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-937">Az.Sql</span></span>
* <span data-ttu-id="83262-938">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-938">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-939">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-939">Az.Storage</span></span>
* <span data-ttu-id="83262-940">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-940">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="83262-941">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-941">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="83262-942">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="83262-942">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="83262-943">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="83262-943">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="83262-944">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-944">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="83262-945">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="83262-945">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-946">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-946">Az.Websites</span></span>
* <span data-ttu-id="83262-947">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-947">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="83262-948">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="83262-948">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-949">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-949">Az.Accounts</span></span>
* <span data-ttu-id="83262-950">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-950">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="83262-951">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="83262-951">Az.ApplicationInsights</span></span>
* <span data-ttu-id="83262-952">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-952">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-953">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-953">Az.Automation</span></span>
* <span data-ttu-id="83262-954">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-954">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-955">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-955">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-956">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-956">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-957">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-957">Az.Compute</span></span>
* <span data-ttu-id="83262-958">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-958">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="83262-959">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="83262-959">Az.ContainerRegistry</span></span>
* <span data-ttu-id="83262-960">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-960">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="83262-961">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="83262-961">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-962">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-962">Az.DataFactory</span></span>
* <span data-ttu-id="83262-963">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-963">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="83262-964">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-964">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-965">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-965">Az.EventHub</span></span>
* <span data-ttu-id="83262-966">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="83262-966">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="83262-967">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-967">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-968">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-968">Az.KeyVault</span></span>
* <span data-ttu-id="83262-969">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-969">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="83262-970">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="83262-970">Az.LogicApp</span></span>
* <span data-ttu-id="83262-971">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-971">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="83262-972">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-972">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="83262-973">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="83262-973">Az.ManagedServices</span></span>
* <span data-ttu-id="83262-974">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-974">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-975">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-975">Az.Network</span></span>
* <span data-ttu-id="83262-976">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-976">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="83262-977">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-977">New cmdlets</span></span>
        - <span data-ttu-id="83262-978">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="83262-978">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="83262-979">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="83262-979">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="83262-980">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-980">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-981">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-981">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-982">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-982">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-983">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-983">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="83262-984">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="83262-984">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="83262-985">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="83262-985">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="83262-986">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="83262-986">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="83262-987">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-987">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="83262-988">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-988">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="83262-989">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-989">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="83262-990">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="83262-990">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="83262-991">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="83262-991">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="83262-992">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-992">Updated cmdlets</span></span>
        - <span data-ttu-id="83262-993">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-993">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="83262-994">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-994">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="83262-995">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-995">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="83262-996">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-996">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="83262-997">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-997">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="83262-998">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-998">Updated cmdlet:</span></span>
        - <span data-ttu-id="83262-999">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="83262-999">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="83262-1000">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1000">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="83262-1001">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1001">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="83262-1002">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="83262-1002">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="83262-1003">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1003">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="83262-1004">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="83262-1004">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1005">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1005">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-1006">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1006">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="83262-1007">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1007">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1008">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1008">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1009">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1009">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="83262-1010">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1010">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="83262-1011">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1011">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="83262-1012">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1012">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="83262-1013">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1013">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="83262-1014">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1014">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="83262-1015">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1015">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="83262-1016">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1016">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="83262-1017">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1017">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="83262-1018">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1018">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1019">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1019">Az.Resources</span></span>
- <span data-ttu-id="83262-1020">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1020">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="83262-1021">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1021">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-1022">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-1022">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-1023">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="83262-1023">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="83262-1024">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1024">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1025">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1025">Az.Sql</span></span>
* <span data-ttu-id="83262-1026">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1026">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="83262-1027">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1027">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="83262-1028">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1028">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1029">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1029">Az.Storage</span></span>
* <span data-ttu-id="83262-1030">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1030">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="83262-1031">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="83262-1031">Az.StorageSync</span></span>
* <span data-ttu-id="83262-1032">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1032">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="83262-1033">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1033">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1034">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1034">Az.Websites</span></span>
* <span data-ttu-id="83262-1035">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1035">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="83262-1036">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1036">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="83262-1037">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1037">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="83262-1038">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="83262-1038">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1039">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1039">Az.Accounts</span></span>
* <span data-ttu-id="83262-1040">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="83262-1040">Add support for profile cmdlets</span></span>
* <span data-ttu-id="83262-1041">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="83262-1041">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="83262-1042">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="83262-1042">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="83262-1043">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="83262-1043">Az.Advisor</span></span>
* <span data-ttu-id="83262-1044">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="83262-1044">GA release of Az.Advisor</span></span>
* <span data-ttu-id="83262-1045">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-1045">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="83262-1046">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-1046">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-1047">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="83262-1047">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="83262-1048">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="83262-1048">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="83262-1049">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1049">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="83262-1050">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1050">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="83262-1051">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="83262-1052">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="83262-1052">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="83262-1053">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1053">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1054">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1054">Az.Automation</span></span>
* <span data-ttu-id="83262-1055">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1055">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1056">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1056">Az.Compute</span></span>
* <span data-ttu-id="83262-1057">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="83262-1057">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-1058">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-1058">Az.DataFactory</span></span>
* <span data-ttu-id="83262-1059">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="83262-1059">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="83262-1060">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="83262-1060">Az.EventGrid</span></span>
* <span data-ttu-id="83262-1061">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1061">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-1062">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-1062">Az.IotHub</span></span>
* <span data-ttu-id="83262-1063">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1063">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1064">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1064">Az.Network</span></span>
* <span data-ttu-id="83262-1065">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1065">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="83262-1066">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-1066">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="83262-1067">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1067">Az.PolicyInsights</span></span>
* <span data-ttu-id="83262-1068">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1068">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="83262-1069">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="83262-1069">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1070">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1070">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-1071">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1071">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1072">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1072">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1073">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1073">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1074">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1074">Az.Resources</span></span>
    - <span data-ttu-id="83262-1075">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1075">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="83262-1076">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1076">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="83262-1077">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1077">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="83262-1078">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1078">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-1079">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-1079">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-1080">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="83262-1080">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1081">Az.Sql</span></span>
* <span data-ttu-id="83262-1082">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1082">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="83262-1083">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1083">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="83262-1084">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1084">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="83262-1085">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1085">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="83262-1086">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1086">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="83262-1087">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1087">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="83262-1088">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1088">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="83262-1089">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="83262-1089">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="83262-1090">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1090">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1091">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1091">Az.Storage</span></span>
* <span data-ttu-id="83262-1092">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1092">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="83262-1093">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="83262-1093">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="83262-1094">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1094">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="83262-1095">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="83262-1095">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="83262-1096">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1096">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="83262-1097">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1097">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="83262-1098">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1098">Set-AzStorageAccount</span></span>
* <span data-ttu-id="83262-1099">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1099">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="83262-1100">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="83262-1100">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="83262-1101">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="83262-1101">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="83262-1102">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="83262-1102">Az.StorageSync</span></span>
* <span data-ttu-id="83262-1103">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-1103">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="83262-1104">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="83262-1104">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1105">Az.Accounts</span></span>
* <span data-ttu-id="83262-1106">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1106">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="83262-1107">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="83262-1107">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="83262-1108">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1108">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="83262-1109">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="83262-1109">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="83262-1110">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="83262-1110">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1111">Az.Compute</span></span>
* <span data-ttu-id="83262-1112">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1112">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="83262-1113">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1113">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="83262-1114">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="83262-1114">Az.Dns</span></span>
* <span data-ttu-id="83262-1115">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1115">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="83262-1116">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="83262-1116">Az.EventGrid</span></span>
* <span data-ttu-id="83262-1117">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1117">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="83262-1118">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-1118">New cmdlets:</span></span>
    - <span data-ttu-id="83262-1119">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="83262-1119">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="83262-1120">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="83262-1120">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="83262-1121">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="83262-1121">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="83262-1122">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="83262-1122">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="83262-1123">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="83262-1123">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="83262-1124">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="83262-1124">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="83262-1125">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="83262-1125">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="83262-1126">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="83262-1126">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="83262-1127">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="83262-1127">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="83262-1128">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="83262-1128">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="83262-1129">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="83262-1129">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="83262-1130">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="83262-1130">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="83262-1131">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="83262-1131">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="83262-1132">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="83262-1132">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="83262-1133">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="83262-1133">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="83262-1134">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="83262-1134">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="83262-1135">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-1135">Updated cmdlets:</span></span>
    - <span data-ttu-id="83262-1136">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="83262-1136">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="83262-1137">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1137">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="83262-1138">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1138">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="83262-1139">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="83262-1139">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="83262-1140">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="83262-1140">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="83262-1141">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="83262-1141">Event subscription expiration date,</span></span>
            - <span data-ttu-id="83262-1142">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="83262-1142">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="83262-1143">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1143">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="83262-1144">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="83262-1144">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="83262-1145">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="83262-1145">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="83262-1146">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1146">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="83262-1147">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="83262-1147">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="83262-1148">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1148">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="83262-1149">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1149">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-1150">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-1150">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-1151">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="83262-1151">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="83262-1152">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1152">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="83262-1153">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="83262-1153">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="83262-1154">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1154">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1155">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1155">Az.Network</span></span>
* <span data-ttu-id="83262-1156">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1156">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="83262-1157">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1157">New cmdlets</span></span>
        - <span data-ttu-id="83262-1158">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="83262-1158">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="83262-1159">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1159">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="83262-1160">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1160">New cmdlets</span></span>
        - <span data-ttu-id="83262-1161">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="83262-1161">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="83262-1162">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1162">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="83262-1163">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1163">New cmdlets</span></span>
        - <span data-ttu-id="83262-1164">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="83262-1164">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="83262-1165">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="83262-1165">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="83262-1166">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="83262-1166">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="83262-1167">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1167">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="83262-1168">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="83262-1168">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="83262-1169">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1169">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="83262-1170">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1170">New cmdlets</span></span>
        - <span data-ttu-id="83262-1171">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="83262-1171">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="83262-1172">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="83262-1172">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="83262-1173">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="83262-1173">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="83262-1174">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="83262-1174">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="83262-1175">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="83262-1175">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="83262-1176">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1176">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="83262-1177">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1177">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="83262-1178">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1178">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="83262-1179">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1179">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="83262-1180">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1180">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="83262-1181">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1181">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="83262-1182">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1182">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="83262-1183">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1183">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="83262-1184">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1184">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="83262-1185">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1185">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="83262-1186">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1186">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="83262-1187">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1187">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="83262-1188">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1188">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="83262-1189">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="83262-1189">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="83262-1190">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1190">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="83262-1191">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1191">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="83262-1192">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="83262-1192">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="83262-1193">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="83262-1193">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="83262-1194">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1194">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="83262-1195">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1195">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="83262-1196">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1196">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="83262-1197">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1197">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1198">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1198">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-1199">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="83262-1199">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1200">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1200">Az.Resources</span></span>
* <span data-ttu-id="83262-1201">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="83262-1201">Support for additional Template Export options</span></span>
    - <span data-ttu-id="83262-1202">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1202">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="83262-1203">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1203">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="83262-1204">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1204">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-1205">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-1205">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-1206">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1206">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1207">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1207">Az.Sql</span></span>
* <span data-ttu-id="83262-1208">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1208">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="83262-1209">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1209">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="83262-1210">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="83262-1210">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="83262-1211">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="83262-1211">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="83262-1212">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="83262-1212">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="83262-1213">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="83262-1213">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="83262-1214">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="83262-1214">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="83262-1215">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="83262-1215">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1216">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1216">Az.Storage</span></span>
* <span data-ttu-id="83262-1217">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1217">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="83262-1218">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1218">New-AzStorageAccount</span></span>
* <span data-ttu-id="83262-1219">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="83262-1219">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="83262-1220">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1220">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1221">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1221">Az.Websites</span></span>
* <span data-ttu-id="83262-1222">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="83262-1222">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="83262-1223">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1223">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="83262-1224">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="83262-1224">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="83262-1225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-1225">Az.Cdn</span></span>
* <span data-ttu-id="83262-1226">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1226">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1227">Az.Compute</span></span>
* <span data-ttu-id="83262-1228">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1228">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="83262-1229">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="83262-1229">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-1230">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-1230">Az.EventHub</span></span>
* <span data-ttu-id="83262-1231">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1231">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="83262-1232">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1232">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1233">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1233">Az.Network</span></span>
* <span data-ttu-id="83262-1234">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1234">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="83262-1235">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1235">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="83262-1236">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1236">Az.PolicyInsights</span></span>
* <span data-ttu-id="83262-1237">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1237">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1238">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1238">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1239">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1239">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-1240">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-1240">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-1241">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1241">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-1242">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-1242">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-1243">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1243">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="83262-1244">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1244">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1245">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1245">Az.Sql</span></span>
* <span data-ttu-id="83262-1246">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1246">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="83262-1247">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="83262-1247">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="83262-1248">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1248">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="83262-1249">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1249">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1250">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1250">Az.Websites</span></span>
* <span data-ttu-id="83262-1251">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1251">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="83262-1252">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="83262-1252">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="83262-1253">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-1253">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-1254">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="83262-1254">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="83262-1255">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="83262-1255">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="83262-1256">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="83262-1256">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="83262-1257">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="83262-1257">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="83262-1258">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="83262-1258">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="83262-1259">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="83262-1259">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="83262-1260">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-1260">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="83262-1261">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="83262-1261">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="83262-1262">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="83262-1262">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="83262-1263">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="83262-1263">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="83262-1264">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-1264">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="83262-1265">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-1265">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="83262-1266">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="83262-1266">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="83262-1267">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1267">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="83262-1268">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="83262-1268">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="83262-1269">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="83262-1269">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="83262-1270">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="83262-1270">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="83262-1271">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="83262-1271">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="83262-1272">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1272">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="83262-1273">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="83262-1273">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="83262-1274">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="83262-1274">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="83262-1275">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="83262-1275">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="83262-1276">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="83262-1276">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="83262-1277">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1277">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="83262-1278">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1278">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="83262-1279">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1279">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="83262-1280">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="83262-1280">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="83262-1281">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="83262-1281">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="83262-1282">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1282">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="83262-1283">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1283">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="83262-1284">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1284">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="83262-1285">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="83262-1285">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="83262-1286">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1286">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="83262-1287">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1287">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="83262-1288">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="83262-1288">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="83262-1289">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="83262-1289">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="83262-1290">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="83262-1290">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="83262-1291">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1291">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="83262-1292">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1292">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="83262-1293">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1293">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="83262-1294">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="83262-1294">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="83262-1295">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="83262-1295">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="83262-1296">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="83262-1296">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="83262-1297">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1297">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="83262-1298">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1298">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="83262-1299">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="83262-1299">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="83262-1300">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="83262-1300">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="83262-1301">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1301">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="83262-1302">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1302">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="83262-1303">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="83262-1303">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="83262-1304">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="83262-1304">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="83262-1305">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="83262-1305">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="83262-1306">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="83262-1306">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="83262-1307">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1307">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="83262-1308">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="83262-1308">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="83262-1309">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="83262-1309">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="83262-1310">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1310">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="83262-1311">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="83262-1311">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="83262-1312">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="83262-1312">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="83262-1313">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1313">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="83262-1314">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1314">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="83262-1315">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="83262-1315">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="83262-1316">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="83262-1316">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="83262-1317">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1317">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="83262-1318">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1318">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="83262-1319">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="83262-1319">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="83262-1320">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="83262-1320">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="83262-1321">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="83262-1321">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="83262-1322">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="83262-1322">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="83262-1323">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="83262-1323">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="83262-1324">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="83262-1324">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="83262-1325">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="83262-1325">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="83262-1326">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="83262-1326">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="83262-1327">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="83262-1327">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="83262-1328">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="83262-1328">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="83262-1329">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="83262-1329">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="83262-1330">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="83262-1330">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1331">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1331">Az.Automation</span></span>
* <span data-ttu-id="83262-1332">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1332">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="83262-1333">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="83262-1333">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="83262-1334">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="83262-1334">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="83262-1335">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1335">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="83262-1336">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="83262-1336">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="83262-1337">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1337">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="83262-1338">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1338">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1339">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1339">Az.Compute</span></span>
* <span data-ttu-id="83262-1340">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1340">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="83262-1341">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-1341">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-1342">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1342">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-1343">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1343">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-1344">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-1344">Az.Monitor</span></span>
* <span data-ttu-id="83262-1345">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1345">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1346">Az.Network</span></span>
* <span data-ttu-id="83262-1347">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1347">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="83262-1348">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="83262-1348">Updated cmdlet:</span></span>
        - <span data-ttu-id="83262-1349">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-1349">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="83262-1350">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1350">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1351">Az.Resources</span></span>
* <span data-ttu-id="83262-1352">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1352">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1353">Az.Sql</span></span>
* <span data-ttu-id="83262-1354">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="83262-1354">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="83262-1355">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="83262-1355">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1356">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1356">Az.Accounts</span></span>
* <span data-ttu-id="83262-1357">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1357">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-1358">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-1358">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-1359">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="83262-1359">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="83262-1360">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1360">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1361">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1361">Az.Compute</span></span>
* <span data-ttu-id="83262-1362">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="83262-1362">Proximity placement group feature.</span></span>
    - <span data-ttu-id="83262-1363">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="83262-1363">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="83262-1364">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1364">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="83262-1365">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1365">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="83262-1366">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1366">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="83262-1367">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1367">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="83262-1368">重大な変更</span><span class="sxs-lookup"><span data-stu-id="83262-1368">Breaking changes</span></span>
    - <span data-ttu-id="83262-1369">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="83262-1369">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="83262-1370">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="83262-1370">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="83262-1371">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="83262-1371">Az.DeploymentManager</span></span>
* <span data-ttu-id="83262-1372">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="83262-1372">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="83262-1373">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="83262-1373">Az.Dns</span></span>
* <span data-ttu-id="83262-1374">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="83262-1374">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="83262-1375">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="83262-1375">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="83262-1376">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1376">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="83262-1377">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-1377">Az.FrontDoor</span></span>
* <span data-ttu-id="83262-1378">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="83262-1378">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="83262-1379">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="83262-1379">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="83262-1380">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-1380">Az.HDInsight</span></span>
* <span data-ttu-id="83262-1381">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1381">Removed two cmdlets:</span></span>
    - <span data-ttu-id="83262-1382">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="83262-1382">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="83262-1383">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="83262-1383">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="83262-1384">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1384">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="83262-1385">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1385">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="83262-1386">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="83262-1386">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="83262-1387">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="83262-1387">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-1388">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-1388">Az.Monitor</span></span>
* <span data-ttu-id="83262-1389">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="83262-1389">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="83262-1390">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="83262-1390">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="83262-1391">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="83262-1391">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="83262-1392">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="83262-1392">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="83262-1393">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="83262-1393">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="83262-1394">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="83262-1394">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="83262-1395">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="83262-1395">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="83262-1396">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="83262-1396">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="83262-1397">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="83262-1397">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="83262-1398">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="83262-1398">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="83262-1399">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="83262-1399">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="83262-1400">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="83262-1400">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="83262-1401">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="83262-1401">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="83262-1402">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1402">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1403">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1403">Az.Network</span></span>
* <span data-ttu-id="83262-1404">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1404">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="83262-1405">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1405">New cmdlets</span></span>
        - <span data-ttu-id="83262-1406">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="83262-1406">New-AzNatGateway</span></span>
        - <span data-ttu-id="83262-1407">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="83262-1407">Get-AzNatGateway</span></span>
        - <span data-ttu-id="83262-1408">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="83262-1408">Set-AzNatGateway</span></span>
        - <span data-ttu-id="83262-1409">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="83262-1409">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="83262-1410">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1410">Updated cmdlets</span></span>
        - <span data-ttu-id="83262-1411">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="83262-1411">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="83262-1412">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="83262-1412">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="83262-1413">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="83262-1413">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="83262-1414">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1414">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="83262-1415">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1415">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="83262-1416">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1416">Az.PolicyInsights</span></span>
* <span data-ttu-id="83262-1417">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-1417">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="83262-1418">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1418">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="83262-1419">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="83262-1419">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1420">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1420">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1421">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-1421">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="83262-1422">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="83262-1422">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="83262-1423">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="83262-1423">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="83262-1424">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="83262-1424">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="83262-1425">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="83262-1425">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="83262-1426">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="83262-1426">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="83262-1427">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="83262-1427">Az.Relay</span></span>
* <span data-ttu-id="83262-1428">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1428">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-1429">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-1429">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-1430">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1430">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1431">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1431">Az.Storage</span></span>
* <span data-ttu-id="83262-1432">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="83262-1432">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="83262-1433">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="83262-1433">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="83262-1434">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1434">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="83262-1435">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1435">New-AzStorageAccount</span></span>
* <span data-ttu-id="83262-1436">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="83262-1436">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="83262-1437">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1437">New-AzStorageAccount</span></span>
    - <span data-ttu-id="83262-1438">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1438">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="83262-1439">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="83262-1439">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1440">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1440">Az.Websites</span></span>
* <span data-ttu-id="83262-1441">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="83262-1441">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="83262-1442">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="83262-1442">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="83262-1443">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="83262-1443">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-1444">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-1444">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-1445">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="83262-1445">General availability of `Az` module</span></span>
* <span data-ttu-id="83262-1446">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="83262-1446">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="83262-1447">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="83262-1447">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="83262-1448">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1448">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="83262-1449">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="83262-1449">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="83262-1450">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1450">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="83262-1451">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1451">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-1452">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1452">Az.Accounts</span></span>
* <span data-ttu-id="83262-1453">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1453">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="83262-1454">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-1454">Az.Batch</span></span>
* <span data-ttu-id="83262-1455">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1455">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-1456">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-1456">Az.Cdn</span></span>
* <span data-ttu-id="83262-1457">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1457">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-1458">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-1458">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-1459">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1459">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1460">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1460">Az.Compute</span></span>
* <span data-ttu-id="83262-1461">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1461">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="83262-1462">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1462">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1463">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1463">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-1464">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-1464">Az.DataFactory</span></span>
* <span data-ttu-id="83262-1465">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1465">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-1466">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1466">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-1467">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1467">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="83262-1468">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="83262-1468">Az.EventGrid</span></span>
* <span data-ttu-id="83262-1469">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1469">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-1470">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-1470">Az.EventHub</span></span>
* <span data-ttu-id="83262-1471">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1471">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="83262-1472">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="83262-1472">Az.HDInsight</span></span>
* <span data-ttu-id="83262-1473">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1473">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-1474">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-1474">Az.IotHub</span></span>
* <span data-ttu-id="83262-1475">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1475">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-1476">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-1476">Az.KeyVault</span></span>
* <span data-ttu-id="83262-1477">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1477">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1478">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1478">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="83262-1479">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="83262-1479">Az.MachineLearning</span></span>
* <span data-ttu-id="83262-1480">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1480">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="83262-1481">Az.Media</span><span class="sxs-lookup"><span data-stu-id="83262-1481">Az.Media</span></span>
* <span data-ttu-id="83262-1482">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1482">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-1483">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-1483">Az.Monitor</span></span>
  * <span data-ttu-id="83262-1484">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1484">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="83262-1485">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="83262-1485">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="83262-1486">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="83262-1486">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="83262-1487">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="83262-1487">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="83262-1488">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="83262-1488">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="83262-1489">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="83262-1489">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="83262-1490">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1490">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1491">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1491">Az.Network</span></span>
* <span data-ttu-id="83262-1492">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1492">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1493">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1493">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="83262-1494">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="83262-1494">Az.NotificationHubs</span></span>
* <span data-ttu-id="83262-1495">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1495">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1496">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1496">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-1497">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1497">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="83262-1498">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="83262-1498">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="83262-1499">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1499">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1500">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1500">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1501">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1501">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1502">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1502">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="83262-1503">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1503">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="83262-1504">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1504">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="83262-1505">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="83262-1505">Az.RedisCache</span></span>
* <span data-ttu-id="83262-1506">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1506">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1507">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1507">Az.Resources</span></span>
* <span data-ttu-id="83262-1508">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1508">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1509">Az.Sql</span></span>
* <span data-ttu-id="83262-1510">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="83262-1510">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="83262-1511">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1511">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1512">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1512">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="83262-1513">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="83262-1513">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="83262-1514">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="83262-1514">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="83262-1515">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="83262-1515">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="83262-1516">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1516">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1517">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1517">Az.Websites</span></span>
* <span data-ttu-id="83262-1518">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1518">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="83262-1519">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1519">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="83262-1520">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1520">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="83262-1521">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1521">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="83262-1522">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="83262-1522">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-1523">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-1523">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-1524">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="83262-1524">General availability of `Az` module</span></span>
* <span data-ttu-id="83262-1525">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="83262-1525">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="83262-1526">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="83262-1526">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="83262-1527">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1527">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="83262-1528">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="83262-1528">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="83262-1529">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1529">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="83262-1530">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1530">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="83262-1531">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1531">Az.Accounts</span></span>
* <span data-ttu-id="83262-1532">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1532">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="83262-1533">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="83262-1533">Az.AnalysisServices</span></span>
* <span data-ttu-id="83262-1534">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="83262-1534">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="83262-1535">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="83262-1535">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1536">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1536">Az.Automation</span></span>
* <span data-ttu-id="83262-1537">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1537">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="83262-1538">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1538">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="83262-1539">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1539">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1540">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1540">Az.Compute</span></span>
* <span data-ttu-id="83262-1541">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1541">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="83262-1542">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1542">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="83262-1543">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1543">Az.ContainerInstance</span></span>
* <span data-ttu-id="83262-1544">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1544">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-1545">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-1545">Az.DataFactory</span></span>
* <span data-ttu-id="83262-1546">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1546">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="83262-1547">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1547">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1548">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1548">Az.Resources</span></span>
* <span data-ttu-id="83262-1549">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-1549">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="83262-1550">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-1550">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="83262-1551">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="83262-1551">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="83262-1552">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="83262-1552">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="83262-1553">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1553">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="83262-1554">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="83262-1554">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1555">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1555">Az.Sql</span></span>
* <span data-ttu-id="83262-1556">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="83262-1556">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1557">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1557">Az.Storage</span></span>
* <span data-ttu-id="83262-1558">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="83262-1558">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="83262-1559">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="83262-1559">New-AzStorageContext</span></span>
* <span data-ttu-id="83262-1560">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="83262-1560">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="83262-1561">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="83262-1561">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="83262-1562">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="83262-1562">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="83262-1563">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1563">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="83262-1564">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1564">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="83262-1565">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="83262-1565">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="83262-1566">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="83262-1566">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="83262-1567">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="83262-1567">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="83262-1568">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="83262-1568">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="83262-1569">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="83262-1569">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="83262-1570">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="83262-1570">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="83262-1571">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="83262-1571">Highlights since the last major release</span></span>
* <span data-ttu-id="83262-1572">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="83262-1572">General availability of `Az` module</span></span>
* <span data-ttu-id="83262-1573">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="83262-1573">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="83262-1574">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="83262-1574">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="83262-1575">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1575">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="83262-1576">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="83262-1576">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="83262-1577">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1577">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="83262-1578">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1578">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1579">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1579">Az.Automation</span></span>
* <span data-ttu-id="83262-1580">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="83262-1580">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="83262-1581">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="83262-1581">Dynamic grouping</span></span>
    * <span data-ttu-id="83262-1582">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="83262-1582">Pre-Post script</span></span>
    * <span data-ttu-id="83262-1583">再起動設定</span><span class="sxs-lookup"><span data-stu-id="83262-1583">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1584">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1584">Az.Compute</span></span>
* <span data-ttu-id="83262-1585">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1585">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="83262-1586">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1586">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-1587">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-1587">Az.KeyVault</span></span>
* <span data-ttu-id="83262-1588">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1588">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1589">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1589">Az.Network</span></span>
* <span data-ttu-id="83262-1590">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1590">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="83262-1591">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1591">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1592">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1592">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1593">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1593">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="83262-1594">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1594">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1595">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1595">Az.Resources</span></span>
* <span data-ttu-id="83262-1596">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="83262-1596">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="83262-1597">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1597">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1598">Az.Sql</span></span>
* <span data-ttu-id="83262-1599">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1599">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1600">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1600">Az.Storage</span></span>
* <span data-ttu-id="83262-1601">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1601">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="83262-1602">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1602">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="83262-1603">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1603">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="83262-1604">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="83262-1604">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="83262-1605">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="83262-1605">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="83262-1606">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="83262-1606">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="83262-1607">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="83262-1607">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1608">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1608">Az.Websites</span></span>
* <span data-ttu-id="83262-1609">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1609">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="83262-1610">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="83262-1610">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1611">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1611">Az.Accounts</span></span>
* <span data-ttu-id="83262-1612">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1612">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="83262-1613">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1613">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1614">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1614">Az.Automation</span></span>
* <span data-ttu-id="83262-1615">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1615">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="83262-1616">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1616">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="83262-1617">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="83262-1617">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-1618">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-1618">Az.Cdn</span></span>
* <span data-ttu-id="83262-1619">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="83262-1619">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1620">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1620">Az.Compute</span></span>
* <span data-ttu-id="83262-1621">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1621">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-1622">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-1622">Az.DataFactory</span></span>
* <span data-ttu-id="83262-1623">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1623">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="83262-1624">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="83262-1624">Az.LogicApp</span></span>
* <span data-ttu-id="83262-1625">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1625">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1626">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1626">Az.Network</span></span>
* <span data-ttu-id="83262-1627">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1627">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1628">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1628">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1629">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1629">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="83262-1630">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="83262-1630">SDK Update</span></span>
* <span data-ttu-id="83262-1631">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1631">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="83262-1632">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1632">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1633">Az.Resources</span></span>
* <span data-ttu-id="83262-1634">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1634">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="83262-1635">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="83262-1635">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="83262-1636">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1636">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="83262-1637">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="83262-1637">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="83262-1638">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1638">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="83262-1639">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="83262-1639">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1640">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1640">Az.Sql</span></span>
* <span data-ttu-id="83262-1641">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1641">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="83262-1642">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1642">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1643">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1643">Az.Storage</span></span>
* <span data-ttu-id="83262-1644">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="83262-1644">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="83262-1645">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="83262-1645">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="83262-1646">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="83262-1646">Az.AnalysisServices</span></span>
* <span data-ttu-id="83262-1647">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="83262-1647">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1648">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1648">Az.Automation</span></span>
* <span data-ttu-id="83262-1649">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1649">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="83262-1650">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1650">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="83262-1651">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="83262-1651">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-1652">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-1652">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-1653">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="83262-1653">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1654">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1654">Az.Compute</span></span>
* <span data-ttu-id="83262-1655">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1655">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="83262-1656">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1656">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="83262-1657">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1657">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="83262-1658">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="83262-1658">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-1659">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1659">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-1660">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1660">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="83262-1661">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="83262-1661">Az.EventHub</span></span>
* <span data-ttu-id="83262-1662">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1662">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-1663">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-1663">Az.KeyVault</span></span>
* <span data-ttu-id="83262-1664">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1664">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="83262-1665">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="83262-1665">Az.LogicApp</span></span>
* <span data-ttu-id="83262-1666">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1666">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="83262-1667">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1667">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="83262-1668">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1668">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="83262-1669">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="83262-1669">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="83262-1670">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="83262-1670">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="83262-1671">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="83262-1671">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="83262-1672">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="83262-1672">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="83262-1673">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1673">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="83262-1674">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-1674">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="83262-1675">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-1675">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="83262-1676">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-1676">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="83262-1677">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-1677">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="83262-1678">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1678">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="83262-1679">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-1679">Az.Monitor</span></span>
* <span data-ttu-id="83262-1680">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1680">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1681">Az.Network</span></span>
* <span data-ttu-id="83262-1682">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1682">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1683">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1683">Az.OperationalInsights</span></span>
* <span data-ttu-id="83262-1684">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1684">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="83262-1685">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1685">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="83262-1686">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1686">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1687">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1687">Az.Resources</span></span>
* <span data-ttu-id="83262-1688">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="83262-1688">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="83262-1689">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="83262-1689">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="83262-1690">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="83262-1690">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="83262-1691">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1691">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1692">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1692">Az.Sql</span></span>
* <span data-ttu-id="83262-1693">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1693">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="83262-1694">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1694">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1695">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1695">Az.Websites</span></span>
* <span data-ttu-id="83262-1696">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1696">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="83262-1697">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="83262-1697">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1698">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1698">Az.Accounts</span></span>
* <span data-ttu-id="83262-1699">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="83262-1699">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="83262-1700">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="83262-1700">Az.AnalysisServices</span></span>
<span data-ttu-id="83262-1701">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="83262-1701">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1702">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1702">Az.Compute</span></span>
* <span data-ttu-id="83262-1703">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1703">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="83262-1704">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1704">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="83262-1705">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1705">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1706">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1706">Az.RecoveryServices</span></span>
<span data-ttu-id="83262-1707">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="83262-1707">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1708">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1708">Az.Resources</span></span>
* <span data-ttu-id="83262-1709">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1709">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="83262-1710">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="83262-1710">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="83262-1711">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1711">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="83262-1712">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="83262-1712">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1713">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1713">Az.Sql</span></span>
* <span data-ttu-id="83262-1714">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="83262-1714">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="83262-1715">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1715">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="83262-1716">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1716">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="83262-1717">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="83262-1717">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1718">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1718">Az.Accounts</span></span>
* <span data-ttu-id="83262-1719">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="83262-1719">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="83262-1720">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="83262-1720">Az.AnalysisServices</span></span>
* <span data-ttu-id="83262-1721">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="83262-1721">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1722">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1722">Az.RecoveryServices</span></span>
* <span data-ttu-id="83262-1723">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="83262-1723">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="83262-1724">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="83262-1724">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1725">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1725">Az.Accounts</span></span>
* <span data-ttu-id="83262-1726">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="83262-1726">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="83262-1727">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1727">Update incorrect online help URLs</span></span>
* <span data-ttu-id="83262-1728">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1728">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="83262-1729">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="83262-1729">Az.Aks</span></span>
* <span data-ttu-id="83262-1730">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1730">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="83262-1731">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1731">Az.Automation</span></span>
* <span data-ttu-id="83262-1732">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1732">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="83262-1733">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1733">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="83262-1734">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="83262-1734">Az.Cdn</span></span>
* <span data-ttu-id="83262-1735">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1735">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1736">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1736">Az.Compute</span></span>
* <span data-ttu-id="83262-1737">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="83262-1737">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="83262-1738">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="83262-1738">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="83262-1739">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1739">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="83262-1740">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="83262-1740">Az.ContainerRegistry</span></span>
* <span data-ttu-id="83262-1741">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1741">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="83262-1742">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83262-1742">Az.DataFactory</span></span>
* <span data-ttu-id="83262-1743">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="83262-1743">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-1744">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1744">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-1745">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="83262-1745">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="83262-1746">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="83262-1746">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="83262-1747">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1747">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-1748">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-1748">Az.IotHub</span></span>
* <span data-ttu-id="83262-1749">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="83262-1749">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="83262-1750">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-1750">Az.KeyVault</span></span>
* <span data-ttu-id="83262-1751">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1751">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-1752">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1752">Az.Network</span></span>
* <span data-ttu-id="83262-1753">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1753">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1754">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1754">Az.Resources</span></span>
* <span data-ttu-id="83262-1755">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1755">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="83262-1756">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1756">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="83262-1757">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1757">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="83262-1758">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="83262-1758">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="83262-1759">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="83262-1759">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="83262-1760">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1760">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="83262-1761">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="83262-1761">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-1762">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-1762">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-1763">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="83262-1763">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="83262-1764">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="83262-1764">Fix some error messages.</span></span>
* <span data-ttu-id="83262-1765">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1765">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="83262-1766">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1766">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="83262-1767">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="83262-1767">Az.SignalR</span></span>
* <span data-ttu-id="83262-1768">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1768">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1769">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1769">Az.Sql</span></span>
* <span data-ttu-id="83262-1770">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1770">Update incorrect online help URLs</span></span>
* <span data-ttu-id="83262-1771">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1771">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="83262-1772">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1772">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="83262-1773">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1773">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1774">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1774">Az.Storage</span></span>
* <span data-ttu-id="83262-1775">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1775">Update incorrect online help URLs</span></span>
* <span data-ttu-id="83262-1776">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="83262-1776">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="83262-1777">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="83262-1777">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="83262-1778">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="83262-1778">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="83262-1779">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="83262-1779">Az.TrafficManager</span></span>
* <span data-ttu-id="83262-1780">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1780">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1781">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1781">Az.Websites</span></span>
* <span data-ttu-id="83262-1782">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="83262-1782">Update incorrect online help URLs</span></span>
* <span data-ttu-id="83262-1783">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1783">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="83262-1784">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="83262-1784">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="83262-1785">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="83262-1785">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="83262-1786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1786">Az.Accounts</span></span>
* <span data-ttu-id="83262-1787">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="83262-1787">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-1788">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1788">Az.Compute</span></span>
* <span data-ttu-id="83262-1789">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1789">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="83262-1790">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="83262-1790">Updated the description of ID in help files</span></span>
* <span data-ttu-id="83262-1791">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1791">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-1792">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1792">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-1793">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1793">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="83262-1794">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1794">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="83262-1795">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="83262-1795">Az.EventGrid</span></span>
* <span data-ttu-id="83262-1796">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1796">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="83262-1797">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="83262-1797">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="83262-1798">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="83262-1798">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="83262-1799">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="83262-1799">Event Time-To-Live,</span></span>
        - <span data-ttu-id="83262-1800">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="83262-1800">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="83262-1801">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="83262-1801">Dead letter endpoint.</span></span>
    - <span data-ttu-id="83262-1802">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="83262-1802">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="83262-1803">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="83262-1803">Event Time-To-Live,</span></span>
        - <span data-ttu-id="83262-1804">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="83262-1804">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="83262-1805">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="83262-1805">Dead letter endpoint.</span></span>
* <span data-ttu-id="83262-1806">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1806">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="83262-1807">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="83262-1807">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="83262-1808">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="83262-1808">Az.IotHub</span></span>
* <span data-ttu-id="83262-1809">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1809">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="83262-1810">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="83262-1810">Az.LogicApp</span></span>
* <span data-ttu-id="83262-1811">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="83262-1811">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-1812">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1812">Az.Resources</span></span>
* <span data-ttu-id="83262-1813">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1813">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="83262-1814">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="83262-1814">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="83262-1815">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1815">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="83262-1816">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1816">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="83262-1817">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="83262-1817">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="83262-1818">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="83262-1818">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="83262-1819">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="83262-1819">Az.SignalR</span></span>
* <span data-ttu-id="83262-1820">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1820">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-1821">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1821">Az.Sql</span></span>
* <span data-ttu-id="83262-1822">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="83262-1822">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="83262-1823">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1823">Az.Storage</span></span>
* <span data-ttu-id="83262-1824">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="83262-1824">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="83262-1825">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="83262-1825">New-AzStorageContext</span></span>
* <span data-ttu-id="83262-1826">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1826">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="83262-1827">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="83262-1827">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-1828">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1828">Az.Websites</span></span>
* <span data-ttu-id="83262-1829">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1829">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="83262-1830">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1830">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="83262-1831">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="83262-1831">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="83262-1832">全般</span><span class="sxs-lookup"><span data-stu-id="83262-1832">General</span></span>

- <span data-ttu-id="83262-1833">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="83262-1833">General Availability of Az Module</span></span>
- <span data-ttu-id="83262-1834">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="83262-1834">Online help for each module</span></span>
- <span data-ttu-id="83262-1835">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1835">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="83262-1836">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1836">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="83262-1837">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="83262-1837">Az.Accounts</span></span>
- <span data-ttu-id="83262-1838">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1838">Changed from Az.Profile</span></span>
- <span data-ttu-id="83262-1839">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1839">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="83262-1840">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-1840">Az.ApiManagement</span></span>
- <span data-ttu-id="83262-1841">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="83262-1841">Fixes for #7002</span></span>
- <span data-ttu-id="83262-1842">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1842">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="83262-1843">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="83262-1843">Az.Batch</span></span>
- <span data-ttu-id="83262-1844">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1844">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="83262-1845">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="83262-1845">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="83262-1846">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1846">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="83262-1847">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="83262-1847">Az.Billing</span></span>
- <span data-ttu-id="83262-1848">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1848">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="83262-1849">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="83262-1849">Az.CognitivServices</span></span>
- <span data-ttu-id="83262-1850">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1850">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="83262-1851">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1851">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="83262-1852">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1852">Az.ContainerInstance</span></span>
- <span data-ttu-id="83262-1853">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1853">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="83262-1854">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="83262-1854">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="83262-1855">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1855">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="83262-1856">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1856">Az.DataLakeStore</span></span>
- <span data-ttu-id="83262-1857">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1857">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="83262-1858">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="83262-1858">Az.Monitor</span></span>
- <span data-ttu-id="83262-1859">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1859">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="83262-1860">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="83262-1860">Az.KeyVault</span></span>
- <span data-ttu-id="83262-1861">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1861">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="83262-1862">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="83262-1862">Az.MachineLearning</span></span>
- <span data-ttu-id="83262-1863">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="83262-1863">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="83262-1864">Az.Media</span><span class="sxs-lookup"><span data-stu-id="83262-1864">Az.Media</span></span>
- <span data-ttu-id="83262-1865">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="83262-1865">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="83262-1866">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1866">Az.Network</span></span>
<span data-ttu-id="83262-1867">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1867">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="83262-1868">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-1868">New cmdlets added:</span></span>
        - <span data-ttu-id="83262-1869">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-1869">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1870">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-1870">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1871">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-1871">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1872">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-1872">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1873">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="83262-1873">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1874">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="83262-1874">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="83262-1875">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="83262-1875">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="83262-1876">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="83262-1876">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="83262-1877">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1877">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="83262-1878">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="83262-1878">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="83262-1879">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="83262-1879">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="83262-1880">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="83262-1880">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="83262-1881">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1881">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="83262-1882">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="83262-1882">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="83262-1883">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1883">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="83262-1884">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1884">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="83262-1885">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="83262-1885">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="83262-1886">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="83262-1886">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="83262-1887">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="83262-1887">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="83262-1888">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1888">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="83262-1889">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1889">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="83262-1890">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="83262-1890">Az.OperationalInsights</span></span>
- <span data-ttu-id="83262-1891">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1891">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="83262-1892">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="83262-1892">Az.Profile</span></span>
- <span data-ttu-id="83262-1893">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1893">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1894">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1894">Az.RecoveryServices</span></span>
- <span data-ttu-id="83262-1895">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1895">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="83262-1896">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1896">Az.Resources</span></span>
- <span data-ttu-id="83262-1897">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1897">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="83262-1898">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-1898">Az.ServiceFabric</span></span>
- <span data-ttu-id="83262-1899">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="83262-1899">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="83262-1900">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1900">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="83262-1901">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="83262-1901">Az.SIgnalR</span></span>
- <span data-ttu-id="83262-1902">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="83262-1902">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="83262-1903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1903">Az.Sql</span></span>
- <span data-ttu-id="83262-1904">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1904">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="83262-1905">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1905">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="83262-1906">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1906">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="83262-1907">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1907">Az.Storage</span></span>
- <span data-ttu-id="83262-1908">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1908">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="83262-1909">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1909">Az.Websites</span></span>
- <span data-ttu-id="83262-1910">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="83262-1910">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="83262-1911">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="83262-1911">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="83262-1912">全般</span><span class="sxs-lookup"><span data-stu-id="83262-1912">General</span></span>

* <span data-ttu-id="83262-1913">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="83262-1913">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="83262-1914">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1914">Az.Compute</span></span>

* <span data-ttu-id="83262-1915">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1915">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="83262-1916">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-1916">Az.DataLakeStore</span></span>

* <span data-ttu-id="83262-1917">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1917">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="83262-1918">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="83262-1918">Az.FrontDoor</span></span>

* <span data-ttu-id="83262-1919">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1919">Fixed some broken links</span></span>
    - <span data-ttu-id="83262-1920">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1920">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="83262-1921">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1921">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="83262-1922">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83262-1922">Az.RecoveryServices</span></span>

* <span data-ttu-id="83262-1923">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1923">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="83262-1924">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="83262-1924">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="83262-1925">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1925">Az.Resources</span></span>

* <span data-ttu-id="83262-1926">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1926">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="83262-1927">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-1927">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="83262-1928">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1928">Az.Sql</span></span>

* <span data-ttu-id="83262-1929">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="83262-1929">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="83262-1930">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1930">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="83262-1931">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1931">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="83262-1932">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-1932">Az.Storage</span></span>

* <span data-ttu-id="83262-1933">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1933">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="83262-1934">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1934">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="83262-1935">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="83262-1935">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="83262-1936">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="83262-1936">Support Static Website configuration</span></span>
    - <span data-ttu-id="83262-1937">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="83262-1937">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="83262-1938">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="83262-1938">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="83262-1939">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-1939">Az.Websites</span></span>

* <span data-ttu-id="83262-1940">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="83262-1940">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="83262-1941">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1941">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="83262-1942">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="83262-1942">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="83262-1943">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="83262-1943">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="83262-1944">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="83262-1944">Az.ApiManagement</span></span>
* <span data-ttu-id="83262-1945">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1945">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="83262-1946">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="83262-1946">Az.Automation</span></span>
* <span data-ttu-id="83262-1947">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="83262-1947">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="83262-1948">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1948">Added Update Management cmdlets</span></span>
* <span data-ttu-id="83262-1949">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1949">Added Source Control cmdlets</span></span>
* <span data-ttu-id="83262-1950">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1950">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="83262-1951">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1951">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="83262-1952">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-1952">Az.Compute</span></span>
* <span data-ttu-id="83262-1953">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1953">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="83262-1954">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1954">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="83262-1955">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1955">Az.ContainerInstance</span></span>
* <span data-ttu-id="83262-1956">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1956">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="83262-1957">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="83262-1957">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="83262-1958">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1958">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="83262-1959">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-1959">Az.Network</span></span>
* <span data-ttu-id="83262-1960">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1960">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="83262-1961">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1961">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="83262-1962">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1962">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="83262-1963">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1963">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="83262-1964">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="83262-1964">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="83262-1965">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1965">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="83262-1966">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="83262-1966">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="83262-1967">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="83262-1967">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="83262-1968">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1968">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="83262-1969">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1969">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="83262-1970">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="83262-1970">Az.Relay</span></span>
* <span data-ttu-id="83262-1971">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="83262-1971">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="83262-1972">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-1972">Az.Resources</span></span>
* <span data-ttu-id="83262-1973">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-1973">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="83262-1974">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1974">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="83262-1975">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="83262-1975">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="83262-1976">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-1976">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-1977">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1977">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="83262-1978">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-1978">Az.Sql</span></span>
* <span data-ttu-id="83262-1979">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1979">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="83262-1980">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1980">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="83262-1981">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1981">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="83262-1982">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1982">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="83262-1983">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="83262-1983">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="83262-1984">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="83262-1984">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="83262-1985">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="83262-1985">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="83262-1986">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="83262-1986">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="83262-1987">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="83262-1987">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="83262-1988">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="83262-1988">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="83262-1989">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-1989">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="83262-1990">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="83262-1990">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="83262-1991">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="83262-1991">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="83262-1992">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="83262-1992">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="83262-1993">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="83262-1993">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="83262-1994">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="83262-1994">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="83262-1995">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-1995">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="83262-1996">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="83262-1996">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="83262-1997">全般</span><span class="sxs-lookup"><span data-stu-id="83262-1997">General</span></span>
* <span data-ttu-id="83262-1998">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="83262-1998">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="83262-1999">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="83262-1999">Az.Profile</span></span>
* <span data-ttu-id="83262-2000">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2000">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="83262-2001">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2001">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="83262-2002">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="83262-2002">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="83262-2003">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2003">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="83262-2004">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2004">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="83262-2005">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2005">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="83262-2006">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2006">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-2007">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-2007">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-2008">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2008">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-2009">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-2009">Az.Compute</span></span>
* <span data-ttu-id="83262-2010">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2010">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="83262-2011">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="83262-2011">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="83262-2012">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2012">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-2013">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-2013">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-2014">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="83262-2014">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="83262-2015">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2015">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="83262-2016">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="83262-2016">Az.Insights</span></span>
* <span data-ttu-id="83262-2017">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2017">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="83262-2018">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="83262-2018">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="83262-2019">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2019">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="83262-2020">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="83262-2020">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-2021">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-2021">Az.Network</span></span>
* <span data-ttu-id="83262-2022">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="83262-2022">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="83262-2023">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-2023">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="83262-2024">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="83262-2024">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="83262-2025">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="83262-2025">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="83262-2026">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="83262-2026">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="83262-2027">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="83262-2027">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="83262-2028">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="83262-2028">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="83262-2029">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="83262-2029">Az.PolicyInsights</span></span>
* <span data-ttu-id="83262-2030">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2030">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-2031">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-2031">Az.Resources</span></span>
* <span data-ttu-id="83262-2032">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2032">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="83262-2033">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="83262-2033">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="83262-2034">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="83262-2034">Az.ServiceBus</span></span>
* <span data-ttu-id="83262-2035">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2035">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="83262-2036">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="83262-2036">Az.ServiceFabric</span></span>
* <span data-ttu-id="83262-2037">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2037">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="83262-2038">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2038">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="83262-2039">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="83262-2039">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="83262-2040">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="83262-2040">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="83262-2041">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2041">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="83262-2042">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="83262-2042">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="83262-2043">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="83262-2043">Az.Profile</span></span>
* <span data-ttu-id="83262-2044">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2044">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="83262-2045">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2045">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-2046">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-2046">Az.Compute</span></span>
* <span data-ttu-id="83262-2047">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2047">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="83262-2048">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2048">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="83262-2049">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="83262-2049">Az.DataLakeStore</span></span>
* <span data-ttu-id="83262-2050">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2050">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="83262-2051">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="83262-2051">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="83262-2052">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="83262-2052">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="83262-2053">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="83262-2053">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="83262-2054">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="83262-2054">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-2055">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-2055">Az.Network</span></span>
* <span data-ttu-id="83262-2056">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2056">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="83262-2057">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2057">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-2058">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-2058">Az.Resources</span></span>
* <span data-ttu-id="83262-2059">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2059">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="83262-2060">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2060">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="83262-2061">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="83262-2061">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="83262-2062">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="83262-2062">Azure.Storage</span></span>
* <span data-ttu-id="83262-2063">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2063">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="83262-2064">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="83262-2064">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="83262-2065">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="83262-2065">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="83262-2066">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2066">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="83262-2067">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="83262-2067">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="83262-2068">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="83262-2068">Az.CognitiveServices</span></span>
* <span data-ttu-id="83262-2069">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="83262-2069">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="83262-2070">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="83262-2070">Az.Compute</span></span>
* <span data-ttu-id="83262-2071">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2071">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="83262-2072">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2072">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="83262-2073">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2073">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="83262-2074">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="83262-2074">Az.DataFactoryV2</span></span>
* <span data-ttu-id="83262-2075">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2075">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="83262-2076">Az.Network</span><span class="sxs-lookup"><span data-stu-id="83262-2076">Az.Network</span></span>
* <span data-ttu-id="83262-2077">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="83262-2077">Added NetworkProfile functionality.</span></span> <span data-ttu-id="83262-2078">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="83262-2078">new cmdlets added</span></span>
    - <span data-ttu-id="83262-2079">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="83262-2079">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="83262-2080">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="83262-2080">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="83262-2081">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="83262-2081">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="83262-2082">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="83262-2082">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="83262-2083">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="83262-2083">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="83262-2084">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="83262-2084">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="83262-2085">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2085">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="83262-2086">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2086">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="83262-2087">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2087">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="83262-2088">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="83262-2088">Az.RedisCache</span></span>
* <span data-ttu-id="83262-2089">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="83262-2089">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="83262-2090">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2090">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="83262-2091">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="83262-2091">Az.Resources</span></span>
* <span data-ttu-id="83262-2092">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="83262-2092">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="83262-2093">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2093">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="83262-2094">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="83262-2094">Az.Sql</span></span>
* <span data-ttu-id="83262-2095">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="83262-2095">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="83262-2096">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="83262-2096">Az.Websites</span></span>
* <span data-ttu-id="83262-2097">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="83262-2097">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="83262-2098">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="83262-2098">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="83262-2099">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="83262-2099">0.2.0 - September 2018</span></span>
 <span data-ttu-id="83262-2100">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="83262-2100">Initial Release</span></span>

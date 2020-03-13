---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 4c7ea19a225d63307ecf4a6fe5ebfa14ccd78d7e
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2020
ms.locfileid: "79036163"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="8ea7d-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-103">Azure PowerShell release notes</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="8ea7d-104">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-104">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-105">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-106">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-106">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="8ea7d-107">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-107">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="8ea7d-108">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-108">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-109">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-110">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-110">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="8ea7d-111">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-111">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="8ea7d-112">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-112">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="8ea7d-113">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-113">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-114">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-114">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-115">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-115">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-116">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-117">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-117">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8ea7d-118">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-118">New Cmdlets are:</span></span>
    - <span data-ttu-id="8ea7d-119">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-119">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-120">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-120">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-121">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-121">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-122">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-122">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="8ea7d-123">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-123">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="8ea7d-124">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-124">New Cmdlets are:</span></span>
    - <span data-ttu-id="8ea7d-125">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-125">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="8ea7d-126">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-126">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="8ea7d-127">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-127">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="8ea7d-128">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-128">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="8ea7d-129">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-129">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8ea7d-130">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-130">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8ea7d-131">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-131">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="8ea7d-132">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-132">New Cmdlets are:</span></span>
    - <span data-ttu-id="8ea7d-133">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-133">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="8ea7d-134">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-134">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="8ea7d-135">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-135">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-136">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-136">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-137">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-137">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-138">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-138">Az.Network</span></span>
* <span data-ttu-id="8ea7d-139">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-139">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="8ea7d-140">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-140">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="8ea7d-141">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-141">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="8ea7d-142">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-142">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-143">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-144">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-144">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="8ea7d-145">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-145">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="8ea7d-146">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-146">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="8ea7d-147">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-147">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="8ea7d-148">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-148">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="8ea7d-149">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-149">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="8ea7d-150">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-150">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="8ea7d-151">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-151">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="8ea7d-152">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8ea7d-152">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8ea7d-153">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8ea7d-153">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8ea7d-154">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8ea7d-154">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="8ea7d-155">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-155">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="8ea7d-156">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8ea7d-156">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="8ea7d-157">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-157">Brought ScopedDeployment from SDK 3.3.0</span></span> 

#### <a name="azsql"></a><span data-ttu-id="8ea7d-158">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-158">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-159">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-159">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="8ea7d-160">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-160">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="8ea7d-161">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-161">Get/Set LTR policy on a managed database</span></span> 
    - <span data-ttu-id="8ea7d-162">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-162">Get LTR backup(s) by managed database, managed instance, or by location</span></span> 
    - <span data-ttu-id="8ea7d-163">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-163">Remove an LTR backup</span></span> 
    - <span data-ttu-id="8ea7d-164">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-164">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="8ea7d-165">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-165">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="8ea7d-166">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-166">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="8ea7d-167">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-167">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-168">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-168">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-169">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-169">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="8ea7d-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-170">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="8ea7d-171">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-171">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="8ea7d-172">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-172">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="8ea7d-173">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-173">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-174">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-174">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-175">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-175">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="8ea7d-176">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-176">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="8ea7d-177">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-177">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="8ea7d-178">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-178">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="8ea7d-179">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-179">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="8ea7d-180">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-180">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-181">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-181">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-182">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-182">Updated client side telemetry.</span></span>
* <span data-ttu-id="8ea7d-183">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-183">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="8ea7d-184">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-184">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-185">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-185">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-186">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-186">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-187">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-188">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-188">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-189">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-189">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-190">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-190">Updated SDK to 7.0</span></span>
* <span data-ttu-id="8ea7d-191">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-191">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-192">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-193">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-193">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-194">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-194">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-195">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-195">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-196">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-196">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-197">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-197">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8ea7d-198">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-198">New Cmdlets are:</span></span>
    - <span data-ttu-id="8ea7d-199">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-199">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-200">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-200">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-201">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-201">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8ea7d-202">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-202">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-203">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-203">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-204">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-204">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-205">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-205">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-206">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-206">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="8ea7d-207">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-207">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="8ea7d-208">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-208">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-209">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-209">Az.Network</span></span>
* <span data-ttu-id="8ea7d-210">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-210">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="8ea7d-211">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-211">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8ea7d-212">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-212">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8ea7d-213">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-213">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="8ea7d-214">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-214">No new cmdlets are added.</span></span> <span data-ttu-id="8ea7d-215">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-215">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-216">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-216">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-217">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-217">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-218">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-219">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-219">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="8ea7d-220">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-220">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="8ea7d-221">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-221">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="8ea7d-222">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-222">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="8ea7d-223">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-223">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="8ea7d-224">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-224">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="8ea7d-225">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-225">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="8ea7d-226">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-226">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-227">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-227">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-228">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-228">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="8ea7d-229">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-229">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="8ea7d-230">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="8ea7d-230">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8ea7d-231">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8ea7d-231">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8ea7d-232">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-232">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ea7d-233">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ea7d-233">Az.StorageSync</span></span>
* <span data-ttu-id="8ea7d-234">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-234">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="8ea7d-235">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-235">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-236">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-236">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-237">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-237">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="8ea7d-238">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-238">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-239">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-239">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-240">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-240">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="8ea7d-241">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-241">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-242">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-242">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-243">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="8ea7d-243">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="8ea7d-244">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="8ea7d-244">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="8ea7d-245">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-245">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="8ea7d-246">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-246">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-247">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-247">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-248">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-248">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="8ea7d-249">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-249">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="8ea7d-250">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-250">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-251">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-251">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="8ea7d-252">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-252">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-253">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-253">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-254">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-254">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8ea7d-255">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8ea7d-255">Az.DeploymentManager</span></span>
* <span data-ttu-id="8ea7d-256">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-256">Adds LIST operations for resources</span></span>
* <span data-ttu-id="8ea7d-257">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-257">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-258">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-258">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-259">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-259">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-260">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-260">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-261">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-261">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-262">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-262">Az.Network</span></span>
* <span data-ttu-id="8ea7d-263">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-263">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="8ea7d-264">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="8ea7d-264">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="8ea7d-265">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-265">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-266">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-266">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="8ea7d-267">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="8ea7d-267">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="8ea7d-268">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-268">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="8ea7d-269">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-269">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="8ea7d-270">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-270">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="8ea7d-271">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-271">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-272">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="8ea7d-273">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-273">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="8ea7d-274">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-274">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="8ea7d-275">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-275">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ea7d-276">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-276">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ea7d-277">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-277">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="8ea7d-278">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-278">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="8ea7d-279">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-279">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="8ea7d-280">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-280">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-281">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-281">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-282">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-282">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="8ea7d-283">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-283">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-284">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-285">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-285">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="8ea7d-286">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-286">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-287">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-287">Az.Sql</span></span>
<span data-ttu-id="8ea7d-288">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-288">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-289">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-289">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-290">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-290">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="8ea7d-291">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-291">New-AzStorageAccount</span></span>
* <span data-ttu-id="8ea7d-292">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-292">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="8ea7d-293">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-293">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-294">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-294">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-295">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-295">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="8ea7d-296">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-296">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="8ea7d-297">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-297">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-298">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-298">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-299">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-299">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-300">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-300">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-301">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-301">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-302">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-302">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-303">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-303">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="8ea7d-304">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-304">Az.ContainerInstance</span></span>
* <span data-ttu-id="8ea7d-305">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-305">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8ea7d-306">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8ea7d-306">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8ea7d-307">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-307">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8ea7d-308">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-308">Get the Edge Storage Container</span></span>
* <span data-ttu-id="8ea7d-309">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-309">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8ea7d-310">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-310">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="8ea7d-311">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-311">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8ea7d-312">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-312">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="8ea7d-313">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-313">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8ea7d-314">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-314">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="8ea7d-315">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-315">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8ea7d-316">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-316">Get the Edge Storage Account</span></span>
* <span data-ttu-id="8ea7d-317">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-317">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8ea7d-318">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-318">Create new Edge Storage Account</span></span>
* <span data-ttu-id="8ea7d-319">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-319">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8ea7d-320">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-320">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="8ea7d-321">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-321">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="8ea7d-322">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-322">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="8ea7d-323">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-323">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="8ea7d-324">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-324">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-325">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-326">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-326">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="8ea7d-327">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-327">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="8ea7d-328">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-328">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="8ea7d-329">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="8ea7d-329">Az.DevTestLabs</span></span>
* <span data-ttu-id="8ea7d-330">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-330">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-331">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-331">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-332">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-332">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-333">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-333">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-334">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-334">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8ea7d-335">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8ea7d-335">Az.MachineLearning</span></span>
* <span data-ttu-id="8ea7d-336">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-336">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="8ea7d-337">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8ea7d-337">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="8ea7d-338">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-338">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="8ea7d-339">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8ea7d-339">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="8ea7d-340">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8ea7d-340">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="8ea7d-341">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8ea7d-341">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="8ea7d-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="8ea7d-342">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="8ea7d-343">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-343">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-344">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-344">Az.Network</span></span>
* <span data-ttu-id="8ea7d-345">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-345">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-346">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-346">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-347">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-347">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="8ea7d-348">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-348">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8ea7d-349">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-349">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8ea7d-350">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-350">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-351">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-351">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-352">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-352">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-353">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-354">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-354">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="8ea7d-355">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-355">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8ea7d-356">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8ea7d-356">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8ea7d-357">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-357">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-358">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-358">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-359">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-359">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="8ea7d-360">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-360">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="8ea7d-361">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-361">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="8ea7d-362">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-362">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="8ea7d-363">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-363">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="8ea7d-364">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-364">General</span></span>
* <span data-ttu-id="8ea7d-365">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-365">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-366">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-366">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-367">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-367">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="8ea7d-368">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-368">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ea7d-369">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-369">Az.Batch</span></span>
* <span data-ttu-id="8ea7d-370">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-370">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-371">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-371">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-372">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-372">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-373">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-373">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-374">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-374">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="8ea7d-375">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-375">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8ea7d-376">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8ea7d-376">Az.HealthcareApis</span></span>
* <span data-ttu-id="8ea7d-377">例外処理</span><span class="sxs-lookup"><span data-stu-id="8ea7d-377">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-378">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-379">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-379">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="8ea7d-380">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="8ea7d-380">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="8ea7d-381">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-381">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-382">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-382">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-383">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-383">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="8ea7d-384">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="8ea7d-384">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="8ea7d-385">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="8ea7d-385">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-386">Az.Network</span></span>
* <span data-ttu-id="8ea7d-387">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-387">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-388">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-388">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-389">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-389">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="8ea7d-390">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-390">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-391">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-391">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-392">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-392">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-393">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-393">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-394">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-394">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="8ea7d-395">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="8ea7d-395">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="8ea7d-396">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8ea7d-396">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="8ea7d-397">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-397">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="8ea7d-398">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="8ea7d-398">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="8ea7d-399">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-399">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="8ea7d-400">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-400">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="8ea7d-401">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-401">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="8ea7d-402">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-402">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="8ea7d-403">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-403">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="8ea7d-404">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="8ea7d-404">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="8ea7d-405">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-405">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="8ea7d-406">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="8ea7d-406">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="8ea7d-407">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-407">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-408">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-408">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-409">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-409">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="8ea7d-410">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-410">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-411">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-411">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-412">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="8ea7d-412">VM Reapply feature</span></span>
    - <span data-ttu-id="8ea7d-413">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-413">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="8ea7d-414">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-414">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="8ea7d-415">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8ea7d-415">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="8ea7d-416">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-416">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="8ea7d-417">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-417">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8ea7d-418">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-418">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="8ea7d-419">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-419">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="8ea7d-420">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-420">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="8ea7d-421">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-421">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="8ea7d-422">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-422">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8ea7d-423">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8ea7d-423">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8ea7d-424">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-424">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8ea7d-425">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-425">Get the Order</span></span>
* <span data-ttu-id="8ea7d-426">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-426">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8ea7d-427">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-427">Create new Order</span></span>
* <span data-ttu-id="8ea7d-428">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-428">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8ea7d-429">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-429">Remove the Order</span></span>
* <span data-ttu-id="8ea7d-430">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="8ea7d-430">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="8ea7d-431">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="8ea7d-431">Now creates Local Share</span></span>
* <span data-ttu-id="8ea7d-432">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-432">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="8ea7d-433">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-433">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="8ea7d-434">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-434">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="8ea7d-435">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-435">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="8ea7d-436">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-436">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8ea7d-437">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-437">Gets the information about Triggers</span></span>
* <span data-ttu-id="8ea7d-438">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-438">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8ea7d-439">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-439">Create new Triggers</span></span>
* <span data-ttu-id="8ea7d-440">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-440">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8ea7d-441">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-441">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-442">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-442">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-443">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-443">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="8ea7d-444">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-444">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-445">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-445">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-446">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-446">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-447">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-447">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-448">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-448">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-449">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-450">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-450">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="8ea7d-451">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-451">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="8ea7d-452">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-452">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="8ea7d-453">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="8ea7d-453">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-454">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-454">Az.Network</span></span>
* <span data-ttu-id="8ea7d-455">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-455">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="8ea7d-456">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="8ea7d-456">Az.PrivateDns</span></span>
* <span data-ttu-id="8ea7d-457">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-457">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-458">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-458">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-459">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-459">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="8ea7d-460">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-460">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="8ea7d-461">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-461">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ea7d-462">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ea7d-462">Az.RedisCache</span></span>
* <span data-ttu-id="8ea7d-463">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-463">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="8ea7d-464">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-464">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="8ea7d-465">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-465">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-466">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-466">Az.Resources</span></span>
- <span data-ttu-id="8ea7d-467">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-467">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="8ea7d-468">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-468">Updated create policy definition help example</span></span>
- <span data-ttu-id="8ea7d-469">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-469">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="8ea7d-470">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-470">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="8ea7d-471">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-471">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-472">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-472">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-473">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-473">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="8ea7d-474">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-474">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="8ea7d-475">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-475">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="8ea7d-476">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-476">General</span></span>
* <span data-ttu-id="8ea7d-477">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-477">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-478">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-478">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-479">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-479">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8ea7d-480">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-480">Az.Advisor</span></span>
* <span data-ttu-id="8ea7d-481">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-481">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ea7d-482">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-482">Az.Batch</span></span>
* <span data-ttu-id="8ea7d-483">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-483">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="8ea7d-484">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-484">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="8ea7d-485">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-485">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="8ea7d-486">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-486">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="8ea7d-487">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-487">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="8ea7d-488">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-488">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="8ea7d-489">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-489">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="8ea7d-490">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-490">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="8ea7d-491">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-491">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="8ea7d-492">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-492">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8ea7d-493">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-493">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="8ea7d-494">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-494">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="8ea7d-495">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-495">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8ea7d-496">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-496">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="8ea7d-497">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-497">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="8ea7d-498">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-498">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="8ea7d-499">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-499">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="8ea7d-500">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-500">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="8ea7d-501">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-501">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="8ea7d-502">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-502">This operation is no longer supported.</span></span>
* <span data-ttu-id="8ea7d-503">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-503">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8ea7d-504">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-504">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8ea7d-505">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-505">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="8ea7d-506">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-506">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="8ea7d-507">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-507">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="8ea7d-508">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-508">New non-verified images are also now returned.</span></span> <span data-ttu-id="8ea7d-509">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-509">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="8ea7d-510">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-510">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="8ea7d-511">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-511">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="8ea7d-512">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-512">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="8ea7d-513">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-513">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="8ea7d-514">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-514">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="8ea7d-515">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-515">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="8ea7d-516">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-516">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="8ea7d-517">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-517">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="8ea7d-518">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-518">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-519">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-520">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-520">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="8ea7d-521">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-521">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-522">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-522">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-523">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="8ea7d-523">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="8ea7d-524">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-524">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="8ea7d-525">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-525">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="8ea7d-526">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="8ea7d-526">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="8ea7d-527">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-527">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8ea7d-528">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-528">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="8ea7d-529">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-529">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="8ea7d-530">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-530">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="8ea7d-531">重大な変更</span><span class="sxs-lookup"><span data-stu-id="8ea7d-531">Breaking changes</span></span>
    - <span data-ttu-id="8ea7d-532">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-532">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="8ea7d-533">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-533">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-534">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-534">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-535">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-535">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-536">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-537">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-537">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="8ea7d-538">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-538">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="8ea7d-539">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-539">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="8ea7d-540">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-540">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="8ea7d-541">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-541">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="8ea7d-542">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-542">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-543">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-543">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-544">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-544">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-545">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-545">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-546">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-546">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="8ea7d-547">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-547">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="8ea7d-548">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-548">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="8ea7d-549">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-549">Removed five cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-550">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8ea7d-550">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8ea7d-551">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8ea7d-551">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8ea7d-552">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8ea7d-552">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8ea7d-553">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ea7d-553">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="8ea7d-554">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ea7d-554">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="8ea7d-555">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-555">Added three cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-556">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-556">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8ea7d-557">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-557">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8ea7d-558">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-558">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="8ea7d-559">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-559">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="8ea7d-560">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-560">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="8ea7d-561">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-561">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="8ea7d-562">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-562">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="8ea7d-563">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-563">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="8ea7d-564">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-564">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="8ea7d-565">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-565">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="8ea7d-566">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-566">Added some scenario test cases.</span></span>
* <span data-ttu-id="8ea7d-567">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-567">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-568">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-568">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-569">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-569">Breaking changes:</span></span>
    - <span data-ttu-id="8ea7d-570">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-570">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8ea7d-571">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-571">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8ea7d-572">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-572">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8ea7d-573">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-573">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8ea7d-574">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-574">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="8ea7d-575">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-575">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="8ea7d-576">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-576">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="8ea7d-577">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-577">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="8ea7d-578">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-578">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8ea7d-579">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-579">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8ea7d-580">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-580">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8ea7d-581">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-581">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-582">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-582">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-583">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-583">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-584">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-584">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="8ea7d-585">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-585">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="8ea7d-586">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-586">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-587">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-587">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-588">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-588">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-589">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-589">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-590">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-590">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-591">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-591">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-592">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-592">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-593">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-593">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-594">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-594">Az.Network</span></span>
* <span data-ttu-id="8ea7d-595">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-595">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="8ea7d-596">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-596">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-597">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-597">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-598">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-598">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-599">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-599">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-600">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-600">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-601">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-601">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8ea7d-602">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-602">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="8ea7d-603">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-603">New cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-604">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="8ea7d-604">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="8ea7d-605">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-605">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="8ea7d-606">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-606">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="8ea7d-607">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-607">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="8ea7d-608">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-608">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="8ea7d-609">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-609">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="8ea7d-610">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-610">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="8ea7d-611">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-611">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="8ea7d-612">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-612">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-613">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-613">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="8ea7d-614">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-614">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8ea7d-615">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-615">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8ea7d-616">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-616">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8ea7d-617">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-617">Set-AzVirtualHub</span></span>
* <span data-ttu-id="8ea7d-618">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-618">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="8ea7d-619">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-619">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8ea7d-620">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-620">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8ea7d-621">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-621">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8ea7d-622">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-622">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="8ea7d-623">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-623">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="8ea7d-624">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-624">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="8ea7d-625">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-625">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-626">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-626">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="8ea7d-627">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-627">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8ea7d-628">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-628">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8ea7d-629">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-629">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8ea7d-630">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-630">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8ea7d-631">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-631">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8ea7d-632">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-632">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="8ea7d-633">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-633">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="8ea7d-634">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-634">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-635">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="8ea7d-635">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="8ea7d-636">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="8ea7d-636">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="8ea7d-637">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="8ea7d-637">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="8ea7d-638">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="8ea7d-638">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="8ea7d-639">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-639">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="8ea7d-640">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-640">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="8ea7d-641">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-641">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8ea7d-642">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-642">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="8ea7d-643">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-643">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="8ea7d-644">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-644">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="8ea7d-645">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-645">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="8ea7d-646">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-646">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8ea7d-647">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-647">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="8ea7d-648">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-648">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="8ea7d-649">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-649">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="8ea7d-650">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-650">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="8ea7d-651">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-651">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="8ea7d-652">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-652">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-653">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-653">New-AzIpGroup</span></span>
        - <span data-ttu-id="8ea7d-654">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-654">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="8ea7d-655">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-655">Get-AzIpGroup</span></span>
        - <span data-ttu-id="8ea7d-656">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-656">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-657">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-657">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-658">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-658">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-659">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-659">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-660">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-660">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="8ea7d-661">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-661">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="8ea7d-662">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-662">Removed deprecated aliases:</span></span>
* <span data-ttu-id="8ea7d-663">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-663">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="8ea7d-664">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-664">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="8ea7d-665">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-665">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8ea7d-666">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-666">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="8ea7d-667">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-667">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="8ea7d-668">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-668">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-669">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-669">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-670">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-670">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="8ea7d-671">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-671">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8ea7d-672">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-672">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8ea7d-673">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-673">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="8ea7d-674">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ea7d-674">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="8ea7d-675">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ea7d-675">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="8ea7d-676">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-676">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="8ea7d-677">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-677">General</span></span>
* <span data-ttu-id="8ea7d-678">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-678">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-679">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-679">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-680">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-680">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-681">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-681">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-682">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-682">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="8ea7d-683">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="8ea7d-683">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-684">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-684">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-685">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-685">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="8ea7d-686">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-686">Az.Batch</span></span>
* <span data-ttu-id="8ea7d-687">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-687">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-688">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-688">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-689">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-689">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8ea7d-690">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-690">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="8ea7d-691">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-691">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="8ea7d-692">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-692">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-693">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-693">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-694">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-694">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="8ea7d-695">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-695">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="8ea7d-696">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-696">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-697">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-697">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-698">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-698">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8ea7d-699">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8ea7d-699">Az.HealthcareApis</span></span>
* <span data-ttu-id="8ea7d-700">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-700">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="8ea7d-701">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-701">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="8ea7d-702">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-702">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="8ea7d-703">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-703">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-704">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-704">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-705">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="8ea7d-705">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="8ea7d-706">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="8ea7d-706">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-707">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-707">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-708">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="8ea7d-708">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="8ea7d-709">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-709">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="8ea7d-710">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="8ea7d-710">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="8ea7d-711">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-711">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-712">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-712">Az.Network</span></span>
* <span data-ttu-id="8ea7d-713">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-713">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="8ea7d-714">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-714">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="8ea7d-715">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-715">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-716">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-716">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="8ea7d-717">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-717">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8ea7d-718">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-718">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="8ea7d-719">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-719">Updated cmdlets:</span></span>
        - <span data-ttu-id="8ea7d-720">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-720">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ea7d-721">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-721">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ea7d-722">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-722">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8ea7d-723">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-723">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="8ea7d-724">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="8ea7d-724">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="8ea7d-725">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-725">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="8ea7d-726">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-726">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ea7d-727">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ea7d-727">Az.RedisCache</span></span>
* <span data-ttu-id="8ea7d-728">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-728">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-729">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-729">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-730">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-730">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-731">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-731">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-732">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-732">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="8ea7d-733">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-733">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8ea7d-734">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="8ea7d-734">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="8ea7d-735">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-735">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8ea7d-736">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-736">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ea7d-737">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ea7d-737">Az.StorageSync</span></span>
* <span data-ttu-id="8ea7d-738">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-738">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-739">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-739">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-740">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-740">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="8ea7d-741">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-741">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-742">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-742">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-743">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-743">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="8ea7d-744">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-744">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="8ea7d-745">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-745">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-746">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-746">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-747">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-747">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="8ea7d-748">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-748">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="8ea7d-749">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-749">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-750">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-751">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-751">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="8ea7d-752">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-752">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8ea7d-753">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-753">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="8ea7d-754">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-754">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="8ea7d-755">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-755">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="8ea7d-756">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-756">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="8ea7d-757">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-757">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="8ea7d-758">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-758">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="8ea7d-759">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-759">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-760">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-760">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-761">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-761">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="8ea7d-762">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-762">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-763">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-763">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-764">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-764">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-765">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-765">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-766">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-766">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="8ea7d-767">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-767">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="8ea7d-768">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-768">New cmdlets are:</span></span>
    - <span data-ttu-id="8ea7d-769">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-769">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8ea7d-770">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-770">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8ea7d-771">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-771">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8ea7d-772">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8ea7d-772">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-773">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-774">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="8ea7d-774">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="8ea7d-775">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-775">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="8ea7d-776">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-776">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="8ea7d-777">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-777">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="8ea7d-778">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-778">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="8ea7d-779">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-779">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="8ea7d-780">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-780">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="8ea7d-781">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-781">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="8ea7d-782">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-782">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8ea7d-783">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-783">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="8ea7d-784">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-784">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8ea7d-785">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-785">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="8ea7d-786">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-786">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="8ea7d-787">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-787">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="8ea7d-788">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-788">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="8ea7d-789">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="8ea7d-789">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="8ea7d-790">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-790">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="8ea7d-791">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-791">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="8ea7d-792">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-792">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="8ea7d-793">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-793">Overall improved help files</span></span>
* <span data-ttu-id="8ea7d-794">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-794">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-795">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-795">Az.Network</span></span>
* <span data-ttu-id="8ea7d-796">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-796">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="8ea7d-797">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-797">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="8ea7d-798">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-798">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="8ea7d-799">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-799">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="8ea7d-800">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-800">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="8ea7d-801">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-801">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="8ea7d-802">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-802">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="8ea7d-803">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-803">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="8ea7d-804">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-804">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="8ea7d-805">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-805">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="8ea7d-806">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-806">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="8ea7d-807">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-807">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="8ea7d-808">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-808">New cmdlets</span></span>
        - <span data-ttu-id="8ea7d-809">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="8ea7d-809">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="8ea7d-810">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-810">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="8ea7d-811">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-811">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-812">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8ea7d-812">New-VpnSite</span></span>
        - <span data-ttu-id="8ea7d-813">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8ea7d-813">Update-VpnSite</span></span>
        - <span data-ttu-id="8ea7d-814">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-814">New-VpnConnection</span></span>
        - <span data-ttu-id="8ea7d-815">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-815">Update-VpnConnection</span></span>
* <span data-ttu-id="8ea7d-816">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-816">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-817">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-817">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-818">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-818">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="8ea7d-819">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-819">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-820">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-820">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-821">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-821">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-822">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-822">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-823">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-823">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="8ea7d-824">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-824">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="8ea7d-825">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8ea7d-825">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8ea7d-826">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8ea7d-826">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8ea7d-827">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8ea7d-827">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8ea7d-828">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-828">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="8ea7d-829">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8ea7d-829">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8ea7d-830">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8ea7d-830">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8ea7d-831">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8ea7d-831">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8ea7d-832">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8ea7d-832">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8ea7d-833">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-833">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="8ea7d-834">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8ea7d-834">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8ea7d-835">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8ea7d-835">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8ea7d-836">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8ea7d-836">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8ea7d-837">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="8ea7d-837">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="8ea7d-838">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-838">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8ea7d-839">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8ea7d-839">Az.SignalR</span></span>
* <span data-ttu-id="8ea7d-840">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-840">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-841">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-841">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-842">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-842">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="8ea7d-843">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-843">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="8ea7d-844">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-844">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="8ea7d-845">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-845">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="8ea7d-846">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-846">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-847">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-847">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-848">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-848">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="8ea7d-849">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-849">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="8ea7d-850">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-850">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="8ea7d-851">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-851">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="8ea7d-852">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-852">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="8ea7d-853">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-853">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="8ea7d-854">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-854">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="8ea7d-855">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-855">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8ea7d-856">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-856">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8ea7d-857">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-857">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8ea7d-858">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8ea7d-858">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-859">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-859">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-860">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-860">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="8ea7d-861">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-861">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="8ea7d-862">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-862">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="8ea7d-863">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-863">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="8ea7d-864">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-864">General</span></span>
* <span data-ttu-id="8ea7d-865">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-865">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-866">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-866">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-867">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-867">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="8ea7d-868">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8ea7d-868">Az.Aks</span></span>
* <span data-ttu-id="8ea7d-869">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-869">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="8ea7d-870">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="8ea7d-870">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-871">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-871">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-872">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="8ea7d-872">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="8ea7d-873">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-873">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="8ea7d-874">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-874">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="8ea7d-875">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="8ea7d-875">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="8ea7d-876">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-876">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ea7d-877">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-877">Az.Batch</span></span>
* <span data-ttu-id="8ea7d-878">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-878">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-879">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-879">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-880">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-880">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-881">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-881">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-882">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-882">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="8ea7d-883">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-883">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="8ea7d-884">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-884">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="8ea7d-885">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-885">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="8ea7d-886">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="8ea7d-886">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="8ea7d-887">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-887">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="8ea7d-888">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-888">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="8ea7d-889">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-889">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-890">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-890">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-891">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-891">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="8ea7d-892">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-892">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="8ea7d-893">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-893">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="8ea7d-894">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-894">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-895">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-895">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-896">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-896">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-897">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-897">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-898">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="8ea7d-898">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="8ea7d-899">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="8ea7d-899">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="8ea7d-900">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-900">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="8ea7d-901">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="8ea7d-901">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="8ea7d-902">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8ea7d-902">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8ea7d-903">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-903">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-904">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-904">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-905">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-905">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-906">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-906">Az.Network</span></span>
* <span data-ttu-id="8ea7d-907">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-907">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="8ea7d-908">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-908">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="8ea7d-909">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-909">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="8ea7d-910">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-910">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="8ea7d-911">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-911">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="8ea7d-912">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-912">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="8ea7d-913">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-913">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-914">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-914">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-915">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-915">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="8ea7d-916">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-916">Added example</span></span>
    - <span data-ttu-id="8ea7d-917">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-917">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="8ea7d-918">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-918">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="8ea7d-919">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-919">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-920">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-920">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-921">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-921">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-922">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-922">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-923">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-923">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="8ea7d-924">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-924">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="8ea7d-925">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-925">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="8ea7d-926">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-926">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-927">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-927">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-928">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="8ea7d-928">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="8ea7d-929">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="8ea7d-929">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="8ea7d-930">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-930">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-931">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-931">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-932">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-932">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="8ea7d-933">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-933">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="8ea7d-934">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="8ea7d-934">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="8ea7d-935">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-935">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="8ea7d-936">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="8ea7d-936">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="8ea7d-937">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-937">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-938">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-938">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-939">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-939">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-940">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-940">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-941">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-941">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="8ea7d-942">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-942">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="8ea7d-943">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-943">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="8ea7d-944">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-944">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="8ea7d-945">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-945">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="8ea7d-946">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-946">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-947">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-948">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-948">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="8ea7d-949">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-949">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-950">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-950">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-951">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-951">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8ea7d-952">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-952">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8ea7d-953">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-953">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-954">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-954">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-955">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-955">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-956">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-956">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-957">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-957">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-958">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-958">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-959">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-959">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8ea7d-960">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8ea7d-960">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8ea7d-961">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-961">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="8ea7d-962">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="8ea7d-962">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-963">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-963">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-964">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-964">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="8ea7d-965">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-965">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-966">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-966">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-967">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8ea7d-967">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8ea7d-968">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-968">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-969">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-969">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-970">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-970">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ea7d-971">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ea7d-971">Az.LogicApp</span></span>
* <span data-ttu-id="8ea7d-972">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-972">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="8ea7d-973">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-973">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="8ea7d-974">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-974">Az.ManagedServices</span></span>
* <span data-ttu-id="8ea7d-975">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-975">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-976">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-976">Az.Network</span></span>
* <span data-ttu-id="8ea7d-977">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-977">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="8ea7d-978">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-978">New cmdlets</span></span>
        - <span data-ttu-id="8ea7d-979">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ea7d-979">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ea7d-980">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-980">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ea7d-981">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-981">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-982">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-982">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-983">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-983">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-984">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-984">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8ea7d-985">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="8ea7d-985">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="8ea7d-986">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-986">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="8ea7d-987">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="8ea7d-987">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="8ea7d-988">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-988">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="8ea7d-989">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-989">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="8ea7d-990">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-990">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="8ea7d-991">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-991">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="8ea7d-992">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-992">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="8ea7d-993">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-993">Updated cmdlets</span></span>
        - <span data-ttu-id="8ea7d-994">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-994">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ea7d-995">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-995">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8ea7d-996">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-996">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8ea7d-997">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-997">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8ea7d-998">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-998">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="8ea7d-999">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-999">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-1000">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1000">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8ea7d-1001">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1001">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8ea7d-1002">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1002">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="8ea7d-1003">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1003">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="8ea7d-1004">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1004">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="8ea7d-1005">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1005">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1006">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1006">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-1007">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1007">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="8ea7d-1008">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1008">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1009">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1009">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1010">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1010">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8ea7d-1011">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1011">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="8ea7d-1012">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1012">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="8ea7d-1013">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1013">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8ea7d-1014">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1014">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="8ea7d-1015">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1015">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8ea7d-1016">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1016">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="8ea7d-1017">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1017">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8ea7d-1018">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1018">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="8ea7d-1019">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1019">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1020">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1020">Az.Resources</span></span>
- <span data-ttu-id="8ea7d-1021">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1021">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="8ea7d-1022">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1022">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-1023">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1023">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-1024">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1024">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8ea7d-1025">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1025">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1026">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1026">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1027">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1027">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="8ea7d-1028">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1028">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="8ea7d-1029">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1029">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1030">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1030">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1031">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1031">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ea7d-1032">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1032">Az.StorageSync</span></span>
* <span data-ttu-id="8ea7d-1033">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1033">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="8ea7d-1034">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1034">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1035">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1035">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1036">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1036">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="8ea7d-1037">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1037">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="8ea7d-1038">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1038">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="8ea7d-1039">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1039">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1040">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1040">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1041">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1041">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8ea7d-1042">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1042">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8ea7d-1043">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1043">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8ea7d-1044">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1044">Az.Advisor</span></span>
* <span data-ttu-id="8ea7d-1045">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1045">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8ea7d-1046">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1046">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-1047">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1047">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-1048">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1048">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8ea7d-1049">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1049">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8ea7d-1050">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1050">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8ea7d-1051">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1051">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8ea7d-1052">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1052">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8ea7d-1053">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1053">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8ea7d-1054">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1054">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1055">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1055">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1056">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1056">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1057">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1057">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1058">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1058">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-1059">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1059">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-1060">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1060">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ea7d-1061">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1061">Az.EventGrid</span></span>
* <span data-ttu-id="8ea7d-1062">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1062">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-1063">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1063">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-1064">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1064">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1065">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1065">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1066">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1066">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8ea7d-1067">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1067">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ea7d-1068">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1068">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ea7d-1069">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1069">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8ea7d-1070">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1070">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1071">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1071">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-1072">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1072">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1073">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1073">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1074">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1074">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1075">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1075">Az.Resources</span></span>
    - <span data-ttu-id="8ea7d-1076">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1076">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8ea7d-1077">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1077">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8ea7d-1078">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1078">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8ea7d-1079">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1079">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-1080">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1080">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-1081">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1081">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1082">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1082">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1083">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1083">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8ea7d-1084">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1084">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8ea7d-1085">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1085">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ea7d-1086">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1086">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ea7d-1087">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1087">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8ea7d-1088">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1088">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8ea7d-1089">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1089">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8ea7d-1090">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1090">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8ea7d-1091">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1091">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1092">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1092">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1093">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1093">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8ea7d-1094">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1094">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8ea7d-1095">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1095">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8ea7d-1096">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1096">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8ea7d-1097">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1097">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8ea7d-1098">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1098">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8ea7d-1099">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1099">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8ea7d-1100">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1100">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8ea7d-1101">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1101">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8ea7d-1102">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1102">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8ea7d-1103">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1103">Az.StorageSync</span></span>
* <span data-ttu-id="8ea7d-1104">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1104">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8ea7d-1105">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1105">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1106">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1107">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1107">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8ea7d-1108">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1108">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8ea7d-1109">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1109">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8ea7d-1110">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1110">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8ea7d-1111">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1111">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1112">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1112">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1113">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1113">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8ea7d-1114">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1114">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8ea7d-1115">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1115">Az.Dns</span></span>
* <span data-ttu-id="8ea7d-1116">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1116">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ea7d-1117">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1117">Az.EventGrid</span></span>
* <span data-ttu-id="8ea7d-1118">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1118">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8ea7d-1119">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1119">New cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-1120">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1120">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ea7d-1121">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1121">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ea7d-1122">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1122">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ea7d-1123">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1123">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8ea7d-1124">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1124">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8ea7d-1125">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1125">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ea7d-1126">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1126">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8ea7d-1127">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1127">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8ea7d-1128">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1128">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8ea7d-1129">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1129">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8ea7d-1130">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1130">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8ea7d-1131">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1131">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8ea7d-1132">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1132">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8ea7d-1133">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1133">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="8ea7d-1134">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1134">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8ea7d-1135">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1135">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8ea7d-1136">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1136">Updated cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-1137">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1137">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8ea7d-1138">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1138">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8ea7d-1139">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1139">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8ea7d-1140">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1140">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8ea7d-1141">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1141">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8ea7d-1142">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1142">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8ea7d-1143">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1143">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8ea7d-1144">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1144">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8ea7d-1145">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1145">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="8ea7d-1146">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1146">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8ea7d-1147">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1147">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8ea7d-1148">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1148">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8ea7d-1149">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1149">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8ea7d-1150">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1150">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-1151">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1151">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-1152">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1152">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8ea7d-1153">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1153">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8ea7d-1154">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1154">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8ea7d-1155">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1155">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1156">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1156">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1157">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1157">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8ea7d-1158">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1158">New cmdlets</span></span>
        - <span data-ttu-id="8ea7d-1159">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1159">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8ea7d-1160">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1160">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8ea7d-1161">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1161">New cmdlets</span></span> 
        - <span data-ttu-id="8ea7d-1162">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1162">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8ea7d-1163">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1163">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8ea7d-1164">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1164">New cmdlets</span></span> 
        - <span data-ttu-id="8ea7d-1165">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1165">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="8ea7d-1166">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1166">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ea7d-1167">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1167">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8ea7d-1168">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1168">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8ea7d-1169">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1169">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8ea7d-1170">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1170">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8ea7d-1171">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1171">New cmdlets</span></span>
        - <span data-ttu-id="8ea7d-1172">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1172">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ea7d-1173">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1173">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ea7d-1174">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1174">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8ea7d-1175">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1175">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8ea7d-1176">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1176">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8ea7d-1177">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1177">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8ea7d-1178">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1178">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8ea7d-1179">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1179">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8ea7d-1180">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1180">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8ea7d-1181">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1181">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8ea7d-1182">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1182">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8ea7d-1183">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1183">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8ea7d-1184">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1184">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8ea7d-1185">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1185">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8ea7d-1186">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1186">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8ea7d-1187">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1187">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8ea7d-1188">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1188">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8ea7d-1189">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1189">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8ea7d-1190">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1190">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-1191">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1191">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8ea7d-1192">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1192">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8ea7d-1193">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1193">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8ea7d-1194">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1194">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="8ea7d-1195">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1195">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="8ea7d-1196">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1196">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8ea7d-1197">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1197">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8ea7d-1198">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1198">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1199">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1199">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-1200">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1200">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1201">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1201">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1202">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1202">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8ea7d-1203">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1203">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8ea7d-1204">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1204">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8ea7d-1205">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1205">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-1206">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1206">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-1207">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1207">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1208">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1208">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1209">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1209">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8ea7d-1210">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1210">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8ea7d-1211">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1211">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8ea7d-1212">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1212">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ea7d-1213">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1213">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ea7d-1214">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1214">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8ea7d-1215">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1215">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8ea7d-1216">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1216">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1217">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1217">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1218">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1218">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8ea7d-1219">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1219">New-AzStorageAccount</span></span>
* <span data-ttu-id="8ea7d-1220">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1220">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8ea7d-1221">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1221">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1222">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1222">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1223">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1223">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8ea7d-1224">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1224">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8ea7d-1225">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1225">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8ea7d-1226">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1226">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-1227">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1227">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1228">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1228">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1229">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1229">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8ea7d-1230">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1230">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-1231">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1231">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-1232">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1232">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8ea7d-1233">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1233">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1234">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1234">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1235">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1235">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8ea7d-1236">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1236">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ea7d-1237">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1237">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ea7d-1238">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1238">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1239">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1239">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1240">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1240">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-1241">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1241">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-1242">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1242">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-1243">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1243">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-1244">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1244">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8ea7d-1245">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1245">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1246">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1246">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1247">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1247">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8ea7d-1248">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1248">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8ea7d-1249">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1249">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8ea7d-1250">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1250">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1251">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1251">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1252">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1252">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8ea7d-1253">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1253">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-1254">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1254">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-1255">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1255">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8ea7d-1256">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1256">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8ea7d-1257">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1257">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8ea7d-1258">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1258">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8ea7d-1259">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1259">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8ea7d-1260">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1260">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8ea7d-1261">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1261">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8ea7d-1262">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1262">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8ea7d-1263">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1263">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8ea7d-1264">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1264">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8ea7d-1265">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1265">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8ea7d-1266">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1266">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8ea7d-1267">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1267">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8ea7d-1268">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1268">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8ea7d-1269">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1269">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8ea7d-1270">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1270">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8ea7d-1271">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1271">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8ea7d-1272">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1272">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8ea7d-1273">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1273">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="8ea7d-1274">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1274">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8ea7d-1275">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1275">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8ea7d-1276">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1276">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8ea7d-1277">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1277">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8ea7d-1278">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1278">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="8ea7d-1279">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1279">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8ea7d-1280">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1280">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8ea7d-1281">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1281">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8ea7d-1282">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1282">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8ea7d-1283">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1283">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8ea7d-1284">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1284">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8ea7d-1285">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1285">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="8ea7d-1286">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1286">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8ea7d-1287">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1287">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8ea7d-1288">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1288">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8ea7d-1289">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1289">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8ea7d-1290">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1290">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8ea7d-1291">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1291">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8ea7d-1292">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1292">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8ea7d-1293">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1293">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8ea7d-1294">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1294">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="8ea7d-1295">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1295">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8ea7d-1296">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1296">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8ea7d-1297">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1297">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8ea7d-1298">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1298">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8ea7d-1299">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1299">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8ea7d-1300">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1300">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8ea7d-1301">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1301">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="8ea7d-1302">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1302">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8ea7d-1303">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1303">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8ea7d-1304">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1304">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8ea7d-1305">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1305">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8ea7d-1306">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1306">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8ea7d-1307">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1307">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8ea7d-1308">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1308">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8ea7d-1309">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1309">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8ea7d-1310">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1310">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8ea7d-1311">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1311">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8ea7d-1312">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1312">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8ea7d-1313">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1313">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8ea7d-1314">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1314">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8ea7d-1315">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1315">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8ea7d-1316">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1316">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8ea7d-1317">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1317">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8ea7d-1318">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1318">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8ea7d-1319">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1319">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8ea7d-1320">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1320">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8ea7d-1321">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1321">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8ea7d-1322">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1322">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8ea7d-1323">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1323">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8ea7d-1324">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1324">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8ea7d-1325">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1325">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8ea7d-1326">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1326">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8ea7d-1327">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1327">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8ea7d-1328">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1328">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8ea7d-1329">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1329">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="8ea7d-1330">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1330">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8ea7d-1331">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1331">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1332">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1332">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1333">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1333">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8ea7d-1334">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1334">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8ea7d-1335">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1335">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8ea7d-1336">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1336">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8ea7d-1337">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1337">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8ea7d-1338">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1338">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8ea7d-1339">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1339">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1340">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1341">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1341">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8ea7d-1342">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1342">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1343">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-1344">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1344">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-1345">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1345">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-1346">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1346">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1347">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1347">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1348">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1348">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8ea7d-1349">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1349">Updated cmdlet:</span></span>
        - <span data-ttu-id="8ea7d-1350">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1350">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8ea7d-1351">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1351">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1352">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1353">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1353">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1354">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1354">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1355">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1355">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8ea7d-1356">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1356">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1357">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1358">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1358">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-1359">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1359">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-1360">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1360">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8ea7d-1361">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1361">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1362">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1363">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1363">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8ea7d-1364">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1364">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8ea7d-1365">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1365">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8ea7d-1366">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1366">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8ea7d-1367">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1367">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8ea7d-1368">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1368">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="8ea7d-1369">重大な変更</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1369">Breaking changes</span></span>
    - <span data-ttu-id="8ea7d-1370">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1370">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8ea7d-1371">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1371">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8ea7d-1372">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1372">Az.DeploymentManager</span></span>
* <span data-ttu-id="8ea7d-1373">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1373">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8ea7d-1374">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1374">Az.Dns</span></span>
* <span data-ttu-id="8ea7d-1375">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1375">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8ea7d-1376">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1376">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8ea7d-1377">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1377">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-1378">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1378">Az.FrontDoor</span></span>
* <span data-ttu-id="8ea7d-1379">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1379">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8ea7d-1380">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1380">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-1381">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1381">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-1382">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1382">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8ea7d-1383">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1383">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8ea7d-1384">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1384">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8ea7d-1385">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1385">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8ea7d-1386">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1386">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8ea7d-1387">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1387">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8ea7d-1388">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1388">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-1389">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1389">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-1390">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1390">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="8ea7d-1391">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1391">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8ea7d-1392">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1392">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8ea7d-1393">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1393">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8ea7d-1394">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1394">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8ea7d-1395">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1395">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8ea7d-1396">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1396">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8ea7d-1397">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1397">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ea7d-1398">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1398">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ea7d-1399">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1399">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ea7d-1400">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1400">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ea7d-1401">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1401">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8ea7d-1402">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1402">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8ea7d-1403">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1403">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1404">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1404">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1405">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1405">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8ea7d-1406">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1406">New cmdlets</span></span>
        - <span data-ttu-id="8ea7d-1407">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1407">New-AzNatGateway</span></span>
        - <span data-ttu-id="8ea7d-1408">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1408">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8ea7d-1409">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1409">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8ea7d-1410">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1410">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8ea7d-1411">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1411">Updated cmdlets</span></span>
        - <span data-ttu-id="8ea7d-1412">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1412">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8ea7d-1413">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1413">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8ea7d-1414">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1414">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8ea7d-1415">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1415">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8ea7d-1416">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1416">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ea7d-1417">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1417">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ea7d-1418">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1418">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8ea7d-1419">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1419">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8ea7d-1420">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1420">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1421">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1421">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1422">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1422">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8ea7d-1423">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1423">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8ea7d-1424">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1424">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8ea7d-1425">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1425">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8ea7d-1426">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1426">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8ea7d-1427">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1427">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8ea7d-1428">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1428">Az.Relay</span></span>
* <span data-ttu-id="8ea7d-1429">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1429">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-1430">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1430">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-1431">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1431">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1432">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1432">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1433">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1433">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8ea7d-1434">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1434">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8ea7d-1435">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1435">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8ea7d-1436">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1436">New-AzStorageAccount</span></span>
* <span data-ttu-id="8ea7d-1437">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1437">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8ea7d-1438">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1438">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8ea7d-1439">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1439">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8ea7d-1440">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1440">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1441">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1442">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1442">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8ea7d-1443">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1443">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8ea7d-1444">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1444">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-1445">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1445">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-1446">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1446">General availability of `Az` module</span></span>
* <span data-ttu-id="8ea7d-1447">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1447">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ea7d-1448">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1448">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ea7d-1449">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1449">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ea7d-1450">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1450">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ea7d-1451">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1451">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1452">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1452">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1453">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1453">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1454">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1454">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8ea7d-1455">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1455">Az.Batch</span></span>
* <span data-ttu-id="8ea7d-1456">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1456">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-1457">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1457">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-1458">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1458">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-1459">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1459">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-1460">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1460">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1461">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1462">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1462">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8ea7d-1463">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1463">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1464">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1464">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-1465">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1465">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-1466">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1466">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1467">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1467">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-1468">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1468">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ea7d-1469">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1469">Az.EventGrid</span></span>
* <span data-ttu-id="8ea7d-1470">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1470">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-1471">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1471">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-1472">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1472">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="8ea7d-1473">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1473">Az.HDInsight</span></span>
* <span data-ttu-id="8ea7d-1474">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1474">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-1475">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1475">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-1476">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1476">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-1477">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1477">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-1478">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1478">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1479">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1479">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8ea7d-1480">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1480">Az.MachineLearning</span></span>
* <span data-ttu-id="8ea7d-1481">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1481">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8ea7d-1482">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1482">Az.Media</span></span>
* <span data-ttu-id="8ea7d-1483">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1483">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-1484">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1484">Az.Monitor</span></span>
  * <span data-ttu-id="8ea7d-1485">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1485">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8ea7d-1486">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1486">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8ea7d-1487">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1487">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8ea7d-1488">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1488">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8ea7d-1489">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1489">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8ea7d-1490">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1490">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8ea7d-1491">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1491">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1492">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1492">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1493">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1493">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1494">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1494">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8ea7d-1495">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1495">Az.NotificationHubs</span></span>
* <span data-ttu-id="8ea7d-1496">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1496">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1497">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1497">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-1498">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1498">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8ea7d-1499">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1499">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8ea7d-1500">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1500">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1501">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1502">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1502">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1503">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1503">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8ea7d-1504">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1504">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8ea7d-1505">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1505">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ea7d-1506">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1506">Az.RedisCache</span></span>
* <span data-ttu-id="8ea7d-1507">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1507">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1508">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1508">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1509">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1509">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1510">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1511">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1511">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8ea7d-1512">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1512">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1513">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1513">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8ea7d-1514">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1514">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8ea7d-1515">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1515">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8ea7d-1516">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1516">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8ea7d-1517">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1517">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1518">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1519">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1519">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8ea7d-1520">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1520">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8ea7d-1521">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1521">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8ea7d-1522">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1522">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8ea7d-1523">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1523">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-1524">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1524">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-1525">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1525">General availability of `Az` module</span></span>
* <span data-ttu-id="8ea7d-1526">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1526">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ea7d-1527">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1527">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ea7d-1528">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1528">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ea7d-1529">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1529">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ea7d-1530">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1530">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1531">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1531">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1532">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1533">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1533">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ea7d-1534">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1534">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ea7d-1535">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1535">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8ea7d-1536">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1536">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1537">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1537">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1538">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1538">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8ea7d-1539">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1539">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8ea7d-1540">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1540">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1541">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1541">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1542">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1542">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8ea7d-1543">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1543">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="8ea7d-1544">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1544">Az.ContainerInstance</span></span>
* <span data-ttu-id="8ea7d-1545">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1545">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-1546">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1546">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-1547">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1547">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8ea7d-1548">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1548">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1549">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1550">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1550">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8ea7d-1551">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1551">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8ea7d-1552">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1552">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8ea7d-1553">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1553">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8ea7d-1554">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1554">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8ea7d-1555">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1555">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1556">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1556">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1557">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1557">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1558">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1558">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1559">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1559">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8ea7d-1560">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1560">New-AzStorageContext</span></span>
* <span data-ttu-id="8ea7d-1561">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1561">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8ea7d-1562">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1562">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8ea7d-1563">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1563">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8ea7d-1564">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1564">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8ea7d-1565">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1565">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8ea7d-1566">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1566">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8ea7d-1567">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1567">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8ea7d-1568">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1568">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8ea7d-1569">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1569">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8ea7d-1570">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1570">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8ea7d-1571">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1571">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8ea7d-1572">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1572">Highlights since the last major release</span></span>
* <span data-ttu-id="8ea7d-1573">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1573">General availability of `Az` module</span></span>
* <span data-ttu-id="8ea7d-1574">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1574">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8ea7d-1575">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1575">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8ea7d-1576">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1576">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8ea7d-1577">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1577">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ea7d-1578">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1578">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1579">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1579">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1580">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1580">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1581">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1581">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8ea7d-1582">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1582">Dynamic grouping</span></span>
    * <span data-ttu-id="8ea7d-1583">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1583">Pre-Post script</span></span>
    * <span data-ttu-id="8ea7d-1584">再起動設定</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1584">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1585">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1585">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1586">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1586">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8ea7d-1587">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1587">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-1588">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1588">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-1589">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1589">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1590">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1590">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1591">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1591">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8ea7d-1592">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1592">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1593">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1593">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1594">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1594">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8ea7d-1595">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1595">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1596">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1596">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1597">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1597">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8ea7d-1598">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1598">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1599">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1599">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1600">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1600">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1601">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1601">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1602">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1602">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8ea7d-1603">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1603">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ea7d-1604">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1604">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ea7d-1605">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1605">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8ea7d-1606">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1606">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8ea7d-1607">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1607">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8ea7d-1608">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1608">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1609">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1609">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1610">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1610">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="8ea7d-1611">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1611">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1612">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1612">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1613">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1613">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8ea7d-1614">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1614">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1615">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1615">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1616">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1616">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8ea7d-1617">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1617">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8ea7d-1618">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1618">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-1619">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1619">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-1620">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1620">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1621">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1621">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1622">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1622">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-1623">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1623">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-1624">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1624">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ea7d-1625">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1625">Az.LogicApp</span></span>
* <span data-ttu-id="8ea7d-1626">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1626">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1627">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1627">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1628">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1628">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1629">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1629">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1630">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1630">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8ea7d-1631">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1631">SDK Update</span></span>
* <span data-ttu-id="8ea7d-1632">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1632">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8ea7d-1633">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1633">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1634">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1634">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1635">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1635">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8ea7d-1636">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1636">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8ea7d-1637">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1637">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8ea7d-1638">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1638">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8ea7d-1639">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1639">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8ea7d-1640">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1640">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1641">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1641">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1642">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1642">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8ea7d-1643">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1643">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1644">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1645">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1645">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8ea7d-1646">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1646">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8ea7d-1647">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1647">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ea7d-1648">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1648">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1649">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1649">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1650">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1650">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8ea7d-1651">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1651">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8ea7d-1652">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1652">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-1653">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1653">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-1654">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1654">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1655">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1656">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1656">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8ea7d-1657">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1657">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8ea7d-1658">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1658">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8ea7d-1659">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1659">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1660">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1660">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-1661">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1661">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8ea7d-1662">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1662">Az.EventHub</span></span>
* <span data-ttu-id="8ea7d-1663">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1663">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-1664">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1664">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-1665">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1665">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ea7d-1666">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1666">Az.LogicApp</span></span>
* <span data-ttu-id="8ea7d-1667">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1667">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8ea7d-1668">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1668">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8ea7d-1669">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1669">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8ea7d-1670">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1670">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ea7d-1671">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1671">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ea7d-1672">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1672">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8ea7d-1673">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1673">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8ea7d-1674">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1674">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8ea7d-1675">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1675">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ea7d-1676">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1676">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ea7d-1677">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1677">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8ea7d-1678">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1678">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8ea7d-1679">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1679">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8ea7d-1680">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1680">Az.Monitor</span></span>
* <span data-ttu-id="8ea7d-1681">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1681">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1682">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1682">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1683">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1683">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1684">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1684">Az.OperationalInsights</span></span>
* <span data-ttu-id="8ea7d-1685">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1685">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8ea7d-1686">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1686">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="8ea7d-1687">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1687">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1688">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1688">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1689">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1689">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8ea7d-1690">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1690">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8ea7d-1691">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1691">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8ea7d-1692">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1692">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1693">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1693">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1694">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1694">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8ea7d-1695">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1695">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1696">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1696">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1697">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1697">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8ea7d-1698">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1698">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1699">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1699">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1700">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1700">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ea7d-1701">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1701">Az.AnalysisServices</span></span>
<span data-ttu-id="8ea7d-1702">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1702">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1703">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1703">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1704">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1704">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8ea7d-1705">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1705">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8ea7d-1706">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1706">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1707">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1707">Az.RecoveryServices</span></span>
<span data-ttu-id="8ea7d-1708">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1708">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1709">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1709">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1710">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1710">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="8ea7d-1711">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1711">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8ea7d-1712">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1712">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="8ea7d-1713">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1713">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1714">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1714">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1715">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1715">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8ea7d-1716">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1716">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8ea7d-1717">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1717">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8ea7d-1718">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1718">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1719">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1719">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1720">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1720">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8ea7d-1721">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1721">Az.AnalysisServices</span></span>
* <span data-ttu-id="8ea7d-1722">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1722">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1723">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1723">Az.RecoveryServices</span></span>
* <span data-ttu-id="8ea7d-1724">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1724">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8ea7d-1725">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1725">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1726">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1726">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1727">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1727">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8ea7d-1728">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1728">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ea7d-1729">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1729">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8ea7d-1730">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1730">Az.Aks</span></span>
* <span data-ttu-id="8ea7d-1731">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1731">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8ea7d-1732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1732">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1733">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1733">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8ea7d-1734">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1734">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8ea7d-1735">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1735">Az.Cdn</span></span>
* <span data-ttu-id="8ea7d-1736">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1736">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1737">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1738">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1738">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8ea7d-1739">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1739">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8ea7d-1740">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1740">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8ea7d-1741">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1741">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8ea7d-1742">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1742">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8ea7d-1743">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1743">Az.DataFactory</span></span>
* <span data-ttu-id="8ea7d-1744">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1744">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1745">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1745">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-1746">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1746">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8ea7d-1747">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1747">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8ea7d-1748">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1748">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-1749">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1749">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-1750">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1750">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-1751">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1751">Az.KeyVault</span></span>
* <span data-ttu-id="8ea7d-1752">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1752">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1753">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1753">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1754">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1754">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1755">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1755">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1756">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1756">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8ea7d-1757">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1757">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8ea7d-1758">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1758">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8ea7d-1759">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1759">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8ea7d-1760">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1760">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8ea7d-1761">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1761">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8ea7d-1762">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1762">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-1763">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1763">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-1764">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1764">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8ea7d-1765">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1765">Fix some error messages.</span></span>
* <span data-ttu-id="8ea7d-1766">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1766">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8ea7d-1767">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1767">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8ea7d-1768">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1768">Az.SignalR</span></span>
* <span data-ttu-id="8ea7d-1769">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1769">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1770">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1770">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1771">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1771">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ea7d-1772">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1772">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8ea7d-1773">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1773">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8ea7d-1774">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1774">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1775">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1775">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1776">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1776">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ea7d-1777">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1777">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8ea7d-1778">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1778">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8ea7d-1779">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1779">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8ea7d-1780">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1780">Az.TrafficManager</span></span>
* <span data-ttu-id="8ea7d-1781">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1781">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1782">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1782">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1783">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1783">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8ea7d-1784">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1784">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8ea7d-1785">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1785">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8ea7d-1786">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1786">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1787">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1787">Az.Accounts</span></span>
* <span data-ttu-id="8ea7d-1788">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1788">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-1789">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1789">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1790">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1790">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8ea7d-1791">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1791">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8ea7d-1792">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1792">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1793">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1793">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-1794">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1794">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8ea7d-1795">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1795">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8ea7d-1796">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1796">Az.EventGrid</span></span>
* <span data-ttu-id="8ea7d-1797">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1797">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8ea7d-1798">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1798">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8ea7d-1799">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1799">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8ea7d-1800">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1800">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8ea7d-1801">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1801">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8ea7d-1802">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1802">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8ea7d-1803">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1803">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8ea7d-1804">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1804">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8ea7d-1805">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1805">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8ea7d-1806">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1806">Dead letter endpoint.</span></span>
* <span data-ttu-id="8ea7d-1807">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1807">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8ea7d-1808">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1808">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8ea7d-1809">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1809">Az.IotHub</span></span>
* <span data-ttu-id="8ea7d-1810">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1810">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8ea7d-1811">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1811">Az.LogicApp</span></span>
* <span data-ttu-id="8ea7d-1812">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1812">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-1813">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1813">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1814">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1814">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8ea7d-1815">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1815">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8ea7d-1816">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1816">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8ea7d-1817">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1817">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8ea7d-1818">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1818">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8ea7d-1819">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1819">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8ea7d-1820">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1820">Az.SignalR</span></span>
* <span data-ttu-id="8ea7d-1821">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1821">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-1822">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1822">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1823">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1823">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8ea7d-1824">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1824">Az.Storage</span></span>
* <span data-ttu-id="8ea7d-1825">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1825">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8ea7d-1826">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1826">New-AzStorageContext</span></span>
* <span data-ttu-id="8ea7d-1827">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1827">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8ea7d-1828">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1828">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1829">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1829">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-1830">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1830">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8ea7d-1831">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1831">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8ea7d-1832">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1832">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8ea7d-1833">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1833">General</span></span>

- <span data-ttu-id="8ea7d-1834">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1834">General Availability of Az Module</span></span>
- <span data-ttu-id="8ea7d-1835">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1835">Online help for each module</span></span>
- <span data-ttu-id="8ea7d-1836">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1836">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8ea7d-1837">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1837">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8ea7d-1838">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1838">Az.Accounts</span></span>
- <span data-ttu-id="8ea7d-1839">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1839">Changed from Az.Profile</span></span>
- <span data-ttu-id="8ea7d-1840">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1840">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-1841">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1841">Az.ApiManagement</span></span>
- <span data-ttu-id="8ea7d-1842">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1842">Fixes for #7002</span></span>
- <span data-ttu-id="8ea7d-1843">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1843">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8ea7d-1844">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1844">Az.Batch</span></span>
- <span data-ttu-id="8ea7d-1845">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1845">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8ea7d-1846">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1846">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8ea7d-1847">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1847">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8ea7d-1848">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1848">Az.Billing</span></span>
- <span data-ttu-id="8ea7d-1849">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1849">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8ea7d-1850">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1850">Az.CognitivServices</span></span>
- <span data-ttu-id="8ea7d-1851">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1851">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8ea7d-1852">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1852">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8ea7d-1853">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1853">Az.ContainerInstance</span></span>
- <span data-ttu-id="8ea7d-1854">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1854">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8ea7d-1855">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1855">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8ea7d-1856">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1856">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1857">Az.DataLakeStore</span></span>
- <span data-ttu-id="8ea7d-1858">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1858">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8ea7d-1859">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1859">Az.Monitor</span></span>
- <span data-ttu-id="8ea7d-1860">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1860">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8ea7d-1861">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1861">Az.KeyVault</span></span>
- <span data-ttu-id="8ea7d-1862">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1862">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8ea7d-1863">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1863">Az.MachineLearning</span></span>
- <span data-ttu-id="8ea7d-1864">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1864">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8ea7d-1865">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1865">Az.Media</span></span>
- <span data-ttu-id="8ea7d-1866">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1866">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1867">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1867">Az.Network</span></span>
<span data-ttu-id="8ea7d-1868">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1868">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8ea7d-1869">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1869">New cmdlets added:</span></span>
        - <span data-ttu-id="8ea7d-1870">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1870">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1871">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1871">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1872">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1872">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1873">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1873">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1874">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1874">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1875">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1875">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8ea7d-1876">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1876">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8ea7d-1877">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1877">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8ea7d-1878">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1878">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8ea7d-1879">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1879">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8ea7d-1880">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1880">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8ea7d-1881">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1881">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8ea7d-1882">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1882">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8ea7d-1883">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1883">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8ea7d-1884">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1884">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8ea7d-1885">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1885">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8ea7d-1886">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1886">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8ea7d-1887">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1887">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8ea7d-1888">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1888">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8ea7d-1889">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1889">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8ea7d-1890">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1890">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8ea7d-1891">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1891">Az.OperationalInsights</span></span>
- <span data-ttu-id="8ea7d-1892">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1892">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8ea7d-1893">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1893">Az.Profile</span></span>
- <span data-ttu-id="8ea7d-1894">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1894">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1895">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1895">Az.RecoveryServices</span></span>
- <span data-ttu-id="8ea7d-1896">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1896">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8ea7d-1897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1897">Az.Resources</span></span>
- <span data-ttu-id="8ea7d-1898">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1898">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-1899">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1899">Az.ServiceFabric</span></span>
- <span data-ttu-id="8ea7d-1900">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1900">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8ea7d-1901">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1901">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8ea7d-1902">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1902">Az.SIgnalR</span></span>
- <span data-ttu-id="8ea7d-1903">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1903">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8ea7d-1904">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1904">Az.Sql</span></span>
- <span data-ttu-id="8ea7d-1905">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1905">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8ea7d-1906">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1906">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8ea7d-1907">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1907">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8ea7d-1908">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1908">Az.Storage</span></span>
- <span data-ttu-id="8ea7d-1909">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1909">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1910">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1910">Az.Websites</span></span>
- <span data-ttu-id="8ea7d-1911">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1911">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8ea7d-1912">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1912">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8ea7d-1913">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1913">General</span></span>

* <span data-ttu-id="8ea7d-1914">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1914">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8ea7d-1915">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1915">Az.Compute</span></span>

* <span data-ttu-id="8ea7d-1916">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1916">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-1917">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1917">Az.DataLakeStore</span></span>

* <span data-ttu-id="8ea7d-1918">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1918">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8ea7d-1919">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1919">Az.FrontDoor</span></span>

* <span data-ttu-id="8ea7d-1920">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1920">Fixed some broken links</span></span>
    - <span data-ttu-id="8ea7d-1921">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1921">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8ea7d-1922">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1922">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8ea7d-1923">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1923">Az.RecoveryServices</span></span>

* <span data-ttu-id="8ea7d-1924">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1924">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8ea7d-1925">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1925">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8ea7d-1926">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1926">Az.Resources</span></span>

* <span data-ttu-id="8ea7d-1927">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1927">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8ea7d-1928">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1928">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8ea7d-1929">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1929">Az.Sql</span></span>

* <span data-ttu-id="8ea7d-1930">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1930">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8ea7d-1931">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1931">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8ea7d-1932">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1932">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8ea7d-1933">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1933">Az.Storage</span></span>

* <span data-ttu-id="8ea7d-1934">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1934">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8ea7d-1935">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1935">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8ea7d-1936">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1936">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8ea7d-1937">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1937">Support Static Website configuration</span></span>
    - <span data-ttu-id="8ea7d-1938">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1938">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8ea7d-1939">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1939">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8ea7d-1940">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1940">Az.Websites</span></span>

* <span data-ttu-id="8ea7d-1941">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1941">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="8ea7d-1942">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1942">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8ea7d-1943">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1943">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8ea7d-1944">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1944">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8ea7d-1945">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1945">Az.ApiManagement</span></span>
* <span data-ttu-id="8ea7d-1946">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1946">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8ea7d-1947">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1947">Az.Automation</span></span>
* <span data-ttu-id="8ea7d-1948">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1948">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8ea7d-1949">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1949">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8ea7d-1950">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1950">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8ea7d-1951">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1951">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8ea7d-1952">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1952">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8ea7d-1953">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1953">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-1954">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1954">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8ea7d-1955">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1955">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8ea7d-1956">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1956">Az.ContainerInstance</span></span>
* <span data-ttu-id="8ea7d-1957">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1957">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8ea7d-1958">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1958">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8ea7d-1959">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1959">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8ea7d-1960">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1960">Az.Network</span></span>
* <span data-ttu-id="8ea7d-1961">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1961">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8ea7d-1962">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1962">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8ea7d-1963">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1963">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="8ea7d-1964">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1964">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8ea7d-1965">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1965">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8ea7d-1966">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1966">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8ea7d-1967">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1967">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8ea7d-1968">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1968">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8ea7d-1969">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1969">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8ea7d-1970">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1970">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8ea7d-1971">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1971">Az.Relay</span></span>
* <span data-ttu-id="8ea7d-1972">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1972">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8ea7d-1973">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1973">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-1974">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1974">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8ea7d-1975">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1975">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8ea7d-1976">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1976">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-1977">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1977">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-1978">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1978">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8ea7d-1979">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1979">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-1980">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1980">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8ea7d-1981">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1981">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ea7d-1982">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1982">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ea7d-1983">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1983">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ea7d-1984">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1984">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8ea7d-1985">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1985">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ea7d-1986">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1986">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ea7d-1987">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1987">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8ea7d-1988">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1988">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8ea7d-1989">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1989">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8ea7d-1990">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1990">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8ea7d-1991">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1991">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8ea7d-1992">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1992">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8ea7d-1993">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1993">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8ea7d-1994">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1994">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8ea7d-1995">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1995">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8ea7d-1996">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1996">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8ea7d-1997">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1997">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8ea7d-1998">全般</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1998">General</span></span>
* <span data-ttu-id="8ea7d-1999">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="8ea7d-1999">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8ea7d-2000">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2000">Az.Profile</span></span>
* <span data-ttu-id="8ea7d-2001">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2001">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8ea7d-2002">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2002">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8ea7d-2003">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2003">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8ea7d-2004">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2004">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8ea7d-2005">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2005">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8ea7d-2006">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2006">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8ea7d-2007">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2007">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-2008">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2008">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-2009">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2009">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-2010">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2010">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-2011">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2011">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8ea7d-2012">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2012">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8ea7d-2013">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2013">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-2014">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2014">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-2015">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2015">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8ea7d-2016">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2016">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8ea7d-2017">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2017">Az.Insights</span></span>
* <span data-ttu-id="8ea7d-2018">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2018">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8ea7d-2019">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2019">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8ea7d-2020">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2020">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8ea7d-2021">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2021">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-2022">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2022">Az.Network</span></span>
* <span data-ttu-id="8ea7d-2023">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2023">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8ea7d-2024">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2024">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8ea7d-2025">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2025">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8ea7d-2026">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2026">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8ea7d-2027">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2027">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8ea7d-2028">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2028">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8ea7d-2029">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2029">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8ea7d-2030">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2030">Az.PolicyInsights</span></span>
* <span data-ttu-id="8ea7d-2031">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2031">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-2032">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2032">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-2033">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2033">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8ea7d-2034">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2034">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8ea7d-2035">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2035">Az.ServiceBus</span></span>
* <span data-ttu-id="8ea7d-2036">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2036">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8ea7d-2037">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2037">Az.ServiceFabric</span></span>
* <span data-ttu-id="8ea7d-2038">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2038">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8ea7d-2039">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2039">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8ea7d-2040">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2040">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8ea7d-2041">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2041">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8ea7d-2042">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2042">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8ea7d-2043">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2043">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8ea7d-2044">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2044">Az.Profile</span></span>
* <span data-ttu-id="8ea7d-2045">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2045">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8ea7d-2046">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2046">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-2047">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2047">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-2048">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2048">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8ea7d-2049">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2049">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8ea7d-2050">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2050">Az.DataLakeStore</span></span>
* <span data-ttu-id="8ea7d-2051">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2051">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8ea7d-2052">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2052">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8ea7d-2053">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2053">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8ea7d-2054">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2054">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8ea7d-2055">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2055">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-2056">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2056">Az.Network</span></span>
* <span data-ttu-id="8ea7d-2057">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2057">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8ea7d-2058">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2058">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-2059">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2059">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-2060">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2060">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8ea7d-2061">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2061">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8ea7d-2062">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2062">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8ea7d-2063">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2063">Azure.Storage</span></span>
* <span data-ttu-id="8ea7d-2064">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2064">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8ea7d-2065">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2065">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8ea7d-2066">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2066">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8ea7d-2067">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2067">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8ea7d-2068">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2068">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="8ea7d-2069">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2069">Az.CognitiveServices</span></span>
* <span data-ttu-id="8ea7d-2070">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2070">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8ea7d-2071">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2071">Az.Compute</span></span>
* <span data-ttu-id="8ea7d-2072">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2072">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8ea7d-2073">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2073">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8ea7d-2074">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2074">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8ea7d-2075">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2075">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8ea7d-2076">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2076">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8ea7d-2077">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2077">Az.Network</span></span>
* <span data-ttu-id="8ea7d-2078">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2078">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8ea7d-2079">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2079">new cmdlets added</span></span>
    - <span data-ttu-id="8ea7d-2080">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2080">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ea7d-2081">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2081">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ea7d-2082">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2082">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ea7d-2083">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2083">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8ea7d-2084">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2084">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8ea7d-2085">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2085">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8ea7d-2086">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2086">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8ea7d-2087">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2087">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8ea7d-2088">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2088">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8ea7d-2089">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2089">Az.RedisCache</span></span>
* <span data-ttu-id="8ea7d-2090">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2090">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8ea7d-2091">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2091">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8ea7d-2092">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2092">Az.Resources</span></span>
* <span data-ttu-id="8ea7d-2093">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2093">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8ea7d-2094">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2094">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8ea7d-2095">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2095">Az.Sql</span></span>
* <span data-ttu-id="8ea7d-2096">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2096">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8ea7d-2097">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2097">Az.Websites</span></span>
* <span data-ttu-id="8ea7d-2098">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2098">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8ea7d-2099">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2099">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8ea7d-2100">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2100">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8ea7d-2101">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="8ea7d-2101">Initial Release</span></span>

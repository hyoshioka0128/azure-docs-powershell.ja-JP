---
title: "Azure PowerShell の変更履歴 | Microsoft Docs"
description: "Azure PowerShell の最新リリースで行われた変更の履歴です。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 143d92384fd270711378f6741ba59e88c12833d1
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="93c5f-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="93c5f-103">Release notes</span></span>
<a id="release-notes" class="xliff"></a>

<span data-ttu-id="93c5f-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="93c5f-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <span data-ttu-id="93c5f-105">バージョン 2.2.0</span><span class="sxs-lookup"><span data-stu-id="93c5f-105">Version 2.2.0</span></span>
<a id="version-220" class="xliff"></a>
* <span data-ttu-id="93c5f-106">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="93c5f-106">Compute</span></span>
  - <span data-ttu-id="93c5f-107">AzureDiskEncryptionForLinux 拡張機能の暗号化状態を照会できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="93c5f-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="93c5f-108">DataFactory</span></span>
  - <span data-ttu-id="93c5f-109">アクティビティ ウィンドウを列挙するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="93c5f-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="93c5f-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="93c5f-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="93c5f-111">DataLake</span></span>
  - <span data-ttu-id="93c5f-112">パラメーター `Host` を `DatabaseHost` に変更し、`Host` へのエイリアスを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="93c5f-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="93c5f-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="93c5f-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="93c5f-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="93c5f-115">新たに ACL と既定の ACL の削除に対応しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="93c5f-116">ファイルやフォルダーに対する無名のアクセス許可を取得したり設定したりできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="93c5f-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="93c5f-117">KeyVault</span></span>
  - <span data-ttu-id="93c5f-118">証明書関連の機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-118">Add support for certificates</span></span>
    + <span data-ttu-id="93c5f-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="93c5f-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="93c5f-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="93c5f-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="93c5f-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="93c5f-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="93c5f-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="93c5f-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="93c5f-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="93c5f-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="93c5f-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="93c5f-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="93c5f-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="93c5f-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="93c5f-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="93c5f-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="93c5f-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="93c5f-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="93c5f-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="93c5f-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="93c5f-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="93c5f-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="93c5f-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="93c5f-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="93c5f-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="93c5f-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="93c5f-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="93c5f-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="93c5f-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="93c5f-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="93c5f-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="93c5f-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="93c5f-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="93c5f-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="93c5f-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="93c5f-138">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="93c5f-138">Network</span></span>

  - <span data-ttu-id="93c5f-139">ネットワーク インターフェイスで高速ネットワークの有効/無効を切り替える新しいスイッチ パラメーターが追加されました (+New-AzureRmNetworkInterface -EnableAcceleratedNetworking)。</span><span class="sxs-lookup"><span data-stu-id="93c5f-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="93c5f-140">アクティブ/アクティブ ゲートウェイ機能を実現する PowerShell コマンドレット</span><span class="sxs-lookup"><span data-stu-id="93c5f-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="93c5f-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="93c5f-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="93c5f-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="93c5f-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="93c5f-143">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-143">Added new cmdlet</span></span>
    + <span data-ttu-id="93c5f-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="93c5f-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="93c5f-145">リソース</span><span class="sxs-lookup"><span data-stu-id="93c5f-145">Resources</span></span>
  - <span data-ttu-id="93c5f-146">プロバイダー コマンドレットとリソース コマンドレットでゾーンに対応しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="93c5f-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="93c5f-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="93c5f-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="93c5f-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="93c5f-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="93c5f-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="93c5f-150">SQL</span><span class="sxs-lookup"><span data-stu-id="93c5f-150">Sql</span></span>
  - <span data-ttu-id="93c5f-151">Azure SQL 脅威検出ポリシーをサーバー レベルで管理するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="93c5f-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="93c5f-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="93c5f-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="93c5f-155">SQL Azure Data Warehouse の GeoBackupPolicy の有効化/無効化に対応する新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="93c5f-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="93c5f-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="93c5f-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="93c5f-158">Azure Sql Advisors と Recommended Actions API 用の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="93c5f-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="93c5f-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="93c5f-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="93c5f-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="93c5f-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="93c5f-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="93c5f-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="93c5f-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="93c5f-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="93c5f-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="93c5f-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="93c5f-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="93c5f-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="93c5f-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="93c5f-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="93c5f-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="93c5f-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="93c5f-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="93c5f-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="93c5f-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="93c5f-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="93c5f-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="93c5f-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="93c5f-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="93c5f-170">Set-AzureRmSqlServerRecommendedActionState</span></span>

---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: a00bc2f13117f1b07f0dcc5808eddbabe1df940f
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821668"
---
# <a name="release-notes"></a><span data-ttu-id="5ebe2-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="5ebe2-103">Release notes</span></span>

<span data-ttu-id="5ebe2-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="5ebe2-105">バージョン 2.2.0</span><span class="sxs-lookup"><span data-stu-id="5ebe2-105">Version 2.2.0</span></span>
* <span data-ttu-id="5ebe2-106">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="5ebe2-106">Compute</span></span>
  - <span data-ttu-id="5ebe2-107">AzureDiskEncryptionForLinux 拡張機能の暗号化状態を照会できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="5ebe2-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="5ebe2-108">DataFactory</span></span>
  - <span data-ttu-id="5ebe2-109">アクティビティ ウィンドウを列挙するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="5ebe2-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="5ebe2-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="5ebe2-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="5ebe2-111">DataLake</span></span>
  - <span data-ttu-id="5ebe2-112">パラメーター `Host` を `DatabaseHost` に変更し、`Host` へのエイリアスを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="5ebe2-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="5ebe2-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="5ebe2-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="5ebe2-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="5ebe2-115">新たに ACL と既定の ACL の削除に対応しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="5ebe2-116">ファイルやフォルダーに対する無名のアクセス許可を取得したり設定したりできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="5ebe2-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5ebe2-117">KeyVault</span></span>
  - <span data-ttu-id="5ebe2-118">証明書関連の機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-118">Add support for certificates</span></span>
    + <span data-ttu-id="5ebe2-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="5ebe2-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="5ebe2-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="5ebe2-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="5ebe2-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="5ebe2-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="5ebe2-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="5ebe2-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="5ebe2-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="5ebe2-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="5ebe2-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="5ebe2-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="5ebe2-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="5ebe2-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="5ebe2-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="5ebe2-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="5ebe2-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="5ebe2-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="5ebe2-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="5ebe2-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="5ebe2-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="5ebe2-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="5ebe2-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="5ebe2-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="5ebe2-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="5ebe2-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="5ebe2-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="5ebe2-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="5ebe2-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="5ebe2-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="5ebe2-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="5ebe2-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="5ebe2-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="5ebe2-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="5ebe2-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="5ebe2-138">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="5ebe2-138">Network</span></span>

  - <span data-ttu-id="5ebe2-139">ネットワーク インターフェイスで高速ネットワークの有効/無効を切り替える新しいスイッチ パラメーターが追加されました (+New-AzureRmNetworkInterface -EnableAcceleratedNetworking)。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="5ebe2-140">アクティブ/アクティブ ゲートウェイ機能を実現する PowerShell コマンドレット</span><span class="sxs-lookup"><span data-stu-id="5ebe2-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="5ebe2-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5ebe2-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="5ebe2-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5ebe2-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="5ebe2-143">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-143">Added new cmdlet</span></span>
    + <span data-ttu-id="5ebe2-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="5ebe2-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="5ebe2-145">リソース</span><span class="sxs-lookup"><span data-stu-id="5ebe2-145">Resources</span></span>
  - <span data-ttu-id="5ebe2-146">プロバイダー コマンドレットとリソース コマンドレットでゾーンに対応しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="5ebe2-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="5ebe2-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="5ebe2-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="5ebe2-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="5ebe2-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="5ebe2-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="5ebe2-150">SQL</span><span class="sxs-lookup"><span data-stu-id="5ebe2-150">Sql</span></span>
  - <span data-ttu-id="5ebe2-151">Azure SQL 脅威検出ポリシーをサーバー レベルで管理するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="5ebe2-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="5ebe2-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="5ebe2-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="5ebe2-155">SQL Azure Data Warehouse の GeoBackupPolicy の有効化/無効化に対応する新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="5ebe2-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="5ebe2-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe2-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="5ebe2-158">Azure Sql Advisors と Recommended Actions API 用の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="5ebe2-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="5ebe2-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="5ebe2-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="5ebe2-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="5ebe2-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="5ebe2-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="5ebe2-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="5ebe2-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="5ebe2-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="5ebe2-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="5ebe2-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="5ebe2-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="5ebe2-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="5ebe2-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="5ebe2-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="5ebe2-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="5ebe2-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="5ebe2-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="5ebe2-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="5ebe2-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="5ebe2-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="5ebe2-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="5ebe2-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="5ebe2-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="5ebe2-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
